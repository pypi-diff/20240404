# Comparing `tmp/shopyo-4.9.3.tar.gz` & `tmp/shopyo-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopyo-4.9.3.tar", last modified: Thu Aug 24 12:52:53 2023, max compression
+gzip compressed data, was "shopyo-4.9.4.tar", last modified: Thu Apr  4 05:50:50 2024, max compression
```

## Comparing `shopyo-4.9.3.tar` & `shopyo-4.9.4.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.433329 shopyo-4.9.3/
--rw-r--r--   0 runner    (1001) docker     (999)     1281 2023-08-24 12:52:41.000000 shopyo-4.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      498 2023-08-24 12:52:41.000000 shopyo-4.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     7207 2023-08-24 12:52:53.433329 shopyo-4.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     6115 2023-08-24 12:52:41.000000 shopyo-4.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.397328 shopyo-4.9.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (999)      106 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (999)     5907 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)       51 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (999)     1513 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       88 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (999)     1094 2023-08-24 12:52:41.000000 shopyo-4.9.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1339 2023-08-24 12:52:53.433329 shopyo-4.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      659 2023-08-24 12:52:41.000000 shopyo-4.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.397328 shopyo-4.9.3/shopyo/
--rw-r--r--   0 runner    (1001) docker     (999)      199 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/.test.prod.env
--rw-r--r--   0 runner    (1001) docker     (999)     6270 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)     1447 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1010 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.401328 shopyo-4.9.3/shopyo/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (999)      478 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.401328 shopyo-4.9.3/shopyo/api/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1862 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/assets.py
--rw-r--r--   0 runner    (1001) docker     (999)    17217 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)    16089 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/cli_content.py
--rw-r--r--   0 runner    (1001) docker     (999)    13086 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/cmd.py
--rw-r--r--   0 runner    (1001) docker     (999)    21141 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/cmd_helper.py
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     2197 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/database.py
--rw-r--r--   0 runner    (1001) docker     (999)      188 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/debug.py
--rw-r--r--   0 runner    (1001) docker     (999)     2374 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/email.py
--rw-r--r--   0 runner    (1001) docker     (999)      194 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/enhance.py
--rw-r--r--   0 runner    (1001) docker     (999)     4774 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/file.py
--rw-r--r--   0 runner    (1001) docker     (999)      567 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)     1258 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/html.py
--rw-r--r--   0 runner    (1001) docker     (999)    16838 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/icons.txt
--rw-r--r--   0 runner    (1001) docker     (999)      441 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/info.py
--rw-r--r--   0 runner    (1001) docker     (999)     2735 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/models.py
--rw-r--r--   0 runner    (1001) docker     (999)     2037 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/module.py
--rw-r--r--   0 runner    (1001) docker     (999)      912 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/security.py
--rw-r--r--   0 runner    (1001) docker     (999)      421 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/api/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2641 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)    25839 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (999)     2377 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (999)      166 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (999)     3494 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_email.py
--rw-r--r--   0 runner    (1001) docker     (999)      115 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_enhance.py
--rw-r--r--   0 runner    (1001) docker     (999)     3563 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (999)      466 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (999)      261 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (999)     2012 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (999)     1792 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/api/validators.py
--rw-r--r--   0 runner    (1001) docker     (999)     9237 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/app.py
--rw-r--r--   0 runner    (1001) docker     (999)     9239 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/app.txt
--rw-r--r--   0 runner    (1001) docker     (999)      482 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/autoapp.py.example
--rw-r--r--   0 runner    (1001) docker     (999)     3000 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/config.py
--rw-r--r--   0 runner    (1001) docker     (999)      240 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/config_demo.json
--rw-r--r--   0 runner    (1001) docker     (999)     7242 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)      987 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/init.py
--rw-r--r--   0 runner    (1001) docker     (999)      275 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/appadmin/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      615 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/admin.py
--rw-r--r--   0 runner    (1001) docker     (999)      278 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/info.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.389328 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/
--rw-r--r--   0 runner    (1001) docker     (999)     3340 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/add.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)      268 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)     3119 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html
--rw-r--r--   0 runner    (1001) docker     (999)     2796 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/index.html
--rw-r--r--   0 runner    (1001) docker     (999)     1654 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/appadmin/tests/
--rw-r--r--   0 runner    (1001) docker     (999)    15217 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (999)     6258 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/appadmin/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/auth/
--rw-r--r--   0 runner    (1001) docker     (999)      379 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/info.json
--rw-r--r--   0 runner    (1001) docker     (999)     3998 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/auth/static/
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.389328 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)     1024 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html
--rw-r--r--   0 runner    (1001) docker     (999)     1483 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.405328 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/emails/
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.html
--rw-r--r--   0 runner    (1001) docker     (999)      249 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1028 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/login.html
--rw-r--r--   0 runner    (1001) docker     (999)      928 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/register.html
--rw-r--r--   0 runner    (1001) docker     (999)      443 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/shop_login.html
--rw-r--r--   0 runner    (1001) docker     (999)      750 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      994 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)     1116 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/test_auth_forms.py
--rw-r--r--   0 runner    (1001) docker     (999)    10645 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/test_auth_functional.py
--rw-r--r--   0 runner    (1001) docker     (999)     8923 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/tests/test_auth_models.py
--rw-r--r--   0 runner    (1001) docker     (999)      563 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/upload.py
--rw-r--r--   0 runner    (1001) docker     (999)     4791 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/auth/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/base/
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/info.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.389328 shopyo-4.9.3/shopyo/modules/box__default/base/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/default_styles.html
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/flashed_messages.html
--rw-r--r--   0 runner    (1001) docker     (999)      376 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/footer.html
--rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/macros.html
--rw-r--r--   0 runner    (1001) docker     (999)     1030 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/resources.html
--rw-r--r--   0 runner    (1001) docker     (999)      399 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/main_base.html
--rw-r--r--   0 runner    (1001) docker     (999)     2611 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/module_base.html
--rw-r--r--   0 runner    (1001) docker     (999)     1337 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/nav_base.html
--rw-r--r--   0 runner    (1001) docker     (999)      759 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/base/view.py
--rw-r--r--   0 runner    (1001) docker     (999)      176 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/box_info.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/dashboard/
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/dashboard/info.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__default/dashboard/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/dashboard/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (999)     1102 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/dashboard/templates/dashboard/index.html
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/dashboard/templates/dashboard/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/dashboard/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1503 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/dashboard/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (999)     2190 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/dashboard/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/i18n/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/global.py
--rw-r--r--   0 runner    (1001) docker     (999)      274 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)      222 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/info.json
--rw-r--r--   0 runner    (1001) docker     (999)      232 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__default/i18n/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/i18n/templates/i18n/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/i18n/templates/i18n/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/templates/i18n/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/i18n/tests/
--rw-r--r--   0 runner    (1001) docker     (999)       49 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/tests/test_i18n_functional.py
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/tests/test_i18n_models.py
--rw-r--r--   0 runner    (1001) docker     (999)     1299 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/i18n/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.409328 shopyo-4.9.3/shopyo/modules/box__default/page/
--rw-r--r--   0 runner    (1001) docker     (999)      952 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      390 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/info.json
--rw-r--r--   0 runner    (1001) docker     (999)     2245 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__default/page/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/
--rw-r--r--   0 runner    (1001) docker     (999)      611 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/all_pages.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)     3663 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/dashboard_edit.html
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/view_page.html
--rw-r--r--   0 runner    (1001) docker     (999)     4151 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html
--rw-r--r--   0 runner    (1001) docker     (999)     3726 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/page/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/settings/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      461 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/info.json
--rw-r--r--   0 runner    (1001) docker     (999)      438 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__default/settings/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (999)      823 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/edit.html
--rw-r--r--   0 runner    (1001) docker     (999)      777 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/nav.html
--rw-r--r--   0 runner    (1001) docker     (999)      642 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/upload.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/settings/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/theme/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)     1932 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/global.py
--rw-r--r--   0 runner    (1001) docker     (999)      322 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/info.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__default/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/theme/templates/theme/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__default/theme/templates/theme/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)      118 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/templates/theme/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)     2584 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/templates/theme/index.html
--rw-r--r--   0 runner    (1001) docker     (999)     3350 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__default/theme/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/
--rw-r--r--   0 runner    (1001) docker     (999)      154 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/box_info.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/test1/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/global.py
--rw-r--r--   0 runner    (1001) docker     (999)      225 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/info.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/test1/static/
--rw-r--r--   0 runner    (1001) docker     (999)       32 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/static/file.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/box__tests/test1/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/test1/templates/test1/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/test1/templates/test1/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/templates/test1/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/templates/test1/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.413329 shopyo-4.9.3/shopyo/modules/box__tests/test1/tests/
--rw-r--r--   0 runner    (1001) docker     (999)       49 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/tests/test_test1_functional.py
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/tests/test_test1_models.py
--rw-r--r--   0 runner    (1001) docker     (999)      759 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/box__tests/test1/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/resource/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/resource/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      231 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/resource/info.json
--rw-r--r--   0 runner    (1001) docker     (999)     1855 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/resource/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/resource/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/resource/templates/resource/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/resource/templates/resource/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/resource/templates/resource/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)     4345 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/resource/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/global.py
--rw-r--r--   0 runner    (1001) docker     (999)      225 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/info.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/tests/static/
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/static/file.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/tests/templates/tests/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/tests/templates/tests/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/templates/tests/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/templates/tests/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      492 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/tests/test_tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/tests/test_tests_models.py
--rw-r--r--   0 runner    (1001) docker     (999)      759 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/tests/view.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/www/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/forms.py
--rw-r--r--   0 runner    (1001) docker     (999)      191 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/global.py
--rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/info.json
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/modules/www/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/www/templates/www/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/modules/www/templates/www/blocks/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/templates/www/blocks/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/templates/www/index.html
--rw-r--r--   0 runner    (1001) docker     (999)     1307 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/modules/www/view.py
--rw-r--r--   0 runner    (1001) docker     (999)     1379 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/shopyo_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/static/
--rw-r--r--   0 runner    (1001) docker     (999)    34244 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (999)     3937 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (999)    78636 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (999)   144878 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (999)     4291 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/box.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.417328 shopyo-4.9.3/shopyo/static/css/
--rw-r--r--   0 runner    (1001) docker     (999)     5330 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/css/b4vtabs.min.css
--rw-r--r--   0 runner    (1001) docker     (999)      964 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/css/simple_sidebar.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.421328 shopyo-4.9.3/shopyo/static/default/
--rw-r--r--   0 runner    (1001) docker     (999)   213806 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/default/default_product.jpg
--rw-r--r--   0 runner    (1001) docker     (999)  3753798 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/default/default_subcategory.jpg
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.425329 shopyo-4.9.3/shopyo/static/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (999)     1548 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.425329 shopyo-4.9.3/shopyo/static/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (999)    68243 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/all.css
--rw-r--r--   0 runner    (1001) docker     (999)    54457 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/brands.css
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/brands.min.css
--rw-r--r--   0 runner    (1001) docker     (999)    66628 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (999)    53030 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (999)      547 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/regular.css
--rw-r--r--   0 runner    (1001) docker     (999)      491 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/regular.min.css
--rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/solid.css
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/solid.min.css
--rw-r--r--   0 runner    (1001) docker     (999)     7270 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/svg-with-js.css
--rw-r--r--   0 runner    (1001) docker     (999)     4689 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/svg-with-js.min.css
--rw-r--r--   0 runner    (1001) docker     (999)    41032 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/v4-shims.css
--rw-r--r--   0 runner    (1001) docker     (999)    26441 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/css/v4-shims.min.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.429329 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (999)   125320 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (999)   659641 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (999)   125016 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    84568 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (999)    72148 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (999)    34388 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (999)   144371 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (999)    34092 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    16812 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (999)    13608 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (999)   186512 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (999)   815282 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (999)   186228 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (999)    96248 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (999)    74320 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (999)    86659 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/jquery_3.2.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.429329 shopyo-4.9.3/shopyo/static/js/
--rw-r--r--   0 runner    (1001) docker     (999)     1237 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/js/python.js
--rw-r--r--   0 runner    (1001) docker     (999)     8789 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/shopyo.png
--rw-r--r--   0 runner    (1001) docker     (999)    11538 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/shopyo.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/static/themes/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.393328 shopyo-4.9.3/shopyo/static/themes/back/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.429329 shopyo-4.9.3/shopyo/static/themes/back/boogle/
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/back/boogle/info.json
--rw-r--r--   0 runner    (1001) docker     (999)     1066 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/back/boogle/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.429329 shopyo-4.9.3/shopyo/static/themes/back/mistrello/
--rw-r--r--   0 runner    (1001) docker     (999)       64 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/back/mistrello/info.json
--rw-r--r--   0 runner    (1001) docker     (999)     1418 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/back/mistrello/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.397328 shopyo-4.9.3/shopyo/static/themes/front/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.433329 shopyo-4.9.3/shopyo/static/themes/front/blogus/
--rw-r--r--   0 runner    (1001) docker     (999)      428 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/index.html
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/info.json
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/render_demo.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.433329 shopyo-4.9.3/shopyo/static/themes/front/blogus/sections/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/sections/nav.html
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/sections/resources.html
--rw-r--r--   0 runner    (1001) docker     (999)      727 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/static/themes/front/blogus/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.433329 shopyo-4.9.3/shopyo/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)     2121 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (999)      707 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/tests/test_dunder_main.py
--rw-r--r--   0 runner    (1001) docker     (999)      200 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (999)     1133 2023-08-24 12:52:41.000000 shopyo-4.9.3/shopyo/wsgi.py.example
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:52:53.401328 shopyo-4.9.3/shopyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     7207 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    10230 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       46 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-24 12:52:53.000000 shopyo-4.9.3/shopyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-04 05:50:46.000000 shopyo-4.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 05:50:46.000000 shopyo-4.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-04 05:50:50.883421 shopyo-4.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-04 05:50:46.000000 shopyo-4.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.839420 shopyo-4.9.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/tests.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-04 05:50:46.000000 shopyo-4.9.4/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-04 05:50:50.883421 shopyo-4.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 05:50:46.000000 shopyo-4.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.839420 shopyo-4.9.4/shopyo/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/.test.prod.env
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.843420 shopyo-4.9.4/shopyo/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.843420 shopyo-4.9.4/shopyo/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16089 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cli_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/cmd_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/icons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25839 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/api/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/autoapp.py.example
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/config_demo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/add.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.847420 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/appadmin/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/emails/activate_user.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/register.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/shop_login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/auth/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/base/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.851420 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/default_styles.html
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/flashed_messages.html
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/main_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/module_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/nav_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/base/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/box_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/dashboard/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/templates/i18n/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/test_i18n_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/tests/test_i18n_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/i18n/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/page/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.855420 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/all_pages.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/page/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/settings/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.831421 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__default/theme/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/box_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/static/file.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.859420 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/templates/test1/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/test_test1_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/tests/test_test1_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/box__tests/test1/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/resource/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/resource/templates/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/resource/templates/resource/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/templates/resource/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/resource/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/static/file.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/templates/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/templates/tests/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/templates/tests/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/templates/tests/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/tests/test_tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/tests/test_tests_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/tests/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/modules/www/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/templates/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.863420 shopyo-4.9.4/shopyo/modules/www/templates/www/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/templates/www/blocks/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/templates/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/modules/www/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/shopyo_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    78636 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   144878 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/box.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/css/b4vtabs.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/css/simple_sidebar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.867421 shopyo-4.9.4/shopyo/static/default/
+-rw-r--r--   0 runner    (1001) docker     (127)   213806 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/default/default_product.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  3753798 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/default/default_subcategory.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.871420 shopyo-4.9.4/shopyo/static/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.875420 shopyo-4.9.4/shopyo/static/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    68243 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54457 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/brands.css
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/brands.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    66628 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (127)    53030 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/regular.css
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/regular.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/solid.css
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/solid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41032 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26441 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   659641 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144371 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   815282 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/jquery_3.2.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/js/python.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/shopyo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/shopyo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/back/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/themes/back/boogle/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/boogle/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/boogle/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.879420 shopyo-4.9.4/shopyo/static/themes/back/mistrello/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/mistrello/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/back/mistrello/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.835420 shopyo-4.9.4/shopyo/static/themes/front/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/static/themes/front/blogus/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/render_demo.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/sections/resources.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/static/themes/front/blogus/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_dunder_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-04 05:50:46.000000 shopyo-4.9.4/shopyo/wsgi.py.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:50:50.883421 shopyo-4.9.4/shopyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 05:50:50.000000 shopyo-4.9.4/shopyo.egg-info/top_level.txt
```

### Comparing `shopyo-4.9.3/LICENSE` & `shopyo-4.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/PKG-INFO` & `shopyo-4.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopyo
-Version: 4.9.3
+Version: 4.9.4
 Summary: Highly modular web framework built for big apps on top of Flask with Django advantages
 Home-page: https://github.com/shopyo/shopyo
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/shopyo/shopyo/
 Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/issues/
@@ -19,14 +19,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Flask>=2.0.2
+Requires-Dist: Flask-Admin>=1.5.8
+Requires-Dist: Flask-Login>=0.5.0
+Requires-Dist: flask-mailman>=0.3.0
+Requires-Dist: Flask-Migrate>=3.1.0
+Requires-Dist: Flask-SQLAlchemy>=2.5.1
+Requires-Dist: Flask-WTF>=1.0.0
+Requires-Dist: SQLAlchemy>=1.4.27
+Requires-Dist: Werkzeug>=2.0.2
+Requires-Dist: WTForms>=3.0.0
+Requires-Dist: email-validator
 
 <h1 align="center">
   <br>
   <a href="https://github.com/shopyo"><img src="https://github.com/shopyo/shopyo/blob/dev/assets/github_banner.png" alt="shopyo" width="" height=""></a>
 
 </h1>
 
@@ -74,25 +85,25 @@
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new -m # add default modules
 cd blog
 shopyo initialise
-shopyo run
+flask run --debug
 ```
 
 
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new
 cd blog
-shopyo run
+flask run --debug
 ```
 
 If errors do (linux, use `set <VAR>` for Windows):
 
 ```
 export SHOPYO_CONFIG_PROFILE=development
 export FLASK_ENV=development # < flask 2.2.x
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: shopyo Version: 4.9.3 Summary: Highly modular web
+Metadata-Version: 2.1 Name: shopyo Version: 4.9.4 Summary: Highly modular web
 framework built for big apps on top of Flask with Django advantages Home-page:
 https://github.com/shopyo/shopyo Author: Abdur-Rahmaan Janhangeer Author-email:
 arj.python@gmail.com License: MIT Project-URL: Source Code, https://github.com/
 shopyo/shopyo/ Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/
 issues/ Project-URL: Changelog, https://github.com/shopyo/shopyo/blob/dev/
 CHANGES.md/ Project-URL: Twitter, https://twitter.com/shopyoproject/ Keywords:
 Flask,Django,web framework,modular Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers Classifier: Development Status :: 4
 - Beta Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE
+File: LICENSE Requires-Dist: Flask>=2.0.2 Requires-Dist: Flask-Admin>=1.5.8
+Requires-Dist: Flask-Login>=0.5.0 Requires-Dist: flask-mailman>=0.3.0 Requires-
+Dist: Flask-Migrate>=3.1.0 Requires-Dist: Flask-SQLAlchemy>=2.5.1 Requires-
+Dist: Flask-WTF>=1.0.0 Requires-Dist: SQLAlchemy>=1.4.27 Requires-Dist:
+Werkzeug>=2.0.2 Requires-Dist: WTForms>=3.0.0 Requires-Dist: email-validator
                                     ************
                                 _[[_ss_hh_oo_pp_yy_oo_]] ************
 [![Downloads](https://static.pepy.tech/badge/shopyo/month)](https://pepy.tech/
 project/shopyo) [![Codecov](https://codecov.io/gh/shopyo/shopyo/branch/dev/
 graph/badge.svg?token=J4TL2MDTSS)](https://codecov.io/gh/shopyo/shopyo) !
 [Tests](https://github.com/shopyo/shopyo/actions/workflows/tests.yaml/
 badge.svg) [![PyPI version shields.io](https://img.shields.io/pypi/v/
@@ -45,21 +49,21 @@
 | Testing, docs etc are covered. Don't make those afterthoughts. | | ð§ Ease
 your life | We've been there. Awesome utils to ease development. | | ðª
 Scaffolding | Don't waste time writing boilerplate code. We've got you covered.
 | | ðï¸ Theming system | You need theme in your apps? We integrate a
 default theme system. | # Features - âï¸ i18n setup - ð Login & Auth -
 ð§ Email - ð¦ 2-level modularity - ðª Designed for really BIG apps - ð
 Assets management # Quick start ```bash pip install shopyo==4.9.3 mkdir blog cd
-blog shopyo new -m # add default modules cd blog shopyo initialise shopyo run
-``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd blog
-shopyo run ``` If errors do (linux, use `set ` for Windows): ``` export
-SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask 2.2.x
-export ENV=development export FLASK_DEBUG=development # < flask 2.2.x export
-FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys of
-`app_config` in `config.py` It is recommended to use a venv in root folder.
+blog shopyo new -m # add default modules cd blog shopyo initialise flask run --
+debug ``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd
+blog flask run --debug ``` If errors do (linux, use `set ` for Windows): ```
+export SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask
+2.2.x export ENV=development export FLASK_DEBUG=development # < flask 2.2.x
+export FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys
+of `app_config` in `config.py` It is recommended to use a venv in root folder.
 `python -m venv venv` If for dev install dev_requirements.txt also. `python -
 m pip install -r requirements/dev.txt` go to http://127.0.0.1:5000/dashboard
 with credentials admin@domain.com / pass ![](https://github.com/shopyo/shopyo/
 blob/dev/comparison.png) - Not framework docs but docs for the project you are
 building. # First time contributing? We have a 100% first-timers friendly
 policy. Check out the [testimonials](https://github.com/shopyo/shopyo/
 discussions/307). > Thank you! One of the best onboarding experiences I've had.
```

### Comparing `shopyo-4.9.3/README.md` & `shopyo-4.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,25 @@
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new -m # add default modules
 cd blog
 shopyo initialise
-shopyo run
+flask run --debug
 ```
 
 
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new
 cd blog
-shopyo run
+flask run --debug
 ```
 
 If errors do (linux, use `set <VAR>` for Windows):
 
 ```
 export SHOPYO_CONFIG_PROFILE=development
 export FLASK_ENV=development # < flask 2.2.x
```

#### html2text {}

```diff
@@ -30,21 +30,21 @@
 | Testing, docs etc are covered. Don't make those afterthoughts. | | ð§ Ease
 your life | We've been there. Awesome utils to ease development. | | ðª
 Scaffolding | Don't waste time writing boilerplate code. We've got you covered.
 | | ðï¸ Theming system | You need theme in your apps? We integrate a
 default theme system. | # Features - âï¸ i18n setup - ð Login & Auth -
 ð§ Email - ð¦ 2-level modularity - ðª Designed for really BIG apps - ð
 Assets management # Quick start ```bash pip install shopyo==4.9.3 mkdir blog cd
-blog shopyo new -m # add default modules cd blog shopyo initialise shopyo run
-``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd blog
-shopyo run ``` If errors do (linux, use `set ` for Windows): ``` export
-SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask 2.2.x
-export ENV=development export FLASK_DEBUG=development # < flask 2.2.x export
-FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys of
-`app_config` in `config.py` It is recommended to use a venv in root folder.
+blog shopyo new -m # add default modules cd blog shopyo initialise flask run --
+debug ``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd
+blog flask run --debug ``` If errors do (linux, use `set ` for Windows): ```
+export SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask
+2.2.x export ENV=development export FLASK_DEBUG=development # < flask 2.2.x
+export FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys
+of `app_config` in `config.py` It is recommended to use a venv in root folder.
 `python -m venv venv` If for dev install dev_requirements.txt also. `python -
 m pip install -r requirements/dev.txt` go to http://127.0.0.1:5000/dashboard
 with credentials admin@domain.com / pass ![](https://github.com/shopyo/shopyo/
 blob/dev/comparison.png) - Not framework docs but docs for the project you are
 building. # First time contributing? We have a 100% first-timers friendly
 policy. Check out the [testimonials](https://github.com/shopyo/shopyo/
 discussions/307). > Thank you! One of the best onboarding experiences I've had.
```

### Comparing `shopyo-4.9.3/requirements/dev.txt` & `shopyo-4.9.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/requirements/docs.txt` & `shopyo-4.9.4/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/requirements/tests.txt` & `shopyo-4.9.4/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/setup.cfg` & `shopyo-4.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/setup.py` & `shopyo-4.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/CHANGELOG.md` & `shopyo-4.9.4/shopyo/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/__init__.py` & `shopyo-4.9.4/shopyo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-version_info = (4, 9, 3)
+version_info = (4, 9, 4)
 __version__ = ".".join([str(v) for v in version_info])
 
 
 """
+4.9.4
+
+- loosen sqlalchemy requirment; initialize still expected to fail, but package usable
+
 4.9.3
 
 - Remove marshmallow from deps
 
 4.9.2
 
 - Fix missing import
```

### Comparing `shopyo-4.9.3/shopyo/__main__.py` & `shopyo-4.9.4/shopyo/__main__.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/assets.py` & `shopyo-4.9.4/shopyo/api/assets.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/cli.py` & `shopyo-4.9.4/shopyo/api/cli.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/cli_content.py` & `shopyo-4.9.4/shopyo/api/cli_content.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/cmd.py` & `shopyo-4.9.4/shopyo/api/cmd.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/cmd_helper.py` & `shopyo-4.9.4/shopyo/api/cmd_helper.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/database.py` & `shopyo-4.9.4/shopyo/api/database.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/email.py` & `shopyo-4.9.4/shopyo/api/email.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/file.py` & `shopyo-4.9.4/shopyo/api/file.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/forms.py` & `shopyo-4.9.4/shopyo/api/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/html.py` & `shopyo-4.9.4/shopyo/api/html.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/icons.txt` & `shopyo-4.9.4/shopyo/api/icons.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/models.py` & `shopyo-4.9.4/shopyo/api/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/module.py` & `shopyo-4.9.4/shopyo/api/module.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/security.py` & `shopyo-4.9.4/shopyo/api/security.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/conftest.py` & `shopyo-4.9.4/shopyo/api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_cli.py` & `shopyo-4.9.4/shopyo/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_cli_integration.py` & `shopyo-4.9.4/shopyo/api/tests/test_cli_integration.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_email.py` & `shopyo-4.9.4/shopyo/api/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_models.py` & `shopyo-4.9.4/shopyo/api/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_print_info.py` & `shopyo-4.9.4/shopyo/api/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/tests/test_validators.py` & `shopyo-4.9.4/shopyo/api/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/api/validators.py` & `shopyo-4.9.4/shopyo/api/validators.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/app.py` & `shopyo-4.9.4/shopyo/app.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/app.txt` & `shopyo-4.9.4/shopyo/app.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/config.py` & `shopyo-4.9.4/shopyo/config.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/conftest.py` & `shopyo-4.9.4/shopyo/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/init.py` & `shopyo-4.9.4/shopyo/init.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/admin.py` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/add.html` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/add.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/edit.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/index.html` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/templates/appadmin/roles.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/tests/test_admin.py` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/appadmin/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/appadmin/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/forms.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/models.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html` & `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/login_form.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html` & `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/blocks/register_form.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/login.html` & `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/register.html` & `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/register.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html` & `shopyo-4.9.4/shopyo/modules/box__default/auth/templates/auth/unconfirmed.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/tests/conftest.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/tests/factories.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/factories.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/tests/test_auth_functional.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_functional.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/tests/test_auth_models.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/tests/test_auth_models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/upload.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/upload.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/auth/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/auth/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/blocks/resources.html` & `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/blocks/resources.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/module_base.html` & `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/module_base.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/base/templates/base/nav_base.html` & `shopyo-4.9.4/shopyo/modules/box__default/base/templates/base/nav_base.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/base/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/base/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/dashboard/templates/dashboard/index.html` & `shopyo-4.9.4/shopyo/modules/box__default/dashboard/templates/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/dashboard/tests/test_dashboard.py` & `shopyo-4.9.4/shopyo/modules/box__default/dashboard/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/dashboard/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/dashboard/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/i18n/global.py` & `shopyo-4.9.4/shopyo/modules/box__default/i18n/global.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/i18n/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/i18n/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/forms.py` & `shopyo-4.9.4/shopyo/modules/box__default/page/forms.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/models.py` & `shopyo-4.9.4/shopyo/modules/box__default/page/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/all_pages.html` & `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/all_pages.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/dashboard.html` & `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/dashboard.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html` & `shopyo-4.9.4/shopyo/modules/box__default/page/templates/page/view_page_dashboard.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/page/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/page/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/edit.html` & `shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/edit.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/settings/templates/settings/index.html` & `shopyo-4.9.4/shopyo/modules/box__default/settings/templates/settings/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/settings/upload.py` & `shopyo-4.9.4/shopyo/modules/box__default/settings/upload.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/theme/global.py` & `shopyo-4.9.4/shopyo/modules/box__default/theme/global.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/theme/templates/theme/index.html` & `shopyo-4.9.4/shopyo/modules/box__default/theme/templates/theme/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__default/theme/view.py` & `shopyo-4.9.4/shopyo/modules/box__default/theme/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/box__tests/test1/view.py` & `shopyo-4.9.4/shopyo/modules/box__tests/test1/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/resource/models.py` & `shopyo-4.9.4/shopyo/modules/resource/models.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/resource/view.py` & `shopyo-4.9.4/shopyo/modules/resource/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/tests/view.py` & `shopyo-4.9.4/shopyo/modules/tests/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/www/templates/www/index.html` & `shopyo-4.9.4/shopyo/modules/www/templates/www/index.html`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/modules/www/view.py` & `shopyo-4.9.4/shopyo/modules/www/view.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/shopyo_admin.py` & `shopyo-4.9.4/shopyo/shopyo_admin.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/bootstrap-grid.min.css` & `shopyo-4.9.4/shopyo/static/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/bootstrap-reboot.min.css` & `shopyo-4.9.4/shopyo/static/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/bootstrap.bundle.min.js` & `shopyo-4.9.4/shopyo/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/bootstrap.min.css` & `shopyo-4.9.4/shopyo/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/box.svg` & `shopyo-4.9.4/shopyo/static/box.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/css/b4vtabs.min.css` & `shopyo-4.9.4/shopyo/static/css/b4vtabs.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/css/simple_sidebar.css` & `shopyo-4.9.4/shopyo/static/css/simple_sidebar.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/default/default_product.jpg` & `shopyo-4.9.4/shopyo/static/default/default_product.jpg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/default/default_subcategory.jpg` & `shopyo-4.9.4/shopyo/static/default/default_subcategory.jpg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/favicon.ico` & `shopyo-4.9.4/shopyo/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/LICENSE.txt` & `shopyo-4.9.4/shopyo/static/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/all.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/all.min.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/brands.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/fontawesome.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/fontawesome.min.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/regular.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/solid.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/svg-with-js.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/svg-with-js.min.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/v4-shims.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/css/v4-shims.min.css` & `shopyo-4.9.4/shopyo/static/fontawesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.eot` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.svg` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.woff` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.eot` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.svg` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.woff` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.eot` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.svg` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.woff` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2` & `shopyo-4.9.4/shopyo/static/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/jquery_3.2.1.min.js` & `shopyo-4.9.4/shopyo/static/jquery_3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/js/python.js` & `shopyo-4.9.4/shopyo/static/js/python.js`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/shopyo.png` & `shopyo-4.9.4/shopyo/static/shopyo.png`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/shopyo.svg` & `shopyo-4.9.4/shopyo/static/shopyo.svg`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/themes/back/boogle/styles.css` & `shopyo-4.9.4/shopyo/static/themes/back/boogle/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/themes/back/mistrello/styles.css` & `shopyo-4.9.4/shopyo/static/themes/back/mistrello/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/static/themes/front/blogus/styles.css` & `shopyo-4.9.4/shopyo/static/themes/front/blogus/styles.css`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/tests/conftest.py` & `shopyo-4.9.4/shopyo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/tests/test_configs.py` & `shopyo-4.9.4/shopyo/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/tests/test_dunder_main.py` & `shopyo-4.9.4/shopyo/tests/test_dunder_main.py`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo/wsgi.py.example` & `shopyo-4.9.4/shopyo/wsgi.py.example`

 * *Files identical despite different names*

### Comparing `shopyo-4.9.3/shopyo.egg-info/PKG-INFO` & `shopyo-4.9.4/shopyo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopyo
-Version: 4.9.3
+Version: 4.9.4
 Summary: Highly modular web framework built for big apps on top of Flask with Django advantages
 Home-page: https://github.com/shopyo/shopyo
 Author: Abdur-Rahmaan Janhangeer
 Author-email: arj.python@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/shopyo/shopyo/
 Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/issues/
@@ -19,14 +19,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Flask>=2.0.2
+Requires-Dist: Flask-Admin>=1.5.8
+Requires-Dist: Flask-Login>=0.5.0
+Requires-Dist: flask-mailman>=0.3.0
+Requires-Dist: Flask-Migrate>=3.1.0
+Requires-Dist: Flask-SQLAlchemy>=2.5.1
+Requires-Dist: Flask-WTF>=1.0.0
+Requires-Dist: SQLAlchemy>=1.4.27
+Requires-Dist: Werkzeug>=2.0.2
+Requires-Dist: WTForms>=3.0.0
+Requires-Dist: email-validator
 
 <h1 align="center">
   <br>
   <a href="https://github.com/shopyo"><img src="https://github.com/shopyo/shopyo/blob/dev/assets/github_banner.png" alt="shopyo" width="" height=""></a>
 
 </h1>
 
@@ -74,25 +85,25 @@
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new -m # add default modules
 cd blog
 shopyo initialise
-shopyo run
+flask run --debug
 ```
 
 
 ```bash
 pip install shopyo==4.9.3
 mkdir blog
 cd blog
 shopyo new
 cd blog
-shopyo run
+flask run --debug
 ```
 
 If errors do (linux, use `set <VAR>` for Windows):
 
 ```
 export SHOPYO_CONFIG_PROFILE=development
 export FLASK_ENV=development # < flask 2.2.x
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: shopyo Version: 4.9.3 Summary: Highly modular web
+Metadata-Version: 2.1 Name: shopyo Version: 4.9.4 Summary: Highly modular web
 framework built for big apps on top of Flask with Django advantages Home-page:
 https://github.com/shopyo/shopyo Author: Abdur-Rahmaan Janhangeer Author-email:
 arj.python@gmail.com License: MIT Project-URL: Source Code, https://github.com/
 shopyo/shopyo/ Project-URL: Issue Tracker, https://github.com/shopyo/shopyo/
 issues/ Project-URL: Changelog, https://github.com/shopyo/shopyo/blob/dev/
 CHANGES.md/ Project-URL: Twitter, https://twitter.com/shopyoproject/ Keywords:
 Flask,Django,web framework,modular Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers Classifier: Development Status :: 4
 - Beta Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE
+File: LICENSE Requires-Dist: Flask>=2.0.2 Requires-Dist: Flask-Admin>=1.5.8
+Requires-Dist: Flask-Login>=0.5.0 Requires-Dist: flask-mailman>=0.3.0 Requires-
+Dist: Flask-Migrate>=3.1.0 Requires-Dist: Flask-SQLAlchemy>=2.5.1 Requires-
+Dist: Flask-WTF>=1.0.0 Requires-Dist: SQLAlchemy>=1.4.27 Requires-Dist:
+Werkzeug>=2.0.2 Requires-Dist: WTForms>=3.0.0 Requires-Dist: email-validator
                                     ************
                                 _[[_ss_hh_oo_pp_yy_oo_]] ************
 [![Downloads](https://static.pepy.tech/badge/shopyo/month)](https://pepy.tech/
 project/shopyo) [![Codecov](https://codecov.io/gh/shopyo/shopyo/branch/dev/
 graph/badge.svg?token=J4TL2MDTSS)](https://codecov.io/gh/shopyo/shopyo) !
 [Tests](https://github.com/shopyo/shopyo/actions/workflows/tests.yaml/
 badge.svg) [![PyPI version shields.io](https://img.shields.io/pypi/v/
@@ -45,21 +49,21 @@
 | Testing, docs etc are covered. Don't make those afterthoughts. | | ð§ Ease
 your life | We've been there. Awesome utils to ease development. | | ðª
 Scaffolding | Don't waste time writing boilerplate code. We've got you covered.
 | | ðï¸ Theming system | You need theme in your apps? We integrate a
 default theme system. | # Features - âï¸ i18n setup - ð Login & Auth -
 ð§ Email - ð¦ 2-level modularity - ðª Designed for really BIG apps - ð
 Assets management # Quick start ```bash pip install shopyo==4.9.3 mkdir blog cd
-blog shopyo new -m # add default modules cd blog shopyo initialise shopyo run
-``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd blog
-shopyo run ``` If errors do (linux, use `set ` for Windows): ``` export
-SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask 2.2.x
-export ENV=development export FLASK_DEBUG=development # < flask 2.2.x export
-FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys of
-`app_config` in `config.py` It is recommended to use a venv in root folder.
+blog shopyo new -m # add default modules cd blog shopyo initialise flask run --
+debug ``` ```bash pip install shopyo==4.9.3 mkdir blog cd blog shopyo new cd
+blog flask run --debug ``` If errors do (linux, use `set ` for Windows): ```
+export SHOPYO_CONFIG_PROFILE=development export FLASK_ENV=development # < flask
+2.2.x export ENV=development export FLASK_DEBUG=development # < flask 2.2.x
+export FLASK_APP=app.py ``` `SHOPYO_CONFIG_PROFILE` is what is defined as keys
+of `app_config` in `config.py` It is recommended to use a venv in root folder.
 `python -m venv venv` If for dev install dev_requirements.txt also. `python -
 m pip install -r requirements/dev.txt` go to http://127.0.0.1:5000/dashboard
 with credentials admin@domain.com / pass ![](https://github.com/shopyo/shopyo/
 blob/dev/comparison.png) - Not framework docs but docs for the project you are
 building. # First time contributing? We have a 100% first-timers friendly
 policy. Check out the [testimonials](https://github.com/shopyo/shopyo/
 discussions/307). > Thank you! One of the best onboarding experiences I've had.
```

### Comparing `shopyo-4.9.3/shopyo.egg-info/SOURCES.txt` & `shopyo-4.9.4/shopyo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 shopyo/wsgi.py.example
 shopyo.egg-info/PKG-INFO
 shopyo.egg-info/SOURCES.txt
 shopyo.egg-info/dependency_links.txt
 shopyo.egg-info/entry_points.txt
 shopyo.egg-info/requires.txt
 shopyo.egg-info/top_level.txt
-shopyo/__pycache__/__init__.cpython-311.pyc
+shopyo/__pycache__/__init__.cpython-312.pyc
 shopyo/api/__init__.py
 shopyo/api/assets.py
 shopyo/api/cli.py
 shopyo/api/cli_content.py
 shopyo/api/cmd.py
 shopyo/api/cmd_helper.py
 shopyo/api/constants.py
```

