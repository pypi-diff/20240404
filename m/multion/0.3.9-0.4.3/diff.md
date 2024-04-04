# Comparing `tmp/multion-0.3.9.tar.gz` & `tmp/multion-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-0.3.9.tar", max compression
+gzip compressed data, was "multion-0.4.3.tar", max compression
```

## Comparing `multion-0.3.9.tar` & `multion-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,37 @@
--rw-r--r--   0        0        0      430 2023-11-13 09:36:59.549533 multion-0.3.9/README.md
--rw-r--r--   0        0        0      673 2023-12-29 10:34:32.121763 multion-0.3.9/multion/__init__.py
--rw-r--r--   0        0        0     5843 2023-12-29 10:24:05.141435 multion-0.3.9/multion/browser.py
--rw-r--r--   0        0        0    26146 2023-12-30 10:53:48.694787 multion-0.3.9/multion/multion.py
--rw-r--r--   0        0        0      204 2023-12-28 04:57:57.148958 multion-0.3.9/multion/secrets.json
--rw-r--r--   0        0        0      326 2023-12-27 09:39:18.632218 multion-0.3.9/multion/setup.py
--rw-r--r--   0        0        0      475 2023-12-30 10:53:56.826492 multion-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 multion-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     3846 2024-04-04 08:18:10.851647 multion-0.4.3/README.md
+-rw-r--r--   0        0        0      592 2024-04-04 08:18:10.851647 multion-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      990 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/__init__.py
+-rw-r--r--   0        0        0    14297 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/client.py
+-rw-r--r--   0        0        0      853 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/request_options.py
+-rw-r--r--   0        0        0      162 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/environment.py
+-rw-r--r--   0        0        0      170 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/py.typed
+-rw-r--r--   0        0        0      247 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    25066 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      341 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0      953 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0      967 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0      812 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0      953 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0      850 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1312 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1361 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1650 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_input.py
+-rw-r--r--   0        0        0     1016 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_input_browser_params.py
+-rw-r--r--   0        0        0     1365 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0      972 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/version.py
+-rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 multion-0.4.3/PKG-INFO
```

