# Comparing `tmp/aiotgm-0.3.3.tar.gz` & `tmp/aiotgm-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.3.3.tar", last modified: Thu Apr  4 05:38:27 2024, max compression
+gzip compressed data, was "aiotgm-0.3.4.tar", last modified: Thu Apr  4 07:17:56 2024, max compression
```

## Comparing `aiotgm-0.3.3.tar` & `aiotgm-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.3/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-04 05:38:27.713581 aiotgm-0.3.3/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.3.3/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.709581 aiotgm-0.3.3/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-04 05:38:19.000000 aiotgm-0.3.3/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)    27882 2024-04-01 16:05:06.000000 aiotgm-0.3.3/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   281920 2024-04-04 04:02:20.000000 aiotgm-0.3.3/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.3/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.3/aiotgm/logging.py
--rw-r--r--   0 kali      (1000) root         (0)   278808 2024-04-04 05:34:44.000000 aiotgm-0.3.3/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.3/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.3/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-04 05:38:16.000000 aiotgm-0.3.3/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-04 05:38:27.713581 aiotgm-0.3.3/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.3/tests/test_func_ok.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 07:17:56.931897 aiotgm-0.3.4/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.4/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-04 07:17:56.931897 aiotgm-0.3.4/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1235 2024-04-04 07:17:27.000000 aiotgm-0.3.4/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 07:17:56.931897 aiotgm-0.3.4/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-04 07:16:57.000000 aiotgm-0.3.4/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    28031 2024-04-04 07:02:24.000000 aiotgm-0.3.4/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   283164 2024-04-04 07:07:39.000000 aiotgm-0.3.4/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.4/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.4/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   284942 2024-04-04 07:16:02.000000 aiotgm-0.3.4/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.4/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.4/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 07:17:56.931897 aiotgm-0.3.4/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42090 2024-04-04 07:17:56.000000 aiotgm-0.3.4/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-04 07:17:56.000000 aiotgm-0.3.4/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-04 07:17:56.000000 aiotgm-0.3.4/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-04 07:17:56.000000 aiotgm-0.3.4/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-04 07:17:56.000000 aiotgm-0.3.4/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-04 07:16:54.000000 aiotgm-0.3.4/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-04 07:17:56.931897 aiotgm-0.3.4/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 07:17:56.931897 aiotgm-0.3.4/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.4/tests/test_func_ok.py
```

### Comparing `aiotgm-0.3.3/LICENSE` & `aiotgm-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.3/PKG-INFO` & `aiotgm-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.3
+Version: 0.3.4
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -683,15 +683,15 @@
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.1
 Requires-Dist: certifi>=2023.11.17
 Requires-Dist: ujson>=5.9.0
 
 [![pypi](https://img.shields.io/badge/pypi-aiotgm-blue)](https://pypi.org/project/aiotgm/) [![tele](https://img.shields.io/badge/telegram-@unixtux-blue)](https://t.me/geko1) [![Documentation Status](https://readthedocs.org/projects/aiotgm/badge/?version=latest)](https://aiotgm.readthedocs.io/?badge=latest)
 
-<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#february-16-2024">7.1</a></h3>
+<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#march-31-2024">7.2</a></h3>
 
 #
 
 * #### Prerequisites
 You require a good python knowledge with the [asyncio module](https://docs.python.org/3/library/asyncio.html) and a Telegram Bot API token, you can get it via [@BotFather](https://t.me/botfather).
 
 #
```

### Comparing `aiotgm-0.3.3/README.md` & `aiotgm-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![pypi](https://img.shields.io/badge/pypi-aiotgm-blue)](https://pypi.org/project/aiotgm/) [![tele](https://img.shields.io/badge/telegram-@unixtux-blue)](https://t.me/geko1) [![Documentation Status](https://readthedocs.org/projects/aiotgm/badge/?version=latest)](https://aiotgm.readthedocs.io/?badge=latest)
 
-<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#february-16-2024">7.1</a></h3>
+<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#march-31-2024">7.2</a></h3>
 
 #
 
 * #### Prerequisites
 You require a good python knowledge with the [asyncio module](https://docs.python.org/3/library/asyncio.html) and a Telegram Bot API token, you can get it via [@BotFather](https://t.me/botfather).
 
 #
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [![pypi](https://img.shields.io/badge/pypi-aiotgm-blue)](https://pypi.org/
 project/aiotgm/) [![tele](https://img.shields.io/badge/telegram-@unixtux-blue)]
 (https://t.me/geko1) [![Documentation Status](https://readthedocs.org/projects/
 aiotgm/badge/?version=latest)](https://aiotgm.readthedocs.io/?badge=latest)
-   ******** AAssyynncchhrroonnoouuss ppyytthhoonn iimmpplleemmeennttaattiioonn ooff tthhee TTeelleeggrraamm BBoott AAPPII _77_.._11 ********
+   ******** AAssyynncchhrroonnoouuss ppyytthhoonn iimmpplleemmeennttaattiioonn ooff tthhee TTeelleeggrraamm BBoott AAPPII _77_.._22 ********
 # * #### Prerequisites You require a good python knowledge with the [asyncio
 module](https://docs.python.org/3/library/asyncio.html) and a Telegram Bot API
 token, you can get it via [@BotFather](https://t.me/botfather). # * ####
 Dependencies * Python >= 3.8 * [aiohttp](https://github.com/aio-libs/aiohttp) *
 Optional [ujson](https://github.com/ultrajson/ultrajson) & [certifi](https://
 github.com/certifi/python-certifi) # * #### Installation Install the module
 using [pip](https://pypi.org/project/aiotgm/) from your shell. ```powershell $
```

### Comparing `aiotgm-0.3.3/aiotgm/api.py` & `aiotgm-0.3.4/aiotgm/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,14 +623,18 @@
         method = 'reopenForumTopic'
         return await self._request(method, params)
 
     async def reopen_general_forum_topic(self, params: dict):
         method = 'reopenGeneralForumTopic'
         return await self._request(method, params)
 
+    async def replace_sticker_in_set(self, params: dict):
+        method = 'replaceStickerInSet'
+        return await self._request(method, params)
+
     async def restrict_chat_member(self, params: dict):
         method = 'restrictChatMember'
         return await self._request(method, params)
 
     async def revoke_chat_invite_link(self, params: dict):
         method = 'revokeChatInviteLink'
         return await self._request(method, params)
```

### Comparing `aiotgm-0.3.3/aiotgm/client.py` & `aiotgm-0.3.4/aiotgm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1068,18 +1068,17 @@
         user_id: int,
         name: str,
         sticker: InputSticker
     ) -> Literal[True]:
         '''
         https://core.telegram.org/bots/api#addstickertoset
 
-        Use this method to add a new sticker to a set created by the bot. The format of the
-        added sticker must match the format of the other stickers in the set. Emoji sticker
-        sets can have up to 200 stickers. Animated and video sticker sets can have up to 50
-        stickers. Static sticker sets can have up to 120 stickers. Returns :obj:`True` on success.
+        Use this method to add a new sticker to a set created by the bot.
+        Emoji sticker sets can have up to 200 stickers.
+        Other sticker sets can have up to 120 stickers. Returns :obj:`True` on success.
 
         :param user_id: User identifier of sticker set owner.
         :type user_id: :obj:`int`
         :param name: Sticker set name.
         :type name: :obj:`str`
         :param sticker: A JSON-serialized object with information about the added sticker. If exactly the same sticker had already been added to the set, then the set isn't changed.
         :type sticker: :obj:`~aiotgm.types.InputSticker`
@@ -1691,15 +1690,14 @@
 
     async def create_new_sticker_set(
         self,
         user_id: int,
         name: str,
         title: str,
         stickers: list[InputSticker],
-        sticker_format: str,
         sticker_type: Optional[str] = None,
         needs_repainting: Optional[bool] = None
     ) -> Literal[True]:
         '''
         https://core.telegram.org/bots/api#createnewstickerset
 
         Use this method to create a new sticker set owned by a user. The bot
@@ -1709,28 +1707,25 @@
         :type user_id: :obj:`int`
         :param name: Short name of sticker set, to be used in ``t.me/addstickers/`` URLs (e.g., *animals*). Can contain only English letters, digits and underscores. Must begin with a letter, can't contain consecutive underscores and must end in ``"_by_<bot_username>"``. ``<bot_username>`` is case insensitive. 1-64 characters.
         :type name: :obj:`str`
         :param title: Sticker set title, 1-64 characters.
         :type title: :obj:`str`
         :param stickers: A JSON-serialized list of 1-50 initial stickers to be added to the sticker set.
         :type stickers: :obj:`list` of :obj:`~aiotgm.types.InputSticker`
-        :param sticker_format: Format of stickers in the set, must be one of “static”, “animated”, “video”.
-        :type sticker_format: :obj:`str`
         :param sticker_type: Type of stickers in the set, pass “regular”, “mask”, or “custom_emoji”. By default, a regular sticker set is created.
         :type sticker_type: :obj:`str`, optional
         :param needs_repainting: Pass :obj:`True` if stickers in the sticker set must be repainted to the color of text when used in messages, the accent color if used as emoji status, white on chat photos, or another appropriate color based on context; for custom emoji sticker sets only.
         :type needs_repainting: :obj:`bool`, optional
         :rtype: :obj:`True`
         '''
         params = {
             'user_id': user_id,
             'name': name,
             'title': title,
-            'stickers': stickers,
-            'sticker_format': sticker_format
+            'stickers': stickers
         }
         if sticker_type is not None: params['sticker_type'] = sticker_type
         if needs_repainting is not None: params['needs_repainting'] = needs_repainting
         return await super().create_new_sticker_set(params)
 
 
     async def decline_chat_join_request(
@@ -3044,14 +3039,48 @@
         '''
         params = {
             'chat_id': chat_id
         }
         return await super().reopen_general_forum_topic(params)
 
 
+    async def replace_sticker_in_set(
+        self,
+        user_id: int,
+        name: str,
+        old_sticker: str,
+        sticker: InputSticker,
+    ) -> Literal[True]:
+        '''
+        https://core.telegram.org/bots/api#replacestickerinset
+
+        Use this method to replace an existing sticker in a sticker set with a new one.
+        The method is equivalent to calling :meth:`~aiotgm.Client.delete_sticker_from_set`,
+        then :meth:`~aiotgm.Client.add_sticker_to_set`, then :meth:`~aiotgm.Client.set_sticker_position_in_set`.
+        Returns :obj:`True` on success.
+
+        :param user_id: User identifier of the sticker set owner.
+        :type user_id: :obj:`int`
+        :param name: Sticker set name.
+        :type name: :obj:`str`
+        :param old_sticker: File identifier of the replaced sticker.
+        :type old_sticker: :obj:`str`
+        :param sticker: A JSON-serialized object with information about the added sticker. If exactly the same sticker had already been added to the set, then the set remains unchanged.
+        :type sticker: :obj:`~aiotgm.types.InputSticker`
+        :rtype: :obj:`True`
+        '''
+        params = {
+            'user_id': user_id,
+            'name': name,
+            'old_sticker': old_sticker,
+            'sticker': sticker
+        }
+        return await super().replace_sticker_in_set(params)
+
+
     async def restrict_chat_member(
         self,
         chat_id: Union[int, str],
         user_id: int,
         permissions: ChatPermissions,
         use_independent_chat_permissions: Optional[bool] = None,
         until_date: Optional[int] = None
@@ -4904,33 +4933,37 @@
         return await super().set_sticker_position_in_set(params)
 
 
     async def set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: int,
+        format: str,
         thumbnail: Optional[Union[InputFile, str]] = None
     ) -> Literal[True]:
         '''
         https://core.telegram.org/bots/api#setstickersetthumbnail
 
         Use this method to set the thumbnail of a regular or mask sticker set. The format of the
         thumbnail file must match the format of the stickers in the set. Returns :obj:`True` on success.
 
         :param name: Sticker set name.
         :type name: :obj:`str`
         :param user_id: User identifier of the sticker set owner.
         :type user_id: :obj:`int`
+        :param format: Format of the thumbnail, must be one of “static” for a **.WEBP** or **.PNG** image, “animated” for a **.TGS** animation, or “video” for a **WEBM** video.
+        :type format: :obj:`str`
         :param thumbnail: A **.WEBP** or **.PNG** image with the thumbnail, must be up to 128 kilobytes in size and have a width and height of exactly 100px, or a **.TGS** animation with a thumbnail up to 32 kilobytes in size (see https://core.telegram.org/stickers#animated-sticker-requirements for animated sticker technical requirements), or a **WEBM** video with the thumbnail up to 32 kilobytes in size; see https://core.telegram.org/stickers#video-sticker-requirements for video sticker technical requirements. Pass a *file_id* as a String to send a file that already exists on the Telegram servers, pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_. Animated and video sticker set thumbnails can't be uploaded via HTTP URL. If omitted, then the thumbnail is dropped and the first sticker is used as the thumbnail.
         :type thumbnail: :obj:`~aiotgm.types.InputFile` or :obj:`str`, optional
         :rtype: :obj:`True`
         '''
         params = {
             'name': name,
-            'user_id': user_id
+            'user_id': user_id,
+            'format': format
         }
         if thumbnail is not None: params['thumbnail'] = thumbnail
         return await super().set_sticker_set_thumbnail(params)
 
 
     async def set_sticker_set_title(
         self,
```

### Comparing `aiotgm-0.3.3/aiotgm/constants.py` & `aiotgm-0.3.4/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.3/aiotgm/logging.py` & `aiotgm-0.3.4/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.3/aiotgm/types.py` & `aiotgm-0.3.4/aiotgm/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 __all__ = (
     'REPLY_MARKUP_TYPES', # Union of all the reply markups
     'Animation',
     'Audio',
+    'Birthdate',
     'BotCommand',
     'BotCommandScope', # No deserialization.
     'BotCommandScopeAllChatAdministrators',
     'BotCommandScopeAllGroupChats',
     'BotCommandScopeAllPrivateChats',
     'BotCommandScopeChat',
     'BotCommandScopeChatAdministrators',
@@ -18,14 +19,16 @@
     'BotDescription',
     'BotName',
     'BotShortDescription',
     'BusinessConnection',
     'BusinessIntro',
     'BusinessLocation',
     'BusinessMessagesDeleted',
+    'BusinessOpeningHours',
+    'BusinessOpeningHoursInterval',
     'CallbackGame',
     'CallbackQuery',
     'Chat',
     'ChatAdministratorRights',
     'ChatBoost',
     'ChatBoostAdded',
     'ChatBoostRemoved',
@@ -160,14 +163,15 @@
     'ReactionTypeCustomEmoji',
     'ReactionTypeEmoji',
     'ReplyKeyboardMarkup',
     'ReplyKeyboardRemove',
     'ReplyParameters',
     'ResponseParameters',
     'SentWebAppMessage',
+    'SharedUser',
     'ShippingAddress',
     'ShippingOption',
     'ShippingQuery',
     'Sticker',
     'StickerSet',
     'Story',
     'SuccessfulPayment',
@@ -360,14 +364,45 @@
         self.title = title
         self.file_name = file_name
         self.mime_type = mime_type
         self.file_size = file_size
         self.thumbnail = thumbnail
 
 
+class Birthdate(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#birthdate
+
+    :param day: Day of the user's birth; 1-31.
+    :type day: :obj:`int`
+    :param month: Month of the user's birth; 1-12.
+    :type month: :obj:`int`
+    :param year: Year of the user's birth.
+    :type year: :obj:`int`, optional
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['day'] = res.get('day')
+        obj['month'] = res.get('month')
+        obj['year'] = res.get('year')
+        return cls(**obj)
+
+    def __init__(
+        self,
+        day: int,
+        month: int,
+        year: Optional[int] = None
+    ):
+        self.day = day
+        self.month = month
+        self.year = year
+
+
 class BotCommand(TelegramType):
     '''
     https://core.telegram.org/bots/api#botcommand
 
     This object represents a bot command.
 
     :param command: Text of the command; 1-32 characters. Can contain only lowercase English letters, digits and underscores.
@@ -691,14 +726,66 @@
         message_ids: list[int]
     ):
         self.business_connection_id = business_connection_id
         self.chat = chat
         self.message_ids = message_ids
 
 
+class BusinessOpeningHours(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businessopeninghours
+
+    :param time_zone_name: Unique name of the time zone for which the opening hours are defined.
+    :type time_zone_name: :obj:`str`
+    :param opening_hours: List of time intervals describing business opening hours.
+    :type opening_hours: :obj:`list` of :obj:`~aiotgm.types.BusinessOpeningHoursInterval`
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['time_zone_name'] = res.get('time_zone_name')
+        obj['opening_hours'] = [BusinessOpeningHoursInterval._dese(kwargs) for kwargs in res.get('opening_hours')]
+        return cls(**obj)
+
+    def __init__(
+        self,
+        time_zone_name: str,
+        opening_hours: list[BusinessOpeningHoursInterval]
+    ):
+        self.time_zone_name = time_zone_name
+        self.opening_hours = opening_hours
+
+
+class BusinessOpeningHoursInterval(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businessopeninghoursinterval
+
+    :param opening_minute: The minute's sequence number in a week, starting on Monday, marking the start of the time interval during which the business is open; 0 - 7 * 24 * 60.
+    :type opening_minute: :obj:`int`
+    :param closing_minute: The minute's sequence number in a week, starting on Monday, marking the end of the time interval during which the business is open; 0 - 8 * 24 * 60.
+    :type closing_minute: :obj:`int`
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['opening_minute'] = res.get('opening_minute')
+        obj['closing_minute'] = res.get('closing_minute')
+        return cls(**obj)
+
+    def __init__(
+        self,
+        opening_minute: int,
+        closing_minute: int
+    ):
+        self.opening_minute = opening_minute
+        self.closing_minute = closing_minute
+
+
 class CallbackGame(TelegramType):
     '''
     https://core.telegram.org/bots/api#callbackgame
 
     A placeholder, currently holds no information. Use `BotFather <https://t.me/botfather>`_ to set up your game.
     '''
     @classmethod
@@ -790,18 +877,24 @@
     :type last_name: :obj:`str`, optional
     :param is_forum: :obj:`True`, if the supergroup chat is a forum (has `topics <https://telegram.org/blog/topics-in-groups-collectible-usernames#topics-in-groups>`_ enabled).
     :type is_forum: :obj:`True`, optional
     :param photo: Chat photo. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type photo: :obj:`~aiotgm.types.ChatPhoto`, optional
     :param active_usernames: If non-empty, the list of all `active chat usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames#collectible-usernames>`_; for private chats, supergroups and channels. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type active_usernames: :obj:`list` of :obj:`str`, optional
+    :param birthdate: For private chats, the date of birth of the user. Returned only in :meth:`~aiotgm.Client.get_chat`.
+    :type birthdate: :obj:`~aiotgm.types.Birthdate`, optional
     :param business_intro: For private chats with business accounts, the intro of the business. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type business_intro: :obj:`~aiotgm.types.BusinessIntro`
     :param business_location: For private chats with business accounts, the location of the business. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type business_location: :obj:`~aiotgm.types.BusinessLocation`
+    :param business_opening_hours: For private chats with business accounts, the opening hours of the business. Returned only in :meth:`~aiotgm.Client.get_chat`.
+    :type business_opening_hours: :obj:`~aiotgm.types.BusinessOpeningHours`, optional
+    :param personal_chat: For private chats, the personal channel of the user. Returned only in :meth:`~aiotgm.Client.get_chat`.
+    :type personal_chat: :obj:`~aiotgm.types.Chat`, optional
     :param available_reactions: List of available reactions allowed in the chat. If omitted, then all :obj:`emoji reactions <aiotgm.types.ReactionTypeEmoji>` are allowed. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type available_reactions: :obj:`list` of :obj:`~aiotgm.types.ReactionType`, optional
     :param accent_color_id: Identifier of the accent color for the chat name and backgrounds of the chat photo, reply header, and link preview. See `accent colors <https://core.telegram.org/bots/api#accent-colors>`_ for more details. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type accent_color_id: :obj:`int`, optional
     :param background_custom_emoji_id: Custom emoji identifier of emoji chosen by the chat for the reply header and link preview background. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type background_custom_emoji_id: :obj:`str`, optional
     :param profile_accent_color_id: Identifier of the accent color for the chat's profile background. See `profile accent colors <https://core.telegram.org/bots/api#profile-accent-colors>`_ for more details. Returned only in :meth:`~aiotgm.Client.get_chat`.
@@ -864,16 +957,19 @@
         obj['title'] = res.get('title')
         obj['username'] = res.get('username')
         obj['first_name'] = res.get('first_name')
         obj['last_name'] = res.get('last_name')
         obj['is_forum'] = res.get('is_forum')
         obj['photo'] = ChatPhoto._dese(res.get('photo'))
         obj['active_usernames'] = res.get('active_usernames')
+        obj['birthdate'] = Birthdate._dese(res.get('birthdate'))
         obj['business_intro'] = BusinessIntro._dese(res.get('business_intro'))
         obj['business_location'] = BusinessLocation._dese(res.get('business_location'))
+        obj['business_opening_hours'] = BusinessOpeningHours._dese(res.get('business_opening_hours'))
+        obj['personal_chat'] = Chat._dese(res.get('personal_chat'))
         obj['available_reactions'] = [_dese_reaction_type(kwargs) for kwargs in res.get('available_reactions')] if 'available_reactions' in res else None
         obj['accent_color_id'] = res.get('accent_color_id')
         obj['background_custom_emoji_id'] = res.get('background_custom_emoji_id')
         obj['profile_accent_color_id'] = res.get('profile_accent_color_id')
         obj['profile_background_custom_emoji_id'] = res.get('profile_background_custom_emoji_id')
         obj['emoji_status_custom_emoji_id'] = res.get('emoji_status_custom_emoji_id')
         obj['emoji_status_expiration_date'] = res.get('emoji_status_expiration_date')
@@ -907,16 +1003,19 @@
         title: Optional[str] = None,
         username: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         is_forum: Optional[Literal[True]] = None,
         photo: Optional[ChatPhoto] = None,
         active_usernames: Optional[list[str]] = None,
+        birthdate: Optional[Birthdate] = None,
         business_intro: Optional[BusinessIntro] = None,
         business_location: Optional[BusinessLocation] = None,
+        business_opening_hours: Optional[BusinessOpeningHours] = None,
+        personal_chat: Optional[Chat] = None,
         available_reactions: Optional[list[ReactionType]] = None,
         accent_color_id: Optional[int] = None,
         background_custom_emoji_id: Optional[str] = None,
         profile_accent_color_id: Optional[int] = None,
         profile_background_custom_emoji_id: Optional[str] = None,
         emoji_status_custom_emoji_id: Optional[str] = None,
         emoji_status_expiration_date: Optional[int] = None,
@@ -947,16 +1046,19 @@
         self.title = title
         self.username = username
         self.first_name = first_name
         self.last_name = last_name
         self.is_forum = is_forum
         self.photo = photo
         self.active_usernames = active_usernames
+        self.birthdate = birthdate
         self.business_intro = business_intro
         self.business_location = business_location
+        self.business_opening_hours = business_opening_hours
+        self.personal_chat = personal_chat
         self.available_reactions = available_reactions
         self.accent_color_id = accent_color_id
         self.background_custom_emoji_id = background_custom_emoji_id
         self.profile_accent_color_id = profile_accent_color_id
         self.profile_background_custom_emoji_id = profile_background_custom_emoji_id
         self.emoji_status_custom_emoji_id = emoji_status_custom_emoji_id
         self.emoji_status_expiration_date = emoji_status_expiration_date
@@ -1944,23 +2046,32 @@
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['request_id'] = res.get('request_id')
         obj['chat_id'] = res.get('chat_id')
+        obj['title'] = res.get('title')
+        obj['username'] = res.get('username')
+        obj['photo'] = [PhotoSize._dese(kwargs) for kwargs in res.get('photo')] if 'photo' in res else None
         return cls(**obj)
 
     def __init__(
         self,
         request_id: int,
-        chat_id: int
+        chat_id: int,
+        title: Optional[str] = None,
+        username: Optional[str] = None,
+        photo: Optional[list[PhotoSize]] = None,
     ):
         self.request_id = request_id
         self.chat_id = chat_id
+        self.title = title
+        self.username = username
+        self.photo = photo
 
 
 class ChosenInlineResult(TelegramType):
     '''
     https://core.telegram.org/bots/api#choseninlineresult
 
     Represents a :obj:`result <aiotgm.types.InlineQueryResult>` of an
@@ -4200,41 +4311,44 @@
         obj['username'] = res.get('username')
         obj['language_code'] = res.get('language_code')
         obj['is_premium'] = res.get('is_premium')
         obj['added_to_attachment_menu'] = res.get('added_to_attachment_menu')
         obj['can_join_groups'] = res.get('can_join_groups')
         obj['can_read_all_group_messages'] = res.get('can_read_all_group_messages')
         obj['supports_inline_queries'] = res.get('supports_inline_queries')
+        obj['can_connect_to_business'] = res.get('can_connect_to_business')
         return cls(**obj)
 
     def __init__(
         self,
         id: int,
         is_bot: bool,
         first_name: str,
         last_name: Optional[str] = None,
         username: Optional[str] = None,
         language_code: Optional[str] = None,
         is_premium: Optional[Literal[True]] = None,
         added_to_attachment_menu: Optional[Literal[True]] = None,
         can_join_groups: Optional[bool] = None,
         can_read_all_group_messages: Optional[bool] = None,
-        supports_inline_queries: Optional[bool] = None
+        supports_inline_queries: Optional[bool] = None,
+        can_connect_to_business: Optional[bool] = None
     ):
         self.id = id
         self.is_bot = is_bot
         self.first_name = first_name
         self.last_name = last_name
         self.username = username
         self.language_code = language_code
         self.is_premium = is_premium
         self.added_to_attachment_menu = added_to_attachment_menu
         self.can_join_groups = can_join_groups
         self.can_read_all_group_messages = can_read_all_group_messages
         self.supports_inline_queries = supports_inline_queries
+        self.can_connect_to_business = can_connect_to_business
 
 
 class MessageEntity(TelegramType):
     '''
     https://core.telegram.org/bots/api#messageentity
 
     This object represents one special entity in a text message. For example, hashtags, usernames, URLs, etc.
@@ -4352,14 +4466,15 @@
         obj['reply_to_message'] = Message._dese(res.get('reply_to_message'))
         obj['external_reply'] = ExternalReplyInfo._dese(res.get('external_reply'))
         obj['quote'] = TextQuote._dese(res.get('quote'))
         obj['reply_to_story'] = Story._dese(res.get('reply_to_story'))
         obj['via_bot'] = User._dese(res.get('via_bot'))
         obj['edit_date'] = res.get('edit_date')
         obj['has_protected_content'] = res.get('has_protected_content')
+        obj['is_from_offline'] = res.get('is_from_offline')
         obj['media_group_id'] = res.get('media_group_id')
         obj['author_signature'] = res.get('author_signature')
         obj['text'] = res.get('text')
         obj['entities'] = [MessageEntity._dese(kwargs) for kwargs in res.get('entities')] if 'entities' in res else None
         obj['link_preview_options'] = LinkPreviewOptions._dese(res.get('link_preview_options'))
         obj['animation'] = Animation._dese(res.get('animation'))
         obj['audio'] = Audio._dese(res.get('audio'))
@@ -4435,14 +4550,15 @@
         reply_to_message: Optional[Message] = None,
         external_reply: Optional[ExternalReplyInfo] = None,
         quote: Optional[TextQuote] = None,
         reply_to_story: Optional[Story] = None,
         via_bot: Optional[User] = None,
         edit_date: Optional[int] = None,
         has_protected_content: Optional[Literal[True]] = None,
+        is_from_offline: Optional[Literal[True]] = None,
         media_group_id: Optional[str] = None,
         author_signature: Optional[str] = None,
         text: str = None,
         entities: Optional[list[MessageEntity]] = None,
         link_preview_options: Optional[LinkPreviewOptions] = None,
         animation: Optional[Animation] = None,
         audio: Optional[Audio] = None,
@@ -4515,14 +4631,15 @@
         self.reply_to_message = reply_to_message
         self.external_reply = external_reply
         self.quote = quote
         self.reply_to_story = reply_to_story
         self.via_bot = via_bot
         self.edit_date = edit_date
         self.has_protected_content = has_protected_content
+        self.is_from_offline = is_from_offline
         self.media_group_id = media_group_id
         self.author_signature = author_signature
         self.text = text or str() # If not text, it's str() instead of None
         self.entities = entities
         self.link_preview_options = link_preview_options
         self.animation = animation
         self.audio = audio
@@ -5222,24 +5339,24 @@
     were shared with the bot using a KeyboardButtonRequestUsers button.
     '''
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['request_id'] = res.get('request_id')
-        obj['user_ids'] = res.get('user_ids')
+        obj['users'] = [SharedUser._dese(kwargs) for kwargs in res.get('users')]
         return cls(**obj)
 
     def __init__(
         self,
         request_id: int,
-        user_ids: list[int]
+        users: list[SharedUser]
     ):
         self.request_id = request_id
-        self.user_ids = user_ids
+        self.users = users
 
 
 class WriteAccessAllowed(TelegramType):
     '''
     https://core.telegram.org/bots/api#writeaccessallowed
 
     This object represents a service message about a user allowing a bot to write
@@ -5339,14 +5456,47 @@
     def __init__(
         self,
         users: list[User]
     ):
         self.users = users
 
 
+class SharedUser(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#shareduser
+
+    This object contains information about a user that was shared with
+    the bot using a :obj:`~aiotgm.types.KeyboardButtonRequestUser` button.
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['user_id'] = res.get('user_id')
+        obj['first_name'] = res.get('first_name')
+        obj['last_name'] = res.get('last_name')
+        obj['username'] = res.get('username')
+        obj['photo'] = [PhotoSize._dese(kwargs) for kwargs in res.get('photo')] if 'photo' in res else None
+        return cls(**obj)
+
+    def __init__(
+        self,
+        user_id: int,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
+        username: Optional[str] = None,
+        photo: Optional[list[PhotoSize]] = None
+    ):
+        self.user_id = user_id
+        self.first_name = first_name
+        self.last_name = last_name
+        self.username = username
+        self.photo = photo
+
+
 class UserProfilePhotos(TelegramType):
     '''
     https://core.telegram.org/bots/api#userprofilephotos
 
     This object represent a user's profile pictures.
     '''
     @classmethod
@@ -5394,20 +5544,26 @@
     The identifiers of the selected users will be shared with the bot when the corresponding button is pressed.
     '''
     def __init__(
         self,
         request_id: int,
         user_is_bot: Optional[bool] = None,
         user_is_premium: Optional[bool] = None,
-        max_quantity: Optional[int] = None
+        max_quantity: Optional[int] = None,
+        request_name: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None
     ):
         self.request_id = request_id
         self.user_is_bot = user_is_bot
         self.user_is_premium = user_is_premium
         self.max_quantity = max_quantity
+        self.request_name = request_name
+        self.request_username = request_username
+        self.request_photo = request_photo
 
 
 class KeyboardButtonRequestChat(TelegramType):
     '''
     https://core.telegram.org/bots/api#keyboardbuttonrequestchat
 
     This object defines the criteria used to request a suitable chat.
@@ -5418,24 +5574,30 @@
         request_id: int,
         chat_is_channel: bool,
         chat_is_forum: Optional[bool] = None,
         chat_has_username: Optional[bool] = None,
         chat_is_created: Optional[bool] = None,
         user_administrator_rights: Optional[ChatAdministratorRights] = None,
         bot_administrator_rights: Optional[ChatAdministratorRights] = None,
-        bot_is_member: Optional[bool] = None
+        bot_is_member: Optional[bool] = None,
+        request_title: Optional[bool] = None,
+        request_username: Optional[bool] = None,
+        request_photo: Optional[bool] = None
     ):
         self.request_id = request_id
         self.chat_is_channel = chat_is_channel
         self.chat_is_forum = chat_is_forum
         self.chat_has_username = chat_has_username
         self.chat_is_created = chat_is_created
         self.user_administrator_rights = user_administrator_rights
         self.bot_administrator_rights = bot_administrator_rights
         self.bot_is_member = bot_is_member
+        self.request_title = request_title
+        self.request_username = request_username
+        self.request_photo = request_photo
 
 
 class KeyboardButtonPollType(TelegramType):
     '''
     https://core.telegram.org/bots/api#keyboardbuttonpolltype
 
     This object represents type of a poll, which is allowed to
@@ -5965,53 +6127,49 @@
     @classmethod
     @_parse_result
     def _dese(cls, res: dict):
         obj = {}
         obj['name'] = res.get('name')
         obj['title'] = res.get('title')
         obj['sticker_type'] = res.get('sticker_type')
-        obj['is_animated'] = res.get('is_animated')
-        obj['is_video'] = res.get('is_video')
         obj['stickers'] = [Sticker._dese(kwargs) for kwargs in res.get('stickers')]
         obj['thumbnail'] = PhotoSize._dese(res.get('thumbnail'))
         return cls(**obj)
 
     def __init__(
         self,
         name: str,
         title: str,
         sticker_type: str,
-        is_animated: bool,
-        is_video: bool,
         stickers: list[Sticker],
         thumbnail: Optional[PhotoSize] = None
     ):
         self.name = name
         self.title = title
         self.sticker_type = sticker_type
-        self.is_animated = is_animated
-        self.is_video = is_video
         self.stickers = stickers
         self.thumbnail = thumbnail
 
 
 class InputSticker(TelegramType):
     '''
     https://core.telegram.org/bots/api#inputsticker
 
     This object describes a sticker to be added to a sticker set.
     '''
     def __init__(
         self,
         sticker: Union[InputFile, str],
+        format: str,
         emoji_list: list[str],
         mask_position: Optional[MaskPosition] = None,
         keywords: Optional[list[str]] = None
     ):
         self.sticker = sticker
+        self.format = format
         self.emoji_list = emoji_list
         self.mask_position = mask_position
         self.keywords = keywords
 
 
 class InlineQueryResultsButton(TelegramType):
     '''
```

### Comparing `aiotgm-0.3.3/aiotgm/update_manager.py` & `aiotgm-0.3.4/aiotgm/update_manager.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.3/aiotgm/utils.py` & `aiotgm-0.3.4/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.3/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.3.4/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.3
+Version: 0.3.4
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -683,15 +683,15 @@
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.1
 Requires-Dist: certifi>=2023.11.17
 Requires-Dist: ujson>=5.9.0
 
 [![pypi](https://img.shields.io/badge/pypi-aiotgm-blue)](https://pypi.org/project/aiotgm/) [![tele](https://img.shields.io/badge/telegram-@unixtux-blue)](https://t.me/geko1) [![Documentation Status](https://readthedocs.org/projects/aiotgm/badge/?version=latest)](https://aiotgm.readthedocs.io/?badge=latest)
 
-<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#february-16-2024">7.1</a></h3>
+<h3 align="center">Asynchronous python implementation of the Telegram Bot API <a href="https://core.telegram.org/bots/api#march-31-2024">7.2</a></h3>
 
 #
 
 * #### Prerequisites
 You require a good python knowledge with the [asyncio module](https://docs.python.org/3/library/asyncio.html) and a Telegram Bot API token, you can get it via [@BotFather](https://t.me/botfather).
 
 #
```

### Comparing `aiotgm-0.3.3/tests/test_func_ok.py` & `aiotgm-0.3.4/tests/test_func_ok.py`

 * *Files identical despite different names*

