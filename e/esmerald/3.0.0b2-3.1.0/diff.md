# Comparing `tmp/esmerald-3.0.0b2.tar.gz` & `tmp/esmerald-3.1.0.tar.gz`

## Comparing `esmerald-3.0.0b2.tar` & `esmerald-3.1.0.tar`

### file list

```diff
@@ -1,229 +1,230 @@
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/__main__.py
--rw-r--r--   0        0        0    92258 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/applications.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/concurrency.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/enums.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/exceptions.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/injector.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/logging.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/param_functions.py
--rw-r--r--   0        0        0    22300 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/py.typed
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/requests.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/testclient.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/types.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/typing.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/websockets.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/enums.py
--rw-r--r--   0        0        0    47254 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/cors.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/csrf.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/jwt.py
--rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/openapi.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/session.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/static_files.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/edgy/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/edgy/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/edgy/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/mongoz/__init__.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/mongoz/base_user.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/mongoz/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/di/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/di/provider.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/json.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/msgspec.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/cors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/https.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/constants.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/models.py
--rw-r--r--   0        0        0    20509 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/base.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/api_key/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/api_key/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/http/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/http/base.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/oauth2/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/oauth2/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/openid_connect/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/openapi/security/openid_connect/base.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/protocols/template.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/responses/base.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/responses/json.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/base.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/events.py
--rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/gateways.py
--rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/router.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/views.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/_metaclasses.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/_mixins.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/base.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/generics.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/apis/views.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/webhooks/__init__.py
--rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/routing/webhooks/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/signature.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/constants.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/inspect.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/models.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/LICENSE
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/README.md
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    22628 2020-02-02 00:00:00.000000 esmerald-3.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/__main__.py
+-rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/applications.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/concurrency.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/enums.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/exceptions.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/injector.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22300 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/py.typed
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/requests.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/testclient.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/types.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/typing.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/websockets.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    47597 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/cors.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/csrf.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/jwt.py
+-rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/openapi.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/session.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/static_files.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/base_user.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/__init__.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/base_user.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/di/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/di/provider.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/msgspec.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/app_settings.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    20509 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/base.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/api_key/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/http/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/http/base.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/oauth2/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/openid_connect/base.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/events.py
+-rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/router.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/views.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/_metaclasses.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/_mixins.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/base.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/generics.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/views.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/webhooks/__init__.py
+-rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/webhooks/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/constants.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/inspect.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/models.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 esmerald-3.1.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.0/LICENSE
+-rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 esmerald-3.1.0/README.md
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 esmerald-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 esmerald-3.1.0/PKG-INFO
```

### Comparing `esmerald-3.0.0b2/esmerald/__init__.py` & `esmerald-3.1.0/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.0-beta2"
+__version__ = "3.1.0"
 
 
 from lilya import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.context import Context
```

### Comparing `esmerald-3.0.0b2/esmerald/applications.py` & `esmerald-3.1.0/esmerald/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 from datetime import timezone as dtimezone
 from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -19,27 +18,28 @@
 from lilya.middleware import DefineMiddleware  # noqa
 from lilya.types import Lifespan, Receive, Scope, Send
 from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme
 from openapi_schemas_pydantic.v3_1_0.open_api import OpenAPI
 from pydantic import AnyUrl, ValidationError
 from typing_extensions import Annotated, Doc
 
-from esmerald.conf import settings as esmerald_settings
+from esmerald.conf import reload_settings, settings as esmerald_settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.config import CORSConfig, CSRFConfig, SessionConfig
 from esmerald.config.openapi import OpenAPIConfig
 from esmerald.config.static_files import StaticFilesConfig
 from esmerald.datastructures import State
 from esmerald.exception_handlers import (
     improperly_configured_exception_handler,
     pydantic_validation_error_handler,
     validation_error_exception_handler,
 )
 from esmerald.exceptions import ImproperlyConfigured, ValidationErrorException
 from esmerald.interceptors.types import Interceptor
+from esmerald.middleware.app_settings import ApplicationSettingsMiddleware
 from esmerald.middleware.asyncexitstack import AsyncExitStackMiddleware
 from esmerald.middleware.cors import CORSMiddleware
 from esmerald.middleware.csrf import CSRFMiddleware
 from esmerald.middleware.exceptions import EsmeraldAPIExceptionMiddleware, ExceptionMiddleware
 from esmerald.middleware.sessions import SessionMiddleware
 from esmerald.middleware.trustedhost import TrustedHostMiddleware
 from esmerald.permissions.types import Permission
@@ -139,30 +139,14 @@
         "title",
         "version",
     )
 
     def __init__(
         self: AppType,
         *,
-        settings_config: Annotated[
-            Optional["SettingsType"],
-            Doc(
-                """
-                Alternative settings parameter. This parameter is an alternative to
-                `ESMERALD_SETTINGS_MODULE` way of loading your settings into an Esmerald application.
-
-                Read more about the [settings module](https://esmerald.dev/application/settings/)
-                and how you can leverage it in your application.
-
-                !!! Warning
-                    This option will be deprecated in the version 2.9 of Esmerald. Please use
-                    `settings_module` instead.
-                """
-            ),
-        ] = None,
         settings_module: Annotated[
             Optional["SettingsType"],
             Doc(
                 """
                 Alternative settings parameter. This parameter is an alternative to
                 `ESMERALD_SETTINGS_MODULE` way of loading your settings into an Esmerald application.
 
@@ -1478,32 +1462,16 @@
 
                 app = Esmerald(openapi_url="/api/v1/openapi.json")
                 ```
                 """
             ),
         ] = None,
     ) -> None:
-        assert (
-            settings_config is None or settings_module is None
-        ), "You can use `settings_module` or `settings_config` but not both."
-
-        if settings_config:
-            warnings.warn(
-                "The `settings_config` is deprecated, and will be removed in version 2.9.0. "  # noqa: E501
-                "Use `settings_module` instead.",  # noqa: E501
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-        self.settings_config = None
         self.settings_module = None
-
-        settings_module = settings_module or settings_config
-
-        if settings_module:
+        if settings_module is not None:
             if not isinstance(settings_module, EsmeraldAPISettings) and not is_class_and_subclass(
                 settings_module, EsmeraldAPISettings
             ):
                 raise ImproperlyConfigured(
                     "settings_module must be a subclass of EsmeraldSettings"
                 )
             elif isinstance(settings_module, EsmeraldAPISettings):
@@ -2413,14 +2381,15 @@
                     exception_handlers=exception_handlers,
                     error_handler=error_handler,
                     debug=debug,
                 ),
             ]
             + self.user_middleware
             + [
+                DefineMiddleware(ApplicationSettingsMiddleware),
                 DefineMiddleware(
                     ExceptionMiddleware,
                     handlers=exception_handlers,
                     debug=debug,
                 ),
                 DefineMiddleware(AsyncExitStackMiddleware, config=self.async_exit_config),
             ]
@@ -2528,24 +2497,33 @@
         Builds the scope for a specific mounted application.
         """
         if "route_root_path" in scope:
             if "root_include_path" not in scope:
                 scope["root_include_path"] = scope["route_root_path"]
         return scope
 
+    async def globalise_settings(self) -> None:
+        """
+        Making sure the global settings remain as is
+        after the request is done.
+        """
+        settings = reload_settings()
+        esmerald_settings.configure(settings())
+
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if scope["type"] == "lifespan":
             await self.router.lifespan(scope, receive, send)
             return
 
         if self.root_path:
             scope["root_path"] = self.root_path
 
         scope["state"] = {}
         await super().__call__(scope, receive, send)
+        await self.globalise_settings()
 
     def route(
         self,
         path: str,
         methods: Optional[List[str]] = None,
         name: Optional[str] = None,
         include_in_schema: bool = True,
```

### Comparing `esmerald-3.0.0b2/esmerald/backgound.py` & `esmerald-3.1.0/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/context.py` & `esmerald-3.1.0/esmerald/context.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/enums.py` & `esmerald-3.1.0/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/exception_handlers.py` & `esmerald-3.1.0/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/exceptions.py` & `esmerald-3.1.0/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/injector.py` & `esmerald-3.1.0/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/logging.py` & `esmerald-3.1.0/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/params.py` & `esmerald-3.1.0/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/parsers.py` & `esmerald-3.1.0/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/requests.py` & `esmerald-3.1.0/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/testclient.py` & `esmerald-3.1.0/esmerald/testclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     def __enter__(self, *args: Any, **kwargs: Dict[str, Any]) -> "EsmeraldTestClient":
         return cast("EsmeraldTestClient", super().__enter__(*args, **kwargs))
 
 
 def create_client(
     routes: Union["APIGateHandler", List["APIGateHandler"]],
     *,
-    settings_config: Optional["SettingsType"] = None,
     settings_module: Optional["SettingsType"] = None,
     debug: Optional[bool] = None,
     app_name: Optional[str] = None,
     title: Optional[str] = None,
     version: Optional[str] = None,
     summary: Optional[str] = None,
     description: Optional[str] = None,
@@ -123,15 +122,14 @@
     cookies: Optional[CookieTypes] = None,
     redirect_slashes: Optional[bool] = None,
     tags: Optional[List[str]] = None,
     webhooks: Optional[Sequence["WebhookGateway"]] = None,
 ) -> EsmeraldTestClient:
     return EsmeraldTestClient(
         app=Esmerald(
-            settings_config=settings_config,
             settings_module=settings_module,
             debug=debug,
             title=title,
             version=version,
             summary=summary,
             description=description,
             contact=contact,
```

### Comparing `esmerald-3.0.0b2/esmerald/types.py` & `esmerald-3.1.0/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/websockets.py` & `esmerald-3.1.0/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/__init__.py` & `esmerald-3.1.0/esmerald/conf/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 import os
+from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Optional, Type
 
 from lilya._internal._module_loading import import_string
 
 from esmerald.utils.functional import LazyObject, empty
 
 if TYPE_CHECKING:
     from esmerald.conf.global_settings import EsmeraldAPISettings
 
 ENVIRONMENT_VARIABLE = "ESMERALD_SETTINGS_MODULE"
 
 
+@lru_cache
+def reload_settings() -> Type["EsmeraldAPISettings"]:
+    """
+    Reloads the global settings.
+    """
+    settings_module: str = os.environ.get(
+        ENVIRONMENT_VARIABLE, "esmerald.conf.global_settings.EsmeraldAPISettings"
+    )
+    settings: Type["EsmeraldAPISettings"] = import_string(settings_module)
+    return settings
+
+
 class EsmeraldLazySettings(LazyObject):
     """
     A lazy proxy for either global Esmerald settings or a custom settings object.
     The user can manually configure settings prior to using them. Otherwise,
     Esmerald uses the settings module pointed to by ESMERALD_SETTINGS_MODULE.
     """
 
     def _setup(self, name: Optional[str] = None) -> None:
         """
         Load the settings module pointed to by the environment variable. This
         is used the first time settings are needed, if the user hasn't
         configured settings manually.
         """
-        settings_module: str = os.environ.get(
-            ENVIRONMENT_VARIABLE, "esmerald.conf.global_settings.EsmeraldAPISettings"
-        )
-
-        settings: Type["EsmeraldAPISettings"] = import_string(settings_module)
+        settings: Type["EsmeraldAPISettings"] = reload_settings()
 
         for setting, _ in settings().model_dump().items():
             assert setting.islower(), "%s should be in lowercase." % setting
 
         self._wrapped = settings()
 
+    def configure(self, override_settings: Type["EsmeraldAPISettings"]) -> None:
+        """
+        Making sure the settings are overriden by the settings_module
+        provided by a given application and therefore use it as the application
+        global.
+        """
+        self._wrapped = override_settings
+
     def __repr__(self: "EsmeraldLazySettings") -> str:
         # Hardcode the class name as otherwise it yields 'Settings'.
         if self._wrapped is empty:
             return "<EsmeraldLazySettings [Unevaluated]>"
         return '<EsmeraldLazySettings "{settings_module}">'.format(
             settings_module=self._wrapped.__class__.__name__
         )
```

### Comparing `esmerald-3.0.0b2/esmerald/conf/global_settings.py` & `esmerald-3.1.0/esmerald/conf/global_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1414,7 +1414,17 @@
 
                 return {
                     "my-extension": pluggable
                 }
         ```
         """
         return {}
+
+    def __hash__(self) -> int:
+        values: Dict[str, Any] = {}
+        for key, value in self.__dict__.items():
+            values[key] = None
+            if isinstance(value, (list, set)):
+                values[key] = tuple(value)
+            else:
+                values[key] = value
+        return hash((type(self),) + tuple(values))
```

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/.gitignore.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/Makefile.e-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/main.py-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/serve.py-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/urls.py-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl` & `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/cors.py` & `esmerald-3.1.0/esmerald/config/cors.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/csrf.py` & `esmerald-3.1.0/esmerald/config/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/jwt.py` & `esmerald-3.1.0/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/openapi.py` & `esmerald-3.1.0/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/session.py` & `esmerald-3.1.0/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/static_files.py` & `esmerald-3.1.0/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/config/template.py` & `esmerald-3.1.0/esmerald/config/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/encoding.py` & `esmerald-3.1.0/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/hashers.py` & `esmerald-3.1.0/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/common/middleware.py` & `esmerald-3.1.0/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/edgy/base_user.py` & `esmerald-3.1.0/esmerald/contrib/auth/edgy/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/edgy/middleware.py` & `esmerald-3.1.0/esmerald/contrib/auth/edgy/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/mongoz/base_user.py` & `esmerald-3.1.0/esmerald/contrib/auth/mongoz/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/mongoz/middleware.py` & `esmerald-3.1.0/esmerald/contrib/auth/mongoz/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-3.1.0/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-3.1.0/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/di/provider.py` & `esmerald-3.1.0/esmerald/core/di/provider.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/cli.py` & `esmerald-3.1.0/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/env.py` & `esmerald-3.1.0/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/templates.py` & `esmerald-3.1.0/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/utils.py` & `esmerald-3.1.0/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/createapp.py` & `esmerald-3.1.0/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/createdeployment.py` & `esmerald-3.1.0/esmerald/core/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/createproject.py` & `esmerald-3.1.0/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/list.py` & `esmerald-3.1.0/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/run.py` & `esmerald-3.1.0/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/runserver.py` & `esmerald-3.1.0/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/show_urls.py` & `esmerald-3.1.0/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/shell/base.py` & `esmerald-3.1.0/esmerald/core/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/shell/ipython.py` & `esmerald-3.1.0/esmerald/core/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/shell/ptpython.py` & `esmerald-3.1.0/esmerald/core/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/directives/operations/shell/utils.py` & `esmerald-3.1.0/esmerald/core/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/terminal/base.py` & `esmerald-3.1.0/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/terminal/print.py` & `esmerald-3.1.0/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/terminal/terminal.py` & `esmerald-3.1.0/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/core/urls/base.py` & `esmerald-3.1.0/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/__init__.py` & `esmerald-3.1.0/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/base.py` & `esmerald-3.1.0/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/encoders.py` & `esmerald-3.1.0/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/file.py` & `esmerald-3.1.0/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/json.py` & `esmerald-3.1.0/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/msgspec.py` & `esmerald-3.1.0/esmerald/datastructures/msgspec.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/redirect.py` & `esmerald-3.1.0/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/stream.py` & `esmerald-3.1.0/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/datastructures/template.py` & `esmerald-3.1.0/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/interceptors/interceptor.py` & `esmerald-3.1.0/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/__init__.py` & `esmerald-3.1.0/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/_exception_handlers.py` & `esmerald-3.1.0/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/asyncexitstack.py` & `esmerald-3.1.0/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/authentication.py` & `esmerald-3.1.0/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/exceptions.py` & `esmerald-3.1.0/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/middleware/settings_middleware.py` & `esmerald-3.1.0/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/_internal.py` & `esmerald-3.1.0/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/datastructures.py` & `esmerald-3.1.0/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/docs.py` & `esmerald-3.1.0/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/models.py` & `esmerald-3.1.0/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/openapi.py` & `esmerald-3.1.0/esmerald/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/responses.py` & `esmerald-3.1.0/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/utils.py` & `esmerald-3.1.0/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/validation.py` & `esmerald-3.1.0/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/security/base.py` & `esmerald-3.1.0/esmerald/openapi/security/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/security/api_key/base.py` & `esmerald-3.1.0/esmerald/openapi/security/api_key/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/security/http/base.py` & `esmerald-3.1.0/esmerald/openapi/security/http/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/security/oauth2/base.py` & `esmerald-3.1.0/esmerald/openapi/security/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/openapi/security/openid_connect/base.py` & `esmerald-3.1.0/esmerald/openapi/security/openid_connect/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/permissions/base.py` & `esmerald-3.1.0/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/permissions/utils.py` & `esmerald-3.1.0/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/pluggables/base.py` & `esmerald-3.1.0/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/protocols/asyncdao.py` & `esmerald-3.1.0/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/protocols/dao.py` & `esmerald-3.1.0/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/protocols/interceptor.py` & `esmerald-3.1.0/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/protocols/template.py` & `esmerald-3.1.0/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/responses/base.py` & `esmerald-3.1.0/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/responses/encoders.py` & `esmerald-3.1.0/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/responses/json.py` & `esmerald-3.1.0/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/responses/template.py` & `esmerald-3.1.0/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/_internal.py` & `esmerald-3.1.0/esmerald/routing/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/base.py` & `esmerald-3.1.0/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/events.py` & `esmerald-3.1.0/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/gateways.py` & `esmerald-3.1.0/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/handlers.py` & `esmerald-3.1.0/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/router.py` & `esmerald-3.1.0/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/apis/_metaclasses.py` & `esmerald-3.1.0/esmerald/routing/apis/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/apis/_mixins.py` & `esmerald-3.1.0/esmerald/routing/apis/_mixins.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/apis/base.py` & `esmerald-3.1.0/esmerald/routing/apis/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/apis/generics.py` & `esmerald-3.1.0/esmerald/routing/apis/generics.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/apis/views.py` & `esmerald-3.1.0/esmerald/routing/apis/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/routing/webhooks/handlers.py` & `esmerald-3.1.0/esmerald/routing/webhooks/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/security/jwt/token.py` & `esmerald-3.1.0/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/template/jinja.py` & `esmerald-3.1.0/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/template/mako.py` & `esmerald-3.1.0/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/transformers/datastructures.py` & `esmerald-3.1.0/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/transformers/model.py` & `esmerald-3.1.0/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/transformers/signature.py` & `esmerald-3.1.0/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/transformers/utils.py` & `esmerald-3.1.0/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/constants.py` & `esmerald-3.1.0/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/dependency.py` & `esmerald-3.1.0/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/functional.py` & `esmerald-3.1.0/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/helpers.py` & `esmerald-3.1.0/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/models.py` & `esmerald-3.1.0/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/sync.py` & `esmerald-3.1.0/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/esmerald/utils/pydantic/schema.py` & `esmerald-3.1.0/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/LICENSE` & `esmerald-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/README.md` & `esmerald-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-3.0.0b2/pyproject.toml` & `esmerald-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 dependencies = [
     "anyio>=3.7.1,<5.0.0",
     "awesome-slugify>=1.6.5,<2",
     "click>=8.1.4,<9.0.0",
     "itsdangerous>=2.1.2,<3.0.0",
     "jinja2>=3.1.2,<4.0.0",
-    "lilya>=0.2.3",
+    "lilya>=0.3.3",
     "loguru>=0.7.0,<0.8.0",
     "pydantic>=2.5.3,<3.0.0",
     "pydantic-settings>=2.0.0,<3.0.0",
     "python-multipart>=0.0.7,<0.0.10",
     "openapi-schemas-pydantic>=3.0.0",
     "orjson>=3.8.5,<4.0.0",
     "msgspec>=0.18.5,<1.0.0",
@@ -89,15 +89,15 @@
 Changelog = "https://esmerald.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1.3,<9.0.0",
-    "pytest-cov>=4.1.0,<5.0.0",
+    "pytest-cov>=4.1.0,<6.0.0",
     "pytest-asyncio>=0.20.0",
     "mypy==1.9.0",
     "flake8>=5.0.4",
     "aiofiles>=0.8.0,<24",
     "a2wsgi>=1.9.0,<2",
     "asyncz>=0.5.0",
     "anyio[trio]>=3.6.2,<5.0.0",
@@ -120,15 +120,15 @@
     "types-ujson==5.9.0.0",
     "types-orjson==3.6.2",
 ]
 
 dev = [
     "a2wsgi>=1.10.0,<2",
     "autoflake>=1.4.0",
-    "black==24.2.0",
+    "black==24.3.0",
     "ipdb",
     "isort>=5.0.6,<6.0.0",
     "flake8>=3.8.3,<8.0.0",
     "uvicorn[standard]>=0.24.0",
     "pre-commit>=3.0.4,<4.0.0",
     "ruff>=0.3.0,<1.0.0",
     "watchfiles>=0.16.1,<0.22.0",
```

### Comparing `esmerald-3.0.0b2/PKG-INFO` & `esmerald-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: esmerald
-Version: 3.0.0b2
+Version: 3.1.0
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -38,28 +38,28 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: anyio<5.0.0,>=3.7.1
 Requires-Dist: awesome-slugify<2,>=1.6.5
 Requires-Dist: click<9.0.0,>=8.1.4
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
 Requires-Dist: jinja2<4.0.0,>=3.1.2
-Requires-Dist: lilya>=0.2.3
+Requires-Dist: lilya>=0.3.3
 Requires-Dist: loguru<0.8.0,>=0.7.0
 Requires-Dist: msgspec<1.0.0,>=0.18.5
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.8
 Requires-Dist: openapi-schemas-pydantic>=3.0.0
 Requires-Dist: orjson<4.0.0,>=3.8.5
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0
 Requires-Dist: pydantic<3.0.0,>=2.5.3
 Requires-Dist: python-multipart<0.0.10,>=0.0.7
 Requires-Dist: rich<14.0.0,>=13.3.1
 Provides-Extra: dev
 Requires-Dist: a2wsgi<2,>=1.10.0; extra == 'dev'
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
-Requires-Dist: black==24.2.0; extra == 'dev'
+Requires-Dist: black==24.3.0; extra == 'dev'
 Requires-Dist: flake8<8.0.0,>=3.8.3; extra == 'dev'
 Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: ruff<1.0.0,>=0.3.0; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.24.0; extra == 'dev'
 Requires-Dist: watchfiles<0.22.0,>=0.16.1; extra == 'dev'
@@ -101,15 +101,15 @@
 Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'test'
 Requires-Dist: mock==5.1.0; extra == 'test'
 Requires-Dist: mongoz>=0.6.0; extra == 'test'
 Requires-Dist: mypy==1.9.0; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
 Requires-Dist: polyfactory<3.0.0,>=2.5.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.20.0; extra == 'test'
-Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == 'test'
+Requires-Dist: pytest-cov<6.0.0,>=4.1.0; extra == 'test'
 Requires-Dist: pytest<9.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: saffier[postgres]>=1.3.7; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Requires-Dist: types-ujson==5.9.0.0; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
```

