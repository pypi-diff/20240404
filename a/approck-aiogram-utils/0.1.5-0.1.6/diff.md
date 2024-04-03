# Comparing `tmp/approck_aiogram_utils-0.1.5.tar.gz` & `tmp/approck_aiogram_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.5.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.6.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.5.tar` & `approck_aiogram_utils-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2024-04-03 22:31:26.121170 approck_aiogram_utils-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5254 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      773 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-03 23:25:30.935647 approck_aiogram_utils-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:25:30.957647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-03 23:25:30.935647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5342 2024-04-03 23:25:30.936647 approck_aiogram_utils-0.1.6/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-03 23:25:30.936647 approck_aiogram_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.6/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/app.py` & `approck_aiogram_utils-0.1.6/approck_aiogram_utils/integration/uprock/app.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.5/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.6/approck_aiogram_utils/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,18 @@
                 caption = None
 
                 if not is_caption_added:
                     caption = message.caption
 
                 if media.type.startswith("image"):
                     media_group.append(InputMediaPhoto(media=URLInputFile(url=str(media.url)), caption=caption))
+                    is_caption_added = True
                 elif media.type.startswith("video"):
                     media_group.append(InputMediaVideo(media=URLInputFile(url=str(media.url)), caption=caption))
+                    is_caption_added = True
 
             # NOTE:
             #  pyo3_runtime.PanicException: called `Result::unwrap()` on an `Err` value: PyErr { type: <class 'KeyError'>, value: KeyError('parse_mode'), traceback: None }
             # if media:
             #     media[0].caption = dto.caption
 
             await bot.send_media_group(chat_id=chat_id, media=media_group)
```

### Comparing `approck_aiogram_utils-0.1.5/pyproject.toml` & `approck_aiogram_utils-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
```

### Comparing `approck_aiogram_utils-0.1.5/PKG-INFO` & `approck_aiogram_utils-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

