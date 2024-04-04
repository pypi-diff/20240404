# Comparing `tmp/projectal-4.3.0.tar.gz` & `tmp/projectal-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectal-4.3.0.tar", last modified: Wed Feb 21 23:56:37 2024, max compression
+gzip compressed data, was "projectal-4.3.1.tar", last modified: Thu Apr  4 00:02:33 2024, max compression
```

## Comparing `projectal-4.3.0.tar` & `projectal-4.3.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.948602 projectal-4.3.0/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.3.0/LICENSE
--rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.3.0/MANIFEST.in
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2024-02-21 23:56:37.948602 projectal-4.3.0/PKG-INFO
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.940602 projectal-4.3.0/docs/
--rw-rw-r--   0 luked     (1003) luked     (1003)      140 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/index.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.940602 projectal-4.3.0/docs/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)   126818 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/api.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    50793 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enum.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.940602 projectal-4.3.0/docs/projectal/dynamic_enums/
--rw-rw-r--   0 luked     (1003) luked     (1003)    38074 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/company_types.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    38158 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/complexity_levels.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    38068 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/currency_list.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    38116 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/priority_levels.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    38053 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/skill_levels.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    38032 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums/staff_types.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    37995 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/dynamic_enums.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.944602 projectal-4.3.0/docs/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)    45618 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/access_policy.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    54635 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/activity.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   118244 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/booking.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    77470 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/calendar.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    82761 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/company.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    61191 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/contact.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    48999 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/customer.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    74473 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/department.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   116609 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/file.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    80179 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/folder.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    69273 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/location.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    74972 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/note.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    52102 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/permission.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    78604 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/project.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    54248 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/project_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    47064 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/rebate.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    47337 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/resource.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    46507 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/skill.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   147305 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/staff.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    45478 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities/stage.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    42962 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entities/tag.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   299759 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entities/task.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   103346 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entities/task_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    81531 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entities/user.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    77623 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entities/webhook.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    43317 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal/entities.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   680048 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/entity.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   135037 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/enums.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   115062 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/errors.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   272729 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/linkers.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    58181 2024-02-21 23:54:52.000000 projectal-4.3.0/docs/projectal/profile.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   143960 2024-02-21 23:54:51.000000 projectal-4.3.0/docs/projectal.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.944602 projectal-4.3.0/examples/
--rw-rw-r--   0 luked     (1003) luked     (1003)     3172 2023-10-18 05:03:25.000000 projectal-4.3.0/examples/linking.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      830 2023-10-18 05:03:24.000000 projectal-4.3.0/examples/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1047 2023-10-18 05:03:24.000000 projectal-4.3.0/examples/webhook.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.944602 projectal-4.3.0/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)    22155 2024-02-21 23:29:15.000000 projectal-4.3.0/projectal/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     9272 2023-11-16 00:16:46.000000 projectal-4.3.0/projectal/api.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      663 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enum.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.944602 projectal-4.3.0/projectal/dynamic_enums/
--rw-rw-r--   0 luked     (1003) luked     (1003)      509 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      112 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/company_types.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      120 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/complexity_levels.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      109 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/currency_list.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      116 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/priority_levels.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      110 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/skill_levels.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      108 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/dynamic_enums/staff_types.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.948602 projectal-4.3.0/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.3.0/projectal/entities/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      396 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/access_policy.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      670 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/activity.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     4743 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/booking.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2234 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/calendar.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2024 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/company.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      983 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/contact.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      477 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/customer.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1878 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/department.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3245 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/file.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1733 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/folder.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1326 2024-01-10 05:22:19.000000 projectal-4.3.0/projectal/entities/location.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1942 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/note.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      614 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/permission.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1657 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/project.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      711 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/project_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      420 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/rebate.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      426 2023-10-18 05:03:24.000000 projectal-4.3.0/projectal/entities/resource.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      396 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/skill.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     4860 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/staff.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      345 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/stage.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      231 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/entities/tag.py
--rw-rw-r--   0 luked     (1003) luked     (1003)    17261 2024-02-21 23:29:15.000000 projectal-4.3.0/projectal/entities/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2676 2023-10-17 06:27:06.000000 projectal-4.3.0/projectal/entities/task_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1884 2023-11-16 00:19:41.000000 projectal-4.3.0/projectal/entities/user.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1672 2023-11-20 22:44:58.000000 projectal-4.3.0/projectal/entities/webhook.py
--rw-rw-r--   0 luked     (1003) luked     (1003)    41797 2024-02-06 06:33:02.000000 projectal-4.3.0/projectal/entity.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2585 2023-11-07 23:27:28.000000 projectal-4.3.0/projectal/enums.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3770 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/errors.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     9396 2024-02-21 23:29:15.000000 projectal-4.3.0/projectal/linkers.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2381 2023-10-18 05:03:25.000000 projectal-4.3.0/projectal/profile.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-02-21 23:56:37.944602 projectal-4.3.0/projectal.egg-info/
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2024-02-21 23:56:37.000000 projectal-4.3.0/projectal.egg-info/PKG-INFO
--rw-rw-r--   0 luked     (1003) luked     (1003)     3005 2024-02-21 23:56:37.000000 projectal-4.3.0/projectal.egg-info/SOURCES.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)        1 2024-02-21 23:56:37.000000 projectal-4.3.0/projectal.egg-info/dependency_links.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2024-02-21 23:56:37.000000 projectal-4.3.0/projectal.egg-info/requires.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2024-02-21 23:56:37.000000 projectal-4.3.0/projectal.egg-info/top_level.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       38 2024-02-21 23:56:37.948602 projectal-4.3.0/setup.cfg
--rw-rw-r--   0 luked     (1003) luked     (1003)      784 2024-02-21 23:40:38.000000 projectal-4.3.0/setup.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.413677 projectal-4.3.1/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.3.1/LICENSE
+-rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.3.1/MANIFEST.in
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2024-04-04 00:02:33.413677 projectal-4.3.1/PKG-INFO
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.401677 projectal-4.3.1/docs/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      140 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/index.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.405677 projectal-4.3.1/docs/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)   126818 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/api.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    50793 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enum.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.405677 projectal-4.3.1/docs/projectal/dynamic_enums/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38074 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/company_types.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38158 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/complexity_levels.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38068 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/currency_list.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38116 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/priority_levels.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38053 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/skill_levels.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    38032 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums/staff_types.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    37995 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/dynamic_enums.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.409677 projectal-4.3.1/docs/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    45618 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/access_policy.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    54635 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/activity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   118244 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/booking.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    77470 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/calendar.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    82761 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/company.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    61191 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/contact.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    48999 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/customer.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    74473 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/department.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   116609 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/file.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    80179 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/folder.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    69273 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/location.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    74972 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/note.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    52102 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/permission.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    78604 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/project.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    54248 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/project_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    47064 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/rebate.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    47337 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/resource.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46507 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/skill.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   147305 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/staff.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    45478 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/stage.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42962 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities/tag.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   299759 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/entities/task.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   103346 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/entities/task_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81531 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/entities/user.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    77623 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/entities/webhook.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    43317 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal/entities.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   680048 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/entity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   135037 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/enums.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   115062 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/errors.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   272729 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/linkers.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    58181 2024-04-04 00:00:57.000000 projectal-4.3.1/docs/projectal/profile.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   144576 2024-04-04 00:00:56.000000 projectal-4.3.1/docs/projectal.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.409677 projectal-4.3.1/examples/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3172 2023-10-18 05:03:25.000000 projectal-4.3.1/examples/linking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      830 2023-10-18 05:03:24.000000 projectal-4.3.1/examples/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1047 2023-10-18 05:03:24.000000 projectal-4.3.1/examples/webhook.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.409677 projectal-4.3.1/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    22244 2024-04-03 23:31:52.000000 projectal-4.3.1/projectal/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9272 2024-04-03 23:01:42.000000 projectal-4.3.1/projectal/api.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      663 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enum.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.409677 projectal-4.3.1/projectal/dynamic_enums/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      509 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      112 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/company_types.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      120 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/complexity_levels.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      109 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/currency_list.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      116 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/priority_levels.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      110 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/skill_levels.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      108 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/dynamic_enums/staff_types.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.413677 projectal-4.3.1/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.3.1/projectal/entities/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      396 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/access_policy.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      670 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/activity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4743 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/booking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2234 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/calendar.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2024 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/company.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      983 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/contact.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      477 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/customer.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1878 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/department.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3245 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/file.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1733 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/folder.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1326 2024-01-10 05:22:19.000000 projectal-4.3.1/projectal/entities/location.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1942 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/note.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      614 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/permission.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1657 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/project.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      711 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/project_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      420 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/rebate.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      426 2023-10-18 05:03:24.000000 projectal-4.3.1/projectal/entities/resource.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      396 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/skill.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4860 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/staff.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      345 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/stage.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      231 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/entities/tag.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)    17261 2024-02-21 23:29:15.000000 projectal-4.3.1/projectal/entities/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2676 2023-10-17 06:27:06.000000 projectal-4.3.1/projectal/entities/task_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1884 2023-11-16 00:19:41.000000 projectal-4.3.1/projectal/entities/user.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1672 2023-11-20 22:44:58.000000 projectal-4.3.1/projectal/entities/webhook.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)    41797 2024-02-06 06:33:02.000000 projectal-4.3.1/projectal/entity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2585 2023-11-07 23:27:28.000000 projectal-4.3.1/projectal/enums.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3770 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/errors.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9396 2024-02-21 23:29:15.000000 projectal-4.3.1/projectal/linkers.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2381 2023-10-18 05:03:25.000000 projectal-4.3.1/projectal/profile.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2024-04-04 00:02:33.409677 projectal-4.3.1/projectal.egg-info/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2024-04-04 00:02:33.000000 projectal-4.3.1/projectal.egg-info/PKG-INFO
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3005 2024-04-04 00:02:33.000000 projectal-4.3.1/projectal.egg-info/SOURCES.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)        1 2024-04-04 00:02:33.000000 projectal-4.3.1/projectal.egg-info/dependency_links.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2024-04-04 00:02:33.000000 projectal-4.3.1/projectal.egg-info/requires.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2024-04-04 00:02:33.000000 projectal-4.3.1/projectal.egg-info/top_level.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       38 2024-04-04 00:02:33.413677 projectal-4.3.1/setup.cfg
+-rw-rw-r--   0 luked     (1003) luked     (1003)      784 2024-04-03 23:36:34.000000 projectal-4.3.1/setup.py
```

### Comparing `projectal-4.3.0/LICENSE` & `projectal-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/PKG-INFO` & `projectal-4.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 4.3.0
+Version: 4.3.1
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-4.3.0/docs/projectal/api.html` & `projectal-4.3.1/docs/projectal/api.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enum.html` & `projectal-4.3.1/docs/projectal/dynamic_enum.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/company_types.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/company_types.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/complexity_levels.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/complexity_levels.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/currency_list.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/currency_list.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/priority_levels.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/priority_levels.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/skill_levels.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/skill_levels.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums/staff_types.html` & `projectal-4.3.1/docs/projectal/dynamic_enums/staff_types.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/dynamic_enums.html` & `projectal-4.3.1/docs/projectal/dynamic_enums.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/access_policy.html` & `projectal-4.3.1/docs/projectal/entities/access_policy.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/activity.html` & `projectal-4.3.1/docs/projectal/entities/activity.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/booking.html` & `projectal-4.3.1/docs/projectal/entities/booking.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/calendar.html` & `projectal-4.3.1/docs/projectal/entities/calendar.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/company.html` & `projectal-4.3.1/docs/projectal/entities/company.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/contact.html` & `projectal-4.3.1/docs/projectal/entities/contact.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/customer.html` & `projectal-4.3.1/docs/projectal/entities/customer.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/department.html` & `projectal-4.3.1/docs/projectal/entities/department.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/file.html` & `projectal-4.3.1/docs/projectal/entities/file.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/folder.html` & `projectal-4.3.1/docs/projectal/entities/folder.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/location.html` & `projectal-4.3.1/docs/projectal/entities/location.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/note.html` & `projectal-4.3.1/docs/projectal/entities/note.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/permission.html` & `projectal-4.3.1/docs/projectal/entities/permission.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/project.html` & `projectal-4.3.1/docs/projectal/entities/project.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/project_template.html` & `projectal-4.3.1/docs/projectal/entities/project_template.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/rebate.html` & `projectal-4.3.1/docs/projectal/entities/rebate.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/resource.html` & `projectal-4.3.1/docs/projectal/entities/resource.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/skill.html` & `projectal-4.3.1/docs/projectal/entities/skill.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/staff.html` & `projectal-4.3.1/docs/projectal/entities/staff.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/stage.html` & `projectal-4.3.1/docs/projectal/entities/stage.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/tag.html` & `projectal-4.3.1/docs/projectal/entities/tag.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/task.html` & `projectal-4.3.1/docs/projectal/entities/task.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/task_template.html` & `projectal-4.3.1/docs/projectal/entities/task_template.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/user.html` & `projectal-4.3.1/docs/projectal/entities/user.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities/webhook.html` & `projectal-4.3.1/docs/projectal/entities/webhook.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entities.html` & `projectal-4.3.1/docs/projectal/entities.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/entity.html` & `projectal-4.3.1/docs/projectal/entity.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/enums.html` & `projectal-4.3.1/docs/projectal/enums.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/errors.html` & `projectal-4.3.1/docs/projectal/errors.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/linkers.html` & `projectal-4.3.1/docs/projectal/linkers.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal/profile.html` & `projectal-4.3.1/docs/projectal/profile.html`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/docs/projectal.html` & `projectal-4.3.1/docs/projectal.html`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 <h2 id="getting-started">Getting started</h2>
 
 <pre><code>import projectal
 import os
 
 # Supply your Projectal server URL and account credentials
-<a href="#api_base">api_base</a> = https://yourcompany.projectal.com
+<a href="#api_base">api_base</a> = 'https://yourcompany.projectal.com'
 <a href="#api_username">api_username</a> = os.environ.get('PROJECTAL_USERNAME')
 <a href="#api_password">api_password</a> = os.environ.get('PROJECTAL_PASSWORD')
 
 # Test communication with server
 status = projectal.status()
 
 # Test account credentials
@@ -113,23 +113,30 @@
 details = projectal.auth_details()
 </code></pre>
 
 <hr />
 
 <h2 id="changelog">Changelog</h2>
 
+<h3 id="431">4.3.1</h3>
+
+<ul>
+<li>Fixed typo in "Getting started" example.</li>
+<li>Fixed typo in 4.3.0 Changelog.</li>
+</ul>
+
 <h3 id="430">4.3.0</h3>
 
 <p><strong>Breaking changes:</strong></p>
 
 <ul>
 <li>Added "PREDECESSOR_TASK" option when fetching projectal.Task with links</li>
 <li>Predecessor tasks will be returned as a list of tasks under the taskList attribute</li>
 <li>This attribute name is different to what you would see when using the REST API directly
-(planLink). This change was necessary to allow for directly manipulating
+(planList). This change was necessary to allow for directly manipulating
 the list of links and then saving the task entity to commit any changes,
 since the REST API is expecting a different key for linking calls (taskList).</li>
 <li>Existing Predecessor Task linking methods were also updated to match the new linking functionality.
 They now work as a reverse linker, automatically inverting the link relationship between
 the task entities. This more closely matches what you would expect to see based on the Web UI.
 I.e. When previously calling <code>some_task.link_predecessor_task(another_task)</code>,
 some_task would be set as a predecessor for another_task instead of the other way around.
@@ -511,15 +518,15 @@
 the library.</li>
 <li><code>Entity.changes()</code> has been extended with an <code>old=True</code> flag. When
 this flag is true, the set of changes will now return both the original
 and the new values. E.g.</li></p>
 
 </ul>
 
-md5-f7279c698f1b0d3b306e87f9e151e7a8
+md5-142fa72e3e0d57466b9f21c68dea103f
 
 
 <ul>
 
 <p><li>Fixed entity link cache causing errors when deleting a link from an entity
 which has not been fetched with links (deleting from empty list).</li></p>
 
@@ -583,15 +590,15 @@
   large request. Values are configurable through
   `<a href="#chunk_size_read">chunk_size_read</a>` and `<a href="#chunk_size_write">chunk_size_write</a>`.
   Default values: Read: 1000 items. Write: 200 items.
 - Added profile get/set functions on entities for easier use. Now you only need to supply
   the key and the data. E.g:
 
 
-md5-659103e2d1bcee22b7bd70e7c18d4bc5
+md5-abcb7a87fe05660543d3b72886774e4a
 
 
 
 <ul>
 <li><p>Entity link methods now automatically update the entity's cached list of links. E.g:
 a task fetched with staff links will have <code>task['staffList'] = [Staff1,Staff2]</code>.
 Before, doing a <code>task.link_staff(staff)</code> did not modify the list to reflect the
@@ -707,15 +714,15 @@
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="sd">## Getting started</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="sd">```</span>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="sd">import projectal</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="sd">import os</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>
 </span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="sd"># Supply your Projectal server URL and account credentials</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">projectal.api_base = https://yourcompany.projectal.com</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">projectal.api_base = &#39;https://yourcompany.projectal.com&#39;</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a><span class="sd">projectal.api_username = os.environ.get(&#39;PROJECTAL_USERNAME&#39;)</span>
 </span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="sd">projectal.api_password = os.environ.get(&#39;PROJECTAL_PASSWORD&#39;)</span>
 </span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
 </span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="sd"># Test communication with server</span>
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="sd">status = projectal.status()</span>
 </span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
 </span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="sd"># Test account credentials</span>
@@ -723,565 +730,569 @@
 </span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">details = projectal.auth_details()</span>
 </span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">```</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
 </span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">----</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">## Changelog</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 4.3.0</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">**Breaking changes:**</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 4.3.1</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">- Fixed typo in &quot;Getting started&quot; example.</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">- Fixed typo in 4.3.0 Changelog.</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">- Added &quot;PREDECESSOR_TASK&quot; option when fetching projectal.Task with links</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">- Predecessor tasks will be returned as a list of tasks under the taskList attribute</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">- This attribute name is different to what you would see when using the REST API directly</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">  (planLink). This change was necessary to allow for directly manipulating</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">  the list of links and then saving the task entity to commit any changes,</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">  since the REST API is expecting a different key for linking calls (taskList).</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">- Existing Predecessor Task linking methods were also updated to match the new linking functionality.</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">  They now work as a reverse linker, automatically inverting the link relationship between</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">  the task entities. This more closely matches what you would expect to see based on the Web UI.</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">  I.e. When previously calling `some_task.link_predecessor_task(another_task)`,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">  some_task would be set as a predecessor for another_task instead of the other way around.</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">  Now another_task would be set as the predecessor for some_task.</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">### 4.2.2</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">- `projectal.User.current_user_permissions()` fixed incorrect query.</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">- `projectal.Webhook.list()` default limit increased to 1000.</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="sd">### 4.3.0</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="sd">**Breaking changes:**</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">- Added &quot;PREDECESSOR_TASK&quot; option when fetching projectal.Task with links</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">- Predecessor tasks will be returned as a list of tasks under the taskList attribute</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">- This attribute name is different to what you would see when using the REST API directly</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">  (planList). This change was necessary to allow for directly manipulating</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">  the list of links and then saving the task entity to commit any changes,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">  since the REST API is expecting a different key for linking calls (taskList).</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">- Existing Predecessor Task linking methods were also updated to match the new linking functionality.</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">  They now work as a reverse linker, automatically inverting the link relationship between</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">  the task entities. This more closely matches what you would expect to see based on the Web UI.</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">  I.e. When previously calling `some_task.link_predecessor_task(another_task)`,</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">  some_task would be set as a predecessor for another_task instead of the other way around.</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">  Now another_task would be set as the predecessor for some_task.</span>
 </span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="sd">### 4.2.1</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">- Added classes allowing for the management of dynamic enums. The user must have the &quot;List Management&quot;</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">  permission to update enums.</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="sd">### 4.2.2</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">- `projectal.User.current_user_permissions()` fixed incorrect query.</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">- `projectal.Webhook.list()` default limit increased to 1000.</span>
 </span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">  New classes:</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">  - `projectal.CompanyTypes`</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">  - `projectal.SkillLevels`</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">  - `projectal.StaffTypes`</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">  - `projectal.PriorityLevels`</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">  - `projectal.ComplexityLevels`</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">  - `projectal.CurrencyList`</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">  The current enum can be retrieved with get(), and updated with set().</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">  For example, to return the current SkillLevels enum:</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">  ```</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">  projectal.SkillLevels.get()</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">  ```</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">### 4.2.1</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">- Added classes allowing for the management of dynamic enums. The user must have the &quot;List Management&quot;</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">  permission to update enums.</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">  New classes:</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">  - `projectal.CompanyTypes`</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">  - `projectal.SkillLevels`</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="sd">  - `projectal.StaffTypes`</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">  - `projectal.PriorityLevels`</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">  - `projectal.ComplexityLevels`</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">  - `projectal.CurrencyList`</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">  The current enum can be retrieved with get(), and updated with set().</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">  For example, to return the current SkillLevels enum:</span>
 </span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">  For each enum the entire list of key value pairs must be provided when calling set(),</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">  any existing values that are omitted from the dictionary will be removed,</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">  and any additional values will be added.</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">  ```</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">  projectal.SkillLevels.get()</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">  ```</span>
 </span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">  To update the SkillLevels enum with a new value:</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">  ```</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">  new_value_added = {</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">      &quot;Senior&quot;: 10,</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">      &quot;Junior&quot;: 30,</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">      # new SkillLevel value &quot;Beginner&quot;</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">      &quot;Beginner&quot;: 40,</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">  }</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">  projectal.SkillLevels.set(new_value_added)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">  ```</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">  To change the name of a value, set a new key name for the original value:</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">  For each enum the entire list of key value pairs must be provided when calling set(),</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">  any existing values that are omitted from the dictionary will be removed,</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">  and any additional values will be added.</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">  To update the SkillLevels enum with a new value:</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">  ```</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">  new_value_added = {</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">      &quot;Senior&quot;: 10,</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">      &quot;Junior&quot;: 30,</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">      # new SkillLevel value &quot;Beginner&quot;</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">      &quot;Beginner&quot;: 40,</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">  }</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">  projectal.SkillLevels.set(new_value_added)</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">  ```</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">  updated_value_name = {</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">      # changing &quot;Senior&quot; SkillLevel to &quot;Expert&quot;</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">      &quot;Expert&quot;: 10,</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">      &quot;Junior&quot;: 30,</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">  }</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">  projectal.SkillLevels.set(updated_value_name)</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">  ```</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">  To remove an existing value, call set on a dictionary with that value removed:</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">  To change the name of a value, set a new key name for the original value:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">  ```</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">  updated_value_name = {</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">      # changing &quot;Senior&quot; SkillLevel to &quot;Expert&quot;</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">      &quot;Expert&quot;: 10,</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">      &quot;Junior&quot;: 30,</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">  }</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">  projectal.SkillLevels.set(updated_value_name)</span>
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">  ```</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">  value_removed = {</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">      &quot;Senior&quot;: 10,</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">      # &quot;Junior&quot; SkillLevel removed</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">  }</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">  projectal.SkillLevels.set(new_value_added)</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="sd">  ```</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  Updating the CurrencyList works differently to the other enums, since the</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">  names of values must match the alphabetic currency code and the value must</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">  match the numeric currency code.</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">  This will cause an exception if you try to change the name for any values.</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">  Adding a new currency:</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">  ```</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">  new_currency_added = {</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">    &quot;AED&quot;: 784</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">    ...</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">    # rest of the existing currencies</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">    ...</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    # new currency to add with the alphabetic and numeric code</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    &quot;ZWL&quot;: 932,</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">  }</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">  projectal.CurrencyList.set(new_currency_added)</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">  ```</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">  Removing an existing currency requires you to provide the numeric code for</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">  the currency as a negative value.</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">  ```</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">  currency_removed = {</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    # this currency will be removed</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    &quot;AED&quot;: -784</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">    ...</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">    # rest of the existing currencies</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    ...</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">  }</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">  projectal.CurrencyList.set(currency_removed)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">  ```</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">### 4.2.0</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">Version 4.2.0 accompanies the release of Projectal 4.1.0</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">- Minimum Projectal version is now 4.1.0.</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">- Changed order of applying link types when an entity is initialized,</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">prevents a type error with reverse linking in certain situations.</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">- `projectal.Task.reset_duration()` now supports adjustments with multi day calendar exceptions.</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">- `projectal.Task.reset_duration()` location working days override base exceptions.</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">  To remove an existing value, call set on a dictionary with that value removed:</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">  ```</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">  value_removed = {</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">      &quot;Senior&quot;: 10,</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="sd">      &quot;Mid&quot;: 20,</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">      # &quot;Junior&quot; SkillLevel removed</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  }</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">  projectal.SkillLevels.set(new_value_added)</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">  ```</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">  Updating the CurrencyList works differently to the other enums, since the</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">  names of values must match the alphabetic currency code and the value must</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">  match the numeric currency code.</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">  This will cause an exception if you try to change the name for any values.</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">  Adding a new currency:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">  ```</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">  new_currency_added = {</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    &quot;AED&quot;: 784</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">    ...</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    # rest of the existing currencies</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">    ...</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    # new currency to add with the alphabetic and numeric code</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">    &quot;ZWL&quot;: 932,</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">  }</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">  projectal.CurrencyList.set(new_currency_added)</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">  ```</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">  Removing an existing currency requires you to provide the numeric code for</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">  the currency as a negative value.</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">  ```</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">  currency_removed = {</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    # this currency will be removed</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">    &quot;AED&quot;: -784</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">    ...</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">    # rest of the existing currencies</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    ...</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">  }</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">  projectal.CurrencyList.set(currency_removed)</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a><span class="sd">  ```</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">### 4.2.0</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">Version 4.2.0 accompanies the release of Projectal 4.1.0</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd">- Minimum Projectal version is now 4.1.0.</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="sd">- Changed order of applying link types when an entity is initialized,</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">prevents a type error with reverse linking in certain situations.</span>
 </span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">- `projectal.TaskTemplate.list()` fixed incorrect query when using inherited method.</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">- `projectal.Task.reset_duration()` now supports adjustments with multi day calendar exceptions.</span>
 </span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">### 4.1.0</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a><span class="sd">- DateLimit.Max enum value changed from &quot;9999-12-31&quot; to &quot;3000-01-01&quot;. This reflects changes to the Projectal</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">backend that defines this as the maximum allowable date value. The front end typically considers this value as</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">equivalent with having no end date.</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">- Updated requirements.txt version for requests package</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">- Minimum Projectal version is now 4.0.40</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">- `projectal.Task.reset_duration()` location working days override base exceptions.</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">- `projectal.TaskTemplate.list()` fixed incorrect query when using inherited method.</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">### 4.1.0</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">- DateLimit.Max enum value changed from &quot;9999-12-31&quot; to &quot;3000-01-01&quot;. This reflects changes to the Projectal</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">backend that defines this as the maximum allowable date value. The front end typically considers this value as</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">equivalent with having no end date.</span>
 </span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">### 4.0.3</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">- When a dict object is passed to the update class method, it will be converted to the corresponding Entity type.</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">  Allows for proper handling of keys that require being treated as links.</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">- Updated requirements.txt version for requests package</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">- Minimum Projectal version is now 4.0.40</span>
 </span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">### 4.0.2</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">- Booking entity is now fetched with project field and either staff or resource field.</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">- Added missing link methods for &#39;Booking&#39; entity (Note, File)</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">- Added missing link methods for &#39;Activity&#39; entity (Booking, Note, File, Rebate)</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">### 4.0.3</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">- When a dict object is passed to the update class method, it will be converted to the corresponding Entity type.</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">  Allows for proper handling of keys that require being treated as links.</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">### 4.0.2</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">- Booking entity is now fetched with project field and either staff or resource field.</span>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">- Reduced maximum number of link methods to 100 for a single batch request to prevent timeouts</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">under heavy load.</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">### 4.0.1</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">- Minimum Projectal version is now 4.0.0.</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">### 4.0.0</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">Version 4.0.0 accompanies the release of Projectal 4.0.</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">- Added missing link methods for &#39;Booking&#39; entity (Note, File)</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">- Added missing link methods for &#39;Activity&#39; entity (Booking, Note, File, Rebate)</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">- Reduced maximum number of link methods to 100 for a single batch request to prevent timeouts</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">under heavy load.</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">### 4.0.1</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">- Minimum Projectal version is now 4.0.0.</span>
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">- Added the `Activity` entity, new in Projectal 4.0.</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">### 4.0.0</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">- Added the `Booking` entity, new in Projectal 4.0.</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">Version 4.0.0 accompanies the release of Projectal 4.0.</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">### 3.1.1</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">### 3.1.0</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">  from a webhook delete event.</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">  the Projectal server settings.</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    ```</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">    resourceList: [</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">        &#39;added&#39;: [],</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">        &#39;updated&#39;: [</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        ],</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        &#39;removed&#39;: []</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">    ]</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">    ```</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">  clearly indicated.</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">### 3.0.2</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">### 3.0.1</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">### 3.0</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">- Added the `Activity` entity, new in Projectal 4.0.</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">- Added the `Booking` entity, new in Projectal 4.0.</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">### 3.1.1</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">### 3.1.0</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">  from a webhook delete event.</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">  the Projectal server settings.</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    ```</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">    resourceList: [</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        &#39;added&#39;: [],</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        &#39;updated&#39;: [</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        ],</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        &#39;removed&#39;: []</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">    ]</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">    ```</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">  clearly indicated.</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">### 3.0.2</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">### 3.0.1</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
 </span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
 </span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">### 3.0</span>
 </span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">    ```</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">    # Before:</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">    # Now:</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">    ```</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">    ```</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">    # Before:</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">    # Now:</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">    ```</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">**Other changes**:</span>
 </span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">  you can now do:</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">    ```</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">    task.save()</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">    ```</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">  capabilities and limitations.</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">    ```</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">    ```</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">  writing something like:</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">    ```</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">    company.link_staff(staff)</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">    ```</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">  strictly support it:</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">    ```</span>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">    staff.link_company(company)</span>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a><span class="sd">    ```</span>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a><span class="sd">  lists, None for dicts).</span>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>
-</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>
-</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">  you can now do:</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">    ```</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">    task.save()</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">    ```</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">  capabilities and limitations.</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">    ```</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="sd">    ```</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">  writing something like:</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">    ```</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">    staff.link_location(location)</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">    company.link_staff(staff)</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">    ```</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a><span class="sd">  strictly support it:</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">    ```</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">    staff.link_location(location)</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">    staff.link_company(company)</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a><span class="sd">    ```</span>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a><span class="sd">  lists, None for dicts).</span>
 </span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
 </span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">  of a uuId.</span>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">  Projectal 3.0.</span>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a><span class="sd">  returned Task object.</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
-</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a>
-</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">  changes for a webhook timestamp.</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">  of a uuId.</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a><span class="sd">  Projectal 3.0.</span>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a>
+</span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">  returned Task object.</span>
+</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
 </span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">**Known issues**:</span>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
-</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">  ```</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">  staff.save()</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a>
-</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a><span class="sd">  # You must do this for now</span>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">  calendar.save()</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">  ```</span>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">  This will be resolved in a future release.</span>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
-</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">  stored in the database.</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">  changes for a webhook timestamp.</span>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
+</span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">**Known issues**:</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">  ```</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
+</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">  staff.save()</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a><span class="sd">  # You must do this for now</span>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">  calendar.save()</span>
+</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">  ```</span>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">  This will be resolved in a future release.</span>
 </span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>
-</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
-</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">### 2.1.0</span>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
-</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
-</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
-</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">  Projectal several versions ago.</span>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
-</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="sd">### 2.0.3</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a><span class="sd">- Better support for calendars.</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
-</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="sd">  the library.</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="sd">  and the new values. E.g.</span>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="sd">```</span>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="sd">task.changes()</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="sd">task.changes(old=True)</span>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">```</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
-</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a>
-</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a><span class="sd">### 2.0.2</span>
-</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="sd">- Fixed updating Webhook entities</span>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="sd">### 2.0.1</span>
-</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
-</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>
-</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a><span class="sd">### 2.0.0</span>
-</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
-</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="sd">  since the previous release.</span>
-</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
-</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
-</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a><span class="sd">  server when an update request is made.</span>
-</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
-</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>
-</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a><span class="sd">### 1.2.0</span>
-</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>
-</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
+</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">  stored in the database.</span>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
+</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a>
+</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">### 2.1.0</span>
+</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">  Projectal several versions ago.</span>
+</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="sd">### 2.0.3</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="sd">- Better support for calendars.</span>
+</span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="sd">  the library.</span>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="sd">  and the new values. E.g.</span>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="sd">```</span>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">task.changes()</span>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
+</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="sd">task.changes(old=True)</span>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
+</span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a><span class="sd">```</span>
+</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="sd">### 2.0.2</span>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a><span class="sd">- Fixed updating Webhook entities</span>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a><span class="sd">### 2.0.1</span>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a><span class="sd">### 2.0.0</span>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a><span class="sd">  since the previous release.</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
+</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a><span class="sd">  server when an update request is made.</span>
+</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
 </span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a>
-</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
-</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
-</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
+</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a><span class="sd">### 1.2.0</span>
+</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a>
+</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a><span class="sd">**Breaking changes**:</span>
 </span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>
-</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
-</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
-</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a><span class="sd">  the database.</span>
+</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
+</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
+</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
 </span><span id="L-437"><a href="#L-437"><span class="linenos">437</span></a>
-</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
-</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
-</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a>
-</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
-</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
-</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
-</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
-</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a>
-</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
-</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
-</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a><span class="sd">  large request. Values are configurable through</span>
-</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
-</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
-</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a><span class="sd">  the key and the data. E.g:</span>
-</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>
-</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a><span class="sd">```</span>
-</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
-</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
-</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a><span class="sd">task.profile_set(key, data)</span>
+</span><span id="L-438"><a href="#L-438"><span class="linenos">438</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
+</span><span id="L-439"><a href="#L-439"><span class="linenos">439</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
+</span><span id="L-440"><a href="#L-440"><span class="linenos">440</span></a><span class="sd">  the database.</span>
+</span><span id="L-441"><a href="#L-441"><span class="linenos">441</span></a>
+</span><span id="L-442"><a href="#L-442"><span class="linenos">442</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
+</span><span id="L-443"><a href="#L-443"><span class="linenos">443</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
+</span><span id="L-444"><a href="#L-444"><span class="linenos">444</span></a>
+</span><span id="L-445"><a href="#L-445"><span class="linenos">445</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
+</span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
+</span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
+</span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
+</span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>
+</span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
+</span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a><span class="sd">  large request. Values are configurable through</span>
+</span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
+</span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
+</span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
+</span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a><span class="sd">  the key and the data. E.g:</span>
+</span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>
 </span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a><span class="sd">```</span>
-</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>
-</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
-</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
-</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
-</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
-</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a><span class="sd">  and delete.</span>
-</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a>
-</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
-</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
-</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a><span class="sd">  the object without requesting the link data as well</span>
-</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
-</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
-</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a><span class="sd">  while the object is held.</span>
-</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a>
-</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
-</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
-</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
-</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
-</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
-</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>
-</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
-</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
-</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
-</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
-</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">  server after creation.</span>
-</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>
-</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
-</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
-</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">  created objects without triggering this error.</span>
+</span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
+</span><span id="L-461"><a href="#L-461"><span class="linenos">461</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
+</span><span id="L-462"><a href="#L-462"><span class="linenos">462</span></a><span class="sd">task.profile_set(key, data)</span>
+</span><span id="L-463"><a href="#L-463"><span class="linenos">463</span></a><span class="sd">```</span>
+</span><span id="L-464"><a href="#L-464"><span class="linenos">464</span></a>
+</span><span id="L-465"><a href="#L-465"><span class="linenos">465</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
+</span><span id="L-466"><a href="#L-466"><span class="linenos">466</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
+</span><span id="L-467"><a href="#L-467"><span class="linenos">467</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
+</span><span id="L-468"><a href="#L-468"><span class="linenos">468</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
+</span><span id="L-469"><a href="#L-469"><span class="linenos">469</span></a><span class="sd">  and delete.</span>
+</span><span id="L-470"><a href="#L-470"><span class="linenos">470</span></a>
+</span><span id="L-471"><a href="#L-471"><span class="linenos">471</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
+</span><span id="L-472"><a href="#L-472"><span class="linenos">472</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
+</span><span id="L-473"><a href="#L-473"><span class="linenos">473</span></a><span class="sd">  the object without requesting the link data as well</span>
+</span><span id="L-474"><a href="#L-474"><span class="linenos">474</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
+</span><span id="L-475"><a href="#L-475"><span class="linenos">475</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
+</span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a><span class="sd">  while the object is held.</span>
+</span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>
+</span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
+</span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
+</span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
+</span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
+</span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
+</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>
+</span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
+</span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
+</span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
+</span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
+</span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a><span class="sd">  server after creation.</span>
 </span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>
-</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
-</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a>
-</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a>
-</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a><span class="sd">### 1.1.1</span>
-</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
-</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a><span class="sd">  any entity. Not currently documented.</span>
-</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
-</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
-</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
-</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
-</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
-</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a><span class="sd">  if no timestamp in response)</span>
-</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>
-</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="sd">### 1.1.0</span>
-</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
-</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>
-</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
-</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
-</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
-</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
-</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a><span class="sd">  down to only the tasks and fields you need.</span>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">  to match the server.</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
-</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>
-</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
-</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
-</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
-</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
-</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>
-</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a><span class="sd">### 1.0.3</span>
-</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
-</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>
-</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a><span class="sd">### 1.0.2</span>
-</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
-</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
-</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
-</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>
-</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a><span class="sd">### 1.0.1</span>
-</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a><span class="sd">- Added `list()` function for all entities</span>
-</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
-</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a><span class="sd">- Added `Company.get_master_company()`</span>
-</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a><span class="sd">- Fixed adding template tasks</span>
-</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a>
-</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a><span class="kn">import</span> <span class="nn">logging</span>
-</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
+</span><span id="L-491"><a href="#L-491"><span class="linenos">491</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
+</span><span id="L-492"><a href="#L-492"><span class="linenos">492</span></a><span class="sd">  created objects without triggering this error.</span>
+</span><span id="L-493"><a href="#L-493"><span class="linenos">493</span></a>
+</span><span id="L-494"><a href="#L-494"><span class="linenos">494</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
+</span><span id="L-495"><a href="#L-495"><span class="linenos">495</span></a>
+</span><span id="L-496"><a href="#L-496"><span class="linenos">496</span></a>
+</span><span id="L-497"><a href="#L-497"><span class="linenos">497</span></a><span class="sd">### 1.1.1</span>
+</span><span id="L-498"><a href="#L-498"><span class="linenos">498</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
+</span><span id="L-499"><a href="#L-499"><span class="linenos">499</span></a><span class="sd">  any entity. Not currently documented.</span>
+</span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
+</span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
+</span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
+</span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
+</span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
+</span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a><span class="sd">  if no timestamp in response)</span>
+</span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>
+</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a><span class="sd">### 1.1.0</span>
+</span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
+</span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>
+</span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
+</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a><span class="sd">  down to only the tasks and fields you need.</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a><span class="sd">  to match the server.</span>
+</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
+</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
+</span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>
+</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
+</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
+</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
+</span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
+</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
+</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
+</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
+</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
+</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
+</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>
+</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a><span class="sd">### 1.0.3</span>
+</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
+</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>
+</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a><span class="sd">### 1.0.2</span>
+</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
+</span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
+</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
+</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>
+</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a><span class="sd">### 1.0.1</span>
+</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a><span class="sd">- Added `list()` function for all entities</span>
+</span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
+</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a><span class="sd">- Added `Company.get_master_company()`</span>
+</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a><span class="sd">- Fixed adding template tasks</span>
 </span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>
-</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a><span class="kn">from</span> <span class="nn">projectal.dynamic_enums</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
-</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>
-</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_URL&quot;</span><span class="p">)</span>
-</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_USERNAME&quot;</span><span class="p">)</span>
-</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_PASSWORD&quot;</span><span class="p">)</span>
-</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
-</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
-</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>
-</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
-</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
-</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
-</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a>
-</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a>
-</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
-</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
-</span><span id="L-572"><a href="#L-572"><span class="linenos">572</span></a><span class="c1"># raise an exception.</span>
-</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4.0.40&quot;</span>
-</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a>
-</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a>
-</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;projectal-api-client&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
+</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a><span class="kn">import</span> <span class="nn">logging</span>
+</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>
+</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a><span class="kn">from</span> <span class="nn">projectal.dynamic_enums</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
+</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>
+</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_URL&quot;</span><span class="p">)</span>
+</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_USERNAME&quot;</span><span class="p">)</span>
+</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;PROJECTAL_PASSWORD&quot;</span><span class="p">)</span>
+</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
+</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
+</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a>
+</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
+</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
+</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
+</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-572"><a href="#L-572"><span class="linenos">572</span></a>
+</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a>
+</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
+</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
+</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a><span class="c1"># raise an exception.</span>
+</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4.0.40&quot;</span>
+</span><span id="L-578"><a href="#L-578"><span class="linenos">578</span></a>
+</span><span id="L-579"><a href="#L-579"><span class="linenos">579</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-580"><a href="#L-580"><span class="linenos">580</span></a>
+</span><span id="L-581"><a href="#L-581"><span class="linenos">581</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;projectal-api-client&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="api_base">
                     <div class="attr variable">
             <span class="name">api_base</span>        =
```

#### html2text {}

```diff
@@ -29,33 +29,36 @@
 ************ pprroojjeeccttaall ************
 A python client for the _P_r_o_j_e_c_t_a_l_ _A_P_I.
 ********** GGeettttiinngg ssttaarrtteedd **********
 import projectal
 import os
 
 # Supply your Projectal server URL and account credentials
-_a_p_i___b_a_s_e = https://yourcompany.projectal.com
+_a_p_i___b_a_s_e = 'https://yourcompany.projectal.com'
 _a_p_i___u_s_e_r_n_a_m_e = os.environ.get('PROJECTAL_USERNAME')
 _a_p_i___p_a_s_s_w_o_r_d = os.environ.get('PROJECTAL_PASSWORD')
 
 # Test communication with server
 status = projectal.status()
 
 # Test account credentials
 projectal.login()
 details = projectal.auth_details()
 ===============================================================================
 ********** CChhaannggeelloogg **********
+******** 44..33..11 ********
+    * Fixed typo in "Getting started" example.
+    * Fixed typo in 4.3.0 Changelog.
 ******** 44..33..00 ********
 BBrreeaakkiinngg cchhaannggeess::
     * Added "PREDECESSOR_TASK" option when fetching projectal.Task with links
     * Predecessor tasks will be returned as a list of tasks under the taskList
       attribute
     * This attribute name is different to what you would see when using the
-      REST API directly (planLink). This change was necessary to allow for
+      REST API directly (planList). This change was necessary to allow for
       directly manipulating the list of links and then saving the task entity
       to commit any changes, since the REST API is expecting a different key
       for linking calls (taskList).
     * Existing Predecessor Task linking methods were also updated to match the
       new linking functionality. They now work as a reverse linker,
       automatically inverting the link relationship between the task entities.
       This more closely matches what you would expect to see based on the Web
@@ -327,15 +330,15 @@
       items within them ("CalendarItem").
     * Allow CalendarItems to be saved directly. E.G item.save()
 Fix 'holder' parameter in contact/staff/location/task_template not permitting
 object type. Now consumes uuId or object to match rest of the library.
 Entity.changes() has been extended with an old=True flag. When this flag is
 true, the set of changes will now return both the original and the new values.
 E.g.
-md5-f7279c698f1b0d3b306e87f9e151e7a8
+md5-142fa72e3e0d57466b9f21c68dea103f
     * Fixed entity link cache causing errors when deleting a link from an
       entity which has not been fetched with links (deleting from empty list).
 ******** 22..00..22 ********
     * Fixed updating Webhook entities
 ******** 22..00..11 ********
     * Fixed application ID not being used correctly.
 ******** 22..00..00 ********
@@ -363,15 +366,15 @@
 (),projectal.timestamp_from_date(), and projectal.timestamp_from_datetime().
 **Other changes**: - Implement request chunking - for methods that consume a
 list of entities, we now automatically batch them up into multiple requests to
 prevent timeouts on really large request. Values are configurable through
 `_c_h_u_n_k___s_i_z_e___r_e_a_d` and `_c_h_u_n_k___s_i_z_e___w_r_i_t_e`. Default values: Read: 1000 items.
 Write: 200 items. - Added profile get/set functions on entities for easier use.
 Now you only need to supply the key and the data. E.g: md5-
-659103e2d1bcee22b7bd70e7c18d4bc5
+abcb7a87fe05660543d3b72886774e4a
     * Entity link methods now automatically update the entity's cached list of
       links. E.g: a task fetched with staff links will have task['staffList'] =
       [Staff1,Staff2]. Before, doing a task.link_staff(staff) did not modify
       the list to reflect the addition. Now, it will turn into
       [Staff1,Staff2,Staff3]. The same applies for update and delete.
       This allows you to modify links and continue working with that object
       without having to fetch it again to obtain the most recent link data. Be
@@ -452,15 +455,15 @@
 _ _ _4## Getting started
 _ _ _5
 _ _ _6```
 _ _ _7import projectal
 _ _ _8import os
 _ _ _9
 _ _1_0# Supply your Projectal server URL and account credentials
-_ _1_1projectal.api_base = https://yourcompany.projectal.com
+_ _1_1projectal.api_base = 'https://yourcompany.projectal.com'
 _ _1_2projectal.api_username = os.environ.get('PROJECTAL_USERNAME')
 _ _1_3projectal.api_password = os.environ.get('PROJECTAL_PASSWORD')
 _ _1_4
 _ _1_5# Test communication with server
 _ _1_6status = projectal.status()
 _ _1_7
 _ _1_8# Test account credentials
@@ -468,664 +471,668 @@
 _ _2_0details = projectal.auth_details()
 _ _2_1```
 _ _2_2
 _ _2_3----
 _ _2_4
 _ _2_5## Changelog
 _ _2_6
-_ _2_7### 4.3.0
-_ _2_8
-_ _2_9**Breaking changes:**
+_ _2_7### 4.3.1
+_ _2_8- Fixed typo in "Getting started" example.
+_ _2_9- Fixed typo in 4.3.0 Changelog.
 _ _3_0
-_ _3_1- Added "PREDECESSOR_TASK" option when fetching projectal.Task with links
-_ _3_2- Predecessor tasks will be returned as a list of tasks under the taskList
+_ _3_1### 4.3.0
+_ _3_2
+_ _3_3**Breaking changes:**
+_ _3_4
+_ _3_5- Added "PREDECESSOR_TASK" option when fetching projectal.Task with links
+_ _3_6- Predecessor tasks will be returned as a list of tasks under the taskList
 attribute
-_ _3_3- This attribute name is different to what you would see when using the REST
+_ _3_7- This attribute name is different to what you would see when using the REST
 API directly
-_ _3_4  (planLink). This change was necessary to allow for directly manipulating
-_ _3_5  the list of links and then saving the task entity to commit any changes,
-_ _3_6  since the REST API is expecting a different key for linking calls
+_ _3_8  (planList). This change was necessary to allow for directly manipulating
+_ _3_9  the list of links and then saving the task entity to commit any changes,
+_ _4_0  since the REST API is expecting a different key for linking calls
 (taskList).
-_ _3_7- Existing Predecessor Task linking methods were also updated to match the
+_ _4_1- Existing Predecessor Task linking methods were also updated to match the
 new linking functionality.
-_ _3_8  They now work as a reverse linker, automatically inverting the link
+_ _4_2  They now work as a reverse linker, automatically inverting the link
 relationship between
-_ _3_9  the task entities. This more closely matches what you would expect to see
+_ _4_3  the task entities. This more closely matches what you would expect to see
 based on the Web UI.
-_ _4_0  I.e. When previously calling `some_task.link_predecessor_task
+_ _4_4  I.e. When previously calling `some_task.link_predecessor_task
 (another_task)`,
-_ _4_1  some_task would be set as a predecessor for another_task instead of the
+_ _4_5  some_task would be set as a predecessor for another_task instead of the
 other way around.
-_ _4_2  Now another_task would be set as the predecessor for some_task.
-_ _4_3
-_ _4_4### 4.2.2
-_ _4_5- `projectal.User.current_user_permissions()` fixed incorrect query.
-_ _4_6- `projectal.Webhook.list()` default limit increased to 1000.
+_ _4_6  Now another_task would be set as the predecessor for some_task.
 _ _4_7
-_ _4_8### 4.2.1
-_ _4_9- Added classes allowing for the management of dynamic enums. The user must
-have the "List Management"
-_ _5_0  permission to update enums.
+_ _4_8### 4.2.2
+_ _4_9- `projectal.User.current_user_permissions()` fixed incorrect query.
+_ _5_0- `projectal.Webhook.list()` default limit increased to 1000.
 _ _5_1
-_ _5_2  New classes:
-_ _5_3  - `projectal.CompanyTypes`
-_ _5_4  - `projectal.SkillLevels`
-_ _5_5  - `projectal.StaffTypes`
-_ _5_6  - `projectal.PriorityLevels`
-_ _5_7  - `projectal.ComplexityLevels`
-_ _5_8  - `projectal.CurrencyList`
-_ _5_9
-_ _6_0  The current enum can be retrieved with get(), and updated with set().
-_ _6_1  For example, to return the current SkillLevels enum:
-_ _6_2
-_ _6_3  ```
-_ _6_4  projectal.SkillLevels.get()
-_ _6_5  ```
+_ _5_2### 4.2.1
+_ _5_3- Added classes allowing for the management of dynamic enums. The user must
+have the "List Management"
+_ _5_4  permission to update enums.
+_ _5_5
+_ _5_6  New classes:
+_ _5_7  - `projectal.CompanyTypes`
+_ _5_8  - `projectal.SkillLevels`
+_ _5_9  - `projectal.StaffTypes`
+_ _6_0  - `projectal.PriorityLevels`
+_ _6_1  - `projectal.ComplexityLevels`
+_ _6_2  - `projectal.CurrencyList`
+_ _6_3
+_ _6_4  The current enum can be retrieved with get(), and updated with set().
+_ _6_5  For example, to return the current SkillLevels enum:
 _ _6_6
-_ _6_7  For each enum the entire list of key value pairs must be provided when
-calling set(),
-_ _6_8  any existing values that are omitted from the dictionary will be removed,
-_ _6_9  and any additional values will be added.
+_ _6_7  ```
+_ _6_8  projectal.SkillLevels.get()
+_ _6_9  ```
 _ _7_0
-_ _7_1  To update the SkillLevels enum with a new value:
-_ _7_2
-_ _7_3  ```
-_ _7_4  new_value_added = {
-_ _7_5      "Senior": 10,
-_ _7_6      "Mid": 20,
-_ _7_7      "Junior": 30,
-_ _7_8      # new SkillLevel value "Beginner"
-_ _7_9      "Beginner": 40,
-_ _8_0  }
-_ _8_1  projectal.SkillLevels.set(new_value_added)
-_ _8_2  ```
-_ _8_3
-_ _8_4  To change the name of a value, set a new key name for the original value:
-_ _8_5
+_ _7_1  For each enum the entire list of key value pairs must be provided when
+calling set(),
+_ _7_2  any existing values that are omitted from the dictionary will be removed,
+_ _7_3  and any additional values will be added.
+_ _7_4
+_ _7_5  To update the SkillLevels enum with a new value:
+_ _7_6
+_ _7_7  ```
+_ _7_8  new_value_added = {
+_ _7_9      "Senior": 10,
+_ _8_0      "Mid": 20,
+_ _8_1      "Junior": 30,
+_ _8_2      # new SkillLevel value "Beginner"
+_ _8_3      "Beginner": 40,
+_ _8_4  }
+_ _8_5  projectal.SkillLevels.set(new_value_added)
 _ _8_6  ```
-_ _8_7  updated_value_name = {
-_ _8_8      # changing "Senior" SkillLevel to "Expert"
-_ _8_9      "Expert": 10,
-_ _9_0      "Mid": 20,
-_ _9_1      "Junior": 30,
-_ _9_2  }
-_ _9_3  projectal.SkillLevels.set(updated_value_name)
-_ _9_4  ```
-_ _9_5
-_ _9_6  To remove an existing value, call set on a dictionary with that value
-removed:
-_ _9_7
+_ _8_7
+_ _8_8  To change the name of a value, set a new key name for the original value:
+_ _8_9
+_ _9_0  ```
+_ _9_1  updated_value_name = {
+_ _9_2      # changing "Senior" SkillLevel to "Expert"
+_ _9_3      "Expert": 10,
+_ _9_4      "Mid": 20,
+_ _9_5      "Junior": 30,
+_ _9_6  }
+_ _9_7  projectal.SkillLevels.set(updated_value_name)
 _ _9_8  ```
-_ _9_9  value_removed = {
-_1_0_0      "Senior": 10,
-_1_0_1      "Mid": 20,
-_1_0_2      # "Junior" SkillLevel removed
-_1_0_3  }
-_1_0_4  projectal.SkillLevels.set(new_value_added)
-_1_0_5  ```
-_1_0_6
-_1_0_7  Updating the CurrencyList works differently to the other enums, since the
-_1_0_8  names of values must match the alphabetic currency code and the value must
-_1_0_9  match the numeric currency code.
-_1_1_0  This will cause an exception if you try to change the name for any values.
-_1_1_1
-_1_1_2  Adding a new currency:
-_1_1_3
-_1_1_4  ```
-_1_1_5  new_currency_added = {
-_1_1_6    "AED": 784
-_1_1_7    ...
-_1_1_8    # rest of the existing currencies
-_1_1_9    ...
-_1_2_0    # new currency to add with the alphabetic and numeric code
-_1_2_1    "ZWL": 932,
-_1_2_2  }
-_1_2_3  projectal.CurrencyList.set(new_currency_added)
-_1_2_4  ```
-_1_2_5
-_1_2_6  Removing an existing currency requires you to provide the numeric code for
-_1_2_7  the currency as a negative value.
-_1_2_8
-_1_2_9  ```
-_1_3_0  currency_removed = {
-_1_3_1    # this currency will be removed
-_1_3_2    "AED": -784
-_1_3_3    ...
-_1_3_4    # rest of the existing currencies
-_1_3_5    ...
-_1_3_6  }
-_1_3_7  projectal.CurrencyList.set(currency_removed)
-_1_3_8  ```
-_1_3_9
-_1_4_0### 4.2.0
-_1_4_1Version 4.2.0 accompanies the release of Projectal 4.1.0
-_1_4_2
-_1_4_3- Minimum Projectal version is now 4.1.0.
-_1_4_4
-_1_4_5- Changed order of applying link types when an entity is initialized,
-_1_4_6prevents a type error with reverse linking in certain situations.
-_1_4_7
-_1_4_8- `projectal.Task.reset_duration()` now supports adjustments with multi day
+_ _9_9
+_1_0_0  To remove an existing value, call set on a dictionary with that value
+removed:
+_1_0_1
+_1_0_2  ```
+_1_0_3  value_removed = {
+_1_0_4      "Senior": 10,
+_1_0_5      "Mid": 20,
+_1_0_6      # "Junior" SkillLevel removed
+_1_0_7  }
+_1_0_8  projectal.SkillLevels.set(new_value_added)
+_1_0_9  ```
+_1_1_0
+_1_1_1  Updating the CurrencyList works differently to the other enums, since the
+_1_1_2  names of values must match the alphabetic currency code and the value must
+_1_1_3  match the numeric currency code.
+_1_1_4  This will cause an exception if you try to change the name for any values.
+_1_1_5
+_1_1_6  Adding a new currency:
+_1_1_7
+_1_1_8  ```
+_1_1_9  new_currency_added = {
+_1_2_0    "AED": 784
+_1_2_1    ...
+_1_2_2    # rest of the existing currencies
+_1_2_3    ...
+_1_2_4    # new currency to add with the alphabetic and numeric code
+_1_2_5    "ZWL": 932,
+_1_2_6  }
+_1_2_7  projectal.CurrencyList.set(new_currency_added)
+_1_2_8  ```
+_1_2_9
+_1_3_0  Removing an existing currency requires you to provide the numeric code for
+_1_3_1  the currency as a negative value.
+_1_3_2
+_1_3_3  ```
+_1_3_4  currency_removed = {
+_1_3_5    # this currency will be removed
+_1_3_6    "AED": -784
+_1_3_7    ...
+_1_3_8    # rest of the existing currencies
+_1_3_9    ...
+_1_4_0  }
+_1_4_1  projectal.CurrencyList.set(currency_removed)
+_1_4_2  ```
+_1_4_3
+_1_4_4### 4.2.0
+_1_4_5Version 4.2.0 accompanies the release of Projectal 4.1.0
+_1_4_6
+_1_4_7- Minimum Projectal version is now 4.1.0.
+_1_4_8
+_1_4_9- Changed order of applying link types when an entity is initialized,
+_1_5_0prevents a type error with reverse linking in certain situations.
+_1_5_1
+_1_5_2- `projectal.Task.reset_duration()` now supports adjustments with multi day
 calendar exceptions.
-_1_4_9
-_1_5_0- `projectal.Task.reset_duration()` location working days override base
+_1_5_3
+_1_5_4- `projectal.Task.reset_duration()` location working days override base
 exceptions.
-_1_5_1
-_1_5_2- `projectal.TaskTemplate.list()` fixed incorrect query when using inherited
+_1_5_5
+_1_5_6- `projectal.TaskTemplate.list()` fixed incorrect query when using inherited
 method.
-_1_5_3
-_1_5_4### 4.1.0
-_1_5_5- DateLimit.Max enum value changed from "9999-12-31" to "3000-01-01". This
+_1_5_7
+_1_5_8### 4.1.0
+_1_5_9- DateLimit.Max enum value changed from "9999-12-31" to "3000-01-01". This
 reflects changes to the Projectal
-_1_5_6backend that defines this as the maximum allowable date value. The front end
+_1_6_0backend that defines this as the maximum allowable date value. The front end
 typically considers this value as
-_1_5_7equivalent with having no end date.
-_1_5_8
-_1_5_9- Updated requirements.txt version for requests package
-_1_6_0
-_1_6_1- Minimum Projectal version is now 4.0.40
+_1_6_1equivalent with having no end date.
 _1_6_2
-_1_6_3### 4.0.3
-_1_6_4- When a dict object is passed to the update class method, it will be
-converted to the corresponding Entity type.
-_1_6_5  Allows for proper handling of keys that require being treated as links.
+_1_6_3- Updated requirements.txt version for requests package
+_1_6_4
+_1_6_5- Minimum Projectal version is now 4.0.40
 _1_6_6
-_1_6_7### 4.0.2
-_1_6_8- Booking entity is now fetched with project field and either staff or
+_1_6_7### 4.0.3
+_1_6_8- When a dict object is passed to the update class method, it will be
+converted to the corresponding Entity type.
+_1_6_9  Allows for proper handling of keys that require being treated as links.
+_1_7_0
+_1_7_1### 4.0.2
+_1_7_2- Booking entity is now fetched with project field and either staff or
 resource field.
-_1_6_9
-_1_7_0- Added missing link methods for 'Booking' entity (Note, File)
-_1_7_1
-_1_7_2- Added missing link methods for 'Activity' entity (Booking, Note, File,
-Rebate)
 _1_7_3
-_1_7_4- Reduced maximum number of link methods to 100 for a single batch request
+_1_7_4- Added missing link methods for 'Booking' entity (Note, File)
+_1_7_5
+_1_7_6- Added missing link methods for 'Activity' entity (Booking, Note, File,
+Rebate)
+_1_7_7
+_1_7_8- Reduced maximum number of link methods to 100 for a single batch request
 to prevent timeouts
-_1_7_5under heavy load.
-_1_7_6
-_1_7_7### 4.0.1
-_1_7_8- Minimum Projectal version is now 4.0.0.
-_1_7_9
-_1_8_0### 4.0.0
-_1_8_1
-_1_8_2Version 4.0.0 accompanies the release of Projectal 4.0.
+_1_7_9under heavy load.
+_1_8_0
+_1_8_1### 4.0.1
+_1_8_2- Minimum Projectal version is now 4.0.0.
 _1_8_3
-_1_8_4- Added the `Activity` entity, new in Projectal 4.0.
+_1_8_4### 4.0.0
 _1_8_5
-_1_8_6- Added the `Booking` entity, new in Projectal 4.0.
+_1_8_6Version 4.0.0 accompanies the release of Projectal 4.0.
 _1_8_7
-_1_8_8### 3.1.1
-_1_8_9- Link requests generated by 'projectal.Entity.create()' and
+_1_8_8- Added the `Activity` entity, new in Projectal 4.0.
+_1_8_9
+_1_9_0- Added the `Booking` entity, new in Projectal 4.0.
+_1_9_1
+_1_9_2### 3.1.1
+_1_9_3- Link requests generated by 'projectal.Entity.create()' and
 'projectal.Entity.update()' are now
-_1_9_0  executed in batches. This is enabled by default with the
+_1_9_4  executed in batches. This is enabled by default with the
 'batch_linking=True' parameter and can
-_1_9_1  be disabled to execute each link request individually. It is recommended
+_1_9_5  be disabled to execute each link request individually. It is recommended
 to leave this parameter
-_1_9_2  enabled as this can greatly reduce the number of network requests.
-_1_9_3
-_1_9_4### 3.1.0
-_1_9_5- Minimum Projectal version is now 3.1.5.
-_1_9_6
-_1_9_7- Added `projectal.Webhook.list_events()`. See API doc for details on how to
+_1_9_6  enabled as this can greatly reduce the number of network requests.
+_1_9_7
+_1_9_8### 3.1.0
+_1_9_9- Minimum Projectal version is now 3.1.5.
+_2_0_0
+_2_0_1- Added `projectal.Webhook.list_events()`. See API doc for details on how to
 use.
-_1_9_8
-_1_9_9- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
+_2_0_2
+_2_0_3- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
 should be a UTC timestamp
-_2_0_0  from a webhook delete event.
-_2_0_1
-_2_0_2- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
+_2_0_4  from a webhook delete event.
+_2_0_5
+_2_0_6- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
 service configured in
-_2_0_3  the Projectal server settings.
-_2_0_4
-_2_0_5- Enhanced output of `projectal.Entity.changes()` function when reporting
+_2_0_7  the Projectal server settings.
+_2_0_8
+_2_0_9- Enhanced output of `projectal.Entity.changes()` function when reporting
 link changes.
-_2_0_6  It no longer dumps the entire before-and-after list with the full content
+_2_1_0  It no longer dumps the entire before-and-after list with the full content
 of each linked entity.
-_2_0_7  Now reports three lists: `added`, `updated`, `removed`. Entities within
+_2_1_1  Now reports three lists: `added`, `updated`, `removed`. Entities within
 the `updated` list
-_2_0_8  follow the same `old` vs `new` dictionary model for the data attributes
+_2_1_2  follow the same `old` vs `new` dictionary model for the data attributes
 within them. E.g:
-_2_0_9
-_2_1_0    ```
-_2_1_1    resourceList: [
-_2_1_2        'added': [],
-_2_1_3        'updated': [
-_2_1_4            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
+_2_1_3
+_2_1_4    ```
+_2_1_5    resourceList: [
+_2_1_6        'added': [],
+_2_1_7        'updated': [
+_2_1_8            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
 {'utilization': {'old': 0.1, 'new': 0.9}}},
-_2_1_5        ],
-_2_1_6        'removed': []
-_2_1_7    ]
-_2_1_8    ```
-_2_1_9  This should result in slimmer logs that are much easier to understand as
+_2_1_9        ],
+_2_2_0        'removed': []
+_2_2_1    ]
+_2_2_2    ```
+_2_2_3  This should result in slimmer logs that are much easier to understand as
 the changes are
-_2_2_0  clearly indicated.
-_2_2_1
-_2_2_2### 3.0.2
-_2_2_3- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
+_2_2_4  clearly indicated.
+_2_2_5
+_2_2_6### 3.0.2
+_2_2_7- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
 definition dictionary.
-_2_2_4  Consumers can inspect which links an Entity knows about and their internal
+_2_2_8  Consumers can inspect which links an Entity knows about and their internal
 settings.
-_2_2_5  Link definitions that appear here are the links valid for `links=[]`
+_2_2_9  Link definitions that appear here are the links valid for `links=[]`
 parameters.
-_2_2_6
-_2_2_7### 3.0.1
-_2_2_8- Fixed fetching project with links=['task'] not being available.
-_2_2_9
-_2_3_0- Improved Permission.list(). Now returns a dict with the permission name as
-_2_3_1  key with Permission objects as the value (instead of list of uuIds).
-_2_3_2
-_2_3_3- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
-_2_3_4Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
-_2_3_5requests made will be done as that user. Restore this value to None to
+_2_3_0
+_2_3_1### 3.0.1
+_2_3_2- Fixed fetching project with links=['task'] not being available.
+_2_3_3
+_2_3_4- Improved Permission.list(). Now returns a dict with the permission name as
+_2_3_5  key with Permission objects as the value (instead of list of uuIds).
+_2_3_6
+_2_3_7- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
+_2_3_8Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
+_2_3_9requests made will be done as that user. Restore this value to None to
 resume
-_2_3_6normal operation. (Some rules and limitations apply. See API for more
+_2_4_0normal operation. (Some rules and limitations apply. See API for more
 details.)
-_2_3_7
-_2_3_8- Added complete support for the Tags entity (including linkers).
-_2_3_9
-_2_4_0### 3.0
 _2_4_1
-_2_4_2Version 3.0 accompanies the release of Projectal 3.0.
+_2_4_2- Added complete support for the Tags entity (including linkers).
 _2_4_3
-_2_4_4**Breaking changes**:
+_2_4_4### 3.0
 _2_4_5
-_2_4_6- The `links` parameter on `Entity` functions now consumes a list of entity
-_2_4_7  names instead of a comma-separated string. For example:
-_2_4_8
-_2_4_9    ```
-_2_5_0    # Before:
-_2_5_1    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
-_2_5_2    # Now:
-_2_5_3    projectal.Staff.get('<uuid>', links=['skill', 'location'])
-_2_5_4    ```
-_2_5_5
-_2_5_6- The `projectal.enums.SkillLevel` enum has had all values renamed to match
+_2_4_6Version 3.0 accompanies the release of Projectal 3.0.
+_2_4_7
+_2_4_8**Breaking changes**:
+_2_4_9
+_2_5_0- The `links` parameter on `Entity` functions now consumes a list of entity
+_2_5_1  names instead of a comma-separated string. For example:
+_2_5_2
+_2_5_3    ```
+_2_5_4    # Before:
+_2_5_5    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
+_2_5_6    # Now:
+_2_5_7    projectal.Staff.get('<uuid>', links=['skill', 'location'])
+_2_5_8    ```
+_2_5_9
+_2_6_0- The `projectal.enums.SkillLevel` enum has had all values renamed to match
 the new values
-_2_5_7  used in Projectal (Junior, Mid, Senior). This includes the properties on
-_2_5_8  Skill entities indicating work time for auto-scheduling (now
+_2_6_1  used in Projectal (Junior, Mid, Senior). This includes the properties on
+_2_6_2  Skill entities indicating work time for auto-scheduling (now
 `juniorLevel`,
-_2_5_9  `midLevel`, `seniorLevel`).
-_2_6_0
-_2_6_1**Other changes**:
-_2_6_2
-_2_6_3- Working with entity links has changed in this release. The previous
-methods
-_2_6_4  are still available and continue to work as before, but there is no need
-_2_6_5  to interact with the `projectal.linkers` methods yourself anymore.
+_2_6_3  `midLevel`, `seniorLevel`).
+_2_6_4
+_2_6_5**Other changes**:
 _2_6_6
-_2_6_7  You can now modify the list of links within an entity and save the entity
-_2_6_8  directly. The library will automatically determine how the links have been
-_2_6_9  modified and issue the correct linker methods on your behalf. E.g.,
-_2_7_0  you can now do:
-_2_7_1
-_2_7_2    ```
-_2_7_3    staff = projectal.Staff.get('<uuid>', links=['skill'])
-_2_7_4    staff['firstName'] = "New name"  # Field update
-_2_7_5    staff['skillList'] = [skill1, skill2, skill3]  # Link update
-_2_7_6    staff.save()  # Both changes are saved
-_2_7_7
-_2_7_8    task = projectal.Task.get('<uuid>', links=['stage'])
-_2_7_9    task['stage'] = stage1  # Uses a single object instead of list
-_2_8_0    task.save()
-_2_8_1    ```
-_2_8_2
-_2_8_3  See `examples/linking.py` for a more complete demonstration of linking
-_2_8_4  capabilities and limitations.
-_2_8_5
-_2_8_6- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
-_2_8_7 type) to link/unlink/relink in bulk. E.g:
-_2_8_8    ```
-_2_8_9    staff.unlink_skill(skill1)  # Before
-_2_9_0    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
-_2_9_1    ```
-_2_9_2
-_2_9_3- Linkers now strip the payload to only the required fields instead of
+_2_6_7- Working with entity links has changed in this release. The previous
+methods
+_2_6_8  are still available and continue to work as before, but there is no need
+_2_6_9  to interact with the `projectal.linkers` methods yourself anymore.
+_2_7_0
+_2_7_1  You can now modify the list of links within an entity and save the entity
+_2_7_2  directly. The library will automatically determine how the links have been
+_2_7_3  modified and issue the correct linker methods on your behalf. E.g.,
+_2_7_4  you can now do:
+_2_7_5
+_2_7_6    ```
+_2_7_7    staff = projectal.Staff.get('<uuid>', links=['skill'])
+_2_7_8    staff['firstName'] = "New name"  # Field update
+_2_7_9    staff['skillList'] = [skill1, skill2, skill3]  # Link update
+_2_8_0    staff.save()  # Both changes are saved
+_2_8_1
+_2_8_2    task = projectal.Task.get('<uuid>', links=['stage'])
+_2_8_3    task['stage'] = stage1  # Uses a single object instead of list
+_2_8_4    task.save()
+_2_8_5    ```
+_2_8_6
+_2_8_7  See `examples/linking.py` for a more complete demonstration of linking
+_2_8_8  capabilities and limitations.
+_2_8_9
+_2_9_0- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
+_2_9_1 type) to link/unlink/relink in bulk. E.g:
+_2_9_2    ```
+_2_9_3    staff.unlink_skill(skill1)  # Before
+_2_9_4    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
+_2_9_5    ```
+_2_9_6
+_2_9_7- Linkers now strip the payload to only the required fields instead of
 passing
-_2_9_4  on the entire Entity object. This cuts down on network traffic
+_2_9_8  on the entire Entity object. This cuts down on network traffic
 significantly.
-_2_9_5
-_2_9_6- Linkers now also work in reverse. The Projectal server currently only
+_2_9_9
+_3_0_0- Linkers now also work in reverse. The Projectal server currently only
 supports
-_2_9_7  linking entities in one direction (e.g., Company to Staff), which often
+_3_0_1  linking entities in one direction (e.g., Company to Staff), which often
 means
-_2_9_8  writing something like:
-_2_9_9    ```
-_3_0_0    staff.link_location(location)
-_3_0_1    company.link_staff(staff)
-_3_0_2    ```
-_3_0_3  The change in direction is not very intuitive and would require you to
+_3_0_2  writing something like:
+_3_0_3    ```
+_3_0_4    staff.link_location(location)
+_3_0_5    company.link_staff(staff)
+_3_0_6    ```
+_3_0_7  The change in direction is not very intuitive and would require you to
 constantly
-_3_0_4  verify which direction is the one available to you in the documentation.
-_3_0_5
-_3_0_6  Reverse linkers hide this from you and figure out the direction of the
+_3_0_8  verify which direction is the one available to you in the documentation.
+_3_0_9
+_3_1_0  Reverse linkers hide this from you and figure out the direction of the
 relationship
-_3_0_7  for you behind the scenes. So now this is possible, even though the API
+_3_1_1  for you behind the scenes. So now this is possible, even though the API
 doesn't
-_3_0_8  strictly support it:
-_3_0_9    ```
-_3_1_0    staff.link_location(location)
-_3_1_1    staff.link_company(company)
-_3_1_2    ```
-_3_1_3    Caveat: the documentation for Staff will not list Company links. You
+_3_1_2  strictly support it:
+_3_1_3    ```
+_3_1_4    staff.link_location(location)
+_3_1_5    staff.link_company(company)
+_3_1_6    ```
+_3_1_7    Caveat: the documentation for Staff will not list Company links. You
 will still
-_3_1_4    have to look up the Company documentation for the link description.
-_3_1_5
-_3_1_6- Requesting entity links with the `links=` parameter will now always ensure
+_3_1_8    have to look up the Company documentation for the link description.
+_3_1_9
+_3_2_0- Requesting entity links with the `links=` parameter will now always ensure
 the
-_3_1_7  link field (e.g., `taskList`) exists in the result, even if there are no
+_3_2_1  link field (e.g., `taskList`) exists in the result, even if there are no
 links.
-_3_1_8  The server may not always return a value, but we can use a default value (
+_3_2_2  The server may not always return a value, but we can use a default value (
 [] for
-_3_1_9  lists, None for dicts).
-_3_2_0
-_3_2_1- Added a `Permission` entity to correctly type Permissions in responses.
-_3_2_2
-_3_2_3- Added a `Tag` entity, new in Projectal 3.0.
+_3_2_3  lists, None for dicts).
 _3_2_4
-_3_2_5- Added `links` parameter to `Company.get_primary_company()`
+_3_2_5- Added a `Permission` entity to correctly type Permissions in responses.
 _3_2_6
-_3_2_7- `Department.tree()`: now consumes a `holder` Entity object instead
-_3_2_8  of a uuId.
-_3_2_9
-_3_3_0- `Department.tree()`: added `generic_staff` parameter, new in
-_3_3_1  Projectal 3.0.
-_3_3_2
-_3_3_3- Don't break on trailing slash in Projectal URL
-_3_3_4
-_3_3_5- When creating tasks, populate the `projectRef` and `parent` fields in the
-_3_3_6  returned Task object.
-_3_3_7
-_3_3_8- Added convenience functions for matching on fields where you only want
-_3_3_9  one result (e.g match_one()) which return the first match found.
-_3_4_0
-_3_4_1- Update the entity `history()` method for Projectal 3.0. Some new
-parameters
-_3_4_2  allow you to restrict the history to a particular range or to get only the
-_3_4_3  changes for a webhook timestamp.
+_3_2_7- Added a `Tag` entity, new in Projectal 3.0.
+_3_2_8
+_3_2_9- Added `links` parameter to `Company.get_primary_company()`
+_3_3_0
+_3_3_1- `Department.tree()`: now consumes a `holder` Entity object instead
+_3_3_2  of a uuId.
+_3_3_3
+_3_3_4- `Department.tree()`: added `generic_staff` parameter, new in
+_3_3_5  Projectal 3.0.
+_3_3_6
+_3_3_7- Don't break on trailing slash in Projectal URL
+_3_3_8
+_3_3_9- When creating tasks, populate the `projectRef` and `parent` fields in the
+_3_4_0  returned Task object.
+_3_4_1
+_3_4_2- Added convenience functions for matching on fields where you only want
+_3_4_3  one result (e.g match_one()) which return the first match found.
 _3_4_4
-_3_4_5- Entity objects can call `.history()` on themselves.
-_3_4_6
-_3_4_7- The library now keeps a reference to the User account that is currently
+_3_4_5- Update the entity `history()` method for Projectal 3.0. Some new
+parameters
+_3_4_6  allow you to restrict the history to a particular range or to get only the
+_3_4_7  changes for a webhook timestamp.
+_3_4_8
+_3_4_9- Entity objects can call `.history()` on themselves.
+_3_5_0
+_3_5_1- The library now keeps a reference to the User account that is currently
 logged
-_3_4_8  in and using the API: `projectal.api_auth_details`.
-_3_4_9
-_3_5_0**Known issues**:
-_3_5_1- You cannot save changes to Notes or Calendars via their holding entity.
+_3_5_2  in and using the API: `projectal.api_auth_details`.
+_3_5_3
+_3_5_4**Known issues**:
+_3_5_5- You cannot save changes to Notes or Calendars via their holding entity.
 You
-_3_5_2  must save the changes on the Note or Calendar directly. To illustrate:
-_3_5_3  ```
-_3_5_4  staff = projectal.Staff.get(<uuid>, links=['calendar'])
-_3_5_5  calendar = staff['calendarList'][0]
-_3_5_6  calendar['name'] = 'Calendar 2'
-_3_5_7
-_3_5_8  # Cannot do this - will not pick up the changes
-_3_5_9  staff.save()
-_3_6_0
-_3_6_1  # You must do this for now
-_3_6_2  calendar.save()
-_3_6_3  ```
-_3_6_4  This will be resolved in a future release.
-_3_6_5
-_3_6_6- When creating Notes, the `created` and `modified` values may differ by
-_3_6_7  1ms in the object you have a reference to compared to what is actually
-_3_6_8  stored in the database.
+_3_5_6  must save the changes on the Note or Calendar directly. To illustrate:
+_3_5_7  ```
+_3_5_8  staff = projectal.Staff.get(<uuid>, links=['calendar'])
+_3_5_9  calendar = staff['calendarList'][0]
+_3_6_0  calendar['name'] = 'Calendar 2'
+_3_6_1
+_3_6_2  # Cannot do this - will not pick up the changes
+_3_6_3  staff.save()
+_3_6_4
+_3_6_5  # You must do this for now
+_3_6_6  calendar.save()
+_3_6_7  ```
+_3_6_8  This will be resolved in a future release.
 _3_6_9
-_3_7_0- Duration calculation is not precise yet (mentioned in 2.1.0)
-_3_7_1
-_3_7_2### 2.1.0
-_3_7_3**Breaking changes**:
-_3_7_4- Getting location calendar is now done on an instance instead of class. So
-_3_7_5  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
-_3_7_6- The `CompanyType.Master` enum has been replaced with
+_3_7_0- When creating Notes, the `created` and `modified` values may differ by
+_3_7_1  1ms in the object you have a reference to compared to what is actually
+_3_7_2  stored in the database.
+_3_7_3
+_3_7_4- Duration calculation is not precise yet (mentioned in 2.1.0)
+_3_7_5
+_3_7_6### 2.1.0
+_3_7_7**Breaking changes**:
+_3_7_8- Getting location calendar is now done on an instance instead of class. So
+_3_7_9  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
+_3_8_0- The `CompanyType.Master` enum has been replaced with
 `CompanyType.Primary`.
-_3_7_7  This was a leftover reference to the Master Company which was renamed in
-_3_7_8  Projectal several versions ago.
-_3_7_9
-_3_8_0**Other changes**:
-_3_8_1- Date conversion functions return None when given None or empty string
-_3_8_2- Added `Task.reset_duration()` as a basic duration calculator for tasks.
-_3_8_3  This is a work-in-progress and will be gradually improved. The duration
-_3_8_4  calculator takes into consideration the location to remove non-work
-_3_8_5  days from the estimate of working duration. It currently does not work
-_3_8_6  for the time component or `isWorking=True` exceptions.
-_3_8_7- Change detection in `Entity.changes()` now excludes cases where the
-_3_8_8  server has no value and the new value is None. Saving this change has
-_3_8_9  no effect and would always detect a change until a non-None value is
-_3_9_0  set, which is noisy and generates more network activity.
-_3_9_1
-_3_9_2### 2.0.3
-_3_9_3- Better support for calendars.
-_3_9_4  - Distinguish between calendar containers ("Calendar") and the
-_3_9_5    calendar items within them ("CalendarItem").
-_3_9_6  - Allow CalendarItems to be saved directly. E.G item.save()
-_3_9_7- Fix 'holder' parameter in contact/staff/location/task_template not
-_3_9_8  permitting object type. Now consumes uuId or object to match rest of
-_3_9_9  the library.
-_4_0_0- `Entity.changes()` has been extended with an `old=True` flag. When
-_4_0_1  this flag is true, the set of changes will now return both the original
-_4_0_2  and the new values. E.g.
-_4_0_3```
-_4_0_4task.changes()
-_4_0_5# {'name': 'current'}
-_4_0_6task.changes(old=True)
-_4_0_7# {'name': {'old': 'original', 'new': 'current'}}
-_4_0_8```
-_4_0_9- Fixed entity link cache causing errors when deleting a link from an entity
-_4_1_0  which has not been fetched with links (deleting from empty list).
-_4_1_1
-_4_1_2### 2.0.2
-_4_1_3- Fixed updating Webhook entities
-_4_1_4
-_4_1_5### 2.0.1
-_4_1_6- Fixed application ID not being used correctly.
-_4_1_7
-_4_1_8### 2.0.0
-_4_1_9- Version 2.0 accompanies the release of Projectal 2.0. There are no major
+_3_8_1  This was a leftover reference to the Master Company which was renamed in
+_3_8_2  Projectal several versions ago.
+_3_8_3
+_3_8_4**Other changes**:
+_3_8_5- Date conversion functions return None when given None or empty string
+_3_8_6- Added `Task.reset_duration()` as a basic duration calculator for tasks.
+_3_8_7  This is a work-in-progress and will be gradually improved. The duration
+_3_8_8  calculator takes into consideration the location to remove non-work
+_3_8_9  days from the estimate of working duration. It currently does not work
+_3_9_0  for the time component or `isWorking=True` exceptions.
+_3_9_1- Change detection in `Entity.changes()` now excludes cases where the
+_3_9_2  server has no value and the new value is None. Saving this change has
+_3_9_3  no effect and would always detect a change until a non-None value is
+_3_9_4  set, which is noisy and generates more network activity.
+_3_9_5
+_3_9_6### 2.0.3
+_3_9_7- Better support for calendars.
+_3_9_8  - Distinguish between calendar containers ("Calendar") and the
+_3_9_9    calendar items within them ("CalendarItem").
+_4_0_0  - Allow CalendarItems to be saved directly. E.G item.save()
+_4_0_1- Fix 'holder' parameter in contact/staff/location/task_template not
+_4_0_2  permitting object type. Now consumes uuId or object to match rest of
+_4_0_3  the library.
+_4_0_4- `Entity.changes()` has been extended with an `old=True` flag. When
+_4_0_5  this flag is true, the set of changes will now return both the original
+_4_0_6  and the new values. E.g.
+_4_0_7```
+_4_0_8task.changes()
+_4_0_9# {'name': 'current'}
+_4_1_0task.changes(old=True)
+_4_1_1# {'name': {'old': 'original', 'new': 'current'}}
+_4_1_2```
+_4_1_3- Fixed entity link cache causing errors when deleting a link from an entity
+_4_1_4  which has not been fetched with links (deleting from empty list).
+_4_1_5
+_4_1_6### 2.0.2
+_4_1_7- Fixed updating Webhook entities
+_4_1_8
+_4_1_9### 2.0.1
+_4_2_0- Fixed application ID not being used correctly.
+_4_2_1
+_4_2_2### 2.0.0
+_4_2_3- Version 2.0 accompanies the release of Projectal 2.0. There are no major
 changes
-_4_2_0  since the previous release.
-_4_2_1- Expose `Entity.changes()` function. It returns a list of fields on an
+_4_2_4  since the previous release.
+_4_2_5- Expose `Entity.changes()` function. It returns a list of fields on an
 entity that
-_4_2_2  have changed since fetching it. These are the changes that will be sent
+_4_2_6  have changed since fetching it. These are the changes that will be sent
 over to the
-_4_2_3  server when an update request is made.
-_4_2_4- Added missing 'packaging' dependency to requirements.
-_4_2_5
-_4_2_6### 1.2.0
-_4_2_7
-_4_2_8**Breaking changes**:
+_4_2_7  server when an update request is made.
+_4_2_8- Added missing 'packaging' dependency to requirements.
 _4_2_9
-_4_3_0- Renamed `request_timestamp` to `response_timestamp` to better reflect its
+_4_3_0### 1.2.0
+_4_3_1
+_4_3_2**Breaking changes**:
+_4_3_3
+_4_3_4- Renamed `request_timestamp` to `response_timestamp` to better reflect its
 purpose.
-_4_3_1- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
+_4_3_5- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
 reverted.
-_4_3_2  All date fields returned from the server remain as UTC timestamps.
-_4_3_3
-_4_3_4  The reason is that date fields on tasks contain a time component and
+_4_3_6  All date fields returned from the server remain as UTC timestamps.
+_4_3_7
+_4_3_8  The reason is that date fields on tasks contain a time component and
 converting them
-_4_3_5  into date strings was erasing the time, resulting in a value that does not
+_4_3_9  into date strings was erasing the time, resulting in a value that does not
 match
-_4_3_6  the database.
-_4_3_7
-_4_3_8  Note: the server supports setting date fields using a date string like
+_4_4_0  the database.
+_4_4_1
+_4_4_2  Note: the server supports setting date fields using a date string like
 `2022-04-05`.
-_4_3_9  You may use this if you prefer but the server will always return a
+_4_4_3  You may use this if you prefer but the server will always return a
 timestamp.
-_4_4_0
-_4_4_1  Note: we provide utility functions for easily converting dates from/to
-_4_4_2  timestamps expected by the Projectal server. See:
-_4_4_3  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
-_4_4_4  `projectal.timestamp_from_datetime()`.
-_4_4_5
-_4_4_6**Other changes**:
-_4_4_7- Implement request chunking - for methods that consume a list of entities,
+_4_4_4
+_4_4_5  Note: we provide utility functions for easily converting dates from/to
+_4_4_6  timestamps expected by the Projectal server. See:
+_4_4_7  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
+_4_4_8  `projectal.timestamp_from_datetime()`.
+_4_4_9
+_4_5_0**Other changes**:
+_4_5_1- Implement request chunking - for methods that consume a list of entities,
 we now
-_4_4_8  automatically batch them up into multiple requests to prevent timeouts on
+_4_5_2  automatically batch them up into multiple requests to prevent timeouts on
 really
-_4_4_9  large request. Values are configurable through
-_4_5_0  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
-_4_5_1  Default values: Read: 1000 items. Write: 200 items.
-_4_5_2- Added profile get/set functions on entities for easier use. Now you only
+_4_5_3  large request. Values are configurable through
+_4_5_4  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
+_4_5_5  Default values: Read: 1000 items. Write: 200 items.
+_4_5_6- Added profile get/set functions on entities for easier use. Now you only
 need to supply
-_4_5_3  the key and the data. E.g:
-_4_5_4
-_4_5_5```
-_4_5_6key = 'hr_connector'
-_4_5_7data = {'staff_source': 'company_z'}
-_4_5_8task.profile_set(key, data)
+_4_5_7  the key and the data. E.g:
+_4_5_8
 _4_5_9```
-_4_6_0
-_4_6_1- Entity link methods now automatically update the entity's cached list of
+_4_6_0key = 'hr_connector'
+_4_6_1data = {'staff_source': 'company_z'}
+_4_6_2task.profile_set(key, data)
+_4_6_3```
+_4_6_4
+_4_6_5- Entity link methods now automatically update the entity's cached list of
 links. E.g:
-_4_6_2  a task fetched with staff links will have `task['staffList'] =
+_4_6_6  a task fetched with staff links will have `task['staffList'] =
 [Staff1,Staff2]`.
-_4_6_3  Before, doing a `task.link_staff(staff)` did not modify the list to
+_4_6_7  Before, doing a `task.link_staff(staff)` did not modify the list to
 reflect the
-_4_6_4  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
+_4_6_8  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
 applies for update
-_4_6_5  and delete.
-_4_6_6
-_4_6_7  This allows you to modify links and continue working with that object
+_4_6_9  and delete.
+_4_7_0
+_4_7_1  This allows you to modify links and continue working with that object
 without having
-_4_6_8  to fetch it again to obtain the most recent link data. Be aware that if
+_4_7_2  to fetch it again to obtain the most recent link data. Be aware that if
 you acquire
-_4_6_9  the object without requesting the link data as well
-_4_7_0  (e.g: `projectal.Task.get(id, links='STAFF')`),
-_4_7_1  these lists will not accurately reflect what's in the database, only the
+_4_7_3  the object without requesting the link data as well
+_4_7_4  (e.g: `projectal.Task.get(id, links='STAFF')`),
+_4_7_5  these lists will not accurately reflect what's in the database, only the
 changes made
-_4_7_2  while the object is held.
-_4_7_3
-_4_7_4- Support new `applicationId` property on login. Set with:
+_4_7_6  while the object is held.
+_4_7_7
+_4_7_8- Support new `applicationId` property on login. Set with:
 `projectal.api_application_id`.
-_4_7_5  The application ID is sent back to you in webhooks so you know which
+_4_7_9  The application ID is sent back to you in webhooks so you know which
 application was
-_4_7_6  the source of the event (and you can choose to filter them accordingly).
-_4_7_7- Added `Entity.set_readonly()` to allow setting values on entities that
+_4_8_0  the source of the event (and you can choose to filter them accordingly).
+_4_8_1- Added `Entity.set_readonly()` to allow setting values on entities that
 will not
-_4_7_8  be sent over to the server when updating/saving the entity.
-_4_7_9
-_4_8_0  The main use case for this is to populate cached entities which you have
+_4_8_2  be sent over to the server when updating/saving the entity.
+_4_8_3
+_4_8_4  The main use case for this is to populate cached entities which you have
 just created
-_4_8_1  with values you already know about. This is mainly a workaround for the
+_4_8_5  with values you already know about. This is mainly a workaround for the
 limitation of
-_4_8_2  the server not sending the full object back after creating it, resulting
+_4_8_6  the server not sending the full object back after creating it, resulting
 in the client
-_4_8_3  needing to fetch the object in full again if it needs some of the fields
+_4_8_7  needing to fetch the object in full again if it needs some of the fields
 set by the
-_4_8_4  server after creation.
-_4_8_5
-_4_8_6  Additionally, some read-only fields will generate an error on the server
+_4_8_8  server after creation.
+_4_8_9
+_4_9_0  Additionally, some read-only fields will generate an error on the server
 if
-_4_8_7  included in the update request. This method lets you set these values on
+_4_9_1  included in the update request. This method lets you set these values on
 newly
-_4_8_8  created objects without triggering this error.
-_4_8_9
-_4_9_0  A common example is setting the `projectRef` of a task you just created.
-_4_9_1
-_4_9_2
-_4_9_3### 1.1.1
-_4_9_4- Add support for 'profiles' API. Profiles are a type of key-value storage
+_4_9_2  created objects without triggering this error.
+_4_9_3
+_4_9_4  A common example is setting the `projectRef` of a task you just created.
+_4_9_5
+_4_9_6
+_4_9_7### 1.1.1
+_4_9_8- Add support for 'profiles' API. Profiles are a type of key-value storage
 that target
-_4_9_5  any entity. Not currently documented.
-_4_9_6- Fix handling error message parsing in ProjectalException for batch create
+_4_9_9  any entity. Not currently documented.
+_5_0_0- Fix handling error message parsing in ProjectalException for batch create
 operation
-_4_9_7- Add `Task.update_order()` to set task order
-_4_9_8- Return empty list when GETing empty list instead of failing (no request to
+_5_0_1- Add `Task.update_order()` to set task order
+_5_0_2- Return empty list when GETing empty list instead of failing (no request to
 server)
-_4_9_9- Expose the timestamp returned by requests that modify the database. Use
-_5_0_0  `projectal.request_timestamp` to get the value of the most recent request
+_5_0_3- Expose the timestamp returned by requests that modify the database. Use
+_5_0_4  `projectal.request_timestamp` to get the value of the most recent request
 (None
-_5_0_1  if no timestamp in response)
-_5_0_2
-_5_0_3### 1.1.0
-_5_0_4- Minimum Projectal version is now 1.9.4.
-_5_0_5
-_5_0_6**Breaking changes**:
-_5_0_7- Entity `list()` now returns a list of UUIDs instead of full objects. You
+_5_0_5  if no timestamp in response)
+_5_0_6
+_5_0_7### 1.1.0
+_5_0_8- Minimum Projectal version is now 1.9.4.
+_5_0_9
+_5_1_0**Breaking changes**:
+_5_1_1- Entity `list()` now returns a list of UUIDs instead of full objects. You
 may provide
-_5_0_8  an `expand` parameter to restore the previous behavior: `Entity.list
+_5_1_2  an `expand` parameter to restore the previous behavior: `Entity.list
 (expand=True)`.
-_5_0_9  This change is made for performance reasons where you may have thousands
+_5_1_3  This change is made for performance reasons where you may have thousands
 of tasks
-_5_1_0  and getting them all may time out. For those cases, we suggest writing a
+_5_1_4  and getting them all may time out. For those cases, we suggest writing a
 query to filter
-_5_1_1  down to only the tasks and fields you need.
-_5_1_2- `Company.get_master_company()` has been renamed to
+_5_1_5  down to only the tasks and fields you need.
+_5_1_6- `Company.get_master_company()` has been renamed to
 `Company.get_primary_company()`
-_5_1_3  to match the server.
-_5_1_4- The following date fields are converted into date strings upon fetch:
-_5_1_5  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
-_5_1_6  These fields are added or updated using date strings (like `2022-03-02`),
+_5_1_7  to match the server.
+_5_1_8- The following date fields are converted into date strings upon fetch:
+_5_1_9  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
+_5_2_0  These fields are added or updated using date strings (like `2022-03-02`),
 but the
-_5_1_7  server returns timestamps (e.g: 1646006400000) upon fetch, which is
+_5_2_1  server returns timestamps (e.g: 1646006400000) upon fetch, which is
 confusing. This
-_5_1_8  change ensures they are always date strings for consistency.
-_5_1_9
-_5_2_0**Other changes**:
-_5_2_1- When updating an entity, only the fields that have changed are sent to the
+_5_2_2  change ensures they are always date strings for consistency.
+_5_2_3
+_5_2_4**Other changes**:
+_5_2_5- When updating an entity, only the fields that have changed are sent to the
 server. When
-_5_2_2  updating a list of entities, unmodified entities are not sent to the
+_5_2_6  updating a list of entities, unmodified entities are not sent to the
 server at all. This
-_5_2_3  dramatically reduces the payload size and should speed things up.
-_5_2_4- When fetching entities, entity links are now typed as well. E.g. `project
+_5_2_7  dramatically reduces the payload size and should speed things up.
+_5_2_8- When fetching entities, entity links are now typed as well. E.g. `project
 ['rebateList']`
-_5_2_5  contains a list of `Rebate` instead of `dict`.
-_5_2_6- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
+_5_2_9  contains a list of `Rebate` instead of `dict`.
+_5_3_0- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
 help with
-_5_2_7  converting to/from dates and Projectal timestamps.
-_5_2_8- Entity history now uses `desc` by default (index 0 is newest)
-_5_2_9- Added `Project.tasks()` to list all task UUIDs within a project.
-_5_3_0
-_5_3_1### 1.0.3
-_5_3_2- Fix another case of automatic JWT refresh not working
-_5_3_3
-_5_3_4### 1.0.2
-_5_3_5- Entity instances can `save()` or `delete()` on themselves
-_5_3_6- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
+_5_3_1  converting to/from dates and Projectal timestamps.
+_5_3_2- Entity history now uses `desc` by default (index 0 is newest)
+_5_3_3- Added `Project.tasks()` to list all task UUIDs within a project.
+_5_3_4
+_5_3_5### 1.0.3
+_5_3_6- Fix another case of automatic JWT refresh not working
+_5_3_7
+_5_3_8### 1.0.2
+_5_3_9- Entity instances can `save()` or `delete()` on themselves
+_5_4_0- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
 instances
-_5_3_7- Fix automatic JWT refresh only working in some cases
-_5_3_8
-_5_3_9### 1.0.1
-_5_4_0- Added `list()` function for all entities
-_5_4_1- Added search functions for all entities (match-, search, query)
-_5_4_2- Added `Company.get_master_company()`
-_5_4_3- Fixed adding template tasks
-_5_4_4
-_5_4_5"""
-_5_4_6import logging
-_5_4_7import os
+_5_4_1- Fix automatic JWT refresh only working in some cases
+_5_4_2
+_5_4_3### 1.0.1
+_5_4_4- Added `list()` function for all entities
+_5_4_5- Added search functions for all entities (match-, search, query)
+_5_4_6- Added `Company.get_master_company()`
+_5_4_7- Fixed adding template tasks
 _5_4_8
-_5_4_9from projectal.entities import *
-_5_5_0from projectal.dynamic_enums import *
-_5_5_1from .api import *
-_5_5_2from . import profile
-_5_5_3
-_5_5_4api_base = os.getenv("PROJECTAL_URL")
-_5_5_5api_username = os.getenv("PROJECTAL_USERNAME")
-_5_5_6api_password = os.getenv("PROJECTAL_PASSWORD")
-_5_5_7api_application_id = None
-_5_5_8api_auth_details = None
-_5_5_9api_alias = None
-_5_6_0cookies = None
-_5_6_1chunk_size_read = 1000
-_5_6_2chunk_size_write = 200
-_5_6_3
-_5_6_4# Records the timestamp generated by the last request (database
-_5_6_5# event time). These are reported on add or updates; if there is
-_5_6_6# no timestamp in the response, this is set to None.
-_5_6_7response_timestamp = None
-_5_6_8
-_5_6_9
-_5_7_0# The minimum version number of the Projectal instance that this
-_5_7_1# API client targets. Lower versions are not supported and will
-_5_7_2# raise an exception.
-_5_7_3MIN_PROJECTAL_VERSION = "4.0.40"
-_5_7_4
-_5_7_5__verify = True
-_5_7_6
-_5_7_7logging.getLogger("projectal-api-client").addHandler(logging.NullHandler())
+_5_4_9"""
+_5_5_0import logging
+_5_5_1import os
+_5_5_2
+_5_5_3from projectal.entities import *
+_5_5_4from projectal.dynamic_enums import *
+_5_5_5from .api import *
+_5_5_6from . import profile
+_5_5_7
+_5_5_8api_base = os.getenv("PROJECTAL_URL")
+_5_5_9api_username = os.getenv("PROJECTAL_USERNAME")
+_5_6_0api_password = os.getenv("PROJECTAL_PASSWORD")
+_5_6_1api_application_id = None
+_5_6_2api_auth_details = None
+_5_6_3api_alias = None
+_5_6_4cookies = None
+_5_6_5chunk_size_read = 1000
+_5_6_6chunk_size_write = 200
+_5_6_7
+_5_6_8# Records the timestamp generated by the last request (database
+_5_6_9# event time). These are reported on add or updates; if there is
+_5_7_0# no timestamp in the response, this is set to None.
+_5_7_1response_timestamp = None
+_5_7_2
+_5_7_3
+_5_7_4# The minimum version number of the Projectal instance that this
+_5_7_5# API client targets. Lower versions are not supported and will
+_5_7_6# raise an exception.
+_5_7_7MIN_PROJECTAL_VERSION = "4.0.40"
+_5_7_8
+_5_7_9__verify = True
+_5_8_0
+_5_8_1logging.getLogger("projectal-api-client").addHandler(logging.NullHandler())
 api_base = None
 api_username = None
 api_password = None
 api_application_id = None
 api_auth_details = None
 api_alias = None
 cookies = None
```

### Comparing `projectal-4.3.0/examples/linking.py` & `projectal-4.3.1/examples/linking.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/examples/task.py` & `projectal-4.3.1/examples/task.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/examples/webhook.py` & `projectal-4.3.1/examples/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/__init__.py` & `projectal-4.3.1/projectal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Getting started
 
 ```
 import projectal
 import os
 
 # Supply your Projectal server URL and account credentials
-projectal.api_base = https://yourcompany.projectal.com
+projectal.api_base = 'https://yourcompany.projectal.com'
 projectal.api_username = os.environ.get('PROJECTAL_USERNAME')
 projectal.api_password = os.environ.get('PROJECTAL_PASSWORD')
 
 # Test communication with server
 status = projectal.status()
 
 # Test account credentials
@@ -20,22 +20,26 @@
 details = projectal.auth_details()
 ```
 
 ----
 
 ## Changelog
 
+### 4.3.1
+- Fixed typo in "Getting started" example.
+- Fixed typo in 4.3.0 Changelog.
+
 ### 4.3.0
 
 **Breaking changes:**
 
 - Added "PREDECESSOR_TASK" option when fetching projectal.Task with links
 - Predecessor tasks will be returned as a list of tasks under the taskList attribute
 - This attribute name is different to what you would see when using the REST API directly
-  (planLink). This change was necessary to allow for directly manipulating
+  (planList). This change was necessary to allow for directly manipulating
   the list of links and then saving the task entity to commit any changes,
   since the REST API is expecting a different key for linking calls (taskList).
 - Existing Predecessor Task linking methods were also updated to match the new linking functionality.
   They now work as a reverse linker, automatically inverting the link relationship between
   the task entities. This more closely matches what you would expect to see based on the Web UI.
   I.e. When previously calling `some_task.link_predecessor_task(another_task)`,
   some_task would be set as a predecessor for another_task instead of the other way around.
```

### Comparing `projectal-4.3.0/projectal/api.py` & `projectal-4.3.1/projectal/api.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/dynamic_enum.py` & `projectal-4.3.1/projectal/dynamic_enum.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/__init__.py` & `projectal-4.3.1/projectal/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/activity.py` & `projectal-4.3.1/projectal/entities/activity.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/booking.py` & `projectal-4.3.1/projectal/entities/booking.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/calendar.py` & `projectal-4.3.1/projectal/entities/calendar.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/company.py` & `projectal-4.3.1/projectal/entities/company.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/contact.py` & `projectal-4.3.1/projectal/entities/contact.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/department.py` & `projectal-4.3.1/projectal/entities/department.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/file.py` & `projectal-4.3.1/projectal/entities/file.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/folder.py` & `projectal-4.3.1/projectal/entities/folder.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/location.py` & `projectal-4.3.1/projectal/entities/location.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/note.py` & `projectal-4.3.1/projectal/entities/note.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/permission.py` & `projectal-4.3.1/projectal/entities/permission.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/project.py` & `projectal-4.3.1/projectal/entities/project.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/project_template.py` & `projectal-4.3.1/projectal/entities/project_template.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/staff.py` & `projectal-4.3.1/projectal/entities/staff.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/task.py` & `projectal-4.3.1/projectal/entities/task.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/task_template.py` & `projectal-4.3.1/projectal/entities/task_template.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/user.py` & `projectal-4.3.1/projectal/entities/user.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entities/webhook.py` & `projectal-4.3.1/projectal/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/entity.py` & `projectal-4.3.1/projectal/entity.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/enums.py` & `projectal-4.3.1/projectal/enums.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/errors.py` & `projectal-4.3.1/projectal/errors.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/linkers.py` & `projectal-4.3.1/projectal/linkers.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal/profile.py` & `projectal-4.3.1/projectal/profile.py`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/projectal.egg-info/PKG-INFO` & `projectal-4.3.1/projectal.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 4.3.0
+Version: 4.3.1
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-4.3.0/projectal.egg-info/SOURCES.txt` & `projectal-4.3.1/projectal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `projectal-4.3.0/setup.py` & `projectal-4.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="projectal",
-    version="4.3.0",
+    version="4.3.1",
     description="Python bindings for the Projectal API",
     long_description="The Python library allows developers to write Python-based apps that talk directly with Projectal. This gives developers immense freedom to access all data points in Projectal and to integrate Projectal with their workflow.",
     long_description_content_type="text/plain",
     url="https://projectal.com/resources/developer",
     author="Projectal",
     author_email="support@projectal.com",
     license="MIT",
```

