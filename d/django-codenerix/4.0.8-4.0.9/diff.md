# Comparing `tmp/django-codenerix-4.0.8.tar.gz` & `tmp/django-codenerix-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-4.0.8.tar", last modified: Sat Jun 18 20:52:09 2022, max compression
+gzip compressed data, was "django-codenerix-4.0.9.tar", last modified: Sat Jun 18 21:06:55 2022, max compression
```

## Comparing `django-codenerix-4.0.8.tar` & `django-codenerix-4.0.9.tar`

### file list

```diff
@@ -1,1266 +1,1266 @@
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.390594 django-codenerix-4.0.8/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1362 2022-06-18 20:51:18.000000 django-codenerix-4.0.8/CHANGELOG
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/LICENSE
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      522 2022-05-18 07:13:55.000000 django-codenerix-4.0.8/MANIFEST.in
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14249 2022-06-18 20:52:09.390594 django-codenerix-4.0.8/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11566 2022-05-18 05:25:04.000000 django-codenerix-4.0.8/README.rst
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.170587 django-codenerix-4.0.8/codenerix/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      863 2022-06-18 20:45:41.000000 django-codenerix-4.0.8/codenerix/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      143 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/apps.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    43380 2022-06-13 06:11:49.000000 django-codenerix-4.0.8/codenerix/authbackend.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1830 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/constants.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4032 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/context.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.170587 django-codenerix-4.0.8/codenerix/contrib/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/contrib/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2057 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/contrib/haystack_engines.py
--rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)    23868 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/debug.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.174587 django-codenerix-4.0.8/codenerix/djng/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1216 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.174587 django-codenerix-4.0.8/codenerix/djng/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1766 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1647 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14378 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_base.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13399 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_base.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4840 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_model.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4439 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_model.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2989 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_validation.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2819 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_validation.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9401 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/field_mixins.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8470 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/djng/__pycache__/field_mixins.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13584 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/djng/angular_base.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4296 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/djng/angular_model.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/djng/angular_validation.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8684 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/djng/field_mixins.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5393 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/djng/widgets.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      717 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/exceptions.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6972 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/fields.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27694 2022-06-18 20:44:43.000000 django-codenerix-4.0.8/codenerix/forms.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18354 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/helpers.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.178587 django-codenerix-4.0.8/codenerix/lib/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.178587 django-codenerix-4.0.8/codenerix/lib/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      362 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/lib/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      134 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      155 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1478 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/colors.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1321 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4607 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/debugger.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4181 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/debugger.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/genmail.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/genmail.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      333 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/helpers.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      347 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/lib/__pycache__/helpers.cpython-39.pyc
--rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     2079 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/lib/colors.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7719 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/lib/debugger.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2937 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/lib/genmail.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      806 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/lib/helpers.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3764 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/lib/pylock.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.162587 django-codenerix-4.0.8/codenerix/locale/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.162587 django-codenerix-4.0.8/codenerix/locale/en/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/locale/en/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14107 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.162587 django-codenerix-4.0.8/codenerix/locale/es/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/locale/es/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8531 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    28792 2022-05-17 13:46:42.000000 django-codenerix-4.0.8/codenerix/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/management/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/management/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      154 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/management/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/management/commands/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.182587 django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      227 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.186588 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      148 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      171 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1228 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/clean.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1552 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/colors.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5215 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/locales.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4723 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/locales.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2062 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/refresh_permissions.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3259 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/management/commands/__pycache__/touch.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6447 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/check_dependencies.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1582 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/clean.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1326 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/clean_memcache.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2115 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/colors.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9104 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/locales.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3248 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/refresh_permissions.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4924 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/management/commands/touch.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3403 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/middleware.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.190588 django-codenerix-4.0.8/codenerix/migrations/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1515 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      421 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0002_auto_20160808_0843.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      431 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0003_auto_20160817_1235.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      430 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0004_auto_20160824_0757.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      433 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0005_auto_20160824_1332.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      431 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0006_auto_20160825_0838.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      338 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0007_corporateimage.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      334 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0008_auto_20170119_1526.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      338 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0009_delete_corporateimage.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      270 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0010_corporateimage.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      263 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0011_delete_corporateimage.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      548 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0012_auto_20170405_0815.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0013_auto_20170410_1429.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      545 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0014_auto_20170418_1011.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0015_auto_20170418_1515.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      541 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0016_auto_20170419_1533.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0017_auto_20170428_0850.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      481 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0018_log_snapshot_txt.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      480 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0019_auto_20170725_1822.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1204 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0020_remotelog.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      936 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/0021_auto_20171218_1039.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.202588 django-codenerix-4.0.8/codenerix/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1526 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1401 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      688 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      666 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      676 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      695 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      699 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      681 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      680 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0007_corporateimage.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0007_corporateimage.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      520 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      496 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0010_corporateimage.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      491 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0010_corporateimage.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      496 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0011_delete_corporateimage.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      491 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0011_delete_corporateimage.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      810 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      755 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      807 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      752 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      803 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      748 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      699 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      676 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1301 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0020_remotelog.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1200 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0020_remotelog.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1023 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      937 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      141 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 13:55:09.000000 django-codenerix-4.0.8/codenerix/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2664 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/mixins.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25135 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/models.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13508 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/models_people.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.202588 django-codenerix-4.0.8/codenerix/multi_email_field/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.202588 django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      169 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1420 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1226 2022-05-17 13:45:38.000000 django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/widgets.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1388 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/fields.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      980 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/forms.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       48 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/models.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.206588 django-codenerix-4.0.8/codenerix/multi_email_field/tests/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       17 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/tests/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      248 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/tests/models.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6114 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/tests/tests.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      899 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multi_email_field/widgets.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13329 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/multiforms.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.166587 django-codenerix-4.0.8/codenerix/static/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.206588 django-codenerix-4.0.8/codenerix/static/codenerix/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.206588 django-codenerix-4.0.8/codenerix/static/codenerix/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8874 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/css/base.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1863 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/css/lists.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.206588 django-codenerix-4.0.8/codenerix/static/codenerix/img/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2027 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/check_green.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    30435 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/codenerix.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4852 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/codenerix_small.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1183 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/false.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2191 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/ko_red.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7634 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/loader.gif
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   120630 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/ok.gif
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1075 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/true.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12451 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/img/warning.gif
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.210588 django-codenerix-4.0.8/codenerix/static/codenerix/js/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.210588 django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      682 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/app.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      988 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/base.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   138815 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/codenerix.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5487 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/controllers.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6505 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/filters.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18438 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/inotify.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9291 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/notify.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      686 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/js/rows.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.214588 django-codenerix-4.0.8/codenerix/static/codenerix/lib/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/1.5.7
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   150696 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25635 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    70647 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    15217 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3924 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8584 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1447 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3388 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      343 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-csp.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17205 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1729 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3838 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    37833 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10306 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    28130 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27897 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2990 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8020 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   108145 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-mocks.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    58196 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21780 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    60234 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    34965 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4509 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11002 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    38728 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4762 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12192 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25757 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5867 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10050 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1504143 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-scenario.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    26512 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3940 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10852 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1174125 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   159127 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   428107 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.min.js.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9444 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/errors.json
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.362593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2535 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-dj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2534 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2535 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2532 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2330 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-na.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2339 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2333 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4028 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4022 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3175 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak-gh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3169 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3243 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3237 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4165 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-001.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4159 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ae.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-bh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4149 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-il.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-iq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-jo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4159 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-km.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-kw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4410 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-lb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4150 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ly.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4059 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4106 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-mr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-om.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4409 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ps.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-qa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-so.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ss.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-td.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-tn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ye.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4157 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4244 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4238 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2742 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast-es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2772 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3930 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl-az.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3924 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2503 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn-az.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2497 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2487 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3310 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3304 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4087 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be-by.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4081 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2791 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem-zm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2785 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3089 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3083 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3783 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg-bg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3777 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2839 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn-ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2833 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2321 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4207 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-bd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4207 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4201 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5745 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-cn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5745 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br-fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2734 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4426 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4420 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4412 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl-ba.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3025 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn-ba.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3019 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3009 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3067 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3064 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-ad.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2832 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es-valencia.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-it.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2808 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2868 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3417 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr-us.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3411 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4865 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-iq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4866 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-ir.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4859 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4855 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-iq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4856 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-ir.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4865 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn-iq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4859 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4849 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3056 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs-cz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3050 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2548 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy-gb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2542 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2949 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-dk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2949 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-gl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2943 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3054 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3048 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2772 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-at.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-be.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2754 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-li.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-lu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2776 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje-ne.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2891 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb-de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2885 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3324 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3318 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo-sn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5542 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz-bt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5536 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3070 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3064 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-gh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-tg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2917 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-cy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-gr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4099 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-001.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2728 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-150.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ag.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ai.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-as.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-au.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-be.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2716 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2714 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ca.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ck.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cx.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2706 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-hk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2718 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ie.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-im.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-io.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-iso.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-je.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-jm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ki.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-kn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ky.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ls.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mp.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ms.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2718 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-my.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-na.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ng.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ph.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-rw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ss.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sx.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-to.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-um.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-us.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ws.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2719 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2706 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2753 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo-001.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2402 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-419.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ar.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-bo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-co.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2405 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-do.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ea.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ec.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2395 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-hn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ic.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2389 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-mx.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ni.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pe.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ph.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2413 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-py.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-sv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2394 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-us.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-uy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ve.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2403 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2810 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et-ee.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2804 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2383 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu-es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2377 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3409 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3403 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3786 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-af.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3883 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-ir.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3877 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-gn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-mr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-sn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2961 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi-fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2955 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2848 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil-ph.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2842 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2799 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo-fo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2793 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2454 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-be.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ca.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ci.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ga.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gp.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ht.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-km.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2454 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-lu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-nc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ne.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-re.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-rw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-td.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-vu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-wf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-yt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur-it.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy-nl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2742 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga-ie.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2735 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2998 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd-gb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2992 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2761 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl-es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2755 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2407 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2410 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2407 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-li.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3938 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3932 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2866 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv-im.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2860 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-gh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ne.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ng.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw-us.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2398 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4351 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he-il.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4345 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3666 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3660 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3059 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-ba.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3059 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-hr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3053 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2893 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb-de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2887 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2577 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu-hu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2571 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4029 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy-am.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4023 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2497 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia-fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2494 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2244 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id-id.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2238 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2906 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig-ng.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2900 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3069 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii-cn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3063 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2238 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3170 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is-is.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3164 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-it.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-sm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4345 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_iw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2513 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja-jp.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2507 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4762 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4756 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4030 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka-ge.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4024 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2887 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab-dz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2881 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3110 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3104 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3154 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3148 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea-cv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2758 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq-ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3028 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3022 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3973 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl-kz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3967 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3957 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3229 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3223 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2873 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl-gl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2867 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2841 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2835 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3784 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km-kh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3778 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4001 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3995 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2534 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kp.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2532 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2526 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4531 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4525 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4288 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4282 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4272 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2725 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3904 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3898 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2911 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh-de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2905 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2784 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw-gb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl-kg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3868 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3858 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3198 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3192 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2822 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb-lu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2816 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2759 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2753 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4132 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt-us.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4126 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3223 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-ao.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3219 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3833 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo-la.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3827 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3112 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt-lt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3106 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2977 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu-cd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2971 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2952 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3177 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv-lv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3171 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3513 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3513 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3507 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2829 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2694 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe-mu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2688 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2733 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg-mg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2727 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3010 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh-mz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3004 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3305 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3299 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4277 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk-mk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4271 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4111 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4985 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl-mn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4979 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4969 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3879 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3873 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2246 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-bn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2240 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-my.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2239 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-sg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2234 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2224 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2571 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt-mt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2565 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3078 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3072 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4025 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my-mm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4019 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3193 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq-na.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3187 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-sj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2348 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2768 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd-zw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2762 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4023 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4019 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-np.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4013 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-aw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-be.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-bq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-cw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-nl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sx.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3312 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3306 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2754 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn-no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4536 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4530 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no-no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2348 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2465 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2462 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2464 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2461 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3111 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus-sd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3105 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2868 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3827 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3821 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4295 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ge.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4311 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4289 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3491 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab-pk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3485 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3608 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3602 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3592 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3117 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl-pl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3111 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4044 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps-af.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4038 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2452 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-ao.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2435 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-br.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-cv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-gw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-pt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2452 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-st.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2451 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-tl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2429 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-bo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2822 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-ec.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2824 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-pe.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2818 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2781 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2775 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2811 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn-bi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2805 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2913 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-md.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2913 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-ro.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2907 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2952 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-by.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4373 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-md.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4386 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4377 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ua.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4380 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2780 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw-rw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4659 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah-ru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4653 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2967 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2961 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2800 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3194 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3174 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3174 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-se.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3168 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2750 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh-mz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2771 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses-ml.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2765 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2989 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg-cf.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2983 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2824 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2818 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4088 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4082 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4072 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4562 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si-lk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4556 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2965 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk-sk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2959 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2973 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl-si.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2967 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2957 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn-fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2951 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn-zw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-dj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2928 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-so.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2921 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-al.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-mk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-xk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4377 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-ba.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4381 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-me.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4378 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-rs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4381 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-xk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4372 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3004 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-ba.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3008 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-me.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3005 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-rs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3008 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-xk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2999 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4362 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2485 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-sz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2483 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2480 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2539 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2536 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2302 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-ls.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2302 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2299 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-ax.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-se.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2862 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-cd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2643 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc-cd.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2640 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3808 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3804 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-lk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3804 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-my.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3803 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-sg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3802 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3921 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3915 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ke.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2800 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3150 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl-tj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3150 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3142 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4009 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th-th.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4003 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3561 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3658 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3652 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3023 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig-er.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3020 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2840 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2482 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-bw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2482 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2479 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2924 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to-to.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2918 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2423 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-cy.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2419 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-tr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2413 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2505 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2502 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2775 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq-ne.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2769 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2839 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2833 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4557 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab-cn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4551 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4541 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4551 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk-ua.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4545 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4103 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-in.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4095 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-pk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4089 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3385 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab-af.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3379 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3432 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl-uz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3426 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2323 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn-uz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2317 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2307 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn-lr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2917 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3334 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii-lr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3328 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3318 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2552 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2549 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2570 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi-vn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2564 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2499 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo-001.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2495 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun-tz.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2931 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae-ch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2925 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2909 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal-et.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2906 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2289 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2286 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2784 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog-ug.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3649 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav-cm.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3643 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4593 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi-001.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4585 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3772 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-bj.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3883 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-ng.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3877 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4084 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh-ma.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2735 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-cn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-cn.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2728 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-hk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-mo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-sg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2564 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-hk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2566 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-mo.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2591 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-tw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2585 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2554 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2581 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-tw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2729 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2352 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu-za.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2346 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/version.json
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        5 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/version.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2213 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-base64-upload.README.md
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1210 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-base64-upload.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1087 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/MIT-LICENSE.txt
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17070 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/colorpicker.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1739 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/alpha.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/hue.png
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8045 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/saturation.png
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17309 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/bootstrap-colorpicker-module.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-switch/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10535 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3139 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      516 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-tabcollapse.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4411 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-checklist-model.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.226589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1083 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/LICENSE.md
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6890 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2870 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4117 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6767 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker-bs3.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    53679 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.230589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1852 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    53486 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1352 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10255 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.230589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/0.5.0
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2915 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9338 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2458 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2841 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.234589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/1.0.9
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   465874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1049182 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   315974 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   348054 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.238589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1516 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/LICENSE
--rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     7594 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/ng-quill.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3321 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/ng-quill.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    22075 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.bubble.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8084 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.core.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   265094 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.core.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   393984 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   195286 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    22726 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.snow.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.238589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1072 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/LICENSE
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14018 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3788 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.242589 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   169870 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    32440 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4502 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/datetimepicker.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6880 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    92332 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4709 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    41590 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   240020 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   110343 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   212215 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    87132 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    72592 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-utils.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23346 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-utils.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.362593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/3.3.6
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.370593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    26132 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    47706 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23409 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5532 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   146082 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   389227 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   121260 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    54416 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.370593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    20127 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   108738 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    45404 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23424 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18028 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.370593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    68954 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    36868 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      484 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/npm.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.166587 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.362593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12351 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11288 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.min.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.362593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    57397 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    35872 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.366593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      940 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ar.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.bg.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ca.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      789 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.cs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      690 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.da.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      714 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.de.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      776 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ee.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      928 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.el.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      685 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.es.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      726 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fi.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      727 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      807 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.he.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      631 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      726 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hu.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      647 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.id.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      747 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.is.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.it.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      679 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ja.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      765 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ko.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      805 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      770 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      659 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ms.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      701 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nb.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      681 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      678 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.no.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      741 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      711 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt-BR.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      745 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      714 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ro.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      679 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs-latin.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      873 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      904 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ru.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      731 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      682 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sl.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      688 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sv.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      811 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sw.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1046 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.th.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      685 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.tr.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      874 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ua.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      927 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.uk.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      813 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-CN.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      813 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-TW.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4725 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-dropdowns-functions.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      469 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-helper.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.366593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6352 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25205 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5612 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14326 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4656 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-tabcollapse.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1136 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-vertical-grid.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      897 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/color-contrast.README.md
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1059 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/color-contrast.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      488 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/file_validation.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.166587 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.370593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    37414 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21778 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css.map
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    31000 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.min.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   134808 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/FontAwesome.otf
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   165742 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   444379 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   165548 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    98024 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    77160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.370593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome-animation/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    33218 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18429 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.min.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2380 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/html5shiv.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/htmlclean/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    24436 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12726 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   247351 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    84245 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   127335 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.min.map
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/moment/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   139009 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/moment/moment.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    58686 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/moment/moment.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/notifyjs/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21577 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/notifyjs/notify.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13637 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/notifyjs/notify.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7982 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/README.md
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6404 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/nspopover.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    16602 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/nspopover.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.374593 django-codenerix-4.0.8/codenerix/static/codenerix/lib/rangy/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   161315 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/rangy/rangy-core.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9546 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/rangy/rangy-selectionsaverestore.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      820 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/sticky-footer-navbar.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      713 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/sticky-footer.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.378594 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    50498 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-rangy.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27842 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7717 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3876 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   130358 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    70592 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.min.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    31999 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngularSetup.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      898 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/logs_rows.html
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.378594 django-codenerix-4.0.8/codenerix/static/codenerix/partials/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.382594 django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      746 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/detail.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18799 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/list.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1478 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/rows.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1523 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/summary.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8384 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/static/codenerix/partials/table.html
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.166587 django-codenerix-4.0.8/codenerix/static/djangular/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.382594 django-codenerix-4.0.8/codenerix/static/djangular/css/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      160 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/djangular/css/bootstrap3.css
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      703 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/djangular/css/styles.css
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.382594 django-codenerix-4.0.8/codenerix/static/djangular/js/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    24374 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/djangular/js/django-angular.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7396 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/static/djangular/js/django-angular.min.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.382594 django-codenerix-4.0.8/codenerix/templates/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14466 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templates/.session.vim
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.386594 django-codenerix-4.0.8/codenerix/templates/codenerix/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2959 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/add.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1664 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/addmodal.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9567 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/details.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      815 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/detailsmodal.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3861 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/detailsmodal_log.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    47851 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/form.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3127 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/formmodal.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2112 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/list.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1984 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/listmodal.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1557 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/remote_log.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1888 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/sublist.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2790 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templates/codenerix/sublistmodal.html
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.386594 django-codenerix-4.0.8/codenerix/templatetags/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.386594 django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1102 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.390594 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      143 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      164 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7959 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_common.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7429 2022-05-17 13:45:50.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_common.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7436 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_lists.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6850 2022-05-17 13:45:49.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_lists.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3297 2022-05-17 11:43:27.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_special.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3948 2022-05-27 10:32:58.000000 django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_special.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7217 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templatetags/codenerix_common.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8936 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/templatetags/codenerix_lists.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4637 2022-05-27 10:32:55.000000 django-codenerix-4.0.8/codenerix/templatetags/codenerix_special.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1658 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/urls.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   177977 2022-06-18 16:04:41.000000 django-codenerix-4.0.8/codenerix/views.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    38707 2022-05-17 12:10:26.000000 django-codenerix-4.0.8/codenerix/widgets.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 20:52:09.390594 django-codenerix-4.0.8/django_codenerix.egg-info/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14249 2022-06-18 20:52:08.000000 django-codenerix-4.0.8/django_codenerix.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    76651 2022-06-18 20:52:09.000000 django-codenerix-4.0.8/django_codenerix.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-06-18 20:52:08.000000 django-codenerix-4.0.8/django_codenerix.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-05-17 11:43:28.000000 django-codenerix-4.0.8/django_codenerix.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      238 2022-06-18 20:52:08.000000 django-codenerix-4.0.8/django_codenerix.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       10 2022-06-18 20:52:08.000000 django-codenerix-4.0.8/django_codenerix.egg-info/top_level.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2022-06-18 20:52:09.390594 django-codenerix-4.0.8/setup.cfg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2137 2022-06-18 20:51:36.000000 django-codenerix-4.0.8/setup.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.806464 django-codenerix-4.0.9/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1475 2022-06-18 21:06:07.000000 django-codenerix-4.0.9/CHANGELOG
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/LICENSE
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      522 2022-05-18 07:13:55.000000 django-codenerix-4.0.9/MANIFEST.in
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14249 2022-06-18 21:06:55.806464 django-codenerix-4.0.9/PKG-INFO
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11566 2022-05-18 05:25:04.000000 django-codenerix-4.0.9/README.rst
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.594457 django-codenerix-4.0.9/codenerix/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      172 2022-06-18 21:06:33.000000 django-codenerix-4.0.9/codenerix/__init__.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      143 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/apps.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    43380 2022-06-13 06:11:49.000000 django-codenerix-4.0.9/codenerix/authbackend.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1830 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/constants.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4032 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/context.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.594457 django-codenerix-4.0.9/codenerix/contrib/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/contrib/__init__.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2057 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/contrib/haystack_engines.py
+-rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)    23868 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/debug.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.594457 django-codenerix-4.0.9/codenerix/djng/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1216 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.594457 django-codenerix-4.0.9/codenerix/djng/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1766 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1647 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14378 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_base.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13399 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_base.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4840 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_model.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4439 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_model.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2989 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_validation.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2819 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_validation.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9401 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/field_mixins.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8470 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/djng/__pycache__/field_mixins.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13584 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/djng/angular_base.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4296 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/djng/angular_model.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/djng/angular_validation.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8684 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/djng/field_mixins.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5393 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/djng/widgets.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      717 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/exceptions.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6972 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/fields.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27694 2022-06-18 20:44:43.000000 django-codenerix-4.0.9/codenerix/forms.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18354 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/helpers.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/lib/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/lib/.ropeproject/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      362 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/lib/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      134 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      155 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1478 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/colors.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1321 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4607 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/debugger.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4181 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/debugger.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/genmail.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/genmail.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      333 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/helpers.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      347 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/lib/__pycache__/helpers.cpython-39.pyc
+-rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     2079 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/lib/colors.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7719 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/lib/debugger.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2937 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/lib/genmail.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      806 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/lib/helpers.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3764 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/lib/pylock.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.582457 django-codenerix-4.0.9/codenerix/locale/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.582457 django-codenerix-4.0.9/codenerix/locale/en/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/locale/en/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14107 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.586457 django-codenerix-4.0.9/codenerix/locale/es/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/locale/es/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8531 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    28792 2022-05-17 13:46:42.000000 django-codenerix-4.0.9/codenerix/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/management/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.598458 django-codenerix-4.0.9/codenerix/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      154 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/management/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.602458 django-codenerix-4.0.9/codenerix/management/commands/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.602458 django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      227 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.602458 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      148 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      171 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1228 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/clean.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1552 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/colors.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5215 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/locales.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4723 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/locales.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2062 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/refresh_permissions.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3259 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/management/commands/__pycache__/touch.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6447 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/check_dependencies.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1582 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/clean.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1326 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/clean_memcache.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2115 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/colors.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9104 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/locales.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3248 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/refresh_permissions.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4924 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/management/commands/touch.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3403 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/middleware.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.606458 django-codenerix-4.0.9/codenerix/migrations/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1515 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      421 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0002_auto_20160808_0843.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      431 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0003_auto_20160817_1235.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      430 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0004_auto_20160824_0757.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      433 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0005_auto_20160824_1332.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      431 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0006_auto_20160825_0838.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      338 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0007_corporateimage.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      334 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0008_auto_20170119_1526.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      338 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0009_delete_corporateimage.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      270 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0010_corporateimage.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      263 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0011_delete_corporateimage.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      548 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0012_auto_20170405_0815.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0013_auto_20170410_1429.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      545 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0014_auto_20170418_1011.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0015_auto_20170418_1515.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      541 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0016_auto_20170419_1533.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      531 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0017_auto_20170428_0850.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      481 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0018_log_snapshot_txt.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      480 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0019_auto_20170725_1822.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1204 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0020_remotelog.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      936 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/0021_auto_20171218_1039.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.614458 django-codenerix-4.0.9/codenerix/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1526 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1401 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      688 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      666 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      676 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      695 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      699 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      681 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      680 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0007_corporateimage.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0007_corporateimage.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      520 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      513 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      496 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0010_corporateimage.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      491 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0010_corporateimage.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      496 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0011_delete_corporateimage.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      491 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0011_delete_corporateimage.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      810 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      755 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      807 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      752 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      803 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      748 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      791 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      699 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      698 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      676 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1301 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0020_remotelog.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1200 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0020_remotelog.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1023 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      937 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      141 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 13:55:09.000000 django-codenerix-4.0.9/codenerix/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2664 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/mixins.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25135 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/models.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13508 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/models_people.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.614458 django-codenerix-4.0.9/codenerix/multi_email_field/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.618458 django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      169 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1420 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1226 2022-05-17 13:45:38.000000 django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/widgets.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1388 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/fields.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      980 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/forms.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       48 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/models.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.618458 django-codenerix-4.0.9/codenerix/multi_email_field/tests/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       17 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/tests/__init__.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      248 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/tests/models.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6114 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/tests/tests.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      899 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multi_email_field/widgets.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13329 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/multiforms.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.590458 django-codenerix-4.0.9/codenerix/static/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.618458 django-codenerix-4.0.9/codenerix/static/codenerix/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.618458 django-codenerix-4.0.9/codenerix/static/codenerix/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8874 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/css/base.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1863 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/css/lists.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.618458 django-codenerix-4.0.9/codenerix/static/codenerix/img/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2027 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/check_green.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    30435 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/codenerix.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4852 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/codenerix_small.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1183 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/false.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2191 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/ko_red.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7634 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/loader.gif
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   120630 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/ok.gif
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1075 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/true.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12451 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/img/warning.gif
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.622458 django-codenerix-4.0.9/codenerix/static/codenerix/js/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.622458 django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      682 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/app.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      988 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/base.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   138815 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/codenerix.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5487 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/controllers.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6505 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/filters.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18438 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/inotify.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9291 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/notify.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      686 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/js/rows.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.626459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/1.5.7
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   150696 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25635 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    70647 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    15217 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3924 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8584 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1447 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3388 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      343 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-csp.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17205 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1729 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3838 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    37833 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10306 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    28130 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27897 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2990 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8020 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   108145 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-mocks.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    58196 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21780 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    60234 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    34965 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4509 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11002 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    38728 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4762 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12192 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25757 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5867 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10050 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1504143 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-scenario.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    26512 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3940 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10852 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1174125 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   159127 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   428107 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.min.js.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9444 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/errors.json
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.774463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2535 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-dj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2534 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2535 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2532 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2330 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-na.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2339 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2333 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4028 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4022 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3175 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak-gh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3169 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3243 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3237 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4165 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-001.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4159 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ae.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-bh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4149 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-il.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-iq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-jo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4159 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-km.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-kw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4410 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-lb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4150 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ly.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4059 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4106 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-mr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-om.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4409 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ps.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-qa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4160 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-so.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4163 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ss.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-td.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-tn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4161 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ye.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4157 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4244 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4238 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2742 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast-es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2772 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3930 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl-az.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3924 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2503 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn-az.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2497 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2487 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3310 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3304 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4087 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be-by.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4081 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2791 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem-zm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2785 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3089 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3083 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3783 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg-bg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3777 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2839 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn-ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2833 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2321 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4207 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-bd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4207 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4201 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5745 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-cn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5745 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br-fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2734 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4426 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4420 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4412 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl-ba.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4406 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3025 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn-ba.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3019 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3009 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3067 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3064 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-ad.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2832 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es-valencia.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2814 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-it.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2808 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2868 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3417 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr-us.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3411 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4865 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-iq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4866 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-ir.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4859 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4855 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-iq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4856 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-ir.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4865 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn-iq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4859 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4849 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3056 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs-cz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3050 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2548 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy-gb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2542 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2949 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-dk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2949 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-gl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2943 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3054 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3048 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2772 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-at.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-be.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2754 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-li.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2757 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-lu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2776 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje-ne.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2891 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb-de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2885 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3324 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3318 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo-sn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5542 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz-bt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5536 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3070 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3064 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-gh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-tg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2917 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-cy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-gr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4099 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-001.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2728 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-150.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ag.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ai.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-as.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-au.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-be.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2716 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2714 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ca.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ck.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cx.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2706 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-hk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2718 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ie.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-im.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-io.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-iso.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-je.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-jm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ki.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-kn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ky.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ls.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mp.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ms.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2718 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-my.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-na.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ng.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ph.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-rw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2708 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2715 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ss.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2713 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sx.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2711 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-to.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-um.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-us.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ws.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2719 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2712 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2710 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2706 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2753 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo-001.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2402 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-419.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ar.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-bo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-co.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2405 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-do.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ea.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ec.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2395 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-hn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ic.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2389 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-mx.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ni.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pe.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ph.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2413 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-py.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-sv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2394 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-us.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-uy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ve.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2403 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2810 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et-ee.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2804 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2383 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu-es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2377 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3409 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3403 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3786 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-af.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3883 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-ir.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3877 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-gn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-mr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-sn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2961 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi-fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2955 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2848 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil-ph.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2842 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2799 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo-fo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2793 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2454 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-be.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ca.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ci.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ga.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gp.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ht.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-km.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2454 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-lu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-nc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ne.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-re.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2455 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-rw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-td.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-vu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2457 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-wf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2459 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-yt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur-it.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy-nl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2742 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga-ie.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2735 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2998 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd-gb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2992 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2761 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl-es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2755 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2407 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2410 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2407 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-li.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2401 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3938 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3932 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2738 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2866 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv-im.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2860 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-gh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ne.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ng.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2404 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw-us.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2398 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4351 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he-il.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4345 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3666 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3660 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3059 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-ba.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3059 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-hr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3053 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2893 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb-de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2887 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2577 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu-hu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2571 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4029 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy-am.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4023 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2497 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia-fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2494 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2244 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id-id.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2238 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2906 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig-ng.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2900 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3069 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii-cn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3063 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2238 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3170 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is-is.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3164 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-it.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2751 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-sm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4345 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_iw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2513 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja-jp.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2507 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4762 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4756 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4030 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka-ge.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4024 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2887 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab-dz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2881 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3110 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3104 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3154 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3148 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea-cv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2758 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq-ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3028 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3022 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3973 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl-kz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3967 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3957 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3229 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3223 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2873 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl-gl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2867 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2841 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2835 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3784 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km-kh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3778 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4001 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3995 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2534 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kp.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2532 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2526 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4531 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4525 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4288 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4282 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4272 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2725 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3904 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3898 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2911 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh-de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2905 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2784 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw-gb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl-kg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3868 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3858 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3198 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3192 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2822 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb-lu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2816 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2759 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2753 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4132 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt-us.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4126 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3223 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-ao.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3225 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3219 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3833 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo-la.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3827 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3112 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt-lt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3106 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2977 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu-cd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2971 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2952 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3177 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv-lv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3171 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3513 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3513 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3507 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2829 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2694 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe-mu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2688 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2733 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg-mg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2727 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3010 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh-mz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3004 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3305 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3299 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4277 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk-mk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4271 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4111 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4105 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4985 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl-mn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4979 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4969 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3879 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3873 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2246 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-bn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2240 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-my.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2239 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-sg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2234 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2224 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2571 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt-mt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2565 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3078 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3072 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4025 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my-mm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4019 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3193 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq-na.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3187 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-sj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2348 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2768 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd-zw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2762 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4023 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4019 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-np.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4013 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-aw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-be.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-bq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-cw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-nl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sx.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2740 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3312 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3306 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2754 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn-no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2748 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4536 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4530 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2354 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no-no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2348 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2465 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2462 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2464 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2461 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3111 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus-sd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3105 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2868 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2747 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2746 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3827 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3821 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4295 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ge.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4311 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4289 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3491 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab-pk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3485 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3608 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3602 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3592 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3117 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl-pl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3111 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4044 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps-af.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4038 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2452 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-ao.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2435 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-br.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-cv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-gw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2453 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2456 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-pt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2452 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-st.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2451 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-tl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2429 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-bo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2822 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-ec.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2824 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-pe.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2818 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2781 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2775 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2811 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn-bi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2805 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2913 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-md.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2913 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-ro.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2907 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2952 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2946 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-by.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4373 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4370 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-md.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4386 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4377 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ua.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4380 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2780 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw-rw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4659 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah-ru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4653 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2967 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2961 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2800 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3194 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3174 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3174 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-se.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3168 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2750 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh-mz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2744 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2771 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses-ml.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2765 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2989 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg-cf.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2983 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2824 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2818 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4088 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4082 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4072 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4562 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si-lk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4556 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2965 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk-sk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2959 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2973 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl-si.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2967 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2957 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn-fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2951 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn-zw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-dj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2928 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2927 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-so.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2921 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-al.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2406 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-mk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2409 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-xk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2400 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4377 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-ba.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4381 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-me.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4378 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-rs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4381 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-xk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4372 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3004 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-ba.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3008 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-me.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3005 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-rs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3008 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-xk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2999 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4362 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2485 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-sz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2483 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2480 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2539 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2536 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2302 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-ls.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2302 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2299 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-ax.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2774 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2770 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-se.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2764 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2862 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-cd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2749 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2743 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2643 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc-cd.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2640 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3808 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3804 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-lk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3804 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-my.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3803 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-sg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3802 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3921 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3915 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ke.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2806 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2800 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3150 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl-tj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3150 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3142 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4009 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th-th.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4003 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3561 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3658 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3652 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3023 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig-er.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3020 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2840 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2482 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-bw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2482 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2479 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2924 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to-to.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2918 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2423 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-cy.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2419 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-tr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2413 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2505 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2502 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2775 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq-ne.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2769 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2839 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2833 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2823 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4557 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab-cn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4551 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4541 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4551 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk-ua.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4545 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4103 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-in.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4095 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-pk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4089 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3385 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab-af.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3379 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3432 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl-uz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3426 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2323 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn-uz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2317 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2307 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2923 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn-lr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2917 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3334 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii-lr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3328 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3318 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2552 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2549 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2570 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi-vn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2564 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2499 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo-001.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2495 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2737 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun-tz.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2731 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2931 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae-ch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2925 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2909 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal-et.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2906 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2289 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2286 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2784 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog-ug.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2778 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3649 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav-cm.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3643 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4593 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi-001.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4585 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3772 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-bj.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3883 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-ng.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3877 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4084 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh-ma.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4078 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2735 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-cn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-cn.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2728 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-hk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2730 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-mo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2732 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-sg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2564 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-hk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2566 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-mo.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2591 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-tw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2585 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2554 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2581 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-tw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2729 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2352 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu-za.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2346 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/version.json
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        5 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/version.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2213 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-base64-upload.README.md
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1210 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-base64-upload.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1087 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/MIT-LICENSE.txt
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17070 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/colorpicker.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1739 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/alpha.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      506 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/hue.png
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8045 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/saturation.png
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    17309 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/bootstrap-colorpicker-module.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-switch/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10535 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3139 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      516 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-tabcollapse.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4411 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-checklist-model.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1083 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/LICENSE.md
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6890 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2870 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4117 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6767 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker-bs3.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    53679 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1852 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    53486 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1352 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10255 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.638459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/0.5.0
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2915 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9338 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2458 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2841 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.642459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/1.0.9
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   465874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)  1049182 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   315974 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   348054 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.650459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1516 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/LICENSE
+-rwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)     7594 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/ng-quill.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3321 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/ng-quill.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    22075 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.bubble.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8084 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.core.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   265094 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.core.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   393984 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   195286 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    22726 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.snow.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.650459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1072 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/LICENSE
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14018 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3788 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.654459 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   169870 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    32440 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4502 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/datetimepicker.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6880 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    92332 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4709 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    41590 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   240020 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   110343 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   212215 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    87132 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    72592 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-utils.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23346 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-utils.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.774463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/3.3.6
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.786464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    26132 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    47706 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23409 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5532 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   146082 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   389227 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   121260 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    54416 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.786464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    20127 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   108738 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    45404 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    23424 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18028 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.786464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    68954 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    36868 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      484 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/npm.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.586457 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.774463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12351 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11288 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.min.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.774463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    57397 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    35872 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.782463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      940 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ar.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.bg.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      677 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ca.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      789 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.cs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      690 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.da.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      714 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.de.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      776 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ee.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      928 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.el.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      685 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.es.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      726 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fi.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      727 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      807 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.he.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      631 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      726 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hu.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      647 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.id.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      747 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.is.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      736 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.it.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      679 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ja.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      765 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ko.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      805 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      770 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      659 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ms.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      701 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nb.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      681 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      678 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.no.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      741 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      711 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt-BR.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      745 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      714 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ro.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      679 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs-latin.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      873 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      904 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ru.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      731 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      682 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sl.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      688 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sv.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      811 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sw.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1046 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.th.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      685 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.tr.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      874 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ua.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      927 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.uk.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      813 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-CN.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      813 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-TW.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4725 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-dropdowns-functions.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      469 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-helper.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.782463 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6352 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    25205 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5612 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14326 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4656 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-tabcollapse.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1136 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-vertical-grid.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      897 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/color-contrast.README.md
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1059 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/color-contrast.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      488 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/file_validation.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.590458 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.790464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    37414 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21778 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css.map
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    31000 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.min.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.790464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   134808 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/FontAwesome.otf
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   165742 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   444379 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   165548 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    98024 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    77160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.786464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome-animation/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    33218 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18429 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.min.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2380 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/html5shiv.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.790464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/htmlclean/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    24436 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12726 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.794464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   247351 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    84245 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   127335 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.min.map
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.794464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/moment/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   139009 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/moment/moment.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    58686 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/moment/moment.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.794464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/notifyjs/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    21577 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/notifyjs/notify.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    13637 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/notifyjs/notify.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.794464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7982 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/README.md
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6404 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/nspopover.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    16602 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/nspopover.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.794464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/rangy/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   161315 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/rangy/rangy-core.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9546 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/rangy/rangy-selectionsaverestore.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      820 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/sticky-footer-navbar.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      713 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/sticky-footer.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    50498 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-rangy.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    27842 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7717 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3876 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   130358 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    70592 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.min.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    31999 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngularSetup.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      898 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/logs_rows.html
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/static/codenerix/partials/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      746 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/detail.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18799 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/list.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1478 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/rows.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1523 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/summary.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8384 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/static/codenerix/partials/table.html
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.590458 django-codenerix-4.0.9/codenerix/static/djangular/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/static/djangular/css/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      160 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/djangular/css/bootstrap3.css
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      703 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/djangular/css/styles.css
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/static/djangular/js/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    24374 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/djangular/js/django-angular.js
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7396 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/static/djangular/js/django-angular.min.js
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.798464 django-codenerix-4.0.9/codenerix/templates/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14466 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templates/.session.vim
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.802464 django-codenerix-4.0.9/codenerix/templates/codenerix/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2959 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/add.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1664 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/addmodal.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9567 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/details.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      815 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/detailsmodal.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3861 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/detailsmodal_log.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    47851 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/form.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3127 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/formmodal.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2112 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/list.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1984 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/listmodal.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1557 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/remote_log.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1888 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/sublist.html
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2790 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templates/codenerix/sublistmodal.html
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.802464 django-codenerix-4.0.9/codenerix/templatetags/
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.802464 django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1102 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/__init__.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.802464 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      143 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      164 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7959 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_common.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7429 2022-05-17 13:45:50.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_common.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7436 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_lists.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6850 2022-05-17 13:45:49.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_lists.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3297 2022-05-17 11:43:27.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_special.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3948 2022-05-27 10:32:58.000000 django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_special.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7217 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templatetags/codenerix_common.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8936 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/templatetags/codenerix_lists.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4637 2022-05-27 10:32:55.000000 django-codenerix-4.0.9/codenerix/templatetags/codenerix_special.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1658 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/urls.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)   177977 2022-06-18 16:04:41.000000 django-codenerix-4.0.9/codenerix/views.py
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    38707 2022-05-17 12:10:26.000000 django-codenerix-4.0.9/codenerix/widgets.py
+drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-06-18 21:06:55.806464 django-codenerix-4.0.9/django_codenerix.egg-info/
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14249 2022-06-18 21:06:55.000000 django-codenerix-4.0.9/django_codenerix.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    76651 2022-06-18 21:06:55.000000 django-codenerix-4.0.9/django_codenerix.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-06-18 21:06:55.000000 django-codenerix-4.0.9/django_codenerix.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-05-17 11:43:28.000000 django-codenerix-4.0.9/django_codenerix.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      230 2022-06-18 21:06:55.000000 django-codenerix-4.0.9/django_codenerix.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       10 2022-06-18 21:06:55.000000 django-codenerix-4.0.9/django_codenerix.egg-info/top_level.txt
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2022-06-18 21:06:55.806464 django-codenerix-4.0.9/setup.cfg
+-rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2350 2022-06-18 21:06:52.000000 django-codenerix-4.0.9/setup.py
```

### Comparing `django-codenerix-4.0.8/CHANGELOG` & `django-codenerix-4.0.9/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [4.0.9] - 2022-06-18
+### Changed
+- Dependency system simplified for setup.py and restricted to Django>=4.0.1
+
 ## [4.0.8] - 2022-06-18
 ### Fixed
 - Repaired GenForm that was preventing rendering of forms on specific situations
 
 ## [4.0.7] - 2022-06-18
 ### Fixed
 - "authjson_details" is using DjangoJSONEncoder for json.dumps(), which prevents authjson_details from failing on newer Django.
```

### Comparing `django-codenerix-4.0.8/LICENSE` & `django-codenerix-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/MANIFEST.in` & `django-codenerix-4.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/PKG-INFO` & `django-codenerix-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-codenerix
-Version: 4.0.8
+Version: 4.0.9
 Summary: Codenerix it is a framework that goes on top of Django so it makes easier development and building of ERPs.
 Home-page: https://github.com/codenerix/django-codenerix
 Author: Juanmi Taboada, Juan Soler Ruiz
 Author-email: juanmi@juanmitaboada.com, soleronline@gmail.com
 License: Apache License Version 2.0
 Description: ================
         django-codenerix
```

### Comparing `django-codenerix-4.0.8/README.rst` & `django-codenerix-4.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/authbackend.py` & `django-codenerix-4.0.9/codenerix/authbackend.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/constants.py` & `django-codenerix-4.0.9/codenerix/constants.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/context.py` & `django-codenerix-4.0.9/codenerix/context.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/contrib/haystack_engines.py` & `django-codenerix-4.0.9/codenerix/contrib/haystack_engines.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/debug.py` & `django-codenerix-4.0.9/codenerix/debug.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__init__.py` & `django-codenerix-4.0.9/codenerix/djng/__init__.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/__init__.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/__init__.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/__init__.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_base.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_base.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_base.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_model.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_model.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_model.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_validation.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_validation.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/angular_validation.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/angular_validation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/field_mixins.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/field_mixins.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/__pycache__/field_mixins.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/djng/__pycache__/field_mixins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/angular_base.py` & `django-codenerix-4.0.9/codenerix/djng/angular_base.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/angular_model.py` & `django-codenerix-4.0.9/codenerix/djng/angular_model.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/angular_validation.py` & `django-codenerix-4.0.9/codenerix/djng/angular_validation.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/field_mixins.py` & `django-codenerix-4.0.9/codenerix/djng/field_mixins.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/djng/widgets.py` & `django-codenerix-4.0.9/codenerix/djng/widgets.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/exceptions.py` & `django-codenerix-4.0.9/codenerix/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/fields.py` & `django-codenerix-4.0.9/codenerix/fields.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/forms.py` & `django-codenerix-4.0.9/codenerix/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/helpers.py` & `django-codenerix-4.0.9/codenerix/helpers.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/.ropeproject/config.py` & `django-codenerix-4.0.9/codenerix/lib/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/colors.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/colors.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/colors.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/colors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/debugger.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/debugger.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/debugger.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/debugger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/genmail.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/genmail.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/__pycache__/genmail.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/lib/__pycache__/genmail.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/colors.py` & `django-codenerix-4.0.9/codenerix/lib/colors.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/debugger.py` & `django-codenerix-4.0.9/codenerix/lib/debugger.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/genmail.py` & `django-codenerix-4.0.9/codenerix/lib/genmail.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/helpers.py` & `django-codenerix-4.0.9/codenerix/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/lib/pylock.py` & `django-codenerix-4.0.9/codenerix/lib/pylock.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/locale/en/LC_MESSAGES/django.po` & `django-codenerix-4.0.9/codenerix/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/locale/es/LC_MESSAGES/django.mo` & `django-codenerix-4.0.9/codenerix/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/locale/es/LC_MESSAGES/django.po` & `django-codenerix-4.0.9/codenerix/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/.ropeproject/config.py` & `django-codenerix-4.0.9/codenerix/management/commands/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/clean.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/clean.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/colors.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/colors.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/locales.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/locales.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/locales.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/locales.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/refresh_permissions.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/refresh_permissions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/__pycache__/touch.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/management/commands/__pycache__/touch.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/check_dependencies.py` & `django-codenerix-4.0.9/codenerix/management/commands/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/clean.py` & `django-codenerix-4.0.9/codenerix/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/clean_memcache.py` & `django-codenerix-4.0.9/codenerix/management/commands/clean_memcache.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/colors.py` & `django-codenerix-4.0.9/codenerix/management/commands/colors.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/locales.py` & `django-codenerix-4.0.9/codenerix/management/commands/locales.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/refresh_permissions.py` & `django-codenerix-4.0.9/codenerix/management/commands/refresh_permissions.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/management/commands/touch.py` & `django-codenerix-4.0.9/codenerix/management/commands/touch.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/middleware.py` & `django-codenerix-4.0.9/codenerix/middleware.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0001_initial.py` & `django-codenerix-4.0.9/codenerix/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0012_auto_20170405_0815.py` & `django-codenerix-4.0.9/codenerix/migrations/0012_auto_20170405_0815.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0013_auto_20170410_1429.py` & `django-codenerix-4.0.9/codenerix/migrations/0013_auto_20170410_1429.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0014_auto_20170418_1011.py` & `django-codenerix-4.0.9/codenerix/migrations/0014_auto_20170418_1011.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0015_auto_20170418_1515.py` & `django-codenerix-4.0.9/codenerix/migrations/0015_auto_20170418_1515.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0016_auto_20170419_1533.py` & `django-codenerix-4.0.9/codenerix/migrations/0016_auto_20170419_1533.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0017_auto_20170428_0850.py` & `django-codenerix-4.0.9/codenerix/migrations/0017_auto_20170428_0850.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0020_remotelog.py` & `django-codenerix-4.0.9/codenerix/migrations/0020_remotelog.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/0021_auto_20171218_1039.py` & `django-codenerix-4.0.9/codenerix/migrations/0021_auto_20171218_1039.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0002_auto_20160808_0843.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0003_auto_20160817_1235.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0004_auto_20160824_0757.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0005_auto_20160824_1332.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0006_auto_20160825_0838.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0007_corporateimage.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0007_corporateimage.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0008_auto_20170119_1526.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0009_delete_corporateimage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0012_auto_20170405_0815.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0013_auto_20170410_1429.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0014_auto_20170418_1011.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0015_auto_20170418_1515.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0016_auto_20170419_1533.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0017_auto_20170428_0850.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0018_log_snapshot_txt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0019_auto_20170725_1822.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0020_remotelog.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0020_remotelog.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0020_remotelog.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0020_remotelog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/migrations/__pycache__/0021_auto_20171218_1039.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/mixins.py` & `django-codenerix-4.0.9/codenerix/mixins.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/models.py` & `django-codenerix-4.0.9/codenerix/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/models_people.py` & `django-codenerix-4.0.9/codenerix/models_people.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/forms.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/forms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/__pycache__/widgets.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/multi_email_field/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/fields.py` & `django-codenerix-4.0.9/codenerix/multi_email_field/fields.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/forms.py` & `django-codenerix-4.0.9/codenerix/multi_email_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/tests/tests.py` & `django-codenerix-4.0.9/codenerix/multi_email_field/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multi_email_field/widgets.py` & `django-codenerix-4.0.9/codenerix/multi_email_field/widgets.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/multiforms.py` & `django-codenerix-4.0.9/codenerix/multiforms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/css/base.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/css/base.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/css/lists.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/css/lists.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/check_green.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/check_green.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/codenerix.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/codenerix.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/codenerix_small.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/codenerix_small.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/false.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/false.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/ko_red.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/ko_red.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/loader.gif` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/loader.gif`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/ok.gif` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/ok.gif`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/true.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/true.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/img/warning.gif` & `django-codenerix-4.0.9/codenerix/static/codenerix/img/warning.gif`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/.ropeproject/config.py` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/app.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/app.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/base.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/base.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/codenerix.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/codenerix.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/controllers.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/controllers.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/filters.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/filters.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/inotify.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/inotify.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/notify.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/notify.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/js/rows.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/js/rows.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-animate.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-animate.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-aria.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-aria.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-cookies.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-cookies.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-loader.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-loader.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-message-format.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-message-format.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-messages.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-messages.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-mocks.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-mocks.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-parse-ext.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-resource.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-resource.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-route.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-route.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-sanitize.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-scenario.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-scenario.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular-touch.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular-touch.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/angular.min.js.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/angular.min.js.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/errors.json` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/errors.json`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-dj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-dj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_aa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-na.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-na.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_af.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_agq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak-gh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak-gh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ak.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_am.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-001.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-001.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ae.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ae.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-bh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-bh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-dz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-eh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-il.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-il.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-iq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-iq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-jo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-jo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-km.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-km.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-kw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-kw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-lb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-lb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ly.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ly.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-mr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-mr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-om.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-om.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ps.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ps.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-qa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-qa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-so.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-so.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ss.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ss.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-sy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-td.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-td.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-tn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-tn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ye.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar-ye.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ar.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_as.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_asa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast-es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast-es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ast.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl-az.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl-az.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn-az.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn-az.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_az.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bas.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be-by.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be-by.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_be.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem-zm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem-zm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bem.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bez.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg-bg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg-bg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn-ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn-ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm-ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-bd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-bd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-cn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-cn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br-fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br-fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_br.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_brx.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl-ba.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl-ba.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn-ba.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn-ba.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_bs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_byn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-ad.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-ad.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es-valencia.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es-valencia.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-it.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca-it.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ca.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cgg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr-us.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr-us.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_chr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-iq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-iq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-ir.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab-ir.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-arab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-iq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-iq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-ir.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-ir.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn-iq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn-iq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ckb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs-cz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs-cz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy-gb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy-gb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_cy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-dk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-dk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-gl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da-gl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_da.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dav.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-at.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-at.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-be.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-be.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-li.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-li.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-lu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de-lu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje-ne.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje-ne.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dje.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb-de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb-de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dsb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dua.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo-sn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo-sn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dyo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz-bt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz-bt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_dz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ebu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-gh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-gh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-tg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee-tg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ee.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-cy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-cy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-gr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el-gr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_el.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-001.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-001.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-150.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-150.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ag.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ag.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ai.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ai.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-as.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-as.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-au.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-au.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-be.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-be.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-bz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ca.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ca.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ck.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ck.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cx.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-cx.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-dm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-fm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-gy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-hk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-hk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ie.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ie.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-im.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-im.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-io.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-io.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-iso.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-iso.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-je.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-je.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-jm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-jm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ki.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ki.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-kn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-kn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ky.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ky.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-lr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ls.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ls.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mp.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mp.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ms.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ms.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-mw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-my.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-my.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-na.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-na.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ng.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ng.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-nz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ph.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ph.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-pw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-rw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-rw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ss.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ss.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sx.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sx.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-sz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-to.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-to.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-um.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-um.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-us.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-us.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-vu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ws.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-ws.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en-zw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_en.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo-001.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo-001.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-419.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-419.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ar.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ar.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-bo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-bo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-co.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-co.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-cu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-do.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-do.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ea.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ea.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ec.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ec.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-gt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-hn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-hn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ic.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ic.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-mx.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-mx.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ni.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ni.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pe.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pe.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ph.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ph.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-pr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-py.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-py.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-sv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-sv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-us.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-us.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-uy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-uy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ve.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es-ve.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et-ee.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et-ee.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu-es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu-es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_eu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ewo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-af.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-af.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-ir.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa-ir.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-gn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-gn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-mr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-mr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-sn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff-sn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ff.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi-fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi-fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil-ph.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil-ph.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fil.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo-fo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo-fo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-be.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-be.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-bl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ca.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ca.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ci.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ci.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-dz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ga.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ga.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gp.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gp.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-gq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ht.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ht.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-km.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-km.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-lu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-lu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-mu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-nc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-nc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ne.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-ne.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-pm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-re.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-re.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-rw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-rw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-sy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-td.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-td.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-tn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-vu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-vu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-wf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-wf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-yt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr-yt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur-it.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur-it.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fur.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy-nl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy-nl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_fy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga-ie.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga-ie.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ga.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd-gb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd-gb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl-es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl-es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-li.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw-li.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gsw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_guz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv-im.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv-im.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_gv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-gh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-gh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ne.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ne.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ng.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn-ng.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ha.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw-us.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw-us.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_haw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he-il.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he-il.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_he.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-ba.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-ba.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-hr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr-hr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb-de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb-de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hsb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu-hu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu-hu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy-am.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy-am.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_hy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia-fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia-fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ia.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id-id.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id-id.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_id.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig-ng.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig-ng.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ig.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii-cn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii-cn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ii.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is-is.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is-is.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_is.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-it.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-it.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-sm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it-sm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_it.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_iw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_iw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja-jp.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja-jp.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ja.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jgo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_jmc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka-ge.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka-ge.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ka.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab-dz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab-dz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kam.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kde.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea-cv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea-cv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kea.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq-ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq-ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_khq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ki.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl-kz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl-kz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kkj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl-gl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl-gl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kln.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km-kh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km-kh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_km.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kp.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kp.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko-kr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ko.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kok.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks-arab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ks.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh-de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh-de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ksh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw-gb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw-gb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_kw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl-kg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl-kg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ky.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lag.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb-lu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb-lu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt-us.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt-us.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lkt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-ao.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-ao.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln-cg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ln.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo-la.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo-la.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt-lt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt-lt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu-cd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu-cd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_luy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv-lv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv-lv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_lv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mas.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mer.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe-mu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe-mu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mfe.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg-mg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg-mg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh-mz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh-mz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mgo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk-mk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk-mk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl-mn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl-mn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-bn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-bn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-my.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-my.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-sg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn-sg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ms.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt-mt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt-mt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_mua.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my-mm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my-mm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_my.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq-na.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq-na.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_naq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-sj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb-sj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd-zw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd-zw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-np.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne-np.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ne.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-aw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-aw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-be.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-be.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-bq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-bq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-cw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-cw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-nl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-nl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sx.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl-sx.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nmg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn-no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn-no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nnh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no-no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no-no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nso.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus-sd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus-sd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nus.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_nyn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_om.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_or.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ge.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ge.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os-ru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_os.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab-pk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab-pk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-arab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa-guru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pa.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl-pl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl-pl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps-af.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps-af.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ps.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-ao.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-ao.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-br.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-br.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-cv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-cv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-gw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-gw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-mz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-pt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-pt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-st.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-st.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-tl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt-tl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_pt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-bo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-bo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-ec.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-ec.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-pe.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu-pe.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_qu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn-bi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn-bi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-md.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-md.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-ro.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro-ro.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ro.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rof.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-by.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-by.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-kz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-md.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-md.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ua.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru-ua.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw-rw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw-rw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_rwk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah-ru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah-ru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sah.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_saq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sbp.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-se.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se-se.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_se.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh-mz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh-mz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_seh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses-ml.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses-ml.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ses.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg-cf.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg-cf.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi-tfng.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_shi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si-lk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si-lk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_si.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk-sk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk-sk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl-si.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl-si.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn-fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn-fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_smn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn-zw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn-zw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-dj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-dj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-so.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so-so.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_so.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-al.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-al.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-mk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-mk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-xk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq-xk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-ba.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-ba.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-me.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-me.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-rs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-rs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-xk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl-xk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-ba.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-ba.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-me.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-me.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-rs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-rs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-xk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn-xk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-sz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-sz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ss.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ssy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-ls.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-ls.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_st.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-ax.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-ax.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-se.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv-se.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-cd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-cd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_sw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc-cd.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc-cd.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_swc.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-lk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-lk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-my.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-my.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-sg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta-sg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ta.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_te.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ke.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ke.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_teo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl-tj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl-tj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th-th.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th-th.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_th.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ti.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig-er.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig-er.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tig.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-bw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-bw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to-to.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to-to.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_to.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-cy.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-cy.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-tr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr-tr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ts.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq-ne.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq-ne.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_twq.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_tzm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab-cn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab-cn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug-arab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk-ua.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk-ua.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-in.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-in.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-pk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur-pk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ur.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab-af.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab-af.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-arab.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl-uz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl-uz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-cyrl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn-uz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn-uz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_uz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn-lr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn-lr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-latn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii-lr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii-lr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai-vaii.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vai.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_ve.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi-vn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi-vn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo-001.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo-001.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun-tz.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun-tz.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_vun.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae-ch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae-ch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wae.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal-et.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal-et.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_wal.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog-ug.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog-ug.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_xog.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav-cm.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav-cm.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yav.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi-001.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi-001.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-bj.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-bj.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-ng.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo-ng.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_yo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh-ma.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh-ma.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zgh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-cn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-cn.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-cn.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-hk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-hk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-mo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-mo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-sg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans-sg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hans.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-hk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-hk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-mo.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-mo.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-tw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant-tw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hant.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-hk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-tw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh-tw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zh.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu-za.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu-za.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular/i18n/angular-locale_zu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-base64-upload.README.md` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-base64-upload.README.md`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-base64-upload.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-base64-upload.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/MIT-LICENSE.txt` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/colorpicker.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/css/colorpicker.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/alpha.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/alpha.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/saturation.png` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/img/saturation.png`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/bootstrap-colorpicker-module.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-colorpicker/js/bootstrap-colorpicker-module.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-switch/angular-bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-bootstrap-tabcollapse.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-bootstrap-tabcollapse.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-checklist-model.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-checklist-model.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/LICENSE.md` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/angular-daterangepicker.min.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker-bs3.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker-bs3.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-daterangepicker/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-hotkeys/hotkeys.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-loading-bar/loading-bar.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-material/angular-material.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-material/angular-material.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/LICENSE` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/ng-quill.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/ng-quill.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/ng-quill.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/ng-quill.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.bubble.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.bubble.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.core.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.core.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.core.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.core.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-quill/quill.snow.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-quill/quill.snow.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/LICENSE` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-recaptcha/angular-recaptcha.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/angular-ui-router.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/datetimepicker.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/datetimepicker.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/select.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/select.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap-tpls.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-utils.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-utils.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/angular-ui/ui-utils.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/angular-ui/ui-utils.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.eot` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.svg` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/css/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ar.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ar.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.bg.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.bg.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ca.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ca.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.cs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.cs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.da.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.da.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.de.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.de.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ee.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ee.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.el.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.el.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.es.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.es.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fi.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fi.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.fr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.he.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.he.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hu.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.hu.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.id.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.id.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.is.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.is.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.it.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.it.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ja.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ja.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ko.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ko.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.lv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ms.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ms.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nb.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nb.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.nl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.no.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.no.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt-BR.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.pt.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ro.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ro.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs-latin.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs-latin.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.rs.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ru.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ru.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sl.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sl.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sw.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.sw.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.th.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.th.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.tr.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.tr.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ua.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.ua.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.uk.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.uk.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-CN.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-TW.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-datetimepicker/js/locales/bootstrap-datetimepicker.zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-dropdowns-functions.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-dropdowns-functions.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-switch/bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-tabcollapse.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-tabcollapse.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/bootstrap-vertical-grid.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/bootstrap-vertical-grid.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/color-contrast.README.md` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/color-contrast.README.md`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/color-contrast.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/color-contrast.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/FontAwesome.otf` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.eot` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.svg` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.ttf` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff2` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.min.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/fontawesome-animation/font-awesome-animation.min.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/html5shiv.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/html5shiv.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/htmlclean/jquery.htmlClean.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/jquery/jquery.min.map` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/moment/moment.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/moment/moment.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/moment/moment.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/notifyjs/notify.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/notifyjs/notify.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/notifyjs/notify.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/notifyjs/notify.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/README.md` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/README.md`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/nspopover.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/nspopover.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/nspopover/nspopover.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/nspopover/nspopover.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/rangy/rangy-core.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/rangy/rangy-core.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/rangy/rangy-selectionsaverestore.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/rangy/rangy-selectionsaverestore.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/sticky-footer-navbar.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/sticky-footer-navbar.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/sticky-footer.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/sticky-footer.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-rangy.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-rangy.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular-sanitize.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.css` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngular.min.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngular.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/lib/textAngular/textAngularSetup.js` & `django-codenerix-4.0.9/codenerix/static/codenerix/lib/textAngular/textAngularSetup.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/logs_rows.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/logs_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/.ropeproject/config.py` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/detail.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/detail.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/list.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/rows.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/summary.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/summary.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/codenerix/partials/table.html` & `django-codenerix-4.0.9/codenerix/static/codenerix/partials/table.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/djangular/css/styles.css` & `django-codenerix-4.0.9/codenerix/static/djangular/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/djangular/js/django-angular.js` & `django-codenerix-4.0.9/codenerix/static/djangular/js/django-angular.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/static/djangular/js/django-angular.min.js` & `django-codenerix-4.0.9/codenerix/static/djangular/js/django-angular.min.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/.session.vim` & `django-codenerix-4.0.9/codenerix/templates/.session.vim`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/add.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/add.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/addmodal.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/addmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/details.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/details.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/detailsmodal.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/detailsmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/detailsmodal_log.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/detailsmodal_log.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/form.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/form.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/formmodal.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/formmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/list.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/listmodal.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/listmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/remote_log.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/remote_log.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/sublist.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templates/codenerix/sublistmodal.html` & `django-codenerix-4.0.9/codenerix/templates/codenerix/sublistmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/config.py` & `django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/.ropeproject/globalnames` & `django-codenerix-4.0.9/codenerix/templatetags/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_common.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_common.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_common.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_lists.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_lists.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_lists.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_lists.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_special.cpython-35.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_special.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/__pycache__/codenerix_special.cpython-39.pyc` & `django-codenerix-4.0.9/codenerix/templatetags/__pycache__/codenerix_special.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/codenerix_common.py` & `django-codenerix-4.0.9/codenerix/templatetags/codenerix_common.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/codenerix_lists.py` & `django-codenerix-4.0.9/codenerix/templatetags/codenerix_lists.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/templatetags/codenerix_special.py` & `django-codenerix-4.0.9/codenerix/templatetags/codenerix_special.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/urls.py` & `django-codenerix-4.0.9/codenerix/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/views.py` & `django-codenerix-4.0.9/codenerix/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/codenerix/widgets.py` & `django-codenerix-4.0.9/codenerix/widgets.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/django_codenerix.egg-info/PKG-INFO` & `django-codenerix-4.0.9/django_codenerix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-codenerix
-Version: 4.0.8
+Version: 4.0.9
 Summary: Codenerix it is a framework that goes on top of Django so it makes easier development and building of ERPs.
 Home-page: https://github.com/codenerix/django-codenerix
 Author: Juanmi Taboada, Juan Soler Ruiz
 Author-email: juanmi@juanmitaboada.com, soleronline@gmail.com
 License: Apache License Version 2.0
 Description: ================
         django-codenerix
```

### Comparing `django-codenerix-4.0.8/django_codenerix.egg-info/SOURCES.txt` & `django-codenerix-4.0.9/django_codenerix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-codenerix-4.0.8/setup.py` & `django-codenerix-4.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 
 with open(os.path.join(os.path.dirname(__file__), "README.rst")) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-requirements = codenerix.__requirements__["all"]
-if sys.version_info[0] < 3:
-    requirements += codenerix.__requirements__["2"]
-else:
-    requirements += codenerix.__requirements__["3"]
-
 setup(
     name="django-codenerix",
     version=codenerix.__version__,
     packages=["codenerix"],
     include_package_data=True,
     zip_safe=False,
     license="Apache License Version 2.0",
@@ -51,9 +45,26 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     # cmdclass={ 'install': CustomInstallCommand, },
-    install_requires=requirements,
+    install_requires=[
+        "pymongo",
+        "python-dateutil",
+        "django-recaptcha>=1.2.1,<1.3",
+        "django-rosetta>=0.9.8",
+        "jsonfield",
+        "openpyxl",
+        "Pillow",
+        "Unidecode",
+        "Django>=4.0.1",
+        "ldap3",
+        "django-haystack>=2.6.1",
+        "pytz",
+        "elasticsearch>=2.0.0,<3.0.0",
+        "django-debug-toolbar==3.2.2",
+        "pyotp",
+        "html5lib",
+    ],
 )
```

