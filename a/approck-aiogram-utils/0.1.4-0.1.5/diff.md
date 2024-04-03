# Comparing `tmp/approck_aiogram_utils-0.1.4.tar.gz` & `tmp/approck_aiogram_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.4.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.5.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.4.tar` & `approck_aiogram_utils-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2024-04-03 22:06:08.758443 approck_aiogram_utils-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-03 22:06:08.759443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5129 2024-04-03 22:06:08.759443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      773 2024-04-03 22:06:08.760443 approck_aiogram_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-03 22:31:26.121170 approck_aiogram_utils-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:31:26.145169 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5254 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-03 22:31:26.122170 approck_aiogram_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.5/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/app.py` & `approck_aiogram_utils-0.1.5/approck_aiogram_utils/integration/uprock/app.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.4/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.5/approck_aiogram_utils/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
     try:
         await _send_message_impl(bot=bot, chat_id=chat_id, message=message, reply_markup=reply_markup)
     except TelegramForbiddenError as exc:
         logger.info("Forbidden: {}", exc.message)
     except TelegramBadRequest as exc:
         if "USER_IS_BLOCKED" in exc.message:
             logger.info("Forbidden: {}", exc.message)
+        elif "VOICE_MESSAGES_FORBIDDEN" in exc.message:
+            logger.info("Voice messages forbidden: {}", exc.message)
         else:
             logger.exception("Unable to send message")
             raise
     except TelegramRetryAfter as exc:
         await asyncio.sleep(exc.retry_after)
         await send_message(bot=bot, chat_id=chat_id, message=message, reply_markup=reply_markup)  # Recursive call
     except Exception:
```

### Comparing `approck_aiogram_utils-0.1.4/pyproject.toml` & `approck_aiogram_utils-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
```

### Comparing `approck_aiogram_utils-0.1.4/PKG-INFO` & `approck_aiogram_utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

