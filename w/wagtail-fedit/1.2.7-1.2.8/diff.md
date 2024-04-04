# Comparing `tmp/wagtail_fedit-1.2.7.tar.gz` & `tmp/wagtail_fedit-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.7.tar", last modified: Thu Apr  4 08:14:21 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.8.tar", last modified: Thu Apr  4 08:37:23 2024, max compression
```

## Comparing `wagtail_fedit-1.2.7.tar` & `wagtail_fedit-1.2.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.167348 wagtail_fedit-1.2.7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-04 08:14:21.167348 wagtail_fedit-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-04 08:14:21.177341 wagtail_fedit-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.768622 wagtail_fedit-1.2.7/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.777622 wagtail_fedit-1.2.7/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.787621 wagtail_fedit-1.2.7/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.788622 wagtail_fedit-1.2.7/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.839636 wagtail_fedit-1.2.7/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.7/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.885638 wagtail_fedit-1.2.7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.7/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.7/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.7/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.927881 wagtail_fedit-1.2.7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1387 2024-04-04 07:56:39.000000 wagtail_fedit-1.2.7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.2.7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.928861 wagtail_fedit-1.2.7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.929860 wagtail_fedit-1.2.7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.752622 wagtail_fedit-1.2.7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.752622 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.944041 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4431 2024-04-03 20:01:24.000000 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.959279 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    12165 2024-04-03 20:03:43.000000 wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.753622 wagtail_fedit-1.2.7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.754622 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.978108 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:20.994114 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.035557 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3270 2024-04-04 08:07:47.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1283 2024-04-03 19:57:11.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1593 2024-04-04 08:07:32.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.055768 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.069982 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.072982 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16924 2024-04-03 19:52:53.000000 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.083980 wagtail_fedit-1.2.7/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.7/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.7/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     8642 2024-04-04 08:12:09.000000 wagtail_fedit-1.2.7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.118991 wagtail_fedit-1.2.7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8783 2024-04-04 08:12:17.000000 wagtail_fedit-1.2.7/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12006 2024-04-04 08:12:00.000000 wagtail_fedit-1.2.7/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.165343 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3204 2024-04-04 07:53:17.000000 wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-04 08:14:21.166343 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-04 08:14:20.000000 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2024-04-04 08:14:20.000000 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 08:14:20.000000 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-04 08:14:20.000000 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-04 08:14:20.000000 wagtail_fedit-1.2.7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.8/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-04 08:37:23.149506 wagtail_fedit-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.886397 wagtail_fedit-1.2.8/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.8/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.917972 wagtail_fedit-1.2.8/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1387 2024-04-04 07:56:39.000000 wagtail_fedit-1.2.8/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      549 2024-04-04 07:11:42.000000 wagtail_fedit-1.2.8/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.950627 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.965635 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4597 2024-04-04 08:36:46.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.999014 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    12165 2024-04-03 20:03:43.000000 wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:22.870274 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.016167 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.021161 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.043715 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     3414 2024-04-04 08:31:26.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1283 2024-04-03 19:57:11.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1593 2024-04-04 08:07:32.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.060784 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.071859 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.074254 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16924 2024-04-03 19:52:53.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.8/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.085223 wagtail_fedit-1.2.8/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.8/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.8/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.8/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.8/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     8857 2024-04-04 08:33:38.000000 wagtail_fedit-1.2.8/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.113138 wagtail_fedit-1.2.8/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8783 2024-04-04 08:12:17.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0    12186 2024-04-04 08:33:10.000000 wagtail_fedit-1.2.8/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-04 07:12:55.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3204 2024-04-04 07:53:17.000000 wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:37:23.136476 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2624 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-04 08:37:22.000000 wagtail_fedit-1.2.8/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.7/LICENSE` & `wagtail_fedit-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/PKG-INFO` & `wagtail_fedit-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.7
+Version: 1.2.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.7/README.md` & `wagtail_fedit-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/setup.cfg` & `wagtail_fedit-1.2.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
+00000030: 380d 0a64 6573 6372 6970 7469 6f6e 203d  8..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.2.7/tests/testapp/manage.py` & `wagtail_fedit-1.2.8/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.8/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.8/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.8/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.8/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.8/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 2% similar despite different names*

```diff
@@ -144,17 +144,22 @@
 #modal-header {
     position: sticky;
     top: 0;
     left: 0;
     right: 0;
     z-index: 100;
 }
+#wagtail-fedit-help-text-section {
+    margin-bottom: 0;
+}
+#wagtail-fedit-help-text-section .w-panel__anchor,
 #wagtail-fedit-editor-section .w-panel__anchor {
     display: none;
 }
+#wagtail-fedit-help-text-section .w-panel__toggle,
 #wagtail-fedit-editor-section .w-panel__toggle {
     align-content: center;
     border-radius: 100%;
     color: var(--w-color-icon-primary);
     display: inline-grid;
     height: 1.5rem;
     justify-content: center;
```

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.8/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,20 @@
         {% block header %}
             <header class="nice-padding" id="modal-header">
                 <h1 id="modal-title">{{ view.get_header_title }}</h1>
             </header>
         {% endblock %}
         <div class="nice-padding">
             {% if help_text %}
-                {% help_block status=help_text.status %}
-                    <p><strong>{{ help_text.title }}</strong></p>
-                    <p>{{ help_text.text }}</p>
-                {% endhelp_block %}
+                {% panel id="wagtail-fedit-help-text" icon="help" heading=help_text.heading %}
+                    {% help_block status=help_text.status %}
+                        <p><strong>{{ help_text.title }}</strong></p>
+                        <p>{{ help_text.text }}</p>
+                    {% endhelp_block %}
+                {% endpanel %}
             {% endif %}
             {% block content %}{% endblock %}
         </div>
     </main>
     <aside>
         <div class="fedit-sidebar-logo">
             {% block sidebar_logo %}{% endblock %}
```

#### html2text {}

```diff
@@ -2,18 +2,20 @@
 static %} {% block titletag %}{{view.get_header_title}}{% endblock %} {% block
 extra_css %} {{ block.super }} {{ form.media.css }}
 {% endblock %} {% block extra_js %}
 {% include "wagtailadmin/pages/_editor_js.html" %} {{ block.super }} {
 { form.media.js }} {% endblock %} {% block furniture %} {% block header %}
 ************ {{{{ vviieeww..ggeett__hheeaaddeerr__ttiittllee }}}} ************
 {% endblock %}
-{% if help_text %} {% help_block status=help_text.status %}
+{% if help_text %} {% panel id="wagtail-fedit-help-text" icon="help"
+heading=help_text.heading %} {% help_block status=help_text.status %}
 {{{{ hheellpp__tteexxtt..ttiittllee }}}}
 {{ help_text.text }}
-{% endhelp_block %} {% endif %} {% block content %}{% endblock %}
+{% endhelp_block %} {% endpanel %} {% endif %} {% block content %}{% endblock
+%}
 {% block sidebar_logo %}{% endblock %}
 {% block sidebar %} {% if admin_edit_url %}
 }" target="_blank"> {% icon name="link-external" %}
 {% endif %}
 }">
 }" viewBox="0 0 16 16">
 }">
```

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.8/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.8/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.8/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.8/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/utils.py` & `wagtail_fedit-1.2.8/wagtail_fedit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,34 +34,38 @@
         ):
             return False
         
         return True
 
 
 class FeditHelpTextMixin:
+    HEADING_SUPPORTS_DRAFTS = _("Publishing Required")
     TITLE_SUPPORTS_DRAFTS = _("The object you are editing supports drafts.")
     TEXT_PUBLISH_DRAFTS = _("You must publish %(model)s to make any changes visible.")
 
+    HEADING_NO_DRAFTS = _("No Publishing Required")
     TITLE_NO_DRAFTS = _("The object you are editing does not support drafts.")
     TEXT_NO_DRAFTS = _("You are not required to publish this object to make this change visible.")
 
 
     def get_help_text(self) -> str:
         # No relations. Maybe draft support.
         if is_draft_capable(self.instance):
             return {
                 "status": "info",
+                "heading": self.HEADING_SUPPORTS_DRAFTS,
                 "title": self.TITLE_SUPPORTS_DRAFTS,
                 "text": mark_safe(self.TEXT_PUBLISH_DRAFTS % {
                     "model": get_model_string(self.instance, publish_url=True, request=self.request),
                 })
             }
         
         return {
             "status": "info",
+            "heading": self.HEADING_NO_DRAFTS,
             "title": self.TITLE_NO_DRAFTS,
             "text": mark_safe(self.TEXT_NO_DRAFTS)
         }
 
 
 def use_related_form(field: models.Field) -> bool:
     for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
```

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.8/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.2.8/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.8/wagtail_fedit/views/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,38 +131,41 @@
     
     def get_help_text(self):
         if is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
                 "status": "info",
+                "heading": _("Publishing required."),
                 "title": _("The objects you are editing support drafts."),
                 "text": mark_safe(_("You must publish %(model)s and the related object of type %(related_verbose_name)s (%(related_model)s) to make any changes visible.") % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                     "related_verbose_name": self.instance._meta.verbose_name,
                     "related_model": get_model_string(self.instance, publish_url=True, request=self.request),
                 })
             }
 
         elif is_draft_capable(self.original_instance)\
                 and not is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
                 "status": "info",
+                "heading": _("Publishing required."),
                 "title": _("The object you are editing supports drafts."),
                 "text": mark_safe(_("You must publish %(model)s to make any changes visible.") % {
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                 })
             }
         
         elif not is_draft_capable(self.original_instance)\
                 and is_draft_capable(self.instance)\
                 and saving_relation(self.instance, self.original_instance):
             return {
                 "status": "info",
+                "heading": _("Publishing related object required."),
                 "title": _("The object you are editing supports drafts."),
                 "text": mark_safe(_("You must publish the related object of type %(type)s (%(model)s) to make any changes visible.") % {
                     "type": self.original_instance._meta.verbose_name,
                     "model": get_model_string(self.original_instance, publish_url=True, request=self.request),
                 })
             }
```

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.2.8/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.8/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.7
+Version: 1.2.8
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.7 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.8 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.8/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

