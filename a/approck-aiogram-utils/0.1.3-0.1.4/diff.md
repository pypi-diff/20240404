# Comparing `tmp/approck_aiogram_utils-0.1.3.tar.gz` & `tmp/approck_aiogram_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.3.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.4.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.3.tar` & `approck_aiogram_utils-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5104 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      773 2024-04-03 21:48:21.401008 approck_aiogram_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-03 22:06:08.758443 approck_aiogram_utils-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:06:08.787443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-03 22:06:08.759443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5129 2024-04-03 22:06:08.759443 approck_aiogram_utils-0.1.4/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-03 22:06:08.760443 approck_aiogram_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.4/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/app.py` & `approck_aiogram_utils-0.1.4/approck_aiogram_utils/integration/uprock/app.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.3/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.4/approck_aiogram_utils/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,38 +31,38 @@
             for media in message.media or []:
                 caption = None
 
                 if not is_caption_added:
                     caption = message.caption
 
                 if media.type.startswith("image"):
-                    media_group.append(InputMediaPhoto(media=URLInputFile(url=media.url), caption=caption))
+                    media_group.append(InputMediaPhoto(media=URLInputFile(url=str(media.url)), caption=caption))
                 elif media.type.startswith("video"):
-                    media_group.append(InputMediaVideo(media=URLInputFile(url=media.url), caption=caption))
+                    media_group.append(InputMediaVideo(media=URLInputFile(url=str(media.url)), caption=caption))
 
             # NOTE:
             #  pyo3_runtime.PanicException: called `Result::unwrap()` on an `Err` value: PyErr { type: <class 'KeyError'>, value: KeyError('parse_mode'), traceback: None }
             # if media:
             #     media[0].caption = dto.caption
 
             await bot.send_media_group(chat_id=chat_id, media=media_group)
         else:
             media = message.media[0]
 
             if media.type.startswith("image"):
                 await bot.send_photo(
                     chat_id=chat_id,
-                    photo=URLInputFile(url=media.url),
+                    photo=URLInputFile(url=str(media.url)),
                     caption=message.caption,
                     reply_markup=reply_markup,
                 )
             elif media.type.startswith("video"):
                 await bot.send_video(
                     chat_id=chat_id,
-                    video=URLInputFile(url=media.url),
+                    video=URLInputFile(url=str(media.url)),
                     caption=message.caption,
                     reply_markup=reply_markup,
                 )
     else:
         if message.caption:
             await bot.send_message(
                 chat_id=chat_id, text=message.caption, disable_web_page_preview=True, reply_markup=reply_markup
@@ -72,15 +72,15 @@
 async def _send_message_video_note(
     bot: Bot,
     chat_id: Union[int, str],
     message: Message,
     reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove, ForceReply]] = None,
 ) -> None:
     await bot.send_video_note(
-        chat_id=chat_id, video_note=URLInputFile(url=message.video_note.url), reply_markup=reply_markup
+        chat_id=chat_id, video_note=URLInputFile(url=str(message.video_note.url)), reply_markup=reply_markup
     )
 
 
 async def _send_message_impl(
     bot: Bot,
     chat_id: Union[int, str],
     message: Message,
```

### Comparing `approck_aiogram_utils-0.1.3/pyproject.toml` & `approck_aiogram_utils-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
```

### Comparing `approck_aiogram_utils-0.1.3/PKG-INFO` & `approck_aiogram_utils-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

