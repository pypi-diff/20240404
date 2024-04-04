# Comparing `tmp/swit_core-4.0.1.tar.gz` & `tmp/swit_core-4.0.2.tar.gz`

## Comparing `swit_core-4.0.1.tar` & `swit_core-4.0.2.tar`

### file list

```diff
@@ -1,947 +1,949 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-4.0.1/.flake8
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 swit_core-4.0.1/log.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 swit_core-4.0.1/mypy.ini
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 swit_core-4.0.1/requirements.txt
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 swit_core-4.0.1/run_tests.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/core.iml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    52825 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/dictionaries/el.xml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/httpRequests/2023-08-08T143300.405.json
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/httpRequests/2023-08-08T143308.500.json
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/httpRequests/2023-08-09T181553.500.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/httpRequests/http-client.cookies
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/httpRequests/http-requests-log.http
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-4.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/__init__.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/async_httpclient.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/constants.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/httpclient.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/py.typed
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/pydantic_base_model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/__init__.py
--rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/activity_router.py
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/async_activity_handler_abc.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/base_activity_handler.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/dependencies.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/exceptions.py
--rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/channel/__init__.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/channel/async_service.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/channel/schemas.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/channel/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/message/__init__.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/message/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/user/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/user/schemas.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/user/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/workspace/__init__.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/workspace/async_service.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/workspace/schemas.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/api/workspace/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/async_repository.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/constants.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/exception.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/models.py
--rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/oauth2.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/repository.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/router.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/signature_verification.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/auth/utils.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/__init__.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/button.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/container.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/datepicker.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/divider.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/element_components.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/header.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/image.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/image_grid.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/info_card.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/input.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/interactive_image.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/item.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/search.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/select.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/select_item.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/tabs.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 swit_core-4.0.1/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/__init__.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_oauth2.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_path_resolver.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_router.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_signature_verification.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_swit_request.py
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/test_swit_response.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/__init__.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_collection_entry.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_container.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_datepicker.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_image_grid.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_info_card.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_interactive_image.py
--rw-r--r--   0        0        0    11181 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_select.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 swit_core-4.0.1/tests/ui/test_static_action.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/.gitignore
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/pyvenv.cfg
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate.csh
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate.fish
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate.nu
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate.ps1
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/activate_this.py
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/pip
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/pip-3.10
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/pip3
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/python -> /usr/local/bin/python3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/python3.10 -> python
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/wheel
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/wheel-3.10
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/wheel3
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/bin/wheel3.10
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.virtualenv
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/py.typed
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0        0        0    74033 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0        0        0   108885 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   134976 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    20105 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/py.typed
--rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/py.typed
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_core_metadata.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_normalization.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    18740 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/build_meta.py
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-32.exe
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-64.exe
--rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    21142 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    37176 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/glob.py
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-32.exe
--rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-64.exe
--rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/modified.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    38376 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/warnings.py
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_log.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_modified.py
--rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17863 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31504 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/py.typed
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/py.typed
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    14977 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/py.typed
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/py.typed
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/_requirestxt.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16433 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    15127 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    86203 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    33582 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26516 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/compat/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/compat/py310.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/compat/py311.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    14758 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16389 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    17349 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25556 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   274908 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/LICENSE
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/METADATA
--rw-r--r--   0        0        0    36910 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/__main__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/_setuptools_logging.py
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/bdist_wheel.py
--rw-r--r--   0        0        0    16143 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/macosx_libfile.py
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/metadata.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/util.py
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/wheelfile.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/convert.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/pack.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/tags.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/unpack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/vendor.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py
--rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/METADATA
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/WHEEL
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-4.0.1/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-4.0.1/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 swit_core-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swit_core-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-4.0.2/.flake8
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 swit_core-4.0.2/log.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 swit_core-4.0.2/mypy.ini
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 swit_core-4.0.2/requirements.txt
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 swit_core-4.0.2/run_tests.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/core.iml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    54533 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/dictionaries/el.xml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/httpRequests/2023-08-08T143300.405.json
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/httpRequests/2023-08-08T143308.500.json
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/httpRequests/2023-08-09T181553.500.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/httpRequests/http-client.cookies
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/httpRequests/http-requests-log.http
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/shelf/_______Changes_.xml
+-rw-r--r--   0        0        0    50536 2020-02-02 00:00:00.000000 swit_core-4.0.2/.idea/shelf/리베이스_전에_커밋되지_않은_변경_내용_[Changes]/shelved.patch
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/__init__.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/async_httpclient.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/constants.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/httpclient.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/py.typed
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/pydantic_base_model.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/__init__.py
+-rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/activity_router.py
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/async_activity_handler_abc.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/base_activity_handler.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/exceptions.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/channel/__init__.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/channel/async_service.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/channel/schemas.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/channel/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/message/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/message/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/user/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/user/schemas.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/user/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/workspace/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/workspace/async_service.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/workspace/schemas.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/api/workspace/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/async_repository.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/exception.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/models.py
+-rw-r--r--   0        0        0     6315 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/oauth2.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/router.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/schemas.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/signature_verification.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/auth/utils.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/button.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/container.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/datepicker.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/element_components.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/header.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/image.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/image_grid.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/info_card.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/input.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/interactive_image.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/item.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/search.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/select.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 swit_core-4.0.2/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_oauth2.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_path_resolver.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_router.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_signature_verification.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_swit_request.py
+-rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/test_swit_response.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/__init__.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_collection_entry.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_container.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_datepicker.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_image_grid.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_info_card.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_interactive_image.py
+-rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_select.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 swit_core-4.0.2/tests/ui/test_static_action.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/.gitignore
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/pyvenv.cfg
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate.csh
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate.fish
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate.nu
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate.ps1
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/pip
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/pip-3.10
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/pip3
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/pip3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/python -> /usr/local/bin/python3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/wheel
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/wheel-3.10
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/wheel3
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/bin/wheel3.10
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.virtualenv
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23634 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8378 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11801 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30064 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28782 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12450 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37843 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    20777 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    28128 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    19018 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17790 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35460 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24551 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    21052 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    32292 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    23623 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22787 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281617 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51965 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51767 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18315 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    67530 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23747 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43958 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0        0        0    74033 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108885 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   134976 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    20105 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0        0        0    25416 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_core_metadata.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_normalization.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    18740 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    21142 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    37176 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/modified.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47354 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    38376 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0    14284 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/warnings.py
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_log.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_modified.py
+-rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48644 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17863 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15602 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31504 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/py.typed
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    14977 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/_requirestxt.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16433 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    15127 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    86203 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    33582 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    26516 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/compat/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/compat/py310.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/compat/py311.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    14758 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16389 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    17349 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25556 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   274908 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0    36910 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/_setuptools_logging.py
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    16143 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/tags.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/vendor.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-4.0.2/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-4.0.2/README.md
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swit_core-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 swit_core-4.0.2/PKG-INFO
```

### Comparing `swit_core-4.0.1/log.txt` & `swit_core-4.0.2/log.txt`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/.idea/workspace.xml` & `swit_core-4.0.2/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `swit_core-4.0.1/.idea/workspace.xml` & `swit_core-4.0.2/.idea/workspace.xml`

```diff
@@ -5,14 +5,20 @@
   </component>
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="| None default value">
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/switcore/action/schemas.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/action/schemas.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/switcore/ui/collection_entry.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/ui/collection_entry.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/switcore/ui/element_components.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/ui/element_components.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_swit_response.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_swit_response.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/ui/test_collection_entry.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/ui/test_collection_entry.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/ui/test_select.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/ui/test_select.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -43,20 +49,20 @@
   &quot;lastFilter&quot;: {
     &quot;state&quot;: &quot;OPEN&quot;
   }
 }</component>
   <component name="GitRewordedCommitMessages">
     <option name="commitMessagesMapping">
       <RewordedCommitMessageMapping>
-        <option name="originalMessage" value="first commit"/>
-        <option name="rewordedMessage" value="first commit"/>
+        <option name="originalMessage" value="코드 정리"/>
+        <option name="rewordedMessage" value="pydantic v2"/>
       </RewordedCommitMessageMapping>
     </option>
     <option name="currentCommit" value="1"/>
-    <option name="onto" value="ee5954fa336de44f7621ba07d3e5fbc4f8272e08"/>
+    <option name="onto" value="68bbeff37a2570d37d7f5d409a94bdbff33a4951"/>
   </component>
   <component name="GithubPullRequestsUISettings">
     <option name="selectedUrlAndAccountId">
       <UrlAndAccount>
         <option name="accountId" value="6091f14e-b66a-418b-a058-82818eac9587"/>
         <option name="url" value="https://github.com/Tech-Switness/ur-pub-sdk.git"/>
       </UrlAndAccount>
@@ -84,14 +90,16 @@
   "keyToString": {
     "Python tests.Python tests for test_router.RouterTest.executor": "Run",
     "Python tests.Python tests for test_swit_request.SwitViewResponseTest.executor": "Run",
     "Python tests.Python tests for test_swit_request.SwitViewResponseTest.test_swit_query_request.executor": "Debug",
     "Python tests.Python tests for test_swit_request.SwitViewResponseTest.test_swit_response_view.executor": "Run",
     "Python tests.Python tests for test_swit_request.SwitViewResponseTest.test_swit_task_request.executor": "Run",
     "Python tests.Python tests for test_swit_response.SwitViewResponseTest.test_swit_response_task_attachments.executor": "Run",
+    "Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry01의 Python 테스트.executor": "Run",
+    "Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry03의 Python 테스트.executor": "Run",
     "Python 테스트.test_collection_entry.CollectionEntryTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_container.ContainerTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_datepicker.DatePickerTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_image_grid.InteractiveImageTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_info_card.InfoCardTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_interactive_image.InteractiveImageTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_oauth2.OAuth2Test.test_oauth2_secure_state의 Python 테스트.executor": "Run",
@@ -105,15 +113,15 @@
     "Python 테스트.test_signature_verification.SignatureVerifierTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_request.SwitViewResponseTest.test_swit_query_request의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_request.SwitViewResponseTest.test_swit_submit_request의 Python 테스트.executor": "Debug",
     "Python 테스트.test_swit_request.SwitViewResponseTest.test_swit_task_request의 Python 테스트.executor": "Debug",
     "Python 테스트.test_swit_request.SwitViewResponseTest의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_attachments의 Python 테스트.executor": "Debug",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion01의 Python 테스트.executor": "Run",
-    "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02의 Python 테스트.executor": "Debug",
+    "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion05의 Python 테스트.executor": "Debug",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion06의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestions03의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestions04의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_view의 Python 테스트.executor": "Run",
     "Python 테스트.test_swit_response.SwitViewResponseTest의 Python 테스트.executor": "Run",
     "RunOnceActivity.OpenProjectViewOnStart": "true",
@@ -145,15 +153,15 @@
       <recent name="$PROJECT_DIR$/tests/ui"/>
       <recent name="$PROJECT_DIR$/switcore"/>
       <recent name="$PROJECT_DIR$/apis/v1"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/switbuilder-core"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python 테스트.test_info_card.InfoCardTest의 Python 테스트">
+  <component name="RunManager" selected="Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry01의 Python 테스트">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
@@ -184,110 +192,110 @@
       <option name="INTERPRETER_PATH" value="/bin/zsh"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="EXECUTE_IN_TERMINAL" value="true"/>
       <option name="EXECUTE_SCRIPT_FILE" value="true"/>
       <envs/>
       <method v="2"/>
     </configuration>
-    <configuration name="test_image_grid.InteractiveImageTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="test_collection_entry.CollectionEntryTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/ui"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_image_grid.InteractiveImageTest&quot;"/>
+      <option name="_new_target" value="&quot;test_collection_entry.CollectionEntryTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="test_info_card.InfoCardTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="test_collection_entry.CollectionEntryTest.test_valid_collection_entry01의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/ui"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_info_card.InfoCardTest&quot;"/>
+      <option name="_new_target" value="&quot;test_collection_entry.CollectionEntryTest.test_valid_collection_entry01&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="test_interactive_image.InteractiveImageTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="test_collection_entry.CollectionEntryTest.test_valid_collection_entry03의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/ui"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_interactive_image.InteractiveImageTest&quot;"/>
+      <option name="_new_target" value="&quot;test_collection_entry.CollectionEntryTest.test_valid_collection_entry03&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="test_select.SelectTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="test_info_card.InfoCardTest의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/ui"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_select.SelectTest&quot;"/>
+      <option name="_new_target" value="&quot;test_info_card.InfoCardTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="test_select.SelectTest.test_select_option_groups_length의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02의 Python 테스트" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests/ui"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_select.SelectTest.test_select_option_groups_length&quot;"/>
+      <option name="_new_target" value="&quot;test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.main"/>
-      <item itemvalue="Python 테스트.test_image_grid.InteractiveImageTest의 Python 테스트"/>
+      <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry01의 Python 테스트"/>
+      <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry03의 Python 테스트"/>
+      <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest의 Python 테스트"/>
       <item itemvalue="Python 테스트.test_info_card.InfoCardTest의 Python 테스트"/>
-      <item itemvalue="Python 테스트.test_interactive_image.InteractiveImageTest의 Python 테스트"/>
-      <item itemvalue="Python 테스트.test_select.SelectTest.test_select_option_groups_length의 Python 테스트"/>
-      <item itemvalue="Python 테스트.test_select.SelectTest의 Python 테스트"/>
+      <item itemvalue="Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02의 Python 테스트"/>
       <item itemvalue="Shell Script.run_test"/>
     </list>
     <recent_temporary>
       <list>
+        <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry01의 Python 테스트"/>
+        <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest의 Python 테스트"/>
+        <item itemvalue="Python 테스트.test_collection_entry.CollectionEntryTest.test_valid_collection_entry03의 Python 테스트"/>
+        <item itemvalue="Python 테스트.test_swit_response.SwitViewResponseTest.test_swit_response_query_suggestion02의 Python 테스트"/>
         <item itemvalue="Python 테스트.test_info_card.InfoCardTest의 Python 테스트"/>
-        <item itemvalue="Python 테스트.test_select.SelectTest.test_select_option_groups_length의 Python 테스트"/>
-        <item itemvalue="Python 테스트.test_select.SelectTest의 Python 테스트"/>
-        <item itemvalue="Python 테스트.test_interactive_image.InteractiveImageTest의 Python 테스트"/>
-        <item itemvalue="Python 테스트.test_image_grid.InteractiveImageTest의 Python 테스트"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
         <option value="bundled-python-sdk-09665e90c3a7-b11f5e8da5ad-com.jetbrains.pycharm.pro.sharedIndexes.bundled-PY-233.15026.15"/>
@@ -509,15 +517,15 @@
       <workItem from="1711932966702" duration="1805000"/>
       <workItem from="1711936441602" duration="2704000"/>
       <workItem from="1711944526666" duration="3273000"/>
       <workItem from="1711954561083" duration="2670000"/>
       <workItem from="1712014550298" duration="3052000"/>
       <workItem from="1712020217271" duration="79000"/>
       <workItem from="1712020304517" duration="3811000"/>
-      <workItem from="1712031034024" duration="7126000"/>
+      <workItem from="1712031034024" duration="14290000"/>
     </task>
     <task id="LOCAL-00035" summary="add searchInput">
       <option name="closed" value="true"/>
       <created>1692337959679</created>
       <option name="number" value="00035"/>
       <option name="presentableId" value="LOCAL-00035"/>
       <option name="project" value="LOCAL"/>
@@ -1021,12 +1029,12 @@
         <watch expression="unquote(response.headers[&quot;location&quot;])" language="Python"/>
       </configuration>
     </watches-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/core$aa.coverage" NAME="aa Coverage Results" MODIFIED="1690410103760" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$APPLICATION_CONFIG_DIR$/scratches"/>
     <SUITE FILE_PATH="coverage/core$document_api.coverage" NAME="document_api Coverage Results" MODIFIED="1691665260943" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$APPLICATION_CONFIG_DIR$/scratches"/>
-    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" 커버리지 결과" MODIFIED="1712037037119" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests/ui"/>
+    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" 커버리지 결과" MODIFIED="1712192843596" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests/ui"/>
     <SUITE FILE_PATH="coverage/core$main.coverage" NAME="main Coverage Results" MODIFIED="1690246417369" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/core$study05.coverage" NAME="study05 Coverage Results" MODIFIED="1691708040860" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$APPLICATION_CONFIG_DIR$/scratches"/>
   </component>
 </project>
```

### Comparing `swit_core-4.0.1/.idea/httpRequests/2023-08-08T143308.500.json` & `swit_core-4.0.2/.idea/httpRequests/2023-08-08T143308.500.json`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/.idea/httpRequests/2023-08-09T181553.500.json` & `swit_core-4.0.2/.idea/httpRequests/2023-08-09T181553.500.json`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/.idea/httpRequests/http-requests-log.http` & `swit_core-4.0.2/.idea/httpRequests/http-requests-log.http`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/.idea/inspectionProfiles/Project_Default.xml` & `swit_core-4.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/async_httpclient.py` & `swit_core-4.0.2/switcore/async_httpclient.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/httpclient.py` & `swit_core-4.0.2/switcore/httpclient.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/logger.py` & `swit_core-4.0.2/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/activity_handler_abc.py` & `swit_core-4.0.2/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/activity_router.py` & `swit_core-4.0.2/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/async_activity_handler_abc.py` & `swit_core-4.0.2/switcore/action/async_activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/base_activity_handler.py` & `swit_core-4.0.2/switcore/action/base_activity_handler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/dependencies.py` & `swit_core-4.0.2/switcore/action/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/action/schemas.py` & `swit_core-4.0.2/switcore/action/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,36 +63,14 @@
         return v
 
 
 class MessageCommentResource(MessageResource):
     resource_type: Literal['message_comment'] = 'message_comment'
 
 
-class TaskPriorityLevel(str, Enum):
-    HIGHEST = 'highest'
-    HIGH = 'high'
-    NORMAL = 'normal'
-    LOW = 'low'
-    LOWEST = 'lowest'
-
-
-class TaskColorLabel(str, Enum):
-    RED = 'red'
-    PINK = 'pink'
-    ORANGE = 'orange'
-    YELLOW = 'yellow'
-    LIGHT_GREEN = 'light_green'
-    GREEN = 'green'
-    CYAN = 'cyan'
-    BLUE = 'blue'
-    NAVY = 'navy'
-    VIOLET = 'violet'
-    GRAY = 'gray'
-
-
 class TaskStatusType(str, Enum):
     NOT_STARTED = 'not_started'
     IN_PROGRESS = 'in_progress'
     DONE = 'done'
 
 
 class TaskPeriod(SwitBaseModel):
@@ -126,16 +104,17 @@
     resource_type: Literal['task'] = 'task'
     id: str
     parent_task_id: str | None = None
     created_at: datetime
     edited_at: datetime | None = None
     title: str
     period: TaskPeriod
-    priority: TaskPriorityLevel
-    color_label: TaskColorLabel | None = None
+    priority: Literal['highest', 'high', 'normal', 'low', 'lowest']
+    color_label: Literal[
+                     'red', 'pink', 'orange', 'yellow', 'light_green', 'green', 'cyan', 'blue', 'navy', 'violet', 'gray'] | None = None
     assignees: List[TaskUser]
     collaborators: List[TaskUser]
     status: TaskStatus
     bucket: TaskBucket
 
     @model_validator(mode='before')
     def parse_empty_strings(cls, values: dict[str, Any]):
```

### Comparing `swit_core-4.0.1/switcore/api/helpers.py` & `swit_core-4.0.2/switcore/api/helpers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/channel/async_service.py` & `swit_core-4.0.2/switcore/api/channel/async_service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/channel/service.py` & `swit_core-4.0.2/switcore/api/channel/service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/message/service.py` & `swit_core-4.0.2/switcore/api/message/service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/user/service.py` & `swit_core-4.0.2/switcore/api/user/service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/workspace/async_service.py` & `swit_core-4.0.2/switcore/api/workspace/async_service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/api/workspace/service.py` & `swit_core-4.0.2/switcore/api/workspace/service.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/async_repository.py` & `swit_core-4.0.2/switcore/auth/async_repository.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/dependencies.py` & `swit_core-4.0.2/switcore/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/exception.py` & `swit_core-4.0.2/switcore/auth/exception.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/models.py` & `swit_core-4.0.2/switcore/auth/models.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/oauth2.py` & `swit_core-4.0.2/switcore/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/repository.py` & `swit_core-4.0.2/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/router.py` & `swit_core-4.0.2/switcore/auth/router.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/signature_verification.py` & `swit_core-4.0.2/switcore/auth/signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/auth/utils.py` & `swit_core-4.0.2/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/ui/collection_entry.py` & `swit_core-4.0.2/switcore/ui/collection_entry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 from typing import Literal
 from enum import Enum
 
+from pydantic import Field
+
 from switcore.pydantic_base_model import SwitBaseModel
 from switcore.ui.element_components import SubText, Tag, StaticAction
 from switcore.ui.image import Image
 from switcore.ui.text_paragraph import TextParagraph
 
 
 class TextStyle(SwitBaseModel):
     bold: bool = False
     color: str
     size: str
     max_lines: int
 
 
-class BackgroundType(str, Enum):
-    none = "none"
-    lightblue = "lightblue"
-
-
 class Background(SwitBaseModel):
-    color: BackgroundType = BackgroundType.none
+    color: Literal['none', 'lightblue'] = 'none'
 
 
 class MetadataItem(SwitBaseModel):
     type: str
     content: str | None = None
     style: dict | None = None
     image_url: str | None = None
 
 
 class TextSection(SwitBaseModel):
     text: TextParagraph
-    metadata_items: list[SubText | Image | Tag] | None = None
-
-
-class VerticalAlignmentTypes(str, Enum):
-    top = "top"
-    middle = "middle"
-    bottom = "bottom"
+    metadata_items: list[SubText | Image | Tag] = Field(default_factory=list, discriminator='type', max_length=4)
 
 
 class CollectionEntry(SwitBaseModel):
     type: Literal['collection_entry'] = 'collection_entry'
     start_section: Image | None = None
     text_sections: list[TextSection]
-    vertical_alignment: VerticalAlignmentTypes = VerticalAlignmentTypes.top
+    vertical_alignment: Literal['top', 'middle', 'bottom'] = 'top'
     background: Background | None = None
     action_id: str | None = None
     static_action: StaticAction | None = None
     draggable: bool = False
```

### Comparing `swit_core-4.0.1/switcore/ui/file.py` & `swit_core-4.0.2/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/ui/select.py` & `swit_core-4.0.2/switcore/ui/select.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/switcore/ui/text_paragraph.py` & `swit_core-4.0.2/switcore/ui/text_paragraph.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_oauth2.py` & `swit_core-4.0.2/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_path_resolver.py` & `swit_core-4.0.2/tests/test_path_resolver.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_router.py` & `swit_core-4.0.2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_signature_verification.py` & `swit_core-4.0.2/tests/test_signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_swit_request.py` & `swit_core-4.0.2/tests/test_swit_request.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/test_swit_response.py` & `swit_core-4.0.2/tests/test_swit_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json  # noqa: F401
 import unittest
 
 from switcore.action.schemas import SwitResponse, ViewCallbackType, View, Body, AttachmentCallbackTypes, AttachmentView, \
     AttachmentBody, SuggestionsCallbackTypes, SuggestionsResult, NoOptionsReason, AttachmentDestinationHint
 from switcore.ui.divider import Divider
-from switcore.ui.element_components import Tag, TagStyle, TagColorTypes, TagShapeTypes
+from switcore.ui.element_components import Tag, TagStyle
 from switcore.ui.header import Header, AttachmentHeader
 from switcore.ui.image import Image
 from switcore.ui.select import Option, OptionGroup
 from switcore.ui.text_paragraph import TextParagraph
 
 
 class SwitViewResponseTest(unittest.TestCase):
@@ -131,15 +131,15 @@
                 ),
                 tag=Tag(content="no style"),
                 action_id="test_action_id1"
             ),
             Option(
                 label="test label2",
                 action_id="test_action_id2",
-                tag=Tag(content="red rounded", style=TagStyle(color=TagColorTypes.danger, shape=TagShapeTypes.rounded)),
+                tag=Tag(content="red rounded", style=TagStyle(color='danger', shape='rounded')),
             ),
             Option(
                 label="test label3",
                 icon=Image(
                     image_url="https://files.swit.dev/webhook_logo.png",
                 ),
                 action_id="test_action_id3",
```

### Comparing `swit_core-4.0.1/tests/utils.py` & `swit_core-4.0.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_container.py` & `swit_core-4.0.2/tests/ui/test_container.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_datepicker.py` & `swit_core-4.0.2/tests/ui/test_datepicker.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_image_grid.py` & `swit_core-4.0.2/tests/ui/test_image_grid.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_info_card.py` & `swit_core-4.0.2/tests/ui/test_info_card.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_interactive_image.py` & `swit_core-4.0.2/tests/ui/test_interactive_image.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/tests/ui/test_select.py` & `swit_core-4.0.2/tests/ui/test_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from switcore.ui.element_components import OpenLink, Tag, TagStyle, TagColorTypes, TagShapeTypes
+from switcore.ui.element_components import OpenLink, Tag, TagStyle
 from switcore.ui.image import Image
 from switcore.ui.select import Select, Option, OptionGroup, SelectQuery, NoOptionsReason
 
 
 class SelectTest(unittest.TestCase):
 
     def test_valid_select01(self):
@@ -72,20 +72,20 @@
     def test_valid_select03(self):
         select = Select(
             trigger_on_input=True,
             options=[
                 Option(
                     label="test label1",
                     action_id="action_id1",
-                    tag=Tag(content="tag1", style=TagStyle(color=TagColorTypes.danger))
+                    tag=Tag(content="tag1", style=TagStyle(color='danger'))
                 ),
                 Option(
                     label="test label2",
                     action_id="action_id2",
-                    tag=Tag(content="tag1", style=TagStyle(color=TagColorTypes.primary, shape=TagShapeTypes.rounded))
+                    tag=Tag(content="tag1", style=TagStyle(color='primary', shape='rounded'))
                 ),
             ]
         )
 
         expected = {
             'type': 'select',
             'multiselect': False,
```

### Comparing `swit_core-4.0.1/tests/ui/test_static_action.py` & `swit_core-4.0.2/tests/ui/test_static_action.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate` & `swit_core-4.0.2/vvenv/bin/activate`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate.csh` & `swit_core-4.0.2/vvenv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate.fish` & `swit_core-4.0.2/vvenv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate.nu` & `swit_core-4.0.2/vvenv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate.ps1` & `swit_core-4.0.2/vvenv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/bin/activate_this.py` & `swit_core-4.0.2/vvenv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_virtualenv.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/_distutils_hack/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/__main__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/__pip-runner__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/build_env.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/configuration.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/pyproject.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/check.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/completion.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/debug.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/download.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/hash.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/help.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/index.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/install.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/list.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/search.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/show.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/base.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/collector.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/index/sources.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/locations/base.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/base.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/candidate.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/format_control.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/index.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/link.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/scheme.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/target_python.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/models/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/auth.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/download.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/session.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/check.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/constructors.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_file.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_install.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_set.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/base.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_log.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/logging.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/misc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/models.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/urls.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/git.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/six.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/core.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/api.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/help.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/models.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/align.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/box.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/console.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/control.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/json.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/status.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/style.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/table.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/text.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pip-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.pyi` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_core_metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_entry_points.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_imp.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_importlib.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_itertools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_normalization.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_path.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_reqs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/archive_util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/build_meta.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-32.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli-arm64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/cli.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/dep_util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/depends.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/discovery.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/dist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/errors.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/extension.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/glob.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-32.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui-arm64.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/gui.exe` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/installer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/launch.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/logging.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/monkey.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/msvc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/namespaces.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/package_index.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/sandbox.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/unicode_utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/warnings.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/warnings.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/windows_support.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_modified.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_modified.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/config.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/core.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/errors.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/extension.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/log.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.pyi` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.pyi` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/_requirestxt.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/_requirestxt.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/alias.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_clib.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_ext.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/build_py.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/develop.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/dist_info.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/easy_install.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/egg_info.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_lib.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/install_scripts.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/rotate.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/saveopts.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/sdist.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/setopt.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/test.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/command/upload_docs.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/expand.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/setupcfg.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools/extern/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/LICENSE` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/METADATA` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/RECORD` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/entry_points.txt` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/setuptools-69.1.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/_setuptools_logging.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/bdist_wheel.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/macosx_libfile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/metadata.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/util.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/wheelfile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/__init__.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/convert.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/pack.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/cli/unpack.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/LICENSE.txt` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/METADATA` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/RECORD` & `swit_core-4.0.2/vvenv/lib/python3.10/site-packages/wheel-0.42.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `swit_core-4.0.1/pyproject.toml` & `swit_core-4.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "swit-core"
-version = "4.0.1"
+version = "4.0.2"
 authors = [
     { name = "ur-team", email = "developers@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-#    'pydantic == 2.6.4',
+    'pydantic == 2.6.4',
     'httpx >=0.26.0',
     'fastapi ~=0.109.2',
     'SQLAlchemy >=2.0.27',
     'PyMySQL >=1.1.0',
     'ur-tunnel>=0.0.13',
     'python-dotenv>=1.0.1',
     'uvicorn>=0.27.1',
```

### Comparing `swit_core-4.0.1/PKG-INFO` & `swit_core-4.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: swit-core
-Version: 4.0.1
+Version: 4.0.2
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <developers@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: fastapi~=0.109.2
 Requires-Dist: httpx>=0.26.0
+Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: pymysql>=1.1.0
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: sqlalchemy>=2.0.27
 Requires-Dist: ur-tunnel>=0.0.13
 Requires-Dist: uvicorn>=0.27.1
 Description-Content-Type: text/markdown
```

