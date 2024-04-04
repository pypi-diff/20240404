# Comparing `tmp/aiotgm-0.3.2.tar.gz` & `tmp/aiotgm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotgm-0.3.2.tar", last modified: Mon Apr  1 15:41:08 2024, max compression
+gzip compressed data, was "aiotgm-0.3.3.tar", last modified: Thu Apr  4 05:38:27 2024, max compression
```

## Comparing `aiotgm-0.3.2.tar` & `aiotgm-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:41:08.581712 aiotgm-0.3.2/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.2/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 15:41:08.581712 aiotgm-0.3.2/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.3.2/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:41:08.577712 aiotgm-0.3.2/aiotgm/
--rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-01 15:39:20.000000 aiotgm-0.3.2/aiotgm/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)    27730 2024-03-30 13:15:28.000000 aiotgm-0.3.2/aiotgm/api.py
--rw-r--r--   0 kali      (1000) root         (0)   273097 2024-04-01 15:19:49.000000 aiotgm-0.3.2/aiotgm/client.py
--rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.2/aiotgm/constants.py
--rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.2/aiotgm/logging.py
--rw-r--r--   0 kali      (1000) root         (0)   275742 2024-04-01 15:40:03.000000 aiotgm-0.3.2/aiotgm/types.py
--rw-r--r--   0 kali      (1000) root         (0)     8932 2024-04-01 15:14:03.000000 aiotgm-0.3.2/aiotgm/update_manager.py
--rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.2/aiotgm/utils.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:41:08.581712 aiotgm-0.3.2/aiotgm.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-01 15:41:08.000000 aiotgm-0.3.2/aiotgm.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-01 15:41:08.000000 aiotgm-0.3.2/aiotgm.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-01 15:41:08.000000 aiotgm-0.3.2/aiotgm.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-01 15:41:08.000000 aiotgm-0.3.2/aiotgm.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 15:41:08.000000 aiotgm-0.3.2/aiotgm.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-01 15:39:18.000000 aiotgm-0.3.2/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-01 15:41:08.581712 aiotgm-0.3.2/setup.cfg
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 15:41:08.581712 aiotgm-0.3.2/tests/
--rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.2/tests/test_func_ok.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2023-12-11 13:46:43.000000 aiotgm-0.3.3/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-04 05:38:27.713581 aiotgm-0.3.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)     1238 2024-03-14 20:23:30.000000 aiotgm-0.3.3/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.709581 aiotgm-0.3.3/aiotgm/
+-rw-r--r--   0 kali      (1000) root         (0)      320 2024-04-04 05:38:19.000000 aiotgm-0.3.3/aiotgm/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)    27882 2024-04-01 16:05:06.000000 aiotgm-0.3.3/aiotgm/api.py
+-rw-r--r--   0 kali      (1000) root         (0)   281920 2024-04-04 04:02:20.000000 aiotgm-0.3.3/aiotgm/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     3123 2024-02-29 15:03:03.000000 aiotgm-0.3.3/aiotgm/constants.py
+-rw-r--r--   0 kali      (1000) root         (0)      740 2024-04-01 12:33:00.000000 aiotgm-0.3.3/aiotgm/logging.py
+-rw-r--r--   0 kali      (1000) root         (0)   278808 2024-04-04 05:34:44.000000 aiotgm-0.3.3/aiotgm/types.py
+-rw-r--r--   0 kali      (1000) root         (0)     9152 2024-04-01 15:47:24.000000 aiotgm-0.3.3/aiotgm/update_manager.py
+-rw-r--r--   0 kali      (1000) root         (0)      623 2024-03-17 17:13:52.000000 aiotgm-0.3.3/aiotgm/utils.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/aiotgm.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    42093 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      348 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)       48 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-04 05:38:27.000000 aiotgm-0.3.3/aiotgm.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      441 2024-04-04 05:38:16.000000 aiotgm-0.3.3/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-04 05:38:27.713581 aiotgm-0.3.3/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-04 05:38:27.713581 aiotgm-0.3.3/tests/
+-rw-r--r--   0 kali      (1000) root         (0)     1471 2024-03-14 20:26:02.000000 aiotgm-0.3.3/tests/test_func_ok.py
```

### Comparing `aiotgm-0.3.2/LICENSE` & `aiotgm-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.2/PKG-INFO` & `aiotgm-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.2
+Version: 0.3.3
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.2/README.md` & `aiotgm-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.2/aiotgm/api.py` & `aiotgm-0.3.3/aiotgm/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,14 +515,18 @@
         method = 'forwardMessage'
         return await self._request(method, params)
 
     async def forward_messages(self, params: dict):
         method = 'forwardMessages'
         return await self._request(method, params)
 
+    async def get_business_connection(self, params: dict):
+        method = 'getBusinessConnection'
+        return await self._request(method, params)
+
     async def get_chat(self, params: dict):
         method = 'getChat'
         return await self._request(method, params)
 
     async def get_chat_administrators(self, params: dict):
         method = 'getChatAdministrators'
         return await self._request(method, params)
```

### Comparing `aiotgm-0.3.2/aiotgm/client.py` & `aiotgm-0.3.3/aiotgm/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     MESSAGE_MANAGER,
     EDITED_MESSAGE_MANAGER, 
     CHANNEL_POST_MANAGER, 
     EDITED_CHANNEL_POST_MANAGER,
     BUSINESS_CONNECTION_MANAGER,
     BUSINESS_MESSAGE_MANAGER,
     EDITED_BUSINESS_MESSAGE_MANAGER,
+    DELETED_BUSINESS_MESSAGES_MANAGER,
     MESSAGE_REACTION_MANAGER,
     MESSAGE_REACTION_COUNT_MANAGER,
     INLINE_QUERY_MANAGER,
     CHOSEN_INLINE_RESULT_MANAGER,
     CALLBACK_QUERY_MANAGER,
     SHIPPING_QUERY_MANAGER,
     PRE_CHECKOUT_QUERY_MANAGER,
@@ -89,14 +90,15 @@
         self._message_manager = UpdateManager(MESSAGE_MANAGER, Message)
         self._edited_message_manager = UpdateManager(EDITED_MESSAGE_MANAGER, Message)
         self._channel_post_manager = UpdateManager(CHANNEL_POST_MANAGER, Message)
         self._edited_channel_post_manager = UpdateManager(EDITED_CHANNEL_POST_MANAGER, Message)
         self._business_connection_manager = UpdateManager(BUSINESS_CONNECTION_MANAGER, BusinessConnection)
         self._business_message_manager = UpdateManager(BUSINESS_MESSAGE_MANAGER, Message)
         self._edited_business_message_manager = UpdateManager(EDITED_BUSINESS_MESSAGE_MANAGER, Message)
+        self._deleted_business_messages_manager = UpdateManager(DELETED_BUSINESS_MESSAGES_MANAGER, BusinessMessagesDeleted)
         self._message_reaction_manager = UpdateManager(MESSAGE_REACTION_MANAGER, MessageReactionUpdated)
         self._message_reaction_count_manager = UpdateManager(MESSAGE_REACTION_COUNT_MANAGER, MessageReactionCountUpdated)
         self._inline_query_manager = UpdateManager(INLINE_QUERY_MANAGER, InlineQuery)
         self._chosen_inline_result_manager = UpdateManager(CHOSEN_INLINE_RESULT_MANAGER, ChosenInlineResult)
         self._callback_query_manager = UpdateManager(CALLBACK_QUERY_MANAGER, CallbackQuery)
         self._shipping_query_manager = UpdateManager(SHIPPING_QUERY_MANAGER, ShippingQuery)
         self._pre_checkout_query_manager = UpdateManager(PRE_CHECKOUT_QUERY_MANAGER, PreCheckoutQuery)
@@ -361,15 +363,45 @@
 
             asyncio.run(bot.long_polling())
 
         :param checker: A function that takes only one argument to check an incoming *edited_business_message* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
         :type checker: :obj:`Callable[[Message], Any]`
         '''
         def wrap(coroutine: Callable[[Message], Awaitable]):
-            self._business_message_manager.add_rule(checker, coroutine)
+            self._edited_business_message_manager.add_rule(checker, coroutine)
+        return wrap
+
+    def manage_deleted_business_messages(self, checker: Callable[[BusinessMessagesDeleted], Any] = lambda deleted_business_messages: ..., /):
+        '''
+        You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
+        inside this decorator to manage an incoming *deleted_business_messages* :obj:`~aiotgm.types.Update`.
+        The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.BusinessMessagesDeleted`.
+        Then you need to call the method :meth:`~aiotgm.Client.long_polling` using the function `asyncio.run() <https://docs.python.org/3/library/asyncio-runner.html#asyncio.run>`_ to process the :obj:`~aiotgm.types.BusinessMessagesDeleted` update.
+
+        Usage:
+
+        .. code-block:: python3
+
+            import aiotgm
+            import asyncio
+            from aiotgm.types import BusinessMessagesDeleted
+
+            bot = aiotgm.Client('<your_api_token>')
+
+            @bot.manage_deleted_business_messages(lambda deleted_business_messages: deleted_business_messages.chat.id == xyz)
+            async def foo(deleted_business_messages: BusinessMessagesDeleted):
+                ...
+
+            asyncio.run(bot.long_polling())
+
+        :param checker: A function that takes only one argument to check an incoming *deleted_business_messages* :obj:`~aiotgm.types.Update`. E.g. a lambda function.
+        :type checker: :obj:`Callable[[BusinessMessagesDeleted], Any]`
+        '''
+        def wrap(coroutine: Callable[[BusinessMessagesDeleted], Awaitable]):
+            self._deleted_business_messages_manager.add_rule(checker, coroutine)
         return wrap
 
     def manage_message_reaction(self, checker: Callable[[MessageReactionUpdated], Any] = lambda message_reaction: ..., /):
         '''
         You must wrap a `coroutine <https://docs.python.org/3/library/asyncio-task.html#coroutines>`_
         inside this decorator to manage an incoming *message_reaction* :obj:`~aiotgm.types.Update`.
         The coroutine must takes only one argument, it will be processed as :obj:`~aiotgm.types.MessageReactionUpdated`.
@@ -920,14 +952,21 @@
         elif update.edited_business_message:
             obj: Message = update.edited_business_message
             for rule in self._edited_business_message_manager:
                 result = await _run_coroutine(rule, obj)
                 if not _is_next_function(result):
                     return
 
+        elif update.deleted_business_messages:
+            obj: BusinessMessagesDeleted = update.deleted_business_messages
+            for rule in self._deleted_business_messages_manager:
+                result = await _run_coroutine(rule, obj)
+                if not _is_next_function(result):
+                    return
+
         elif update.message_reaction:
             obj: MessageReactionUpdated = update.message_reaction
             for rule in self._message_reaction_manager:
                 result = await _run_coroutine(rule, obj)
                 if not _is_next_function(result):
                     return
 
@@ -2331,14 +2370,35 @@
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         result = await super().forward_messages(params)
         return [MessageId._dese(mid) for mid in result]
 
 
+    async def get_business_connection(
+        self,
+        business_connection_id: str
+    ) -> BusinessConnection:
+        '''
+        https://core.telegram.org/bots/api#getbusinessconnection
+
+        Use this method to get information about the connection of the bot with a business account.
+        Returns a :obj:`~aiotgm.types.BusinessConnection` object on success.
+
+        :param business_connection_id: Unique identifier of the business connection.
+        :type business_connection_id: :obj:`str`
+        :rtype: :obj:`~aiotgm.types.BusinessConnection`
+        '''
+        params = {
+            'business_connection_id': business_connection_id
+        }
+        result = await super().get_business_connection(params)
+        return BusinessConnection._dese(result)
+
+
     async def get_chat(
         self,
         chat_id: Union[int, str]
     ) -> Chat:
         '''
         https://core.telegram.org/bots/api#getchat
 
@@ -3051,14 +3111,15 @@
         return ChatInviteLink._dese(result)
 
 
     async def send_animation(
         self,
         chat_id: Union[int, str],
         animation: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
@@ -3076,14 +3137,16 @@
         On success, the sent :obj:`~aiotgm.types.Message` is returned. Bots can currently
         send animation files of up to 50 MB in size, this limit may be changed in the future.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param animation: Animation to send. Pass a file_id as String to send an animation that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get an animation from the Internet, or upload a new animation using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type animation: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param duration: Duration of sent animation in seconds.
         :type duration: :obj:`int`, optional
         :param width: Animation width.
         :type width: :obj:`int`, optional
         :param height: Animation height.
@@ -3108,14 +3171,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'animation': animation
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if duration is not None: params['duration'] = duration
         if width is not None: params['width'] = width
         if height is not None: params['height'] = height
         if thumbnail is not None: params['thumbnail'] = thumbnail
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
@@ -3131,14 +3195,15 @@
         return Message._dese(result)
 
 
     async def send_audio(
         self,
         chat_id: Union[int, str],
         audio: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[list[MessageEntity]] = None,
         duration: Optional[int] = None,
         performer: Optional[str] = None,
         title: Optional[str] = None,
@@ -3156,14 +3221,16 @@
         is returned. Bots can currently send audio files of up to 50 MB in size, this limit may be changed in the
         future. For sending voice messages, use the :meth:`~aiotgm.Client.send_voice` method instead.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param audio: Audio file to send. Pass a file_id as String to send an audio file that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get an audio file from the Internet, or upload a new one using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type audio: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param caption: Audio caption, 0-1024 characters after entities parsing.
         :type caption: :obj:`str`, optional
         :param parse_mode: Mode for parsing entities in the audio caption. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
         :type parse_mode: :obj:`str`, optional
         :param caption_entities: A JSON-serialized list of special entities that appear in the caption, which can be specified instead of *parse_mode*.
@@ -3186,14 +3253,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'audio': audio
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
         elif self.parse_mode is not None: params['parse_mode'] = self.parse_mode
         if caption_entities is not None: params['caption_entities'] = caption_entities
         if duration is not None: params['duration'] = duration
         if performer is not None: params['performer'] = performer
@@ -3208,14 +3276,15 @@
         return Message._dese(result)
 
 
     async def send_chat_action(
         self,
         chat_id: Union[int, str],
         action: str,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None
     ) -> Literal[True]:
         '''
         https://core.telegram.org/bots/api#sendchataction
 
         Use this method when you need to tell the user that something is happening on
         the bot's side. The status is set for 5 seconds or less (when a message arrives
@@ -3228,31 +3297,35 @@
 
         We only recommend using this method when a response from the bot will take a **noticeable** amount of time to arrive.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param action: Type of action to broadcast. Choose one, depending on what the user is about to receive: *typing* for :obj:`text messages <aiotgm.Client.send_message>`, *upload_photo* for :obj:`photos <aiotgm.Client.send_photo>`, *record_video* or *upload_video* for :obj:`videos <aiotgm.Client.send_video>`, *record_voice* or *upload_voice* for :obj:`voice notes <aiotgm.Client.send_voice>`, *upload_document* for :obj:`general files <aiotgm.Client.send_document>`, *choose_sticker* for :obj:`stickers <aiotgm.Client.send_sticker>`, *find_location* for :obj:`location data <aiotgm.Client.send_location>`, *record_video_note* or *upload_video_note* for :obj:`video notes <aiotgm.Client.send_video_note>`.
         :type action: :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the action will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread; for supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :rtype: :obj:`True`
         '''
         params = {
             'chat_id': chat_id,
             'action': action
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         return await super().send_chat_action(params)
 
 
     async def send_contact(
         self,
         chat_id: Union[int, str],
         phone_number: str,
         first_name: str,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         last_name: Optional[str] = None,
         vcard: Optional[str] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
         reply_markup: Optional[REPLY_MARKUP_TYPES] = None
@@ -3265,14 +3338,16 @@
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param phone_number: Contact's phone number.
         :type phone_number: :obj:`str`
         :param first_name: Contact's first name.
         :type first_name: :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param last_name: Contact's last name.
         :type last_name: :obj:`str`, optional
         :param vcard: Additional data about the contact in the form of a `vCard <https://en.wikipedia.org/wiki/VCard>`_, 0-2048 bytes.
         :type vcard: :obj:`str`, optional
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
@@ -3286,14 +3361,15 @@
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'phone_number': phone_number,
             'first_name': first_name
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if last_name is not None: params['last_name'] = last_name
         if vcard is not None: params['vcard'] = vcard
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         if reply_parameters is not None: params['reply_parameters'] = reply_parameters
@@ -3301,14 +3377,15 @@
         result = await super().send_contact(params)
         return Message._dese(result)
 
 
     async def send_dice(
         self,
         chat_id: Union[int, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         emoji: Optional[str] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
         reply_markup: Optional[REPLY_MARKUP_TYPES] = None
     ) -> Message:
@@ -3316,14 +3393,16 @@
         https://core.telegram.org/bots/api#senddice
 
         Use this method to send an animated emoji that will display a random
         value. On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param emoji: Emoji on which the dice throw animation is based. Currently, must be one of “🎲”, “🎯”, “🏀”, “⚽”, “🎳”, or “🎰”. Dice can have values 1-6 for “🎲”, “🎯” and “🎳”, values 1-5 for “🏀” and “⚽”, and values 1-64 for “🎰”. Defaults to “🎲”.
         :type emoji: :obj:`str`, optional
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding.
@@ -3333,14 +3412,15 @@
         :param reply_markup: Additional interface options. A JSON-serialized object for an `inline keyboard <https://core.telegram.org/bots/features#inline-keyboards>`_, `custom reply keyboard <https://core.telegram.org/bots/features#keyboards>`_, instructions to remove reply keyboard or to force a reply from the user.
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if emoji is not None: params['emoji'] = emoji
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         if reply_parameters is not None: params['reply_parameters'] = reply_parameters
         if reply_markup is not None: params['reply_markup'] = reply_markup
@@ -3348,14 +3428,15 @@
         return Message._dese(result)
 
 
     async def send_document(
         self,
         chat_id: Union[int, str],
         document: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[list[MessageEntity]] = None,
         disable_content_type_detection: Optional[bool] = None,
         disable_notification: Optional[bool] = None,
@@ -3370,14 +3451,16 @@
         On success, the sent :obj:`~aiotgm.types.Message` is returned.
         Bots can currently send files of any type of up to 50 MB in size, this limit may be changed in the future.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param document: File to send. Pass a file_id as String to send a file that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type document: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the file is supported server-side. The thumbnail should be in JPEG format and less than 200 kB in size. A thumbnail's width and height should not exceed 320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails can't be reused and can be only uploaded as a new file, so you can pass “attach://<file_attach_name>” if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type thumbnail: :obj:`~aiotgm.types.InputFile` or :obj:`str`, optional
         :param caption: Document caption (may also be used when resending documents by *file_id*), 0-1024 characters after entities parsing.
         :type caption: :obj:`str`, optional
         :param parse_mode: Mode for parsing entities in the document caption. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
@@ -3396,14 +3479,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'document': document
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if thumbnail is not None: params['thumbnail'] = thumbnail
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
         elif self.parse_mode is not None: params['parse_mode'] = self.parse_mode
         if caption_entities is not None: params['caption_entities'] = caption_entities
         if disable_content_type_detection is not None: params['disable_content_type_detection'] = disable_content_type_detection
@@ -3416,14 +3500,15 @@
         return Message._dese(result)
 
 
     async def send_game(
         self,
         chat_id: int,
         game_short_name: str,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
         reply_markup: Optional[InlineKeyboardMarkup] = None
     ) -> Message:
         '''
@@ -3432,14 +3517,16 @@
         Use this method to send a game.
         On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat.
         :type chat_id: :obj:`int`
         :param game_short_name: Short name of the game, serves as the unique identifier for the game. Set up your games via `@BotFather <https://t.me/botfather>`_.
         :type game_short_name: :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
@@ -3448,14 +3535,15 @@
         :type reply_markup: :obj:`~aiotgm.types.InlineKeyboardMarkup`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'game_short_name': game_short_name
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         if reply_parameters is not None: params['reply_parameters'] = reply_parameters
         if reply_markup is not None: params['reply_markup'] = reply_markup
         result = await super().send_game(params)
@@ -3589,14 +3677,15 @@
 
 
     async def send_location(
         self,
         chat_id: Union[int, str],
         latitude: float,
         longitude: float,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         live_period: Optional[int] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
@@ -3611,14 +3700,16 @@
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param latitude: Latitude of the location.
         :type latitude: :obj:`float`
         :param longitude: Longitude of the location.
         :type longitude: :obj:`float`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500.
         :type horizontal_accuracy: :obj:`float`, optional
         :param live_period: Period in seconds for which the location will be updated (see `Live Locations <https://telegram.org/blog/live-locations>`_, should be between 60 and 86400.
         :type live_period: :obj:`int`, optional
         :param heading: For live locations, a direction in which the user is moving, in degrees. Must be between 1 and 360 if specified.
@@ -3636,14 +3727,15 @@
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'latitude': latitude,
             'longitude': longitude
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if horizontal_accuracy is not None: params['horizontal_accuracy'] = horizontal_accuracy
         if live_period is not None: params['live_period'] = live_period
         if heading is not None: params['heading'] = heading
         if proximity_alert_radius is not None: params['proximity_alert_radius'] = proximity_alert_radius
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
@@ -3654,14 +3746,15 @@
         return Message._dese(result)
 
 
     async def send_media_group(
         self,
         chat_id: Union[int, str],
         media: list[Union[InputMediaAudio, InputMediaDocument, InputMediaPhoto, InputMediaVideo]],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None
     ) -> list[Message]:
         '''
         https://core.telegram.org/bots/api#sendmediagroup
@@ -3670,41 +3763,45 @@
         Documents and audio files can be only grouped in an album with messages of the same type.
         On success, an array of :obj:`Messages <aiotgm.types.Message>` that were sent is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param media: A JSON-serialized array describing messages to be sent, must include 2-10 items.
         :type media: :obj:`list` of :obj:`~aiotgm.types.InputMediaAudio`, :obj:`~aiotgm.types.InputMediaDocument`, :obj:`~aiotgm.types.InputMediaPhoto` and :obj:`~aiotgm.types.InputMediaVideo`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param disable_notification: Sends messages `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent messages from forwarding and saving.
         :type protect_content: :obj:`bool`, optional
         :param reply_parameters: Description of the message to reply to.
         :type reply_parameters: :obj:`~aiotgm.types.ReplyParameters`, optional
         :rtype: :obj:`list` of :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'media': media
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         if reply_parameters is not None: params['reply_parameters'] = reply_parameters
         result = await super().send_media_group(params)
         return [Message._dese(message) for message in result]
 
 
     async def send_message(
         self,
         chat_id: Union[int, str],
         text: str,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         parse_mode: Optional[str] = None,
         entities: Optional[list[MessageEntity]] = None,
         link_preview_options: Optional[LinkPreviewOptions] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
@@ -3716,14 +3813,16 @@
         Use this method to send text messages.
         On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param text: Text of the message to be sent, 1-4096 characters after entities parsing.
         :type text: :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param parse_mode: Mode for parsing entities in the message text. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
         :type parse_mode: :obj:`str`, optional
         :param entities: A JSON-serialized list of special entities that appear in message text, which can be specified instead of *parse_mode*.
         :type entities: :obj:`list` of :obj:`~aiotgm.types.MessageEntity`, optional
         :param link_preview_options: Link preview generation options for the message.
@@ -3738,14 +3837,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'text': text
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if parse_mode is not None: params['parse_mode'] = parse_mode
         elif self.parse_mode is not None: params['parse_mode'] = self.parse_mode
         if entities is not None: params['entities'] = entities
         if link_preview_options is not None: params['link_preview_options'] = link_preview_options
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
@@ -3756,14 +3856,15 @@
         return Message._dese(result)
 
 
     async def send_photo(
         self,
         chat_id: Union[int, str],
         photo: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[list[MessageEntity]] = None,
         has_spoiler: Optional[bool] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
@@ -3776,14 +3877,16 @@
         Use this method to send photos.
         On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param photo: Photo to send. Pass a file_id as String to send a photo that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get a photo from the Internet, or upload a new photo using multipart/form-data. The photo must be at most 10 MB in size. The photo's width and height must not exceed 10000 in total. Width and height ratio must be at most 20. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type photo: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param caption: Photo caption (may also be used when resending photos by *file_id*), 0-1024 characters after entities parsing.
         :type caption: :obj:`str`, optional
         :param parse_mode: Mode for parsing entities in the photo caption. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
         :type parse_mode: :obj:`str`, optional
         :param caption_entities: A JSON-serialized list of special entities that appear in the caption, which can be specified instead of *parse_mode*.
@@ -3800,14 +3903,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'photo': photo
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
         elif self.parse_mode is not None: params['parse_mode'] = self.parse_mode
         if caption_entities is not None: params['caption_entities'] = caption_entities
         if has_spoiler is not None: params['has_spoiler'] = has_spoiler
         if disable_notification is not None: params['disable_notification'] = disable_notification
@@ -3820,14 +3924,15 @@
 
 
     async def send_poll(
         self,
         chat_id: Union[int, str],
         question: str,
         options: list[str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,
         allows_multiple_answers: Optional[bool] = None,
         correct_option_id: Optional[int] = None,
         explanation: Optional[str] = None,
         explanation_parse_mode: Optional[str] = None,
@@ -3848,14 +3953,16 @@
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param question: Poll question, 1-300 characters.
         :type question: :obj:`str`
         :param options: A JSON-serialized list of answer options, 2-10 strings 1-100 characters each.
         :type options: :obj:`list` of :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param is_anonymous: :obj:`True`, if the poll needs to be anonymous, defaults to :obj:`True`.
         :type is_anonymous: :obj:`bool`, optional
         :param type: Poll type, “quiz” or “regular”, defaults to “regular”.
         :type type: :obj:`str`, optional
         :param allows_multiple_answers: :obj:`True`, if the poll allows multiple answers, ignored for polls in quiz mode, defaults to :obj:`False`.
@@ -3885,14 +3992,15 @@
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'question': question,
             'options': options
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if is_anonymous is not None: params['is_anonymous'] = is_anonymous
         if type is not None: params['type'] = type
         if allows_multiple_answers is not None: params['allows_multiple_answers'] = allows_multiple_answers
         if correct_option_id is not None: params['correct_option_id'] = correct_option_id
         if explanation is not None: params['explanation'] = explanation
         if explanation_parse_mode is not None: params['explanation_parse_mode'] = explanation_parse_mode
@@ -3909,14 +4017,15 @@
         return Message._dese(result)
 
 
     async def send_sticker(
         self,
         chat_id: Union[int, str],
         sticker: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         emoji: Optional[str] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
         reply_markup: Optional[REPLY_MARKUP_TYPES] = None
     ) -> Message:
@@ -3926,14 +4035,16 @@
         Use this method to send static .WEBP, `animated <https://telegram.org/blog/animated-stickers>`_ .TGS, or `video <https://telegram.org/blog/video-stickers-better-reactions>`_ .WEBM stickers.
         On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param sticker: Sticker to send. Pass a file_id as String to send a file that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get a .WEBP sticker from the Internet, or upload a new .WEBP or .TGS sticker using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_. Video stickers can only be sent by a file_id. Animated stickers can't be sent via an HTTP URL.
         :type sticker: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param emoji: Emoji associated with the sticker; only for just uploaded stickers.
         :type emoji: :obj:`str`, optional
         :param disable_notification: Sends the message `silently <https://telegram.org/blog/channels-2-0#silent-messages>`_. Users will receive a notification with no sound.
         :type disable_notification: :obj:`bool`, optional
         :param protect_content: Protects the contents of the sent message from forwarding and saving.
@@ -3944,14 +4055,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'sticker': sticker
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if emoji is not None: params['emoji'] = emoji
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
         if reply_parameters is not None: params['reply_parameters'] = reply_parameters
         if reply_markup is not None: params['reply_markup'] = reply_markup
@@ -3962,14 +4074,15 @@
     async def send_venue(
         self,
         chat_id: Union[int, str],
         latitude: float,
         longitude: float,
         title: str,
         address: str,
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         foursquare_id: Optional[str] = None,
         foursquare_type: Optional[str] = None,
         google_place_id: Optional[str] = None,
         google_place_type: Optional[str] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
@@ -3988,14 +4101,16 @@
         :type latitude: :obj:`float`
         :param longitude: Longitude of the venue.
         :type longitude: :obj:`float`
         :param title: Name of the venue.
         :type title: :obj:`str`
         :param address: Address of the venue.
         :type address: :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param foursquare_id: Foursquare identifier of the venue.
         :type foursquare_id: :obj:`str`, optional
         :param foursquare_type: Foursquare type of the venue, if known. (For example, “arts_entertainment/default”, “arts_entertainment/aquarium” or “food/icecream”.)
         :type foursquare_type: :obj:`str`, optional
         :param google_place_id: Google Places identifier of the venue.
@@ -4015,14 +4130,15 @@
         params = {
             'chat_id': chat_id,
             'latitude': latitude,
             'longitude': longitude,
             'title': title,
             'address': address
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if foursquare_id is not None: params['foursquare_id'] = foursquare_id
         if foursquare_type is not None: params['foursquare_type'] = foursquare_type
         if google_place_id is not None: params['google_place_id'] = google_place_id
         if google_place_type is not None: params['google_place_type'] = google_place_type
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
@@ -4033,14 +4149,15 @@
         return Message._dese(result)
 
 
     async def send_video(
         self,
         chat_id: Union[int, str],
         video: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
@@ -4060,14 +4177,16 @@
         the sent :obj:`~aiotgm.types.Message` is returned. Bots can currently send
         video files of up to 50 MB in size, this limit may be changed in the future.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param video: Video to send. Pass a file_id as String to send a video that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get a video from the Internet, or upload a new video using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type video: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param duration: Duration of sent video in seconds.
         :type duration: :obj:`int`, optional
         :param width: Video width.
         :type width: :obj:`int`, optional
         :param height: Video height.
@@ -4094,14 +4213,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'video': video
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if duration is not None: params['duration'] = duration
         if width is not None: params['width'] = width
         if height is not None: params['height'] = height
         if thumbnail is not None: params['thumbnail'] = thumbnail
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
@@ -4118,14 +4238,15 @@
         return Message._dese(result)
 
 
     async def send_video_note(
         self,
         chat_id: Union[int, str],
         video_note: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         length: Optional[int] = None,
         thumbnail: Optional[Union[InputFile, str]] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_parameters: Optional[ReplyParameters] = None,
@@ -4138,14 +4259,16 @@
         Telegram clients support rounded square MPEG4 videos of up to 1 minute long. Use this
         method to send video messages. On success, the sent :obj:`~aiotgm.types.Message` is returned.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param video_note: Video note to send. Pass a file_id as String to send a video note that exists on the Telegram servers (recommended) or upload a new video using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_. Sending video notes by a URL is currently unsupported.
         :type video_note: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param duration: Duration of sent video in seconds.
         :type duration: :obj:`int`, optional
         :param length: Video width and height, i.e. diameter of the video message.
         :type length: :obj:`int`, optional
         :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the file is supported server-side. The thumbnail should be in JPEG format and less than 200 kB in size. A thumbnail's width and height should not exceed 320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails can't be reused and can be only uploaded as a new file, so you can pass “attach://<file_attach_name>” if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
@@ -4160,14 +4283,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'video_note': video_note
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if duration is not None: params['duration'] = duration
         if length is not None: params['length'] = length
         if thumbnail is not None: params['thumbnail'] = thumbnail
         if disable_notification is not None: params['disable_notification'] = disable_notification
         if protect_content is not None: params['protect_content'] = protect_content
         elif self.protect_content is not None: params['protect_content'] = self.protect_content
@@ -4177,14 +4301,15 @@
         return Message._dese(result)
 
 
     async def send_voice(
         self,
         chat_id: Union[int, str],
         voice: Union[InputFile, str],
+        business_connection_id: Optional[str] = None,
         message_thread_id: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[list[MessageEntity]] = None,
         duration: Optional[int] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
@@ -4200,14 +4325,16 @@
         On success, the sent :obj:`~aiotgm.types.Message` is returned. Bots can currently send voice
         messages of up to 50 MB in size, this limit may be changed in the future.
 
         :param chat_id: Unique identifier for the target chat or username of the target channel (in the format ``@channelusername``).
         :type chat_id: :obj:`int` or :obj:`str`
         :param voice: Audio file to send. Pass a file_id as String to send a file that exists on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one using multipart/form-data. `More information on Sending Files » <https://core.telegram.org/bots/api#sending-files>`_.
         :type voice: :obj:`~aiotgm.types.InputFile` or :obj:`str`
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message will be sent.
+        :type business_connection_id: :obj:`str`, optional
         :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for forum supergroups only.
         :type message_thread_id: :obj:`int`, optional
         :param caption: Voice message caption, 0-1024 characters after entities parsing.
         :type caption: :obj:`str`, optional
         :param parse_mode: Mode for parsing entities in the voice message caption. See `formatting options <https://core.telegram.org/bots/api#formatting-options>`_ for more details.
         :type parse_mode: :obj:`str`, optional
         :param caption_entities: A JSON-serialized list of special entities that appear in the caption, which can be specified instead of *parse_mode*.
@@ -4224,14 +4351,15 @@
         :type reply_markup: :obj:`~aiotgm.types.REPLY_MARKUP_TYPES`, optional
         :rtype: :obj:`~aiotgm.types.Message`
         '''
         params = {
             'chat_id': chat_id,
             'voice': voice
         }
+        if business_connection_id is not None: params['business_connection_id'] = business_connection_id
         if message_thread_id is not None: params['message_thread_id'] = message_thread_id
         if caption is not None: params['caption'] = caption
         if parse_mode is not None: params['parse_mode'] = parse_mode
         elif self.parse_mode is not None: params['parse_mode'] = self.parse_mode
         if caption_entities is not None: params['caption_entities'] = caption_entities
         if duration is not None: params['duration'] = duration
         if disable_notification is not None: params['disable_notification'] = disable_notification
```

### Comparing `aiotgm-0.3.2/aiotgm/constants.py` & `aiotgm-0.3.3/aiotgm/constants.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.2/aiotgm/logging.py` & `aiotgm-0.3.3/aiotgm/logging.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.2/aiotgm/types.py` & `aiotgm-0.3.3/aiotgm/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     'BotCommandScopeChatAdministrators',
     'BotCommandScopeChatMember',
     'BotCommandScopeDefault',
     'BotDescription',
     'BotName',
     'BotShortDescription',
     'BusinessConnection',
+    'BusinessIntro',
+    'BusinessLocation',
     'BusinessMessagesDeleted',
     'CallbackGame',
     'CallbackQuery',
     'Chat',
     'ChatAdministratorRights',
     'ChatBoost',
     'ChatBoostAdded',
@@ -599,14 +601,71 @@
         self.user = user
         self.user_chat_id = user_chat_id
         self.date = date
         self.can_reply = can_reply
         self.is_enabled = is_enabled
 
 
+class BusinessIntro(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businessintro
+
+    :param title: Title text of the business intro.
+    :type title: :obj:`str`, optional
+    :param message: Message text of the business intro.
+    :type message: :obj:`str`, optional
+    :param sticker: Sticker of the business intro.
+    :type sticker: :obj:`~aiotgm.types.Sticker`, optional
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['title'] = res.get('title')
+        obj['message'] = res.get('message')
+        obj['sticker'] = Sticker._dese(res.get('sticker'))
+        return cls(**obj)
+
+    def __init__(
+        self,
+        title: Optional[str] = None,
+        message: Optional[str] = None,
+        sticker: Optional[Sticker] = None
+    ):
+        self.title = title
+        self.message = message
+        self.sticker = sticker
+
+
+class BusinessLocation(TelegramType):
+    '''
+    https://core.telegram.org/bots/api#businesslocation
+
+    :param address: Address of the business.
+    :type address: :obj:`str`
+    :param location: Location of the business.
+    :type location: :obj:`~aiotgm.types.Location`, optional
+    '''
+    @classmethod
+    @_parse_result
+    def _dese(cls, res: dict):
+        obj = {}
+        obj['address'] = res.get('address')
+        obj['location'] = Location._dese(res.get('location'))
+        return cls(**obj)
+
+    def __init__(
+        self,
+        address: str,
+        location: Optional[Location] = None
+    ):
+        self.address = address
+        self.location = location
+
+
 class BusinessMessagesDeleted(TelegramType):
     '''
     https://core.telegram.org/bots/api#businessmessagesdeleted
 
     This object is received when messages are deleted from a connected business account.
 
     :param business_connection_id: Unique identifier of the business connection.
@@ -731,14 +790,18 @@
     :type last_name: :obj:`str`, optional
     :param is_forum: :obj:`True`, if the supergroup chat is a forum (has `topics <https://telegram.org/blog/topics-in-groups-collectible-usernames#topics-in-groups>`_ enabled).
     :type is_forum: :obj:`True`, optional
     :param photo: Chat photo. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type photo: :obj:`~aiotgm.types.ChatPhoto`, optional
     :param active_usernames: If non-empty, the list of all `active chat usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames#collectible-usernames>`_; for private chats, supergroups and channels. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type active_usernames: :obj:`list` of :obj:`str`, optional
+    :param business_intro: For private chats with business accounts, the intro of the business. Returned only in :meth:`~aiotgm.Client.get_chat`.
+    :type business_intro: :obj:`~aiotgm.types.BusinessIntro`
+    :param business_location: For private chats with business accounts, the location of the business. Returned only in :meth:`~aiotgm.Client.get_chat`.
+    :type business_location: :obj:`~aiotgm.types.BusinessLocation`
     :param available_reactions: List of available reactions allowed in the chat. If omitted, then all :obj:`emoji reactions <aiotgm.types.ReactionTypeEmoji>` are allowed. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type available_reactions: :obj:`list` of :obj:`~aiotgm.types.ReactionType`, optional
     :param accent_color_id: Identifier of the accent color for the chat name and backgrounds of the chat photo, reply header, and link preview. See `accent colors <https://core.telegram.org/bots/api#accent-colors>`_ for more details. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type accent_color_id: :obj:`int`, optional
     :param background_custom_emoji_id: Custom emoji identifier of emoji chosen by the chat for the reply header and link preview background. Returned only in :meth:`~aiotgm.Client.get_chat`.
     :type background_custom_emoji_id: :obj:`str`, optional
     :param profile_accent_color_id: Identifier of the accent color for the chat's profile background. See `profile accent colors <https://core.telegram.org/bots/api#profile-accent-colors>`_ for more details. Returned only in :meth:`~aiotgm.Client.get_chat`.
@@ -801,14 +864,16 @@
         obj['title'] = res.get('title')
         obj['username'] = res.get('username')
         obj['first_name'] = res.get('first_name')
         obj['last_name'] = res.get('last_name')
         obj['is_forum'] = res.get('is_forum')
         obj['photo'] = ChatPhoto._dese(res.get('photo'))
         obj['active_usernames'] = res.get('active_usernames')
+        obj['business_intro'] = BusinessIntro._dese(res.get('business_intro'))
+        obj['business_location'] = BusinessLocation._dese(res.get('business_location'))
         obj['available_reactions'] = [_dese_reaction_type(kwargs) for kwargs in res.get('available_reactions')] if 'available_reactions' in res else None
         obj['accent_color_id'] = res.get('accent_color_id')
         obj['background_custom_emoji_id'] = res.get('background_custom_emoji_id')
         obj['profile_accent_color_id'] = res.get('profile_accent_color_id')
         obj['profile_background_custom_emoji_id'] = res.get('profile_background_custom_emoji_id')
         obj['emoji_status_custom_emoji_id'] = res.get('emoji_status_custom_emoji_id')
         obj['emoji_status_expiration_date'] = res.get('emoji_status_expiration_date')
@@ -842,14 +907,16 @@
         title: Optional[str] = None,
         username: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         is_forum: Optional[Literal[True]] = None,
         photo: Optional[ChatPhoto] = None,
         active_usernames: Optional[list[str]] = None,
+        business_intro: Optional[BusinessIntro] = None,
+        business_location: Optional[BusinessLocation] = None,
         available_reactions: Optional[list[ReactionType]] = None,
         accent_color_id: Optional[int] = None,
         background_custom_emoji_id: Optional[str] = None,
         profile_accent_color_id: Optional[int] = None,
         profile_background_custom_emoji_id: Optional[str] = None,
         emoji_status_custom_emoji_id: Optional[str] = None,
         emoji_status_expiration_date: Optional[int] = None,
@@ -880,14 +947,16 @@
         self.title = title
         self.username = username
         self.first_name = first_name
         self.last_name = last_name
         self.is_forum = is_forum
         self.photo = photo
         self.active_usernames = active_usernames
+        self.business_intro = business_intro
+        self.business_location = business_location
         self.available_reactions = available_reactions
         self.accent_color_id = accent_color_id
         self.background_custom_emoji_id = background_custom_emoji_id
         self.profile_accent_color_id = profile_accent_color_id
         self.profile_background_custom_emoji_id = profile_background_custom_emoji_id
         self.emoji_status_custom_emoji_id = emoji_status_custom_emoji_id
         self.emoji_status_expiration_date = emoji_status_expiration_date
@@ -4271,14 +4340,16 @@
         obj['message_id'] = res.get('message_id')
         obj['date'] = res.get('date')
         obj['chat'] = Chat._dese(res.get('chat'))
         obj['message_thread_id'] = res.get('message_thread_id')
         obj['from_user'] = User._dese(res.get('from_user'))
         obj['sender_chat'] = Chat._dese(res.get('sender_chat'))
         obj['sender_boost_count'] = res.get('sender_boost_count')
+        obj['sender_business_bot'] = User._dese(res.get('sender_business_bot'))
+        obj['business_connection_id'] = res.get('business_connection_id')
         obj['forward_origin'] = _dese_message_origin(res.get('forward_origin'))
         obj['is_topic_message'] = res.get('is_topic_message')
         obj['is_automatic_forward'] = res.get('is_automatic_forward')
         obj['reply_to_message'] = Message._dese(res.get('reply_to_message'))
         obj['external_reply'] = ExternalReplyInfo._dese(res.get('external_reply'))
         obj['quote'] = TextQuote._dese(res.get('quote'))
         obj['reply_to_story'] = Story._dese(res.get('reply_to_story'))
@@ -4352,14 +4423,16 @@
         message_id: int,
         date: int,
         chat: Chat,
         message_thread_id: Optional[int] = None,
         from_user: Optional[User] = None,
         sender_chat: Optional[Chat] = None,
         sender_boost_count: Optional[int] = None,
+        sender_business_bot: Optional[User] = None,
+        business_connection_id: Optional[str] = None,
         forward_origin: Optional[MessageOrigin] = None,
         is_topic_message: Optional[Literal[True]] = None,
         is_automatic_forward: Optional[Literal[True]] = None,
         reply_to_message: Optional[Message] = None,
         external_reply: Optional[ExternalReplyInfo] = None,
         quote: Optional[TextQuote] = None,
         reply_to_story: Optional[Story] = None,
@@ -4430,14 +4503,16 @@
         self.message_id = message_id
         self.date = date
         self.chat = chat
         self.message_thread_id = message_thread_id
         self.from_user = from_user
         self.sender_chat = sender_chat
         self.sender_boost_count = sender_boost_count
+        self.sender_business_bot = sender_business_bot
+        self.business_connection_id = business_connection_id
         self.forward_origin = forward_origin
         self.is_topic_message = is_topic_message
         self.is_automatic_forward = is_automatic_forward
         self.reply_to_message = reply_to_message
         self.external_reply = external_reply
         self.quote = quote
         self.reply_to_story = reply_to_story
@@ -6857,14 +6932,15 @@
         obj['message'] = Message._dese(res.get('message'))
         obj['edited_message'] = Message._dese(res.get('edited_message'))
         obj['channel_post'] = Message._dese(res.get('channel_post'))
         obj['edited_channel_post'] = Message._dese(res.get('edited_channel_post'))
         obj['business_connection'] = BusinessConnection._dese(res.get('business_connection'))
         obj['business_message'] = Message._dese(res.get('business_message'))
         obj['edited_business_message'] = Message._dese(res.get('edited_business_message'))
+        obj['deleted_business_messages'] = BusinessMessagesDeleted._dese(res.get('deleted_business_messages'))
         obj['message_reaction'] = MessageReactionUpdated._dese(res.get('message_reaction'))
         obj['message_reaction_count'] = MessageReactionCountUpdated._dese(res.get('message_reaction_count'))
         obj['inline_query'] = InlineQuery._dese(res.get('inline_query'))
         obj['chosen_inline_result'] = ChosenInlineResult._dese(res.get('chosen_inline_result'))
         obj['callback_query'] = CallbackQuery._dese(res.get('callback_query'))
         obj['shipping_query'] = ShippingQuery._dese(res.get('shipping_query'))
         obj['pre_checkout_query'] = PreCheckoutQuery._dese(res.get('pre_checkout_query'))
@@ -6883,14 +6959,15 @@
         message: Optional[Message] = None,
         edited_message: Optional[Message] = None,
         channel_post: Optional[Message] = None,
         edited_channel_post: Optional[Message] = None,
         business_connection: Optional[BusinessConnection] = None,
         business_message: Optional[Message] = None,
         edited_business_message: Optional[Message] = None,
+        deleted_business_messages: Optional[BusinessMessagesDeleted] = None,
         message_reaction: Optional[MessageReactionUpdated] = None,
         message_reaction_count: Optional[MessageReactionCountUpdated] = None,
         inline_query: Optional[InlineQuery] = None,
         chosen_inline_result: Optional[ChosenInlineResult] = None,
         callback_query: Optional[CallbackQuery] = None,
         shipping_query: Optional[ShippingQuery] = None,
         pre_checkout_query: Optional[PreCheckoutQuery] = None,
@@ -6906,14 +6983,15 @@
         self.message = message
         self.edited_message = edited_message
         self.channel_post = channel_post
         self.edited_channel_post = edited_channel_post
         self.business_connection = business_connection
         self.business_message = business_message
         self.edited_business_message = edited_business_message
+        self.deleted_business_messages = deleted_business_messages
         self.message_reaction = message_reaction
         self.message_reaction_count = message_reaction_count
         self.inline_query = inline_query
         self.chosen_inline_result = chosen_inline_result
         self.callback_query = callback_query
         self.shipping_query = shipping_query
         self.pre_checkout_query = pre_checkout_query
```

### Comparing `aiotgm-0.3.2/aiotgm/update_manager.py` & `aiotgm-0.3.3/aiotgm/update_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 MESSAGE_MANAGER = 'message_manager'
 EDITED_MESSAGE_MANAGER = 'edited_message_manager'
 CHANNEL_POST_MANAGER = 'channel_post_manager'
 EDITED_CHANNEL_POST_MANAGER = 'edited_channel_post_manager'
 BUSINESS_CONNECTION_MANAGER = 'business_connection_manager'
 BUSINESS_MESSAGE_MANAGER = 'business_message_manager'
 EDITED_BUSINESS_MESSAGE_MANAGER = 'edited_business_message_manager'
+DELETED_BUSINESS_MESSAGES_MANAGER = 'deleted_business_messages_manager'
 MESSAGE_REACTION_MANAGER = 'message_reaction_manager'
 MESSAGE_REACTION_COUNT_MANAGER = 'message_reaction_count_manager'
 INLINE_QUERY_MANAGER = 'inline_query_manager'
 CHOSEN_INLINE_RESULT_MANAGER = 'chosen_inline_result_manager'
 CALLBACK_QUERY_MANAGER = 'callback_query_manager'
 SHIPPING_QUERY_MANAGER = 'shipping_query_manager'
 PRE_CHECKOUT_QUERY_MANAGER = 'pre_checkout_query_manager'
@@ -38,14 +39,15 @@
     MESSAGE_MANAGER : ("message", "lambda message: message.chat.id == xyz"),
     EDITED_MESSAGE_MANAGER : ("edited_message", "lambda edited_message: edited_message.chat.id == xyz"),
     CHANNEL_POST_MANAGER : ("channel_post", "lambda channel_post: channel_post.chat.id == xyz"),
     EDITED_CHANNEL_POST_MANAGER : ("edited_channel_post", "lambda edited_channel_post: edited_channel_post.chat.id == xyz"),
     BUSINESS_CONNECTION_MANAGER: ("business_connection", "lambda business_connection: business_connection.user.id == xyz"),
     BUSINESS_MESSAGE_MANAGER: ("business_message", "lambda business_message: business_message.chat.id == xyz"),
     EDITED_BUSINESS_MESSAGE_MANAGER: ("edited_business_message", "lambda edited_business_message: edited_business_message.chat.id == xyz"),
+    DELETED_BUSINESS_MESSAGES_MANAGER: ("deleted_business_messages", "lambda deleted_business_messages: deleted_business_messages.chat.id == xyz"),
     MESSAGE_REACTION_MANAGER: ("message_reaction", "lambda message_reaction: message_reaction.chat.id == xyz"),
     MESSAGE_REACTION_COUNT_MANAGER: ("message_reaction_count", "lambda message_reaction_count: message_reaction_count.chat.id == xyz"),
     INLINE_QUERY_MANAGER : ("inline_query", "lambda inline_query: inline_query.from_user.id == xyz"),
     CHOSEN_INLINE_RESULT_MANAGER : ("chosen_inline_result", "lambda chosen_inline_result: chosen_inline_result.from_user.id == xyz"),
     CALLBACK_QUERY_MANAGER : ("callback_query", "lambda callback_query: callback_query.from_user.id == xyz"),
     SHIPPING_QUERY_MANAGER : ("shipping_query", "lambda shipping_query: shipping_query.from_user.id == xyz"),
     PRE_CHECKOUT_QUERY_MANAGER : ("pre_checkout_query", "lambda pre_checkout_query: pre_checkout_query.from_user.id == xyz"),
```

### Comparing `aiotgm-0.3.2/aiotgm/utils.py` & `aiotgm-0.3.3/aiotgm/utils.py`

 * *Files identical despite different names*

### Comparing `aiotgm-0.3.2/aiotgm.egg-info/PKG-INFO` & `aiotgm-0.3.3/aiotgm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotgm
-Version: 0.3.2
+Version: 0.3.3
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `aiotgm-0.3.2/tests/test_func_ok.py` & `aiotgm-0.3.3/tests/test_func_ok.py`

 * *Files identical despite different names*

