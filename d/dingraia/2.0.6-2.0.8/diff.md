# Comparing `tmp/dingraia-2.0.6.tar.gz` & `tmp/dingraia-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingraia-2.0.6.tar", last modified: Mon Feb 26 14:35:07 2024, max compression
+gzip compressed data, was "dingraia-2.0.8.tar", last modified: Thu Apr  4 16:19:37 2024, max compression
```

## Comparing `dingraia-2.0.6.tar` & `dingraia-2.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-02-26 14:34:59.000000 dingraia-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-26 14:35:07.638211 dingraia-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-02-26 14:34:59.000000 dingraia-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.634211 dingraia-2.0.6/dingraia/
--rw-r--r--   0 runner    (1001) docker     (127)    79590 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/DingTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.634211 dingraia-2.0.6/dingraia/event/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/event/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/event/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.634211 dingraia-2.0.6/dingraia/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/message/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/message/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.634211 dingraia-2.0.6/dingraia/model/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/dingraia/saya/
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/dingraia/saya/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/builtins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/dingraia/saya/builtins/broadcast/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/builtins/broadcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/builtins/broadcast/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/saya/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/dingraia/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/tools/color_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/tools/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/tools/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-26 14:34:59.000000 dingraia-2.0.6/dingraia/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:35:07.638211 dingraia-2.0.6/dingraia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:35:07.000000 dingraia-2.0.6/dingraia.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:35:07.638211 dingraia-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-26 14:34:59.000000 dingraia-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-04 16:19:29.000000 dingraia-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 16:19:37.429083 dingraia-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-04 16:19:29.000000 dingraia-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.425083 dingraia-2.0.8/dingraia/
+-rw-r--r--   0 runner    (1001) docker     (127)    82954 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/DingTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/event/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/message/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/message/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/saya/
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/saya/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/builtins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/saya/builtins/broadcast/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/builtins/broadcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/builtins/broadcast/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/saya/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/tools/color_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/tools/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/tools/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 16:19:29.000000 dingraia-2.0.8/dingraia/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:19:37.429083 dingraia-2.0.8/dingraia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:19:37.000000 dingraia-2.0.8/dingraia.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:19:37.429083 dingraia-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-04 16:19:29.000000 dingraia-2.0.8/setup.py
```

### Comparing `dingraia-2.0.6/LICENSE` & `dingraia-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/README.md` & `dingraia-2.0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-此文档最后更新于24/1/14 v2.0.3
+此文档最后更新于24/4/5 v2.0.8
 
 # 这是什么？
 
 这个是一个关于能套用Graia-Ariadne部分项目的模块
 并运行的异步钉钉机器人代码，用来运行 基础 的Webhook类型
 的微型机器人，只实现了30%的功能，将来可能会完善。
 作者是Python废物，请不要催，你行你上。
@@ -78,28 +78,29 @@
 pip install --upgrade dingraia
 ```
 
 ## 接收函数
 
 ```python
 @channel.use(ListenerSchema(listening_events[GroupMessage]))  # 目前只支持GroupMessage
-async def example(group: Group):  # 此处暂不支持传入机器人实例
+async def example(app: Dingtalk, group: Group):
     ...
 ```
 
 当然，也可以这样
 
 ```python
 @channel.use(ListenerSchema(listening_events[GroupMessage]))
-def example(group: Group):  # 此处暂不支持传入机器人实例
+def example(app: Dingtalk, group: Group):
     ...
 ```
 
 它们都会并发执行
 ~~(你不会异步的话建议直接使用def，这样理论上效率会快一点)~~
+框架全部是异步法方法，虽然提供了函数来运行异步函数，但是还是建议使用异步函数
 
 ## 发送消息
 
 ```python
 await app.send_message(Target, MessageChain("Message"))  # 当然也可以传入任意对象，前提是支持str方法
 # 从 element 导入元素即可发送 MarkDown, ActionCard等支持的消息卡片
 # Target 可以是 Group, Member, OpenConversationId, Webhook, str(链接)
@@ -127,28 +128,35 @@
 
 注意：机器人的发送提示实际是在准备发送时提示的，不一定代表确实发送成功
 
 # 在同步函数中执行异步函数
 
 使用如下代码即可
 ```python
-from  dingraia.lazy import *
-@channel.use(...)
+from dingraia.lazy import *
+
+
+@channel.use(ListenerSchema(listening_events[GroupMessage]))
 def sync_example(app: Dingtalk):
     app.run_coroutine(app.mute_all(...)) # 使用的是app.loop执行的
 ```
 
 # 兼容度
 
-30%...
+20%...
 （简单的模块只需要替换import的模块和app）
 
 # TODO
 
 让我想想...
 
+# 衍生项目
+
+[DingtalkStreamPushForward](https://github.com/MeiHuaGuangShuo/DingtalkStreamPushForward) - 
+通过Stream模式转发钉钉服务器的消息到WebSocket和Webhook，支持本项目的连接
+
 # 最后要说
 
 本项目基于[Graia](https://github.com/GraiaProject/Ariadne)QQ机器人框架模仿开发，
 有兴趣的话去点个star吧
```

### Comparing `dingraia-2.0.6/dingraia/DingTalk.py` & `dingraia-2.0.8/dingraia/DingTalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Dict, Coroutine, Literal
 
 import aiohttp
 import websockets
 from aiohttp import ClientSession, ClientResponse
 from .VERSION import VERSION
 from .callback_handler import callback_handler
-from .config import Config, Stream
+from .config import Config, Stream, CustomStreamConnect
 from .element import *
 from .event import MessageEvent
 from .event.event import *
 from .event.message import *
 from .exceptions import *
 from .message.chain import MessageChain
 from .message.element import *
@@ -70,21 +70,22 @@
     config: Config = None
     _loop: asyncio.AbstractEventLoop = None
     _access_token: AccessToken = None
     api_request: "Dingtalk._api_request" = None
     oapi_request: "Dingtalk._oapi_request" = None
     async_tasks = []
     stream_checker = {}
-    stream_connect = None
     """用于检测重复的回调, 键为任务名, 值为容纳50个StreamID的列表"""
+    stream_connect: CustomStreamConnect = None
     
     def __init__(self, config: Config = None):
         if Dingtalk.config is None:
             Dingtalk.config = config
             cache.enable = config.useDatabase
+            self.stream_connect = config.customStreamConnect
     
     async def send_message(self, target: Union[Group, Member, OpenConversationId, str, Webhook, None], msg,
                            headers=None):
         """发送普通的文本信息
         
         Args:
             target: 要发送的地址，可以是Group, OpenConversationId, str格式的链接, 或者None发送到测试群
@@ -107,21 +108,21 @@
         if isinstance(msg, BaseElement):
             if not isinstance(target, OpenConversationId) and not isinstance(target, Member):
                 send_data = msg.data
             else:
                 send_data = msg.template
         elif isinstance(msg, File):
             if not msg.mediaId:
-                res = await self.upload_file(msg)
-                send_data = msg.template
-                send_data['media_id'] = res.mediaId
-            else:
-                send_data['media_id'] = msg.mediaId
+                msg = await self.upload_file(msg)
+            send_data = msg.template
+            send_data['media_id'] = msg.mediaId
             if isinstance(target, Group):
                 target = target.openConversationId
+            send_data['robotCode'] = self.config.bot.robotCode
+            send_data['openConversationId'] = str(target)
         else:
             if isinstance(target, OpenConversationId) or isinstance(target, Member):
                 send_data = {
                     'msgKey'  : "sampleText",
                     'msgParam': json.dumps({
                         'content': str(msg)
                     })
@@ -174,15 +175,15 @@
         elif isinstance(target, OpenConversationId):
             url = 'https://api.dingtalk.com/v1.0/robot/groupMessages/send'
             response.recallType = "group"
             response.recallOpenConversationId = target
             self.log.info(f"[SEND][{target.name}({int(target)})] <- {repr(str(msg))[1:-1]}")
         else:
             url = str(target)
-            self.log.info(f"[SEND] <- {repr(str(msg))[1:-1]}")
+            self.log.info(f"[SEND][WebHook] <- {repr(str(msg))[1:-1]}")
         delog.info(send_data, no=60)
         if url and "http" not in url:
             logger.error(f"Wrong send url [{url}]!")
             response.ok = False
             response.text = ""
             response.url = url
             response.recall_type = "Not completed request"
@@ -235,64 +236,60 @@
     async def recall_message(
             self,
             message: Response = None,
             *,
             openConversationId: Union[OpenConversationId, Group, str] = None,
             processQueryKeys: Union[str, List[str]] = None,
             robotCode: str = None,
-            access_token: str = None,
             inThreadTime: int = 0
     ):
         """撤回一条消息
         
         Args:
             message: 通过send_message发送消息返回的对象
             openConversationId: 群对话ID, 可以是OpenConversationId或Group对象
             processQueryKeys: 消息的加密ID
             robotCode: 机器人的机器码
-            access_token: 企业的AccessToken
             inThreadTime: 是否不等待撤回
 
         Returns:
             text
 
         """
+        if message:
+            processQueryKeys = message.json()['processQueryKey']
+            openConversationId = message.recallOpenConversationId
+        processQueryKeys = [str(x) for x in
+                            (processQueryKeys if isinstance(processQueryKeys, list) else [processQueryKeys])]
+        if isinstance(openConversationId, Group):
+            openConversationId = openConversationId.openConversationId
+        if openConversationId is not None:
+            openConversationId = str(openConversationId)
+        if robotCode is None:
+            robotCode = self.config.bot.robotCode
+        post_data = {
+            "processQueryKeys": processQueryKeys,
+            "robotCode"       : robotCode
+        }
+        url = "/v1.0/robot/otoMessages/batchRecall"
+        if openConversationId:
+            url = "/v1.0/robot/groupMessages/recall"
+            post_data['openConversationId'] = openConversationId
         
-        async def _run(_message, _openConversationId, _processQueryKeys, _robotCode, _access_token, _inThreadTime):
-            _access_token = _access_token or self.access_token
-            if message:
-                _processQueryKeys = message.json['processQueryKey']
-                _openConversationId = message.recallOpenConversationId
-            _processQueryKeys = [str(x) for x in
-                                 (_processQueryKeys if isinstance(_processQueryKeys, list) else [_processQueryKeys])]
-            if isinstance(openConversationId, Group):
-                _openConversationId = _openConversationId.conversationId
-            if _openConversationId is not None:
-                _openConversationId = str(_openConversationId)
-            if _robotCode is None:
-                _robotCode = self.config.bot.robotCode
-            post_data = {
-                "processQueryKeys": _processQueryKeys,
-                "robotCode"       : _robotCode
-            }
-            url = "/v1.0/robot/otoMessages/batchRecall"
-            if _openConversationId:
-                url = "/v1.0/robot/groupMessages/recall"
-                post_data['openConversationId'] = _openConversationId
+        async def _run(_inThreadTime):
             await asyncio.sleep(_inThreadTime)
             res = await self.api_request.post(url, json=post_data)
             return await res.json()
         
         if message.recallType not in ['group', 'personal']:
             raise UnsupportedRecallType(f"The recall type '{message.recallType}' is not supported for recall")
         if not inThreadTime:
-            return await _run(message, openConversationId, processQueryKeys, robotCode, access_token, inThreadTime)
+            return await _run(inThreadTime)
         else:
-            return self.loop.create_task(
-                _run(message, openConversationId, processQueryKeys, robotCode, access_token, inThreadTime))
+            return self.loop.create_task(_run(inThreadTime))
     
     async def _send_card(
             self,
             cardTemplateId,
             outTrackId,
             cardData,
             openSpaceId,
@@ -367,15 +364,16 @@
             if isinstance(target, Group):
                 target = target.openConversationId
             openConversationId = str(target)
             body['openSpaceId'] = f"dtv1.card//IM_GROUP.{openConversationId}"
             body["imGroupOpenDeliverModel"] = {"robotCode": self.config.bot.appKey}
         resp = await self.api_request.post('/v1.0/card/instances/deliver', json=body)
         if not resp.ok:
-            raise DingtalkAPIError(f"Error while deliver the card.Code={resp.status} text={await resp.text()}")
+            errCode = (await resp.json()).get("errcode")
+            raise err_reason[errCode](f"Error while deliver the card.Code={resp.status} text={await resp.text()}")
         return outTrackId
     
     async def send_markdown_card(
             self,
             target: Union[OpenConversationId, Group, Member],
             markdown: Markdown,
             logo: Union[File, str] = "@lALPDfJ6V_FPDmvNAfTNAfQ",
@@ -452,16 +450,14 @@
                            ):
         userIds = userIds or [ownerUserId]
         userIds = [str(x) for x in userIds]
         userIds = ",".join(userIds)
         subAdminIds = subAdminIds or [ownerUserId]
         subAdminIds = [str(x) for x in subAdminIds]
         subAdminIds = ",".join(subAdminIds)
-        access_token = access_token or self.access_token
-        url = f"https://oapi.dingtalk.com/topapi/im/chat/scenegroup/create?access_token={access_token}"
         data = {
             "title"                          : name,
             "template_id"                    : templateId,
             "owner_user_id"                  : ownerUserId,
             "user_ids"                       : userIds,
             "subadmin_ids"                   : subAdminIds,
             "uuid"                           : UUID,
@@ -477,17 +473,19 @@
             "all_members_can_create_calendar": 0,
             "group_email_disabled"           : 0,
             "only_admin_can_set_msg_top"     : 1,
             "add_friend_forbidden"           : 0,
             "group_live_switch"              : 1,
             "members_to_admin_chat"          : 0
         }
-        res = await url_res(url,
-                            'POST',
-                            json=data, res='json')
+        if access_token:
+            url = f"https://oapi.dingtalk.com/topapi/im/chat/scenegroup/create?access_token={access_token}"
+            res = await url_res(url, 'POST', json=data, res='json')
+        else:
+            res = await self.oapi_request.jpost("/topapi/im/chat/scenegroup/create", json=data)
         if not res['success']:
             logger.error(f"Cannot create the group!Response: {json.dumps(res, ensure_ascii=False, indent=4)}")
         return res
     
     async def get_group(self, openConversationId: Union[OpenConversationId, Group, str], access_token: str = None):
         """获取场景群信息, `2` API 调用量
         
@@ -500,33 +498,31 @@
         """
         openConversationId = self._openConversationId2str(openConversationId)
         if access_token:
             res = await url_res(f'https://oapi.dingtalk.com/topapi/im/chat/scenegroup/get?access_token={access_token}',
                                 'POST',
                                 json={'open_conversation_id': openConversationId}, res='json')
         else:
-            resp = await self.oapi_request.post("/topapi/im/chat/scenegroup/get",
+            res = await self.oapi_request.jpost("/topapi/im/chat/scenegroup/get",
                                                 json={'open_conversation_id': openConversationId})
-            res = await resp.json()
         if res['errcode']:
             if res['errcode'] == 4000003:
                 logger.error(f"OpenConversationId 对应的群不是由群模板创建的或没有酷应用支持！")
             res['success'] = False
             return res
         if access_token:
             users_res = await url_res(
                 f'https://oapi.dingtalk.com/topapi/im/chat/scenegroup/member/get?access_token={access_token}',
                 'POST',
                 json={'openConversationId': openConversationId, "maxResults": 1000},
                 res='json')
         else:
-            resp = await self.oapi_request.post('/topapi/im/chat/scenegroup/member/get',
+            users_res = await self.oapi_request.jpost('/topapi/im/chat/scenegroup/member/get',
                                                 json={'open_conversation_id': openConversationId, "size": 1000,
                                                       "cursor"              : 0})
-            users_res = await resp.json()
             users_res = users_res.get('result', {})
         res: dict = res['result']
         res['user_ids'] = users_res.get('member_user_ids')
         res['staff_id_nick_map'] = users_res.get('staff_id_nick_map')
         res['success'] = True
         return res
     
@@ -541,52 +537,56 @@
 
         """
         access_token = access_token or self.access_token
         if access_token:
             url = f"https://oapi.dingtalk.com/topapi/v2/department/listsub?access_token={access_token}"
             res = await url_res(url, 'POST', json={'dept_id': deptId}, res='json')
         else:
-            resp = await self.oapi_request.post('/topapi/v2/department/listsub', json={'dept_id': deptId})
-            res = await resp.json()
+            res = await self.oapi_request.jpost('/topapi/v2/department/listsub', json={'dept_id': deptId})
         return res
     
     async def get_user(self, userStaffId: Union[Member, str], language: str = "zh_CN", access_token: str = None):
         """获取用户详细信息
         
         Args:
             userStaffId: 用户的StaffID
             language: 语言. 默认zh-CN
 
         Returns:
 
         """
         userStaffId = self._staffId2str(userStaffId)
-        access_token = access_token or self.access_token
-        res = await url_res(
-            f'https://oapi.dingtalk.com/topapi/v2/user/get?access_token={access_token}',
-            'POST',
-            json={"language": language, "userid": userStaffId}, res='json')
+        if access_token:
+            res = await url_res(
+                f'https://oapi.dingtalk.com/topapi/v2/user/get?access_token={access_token}',
+                'POST',
+                json={"language": language, "userid": userStaffId}, res='json')
+        else:
+            res = await self.oapi_request.jpost("/topapi/v2/user/get",
+                                                json={"language": language, "userid": userStaffId})
         return res
     
     async def remove_user(self, userStaffId: Union[Member, str], access_token: str = None):
         """从组织中直接移除用户
         
         Args:
             userStaffId: 用户的StaffID
             access_token: 组织的AccessToken
 
         Returns:
 
         """
         userStaffId = self._staffId2str(userStaffId)
-        access_token = access_token or self.access_token
-        res = await url_res(
-            f'https://oapi.dingtalk.com/topapi/v2/user/delete?access_token={access_token}',
-            'POST',
-            json={"userid": userStaffId}, res='json')
+        if access_token:
+            res = await url_res(
+                f'https://oapi.dingtalk.com/topapi/v2/user/delete?access_token={access_token}',
+                'POST',
+                json={"userid": userStaffId}, res='json')
+        else:
+            res = await self.oapi_request.jpost("/topapi/v2/user/delete", json={"userid": userStaffId})
         return res
     
     async def create_user(
             self,
             name: str,
             mobilePhone: Union[str, int],
             deptIds: Union[str, List[str]],
@@ -656,16 +656,15 @@
             data['extension'] = extension
         if isSenior:
             data['senior_mode'] = isSenior
         if managerUserId:
             data['manager_userid'] = managerUserId
         if loginEmail:
             data['login_email'] = loginEmail
-        resp = await self.oapi_request.post('/topapi/v2/user/create', json=data)
-        res = await resp.json()
+        res = await self.oapi_request.jpost('/topapi/v2/user/create', json=data)
         return res
     
     async def update_user(
             self,
             userId,
             name: str = None,
             hide_mobile: bool = None,
@@ -721,16 +720,15 @@
             data['senior_mode'] = senior_mode
         if hired_date:
             data['hired_date'] = int(hired_date)
         if language:
             data['language'] = language
         if force_update_fields:
             data['force_update_fields'] = ",".join([str(x) for x in force_update_fields])
-        resp = await self.oapi_request.post('/topapi/v2/user/update', json=data)
-        res = await resp.json()
+        res = await self.oapi_request.jpost('/topapi/v2/user/update', json=data)
         return res
     
     async def mirror_group(self, openConversationId: Union[OpenConversationId, Group, str]):
         """复制群信息和群成员到一个新群. 群必须是场景群
         
         Args:
             openConversationId: 群对话ID, 可以是OpenConversationId或Group对象
@@ -867,17 +865,16 @@
             data['plugin_customize_verify'] = 1 if plugin_customize_verify else 0
         if access_token:
             res = await url_res(
                 f'https://oapi.dingtalk.com/topapi/im/chat/scenegroup/update?access_token={access_token}',
                 'POST',
                 json=data, res='json')
         else:
-            resp = await self.oapi_request.post("/topapi/im/chat/scenegroup/update",
+            res = await self.oapi_request.jpost("/topapi/im/chat/scenegroup/update",
                                                 json=data)
-            res = await resp.json()
         return res
     
     async def change_group_title(self, openConversationId: Union[OpenConversationId, Group, str], title: str):
         """
         
         Args:
             openConversationId:
@@ -916,18 +913,17 @@
 
         Returns:
 
         """
         openConversationId = self._openConversationId2str(openConversationId)
         memberStaffIds = self._staffId2list(memberStaffIds)
         memberStaffIds = ','.join(memberStaffIds)
-        resp = await self.oapi_request.post('/topapi/im/chat/scenegroup/member/delete',
+        res = await self.oapi_request.jpost('/topapi/im/chat/scenegroup/member/delete',
                                             json={"open_conversation_id": openConversationId,
                                                   "user_ids"            : memberStaffIds})
-        res = await resp.json()
         return res
     
     async def add_member(self, openConversationId: Union[OpenConversationId, Group, str],
                          memberStaffIds: Union[Member, str, List[Union[Member, str]]]):
         """添加一个成员到群组. 群组必须是场景群
         
         Args:
@@ -936,18 +932,17 @@
 
         Returns:
 
         """
         openConversationId = self._openConversationId2str(openConversationId)
         memberStaffIds = self._staffId2list(memberStaffIds)
         memberStaffIds = ','.join(memberStaffIds)
-        resp = await self.oapi_request.post('/topapi/im/chat/scenegroup/member/add',
+        res = await self.oapi_request.jpost('/topapi/im/chat/scenegroup/member/add',
                                             json={"open_conversation_id": openConversationId,
                                                   "user_ids"            : memberStaffIds})
-        res = await resp.json()
         return res
     
     async def set_admin(self, openConversationId: Union[OpenConversationId, Group, str],
                         memberStaffIds: Union[Member, str, List[Union[Member, str]]], set_admin: bool = True):
         """设置一个成员是否为管理员. 群组必须是场景群
         
         Args:
@@ -956,18 +951,17 @@
             set_admin: 是否设置为群组管理员
 
         Returns:
 
         """
         openConversationId = self._openConversationId2str(openConversationId)
         memberStaffIds = self._staffId2list(memberStaffIds)
-        resp = await self.api_request.put('/v1.0/im/sceneGroups/subAdmins',
+        res = await self.api_request.jput('/v1.0/im/sceneGroups/subAdmins',
                                           json={"openConversationId": openConversationId, "userIds": memberStaffIds,
                                                 'role'              : 2 if set_admin else 3})
-        res = await resp.json()
         return res
     
     async def mute_member(
             self,
             openConversationId: Union[OpenConversationId, Group, str],
             memberStaffIds: Union[Member, str, List[Union[Member, str]]],
             muteTime: int = 0
@@ -978,26 +972,24 @@
             openConversationId: 群对话ID, 可以是OpenConversationId或Group对象
             memberStaffIds: 成员的StaffID
             muteTime: 禁言时长, 单位为秒, 值为0则解除禁言
 
         Returns:
 
         """
-        url = f"https://api.dingtalk.com/v1.0/im/sceneGroups/muteMembers/set"
         memberStaffIds = [str(x) for x in (memberStaffIds if isinstance(memberStaffIds, list) else [memberStaffIds])]
         openConversationId = self._openConversationId2str(openConversationId)
         memberStaffIds = self._staffId2list(memberStaffIds)
-        resp = await self.api_request.post('/v1.0/im/sceneGroups/muteMembers/set',
+        res = await self.api_request.jpost('/v1.0/im/sceneGroups/muteMembers/set',
                                            json={
                                                "openConversationId": openConversationId,
                                                "userIdList"        : memberStaffIds,
                                                "muteStatus"        : 1 if muteTime else 0,
                                                "muteDuration"      : muteTime * 1000
                                            })
-        res = await resp.json()
         return res
     
     async def unmute_member(
             self,
             openConversationId: Union[OpenConversationId, Group, str],
             memberStaffIds: Union[Member, str, List[Union[Member, str]]]
     ):
@@ -1040,19 +1032,22 @@
         }
         data = {
             "robotCode"     : robotCode or self.config.bot.robotCode,
             "cardData"      : json.dumps(card_data),
             "cardTemplateId": "StandardCard"
         }
         logger.debug(data)
-        res = await url_res(
-            url, "POST",
-            headers={'x-acs-dingtalk-access-token': access_token},
-            json=data
-        )
+        if access_token:
+            res = await url_res(
+                url, "POST",
+                headers={'x-acs-dingtalk-access-token': access_token},
+                json=data
+            )
+        else:
+            res = await self.api_request.jpost(url, json=data)
         return res
     
     @staticmethod
     class log:
         def info(*mes):
             logger.info(*mes)
         
@@ -1117,16 +1112,21 @@
             if size > 20 * MiB:
                 raise UploadFileSizeError("Normal file is limited under 20M, but %sM given!" % (size / (1024 ** 2)))
         if not access_token:
             access_token = self.access_token
         async with aiohttp.ClientSession() as session:
             async with session.post(f'https://oapi.dingtalk.com/media/upload?access_token={access_token}',
                                     data={'type': file_type, 'media': f}) as resp:
-                resp = await resp.json()
-        res.mediaId = resp['media_id']
+                res_json = await resp.json()
+                if res_json.get("errcode"):
+                    raise err_reason[res_json.get("errcode")](
+                        f"Error while uploading the file.Server response: {res_json}")
+                cache.add_openapi_count()
+        
+        res.mediaId = res_json['media_id']
         return res
     
     async def download_file(self, downloadCode: Union[File, str], path: Union[Path, str]):
         """下载机器人接收的文件, 1 API 消耗量
         文档: https://open.dingtalk.com/document/isvapp/download-the-file-content-of-the-robot-receiving-message
         
         Args:
@@ -1345,14 +1345,18 @@
         sign_str = timestamp + '\n' + secure_key
         sign = hmac.new(secure_key.encode("utf-8"), sign_str.encode("utf-8"), hashlib.sha256).digest()
         sign = base64.b64encode(sign)
         sign = urllib.parse.quote_plus(sign)
         return sign, timestamp, secure_key
     
     @staticmethod
+    def get_api_counts():
+        return cache.get_api_counts()
+    
+    @staticmethod
     async def _send(url, send_data, headers=None):
         delog.info(f"发送中:{url}", no=40)
         if url and "http" not in url:
             url = 'http://' + url
         if not url:
             logger.error("Empty send url!")
             return [False]
@@ -1383,40 +1387,56 @@
         
         def __init__(self, clientSession: ClientSession, access_token: Union[AccessToken, str]):
             self.clientSession = clientSession
             self.access_token = access_token
         
         async def get(self, urlPath, *, headers=None, **kwargs) -> ClientResponse:
             headers = self._header_resolve(headers)
-            self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
             resp = await self.clientSession.get(self._url_resolve(urlPath), headers=headers, **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def post(self, urlPath, *, headers=None, **kwargs) -> ClientResponse:
             headers = self._header_resolve(headers)
-            self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
             resp = await self.clientSession.post(self._url_resolve(urlPath), headers=headers, **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def put(self, urlPath, *, headers=None, **kwargs) -> ClientResponse:
             headers = self._header_resolve(headers)
-            self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
             resp = await self.clientSession.put(self._url_resolve(urlPath), headers=headers, **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def delete(self, urlPath, *, headers=None, **kwargs) -> ClientResponse:
             headers = self._header_resolve(headers)
-            self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, headers=headers, kwargs=kwargs)
             resp = await self.clientSession.delete(self._url_resolve(urlPath), headers=headers, **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
+        async def jget(self, urlPath, *, headers=None, **kwargs) -> dict:
+            resp = await self.get(urlPath=urlPath, headers=headers, **kwargs)
+            return await resp.json()
+        
+        async def jpost(self, urlPath, *, headers=None, **kwargs) -> dict:
+            resp = await self.post(urlPath=urlPath, headers=headers, **kwargs)
+            return await resp.json()
+        
+        async def jput(self, urlPath, *, headers=None, **kwargs) -> dict:
+            resp = await self.put(urlPath=urlPath, headers=headers, **kwargs)
+            return await resp.json()
+        
+        async def jdelete(self, urlPath, *, headers=None, **kwargs) -> dict:
+            resp = await self.delete(urlPath=urlPath, headers=headers, **kwargs)
+            return await resp.json()
+        
         @staticmethod
         def _url_resolve(urlPath: str) -> str:
             if "http" not in urlPath and not urlPath.startswith('/'):
                 urlPath = '/' + urlPath
             url = ("https://api.dingtalk.com" + urlPath) if "https" not in urlPath else urlPath
             return url
         
@@ -1424,80 +1444,116 @@
             if headers is None:
                 headers = {}
             if "x-acs-dingtalk-access-token" not in headers:
                 headers["x-acs-dingtalk-access-token"] = self.access_token.safe()
             return headers
 
         @staticmethod
-        def before_request(urlPath: str, headers=None, **kwargs):
-            ...
+        async def before_request(urlPath: str, headers=None, **kwargs):
+            try:
+                ...
+            except Exception as e:
+                logger.exception(f"在处理 {urlPath} 的请求时发生异常。请求头: {headers}请求参数: {kwargs}", e)
 
         @staticmethod
-        def after_request(response: ClientResponse):
-            if response.ok:
-                is_exist = cache.execute(f"SELECT * FROM `counts` WHERE type='openApi'", result=True)
-                if is_exist:
-                    cache.execute(f"UPDATE `counts` SET count=count+1 WHERE type='openApi';")
-                else:
-                    cache.execute(f"INSERT INTO `counts` (type, count) VALUES ('openApi', 1);")
-                cache.commit()
+        async def after_request(response: ClientResponse):
+            try:
+                if response.ok:
+                    try:
+                        resp = await response.json()
+                        if resp.get("errcode"):
+                            return
+                    except json.JSONDecodeError:
+                        pass
+                    except Exception as e:
+                        logger.exception(e)
+                        logger.warning("此次请求会继续提交到次数")
+                    cache.add_openapi_count()
+            except Exception as e:
+                logger.exception(f"在处理 {response.url} 的返回时发生异常。返回体: {await response.text()}", e)
     
     class _oapi_request:
         
         def __init__(self, clientSession: ClientSession, access_token: Union[AccessToken, str]):
             self.clientSession = clientSession
             self.access_token = access_token
         
         async def get(self, urlPath: str, **kwargs) -> ClientResponse:
-            self.before_request(urlPath=urlPath, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, kwargs=kwargs)
             resp = await self.clientSession.get(self._url_resolve(urlPath), **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def post(self, urlPath, **kwargs) -> ClientResponse:
-            self.before_request(urlPath=urlPath, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, kwargs=kwargs)
             resp = await self.clientSession.post(self._url_resolve(urlPath), **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def put(self, urlPath, **kwargs) -> ClientResponse:
-            self.before_request(urlPath=urlPath, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, kwargs=kwargs)
             resp = await self.clientSession.put(self._url_resolve(urlPath), **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
         async def delete(self, urlPath, **kwargs) -> ClientResponse:
-            self.before_request(urlPath=urlPath, kwargs=kwargs)
+            await self.before_request(urlPath=urlPath, kwargs=kwargs)
             resp = await self.clientSession.delete(self._url_resolve(urlPath), **kwargs)
-            self.after_request(resp)
+            await self.after_request(resp)
             return resp
         
+        async def jget(self, urlPath, **kwargs) -> dict:
+            resp = await self.get(urlPath=urlPath, **kwargs)
+            return await resp.json()
+        
+        async def jpost(self, urlPath, **kwargs) -> dict:
+            resp = await self.post(urlPath=urlPath, **kwargs)
+            return await resp.json()
+        
+        async def jput(self, urlPath, **kwargs) -> dict:
+            resp = await self.put(urlPath=urlPath, **kwargs)
+            return await resp.json()
+        
+        async def jdelete(self, urlPath, **kwargs) -> dict:
+            resp = await self.delete(urlPath=urlPath, **kwargs)
+            return await resp.json()
+        
         def _url_resolve(self, urlPath: str):
             if "http" not in urlPath and not urlPath.startswith('/'):
                 urlPath = '/' + urlPath
             url = ("https://oapi.dingtalk.com" + urlPath) if "https" not in urlPath else urlPath
             if '?' not in url:
                 url += f"?access_token={self.access_token.safe()}"
             elif '?' in url and 'access_token' not in url:
                 url += f"&access_token={self.access_token.safe()}"
             return url
 
         @staticmethod
-        def before_request(urlPath: str, **kwargs):
-            ...
+        async def before_request(urlPath: str, **kwargs):
+            try:
+                ...
+            except Exception as e:
+                logger.exception(f"在处理 {urlPath} 的请求时发生异常。请求参数: {kwargs}", e)
 
         @staticmethod
-        def after_request(response: ClientResponse):
-            if response.ok:
-                is_exist = cache.execute(f"SELECT * FROM `counts` WHERE type='openApi'", result=True)
-                if is_exist:
-                    cache.execute(f"UPDATE `counts` SET count=count+1 WHERE type='openApi';")
-                else:
-                    cache.execute(f"INSERT INTO `counts` (type, count) VALUES ('openApi', 1);")
-                cache.commit()
+        async def after_request(response: ClientResponse):
+            try:
+                if response.ok:
+                    try:
+                        resp = await response.json()
+                        if resp.get("errcode"):
+                            return
+                    except json.JSONDecodeError:
+                        pass
+                    except Exception as e:
+                        logger.exception(e)
+                        logger.warning("此次请求会继续提交到次数")
+                    cache.add_openapi_count()
+            except Exception as e:
+                logger.exception(f"在处理 {response.url} 的返回时发生异常。返回体: {await response.text()}", e)
     
     def start(self, flask_app: "flask.Flask" = None, **kwargs):
         """
         
         Args:
             flask_app: 你的 Flask app 对象
             **kwargs: 传递给 Flask 的参数
@@ -1598,24 +1654,25 @@
 
         Returns:
             None
 
         """
         
         def get_host_ip():
-            ip = ""
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             try:
-                s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
                 s.connect(('8.8.8.8', 80))
                 ip = s.getsockname()[0]
+            except:
+                ip = '127.0.0.1'
             finally:
                 s.close()
-                return ip
+            return ip
         
-        async def open_connection(task_name: str):
+        async def open_connection(task_name: str, url: str = self.WS_CONNECT_URL):
             logger.info(f'[{task_name}] Requesting stream')
             request_headers = {
                 'User-Agent': f'Dingraia/{VERSION} (+https://github.com/MeiHuaGuangShuo/Dingraia)'
             }
             request_body = {
                 'clientId'     : stream.AppKey,
                 'clientSecret' : stream.AppSecret,
@@ -1624,15 +1681,15 @@
                     {'type': 'CALLBACK', 'topic': '/v1.0/im/bot/messages/get'},
                     {'type': 'CALLBACK', 'topic': '/v1.0/im/bot/messages/delegate'},
                     {'type': 'CALLBACK', 'topic': '/v1.0/card/instances/callback'},
                 ],
                 'ua'           : f'Dingraia/{VERSION}',
                 'localIp'      : get_host_ip()
             }
-            response = requests.post(self.WS_CONNECT_URL,
+            response = requests.post(url,
                                      headers=request_headers,
                                      json=request_body)
             try:
                 http_body = response.json()
             except Exception as err:
                 logger.error(f"{err.__class__.__name__}: {err} Body: {response.text}")
                 await asyncio.sleep(5)
@@ -1696,26 +1753,32 @@
                         'message': 'OK',
                         'data'   : json_message.get('data', ""),
                     }))
             except Exception as err:
                 logger.exception(f"[{task_name}] Error happened while handing the message", err)
             return result
         
-        async def main_stream(task_name: str, dingtalk: "Dingtalk"):
+        async def main_stream(task_name: str):
             while ...:
-                if not dingtalk.stream_connect:
+                if not self.stream_connect:
                     connection = await open_connection(task_name)
                 else:
-                    key = dingtalk.config.bot.appKey
-                    secret = dingtalk.config.bot.appSecret
-                    if dingtalk.stream_connect[1]:
-                        if inspect.iscoroutinefunction(dingtalk.stream_connect[1]):
-                            connection = await dingtalk.stream_connect[1](key, secret)
+                    key = self.config.bot.appKey
+                    secret = self.config.bot.appSecret
+                    if self.stream_connect.SignHandler:
+                        if inspect.iscoroutinefunction(self.stream_connect.SignHandler):
+                            connection = await self.stream_connect.SignHandler(key, secret)
+                        elif inspect.isfunction(self.stream_connect.SignHandler):
+                            connection = self.stream_connect.SignHandler(key, secret)
+                        elif isinstance(self.stream_connect.SignHandler, str):
+                            if "http" not in self.stream_connect.SignHandler:
+                                raise ValueError(f"Incorrect signer url, consider use None to skip sign")
+                            connection = await open_connection(task_name, self.stream_connect.SignHandler)
                         else:
-                            connection = dingtalk.stream_connect[1](key, secret)
+                            raise ValueError(f"Incorrect signer param, consider use None to skip sign")
                     else:
                         connection = {"endpoint": "Pass", "ticket": "Pass"}
                 
                 if not connection:
                     if connection is None:
                         logger.error(f'[{task_name}] Open websocket connection failed')
                         logger.warning(f"[{task_name}] Websocket Connection will be reconnected after 5 seconds")
@@ -1723,19 +1786,25 @@
                         logger.warning(f"[{task_name}] Reconnecting...")
                         continue
                     if not connection:
                         logger.error(f'[{task_name}] Request connection failed!')
                     return
                 uri = '%s?ticket=%s' % (connection['endpoint'], urllib.parse.quote_plus(connection['ticket']))
                 headers = {'User-Agent': f'Dingraia/{VERSION} (+https://github.com/MeiHuaGuangShuo/Dingraia)'}
-                if dingtalk.stream_connect:
-                    if dingtalk.stream_connect[0]:
-                        uri = dingtalk.stream_connect[0]
-                    if len(dingtalk.stream_connect) > 2 and dingtalk.stream_connect[2]:
-                        headers = dingtalk.stream_connect[2]
+                if self.stream_connect:
+                    if self.stream_connect.StreamUrl:
+                        uri = self.stream_connect.StreamUrl
+                    if self.stream_connect.ExtraHeaders:
+                        headers = self.stream_connect.ExtraHeaders
+                if connection:
+                    if "?" not in uri:
+                        uri = f"{uri}?ticket={urllib.parse.quote_plus(connection['ticket'])}"
+                    else:
+                        if "ticket" not in uri:
+                            uri = f"{uri}&ticket={urllib.parse.quote_plus(connection['ticket'])}"
                 try:
                     async with websockets.connect(uri, extra_headers=headers) as websocket:
                         logger.success(f"[{task_name}] Websocket connected")
                         try:
                             async for raw_message in websocket:
                                 json_message = json.loads(raw_message)
                                 route_result = await route_message(json_message, websocket, task_name)
@@ -1756,17 +1825,17 @@
             
             logger.info(f"[{task_name}] Stream connection was stopped.")
         
         try:
             no = next(_no)
             name = f"#{no} Main Stream"
             if not is_debug:
-                self.async_tasks.append(self.loop.create_task(main_stream(name, self), name=name))
+                self.async_tasks.append(self.loop.create_task(main_stream(name), name=name))
             else:
-                self.create_task(self.coroutine_watcher(main_stream, name, self))
+                self.create_task(self.coroutine_watcher(main_stream, name))
             logger.info(f"Create Stream Task - {name}")
             # 为了使用序号所以不会使用内置的create_task
         except asyncio.exceptions.CancelledError:
             logger.warning("Program forced to be exit!")
     
     def create_task(self, coroutine: Coroutine, name: str = "Task", show_info=True):
         """创建一个异步任务, 此任务会在stop函数被调用时取消
@@ -1837,17 +1906,15 @@
                         stop = True
                         break
     
     @staticmethod
     def _openConversationId2str(openConversationId: Union[OpenConversationId, Group, str]) -> str:
         if isinstance(openConversationId, Group):
             openConversationId = openConversationId.openConversationId
-        else:
-            openConversationId = str(openConversationId)
-        return openConversationId
+        return str(openConversationId)
     
     @staticmethod
     def _staffId2str(staffId: Union[Member, str]) -> str:
         if isinstance(staffId, Member):
             staffId = staffId.staffid
         staffId = str(staffId)
         return staffId
```

### Comparing `dingraia-2.0.6/dingraia/__main__.py` & `dingraia-2.0.8/dingraia/__main__.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/cache.py` & `dingraia-2.0.8/dingraia/cache.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import sqlite3
+from .exceptions import *
 
 
 class Cache:
     db: sqlite3.Connection = None
     cursor: sqlite3.Cursor = None
     enable: bool = True
 
     def __init__(self):
         pass
 
     def connect(self, databaseName: str = "Dingraia_cache.db", **kwargs):
         self.db = sqlite3.connect(databaseName, **kwargs)
         self.cursor = self.db.cursor()
+        self.init_tables()
         
     def change_database(self, databaseName):
         self.close()
         self.enable = True
         self.connect(databaseName=databaseName)
         
     def execute(self, command, result=False):
@@ -89,20 +91,42 @@
                 "count": int
             }
         }
         tables = self.get_tables()
         for t, v in to_tables.items():
             if t not in tables:
                 self.create_table(t, v)
+    
+    def key_exists(self, table, column, name) -> bool:
+        return bool(self.execute(f"SELECT * FROM `{table}` WHERE {column}='{name}'", result=True))
+    
+    def add_value(self, table, column, name, index, add: int = 1):
+        if self.key_exists(table, column, name):
+            self.execute(f"UPDATE `{table}` SET {name}={name}+{add} WHERE {index}='openApi';")
+            self.commit()
+        else:
+            raise SQLError(f"Index '{index}' does not found in the table '{table}'")
+    
+    def add_openapi_count(self, times: int = 1):
+        if self.key_exists('counts', 'type', 'openApi'):
+            self.execute(f"UPDATE `counts` SET count=count+{times} WHERE type='openApi';")
+        else:
+            self.execute(f"INSERT INTO `counts` (type, count) VALUES ('openApi', {times});")
+        self.commit()
+    
+    def get_api_counts(self):
+        res = self.execute("SELECT * FROM `counts` WHERE type='openApi'", result=True)
+        if res:
+            return res[0][1]
+        return 0
                 
     def commit(self):
         if self.enable:
             self.db.commit()
 
     def close(self):
         self.cursor.close()
         self.db.close()
         
         
 cache = Cache()
 cache.connect(check_same_thread=False)
-
```

### Comparing `dingraia-2.0.6/dingraia/callback_handler.py` & `dingraia-2.0.8/dingraia/callback_handler.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/config.py` & `dingraia-2.0.8/dingraia/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Union, Callable
 
 
 class Bot:
     
     def __init__(self, AppKey: str, AppSecret: str, robotCode: str, GroupWebhookAccessToken: str = None,
                  GroupWebhookSecureKey: str = None):
         self.appKey = AppKey
@@ -30,21 +30,31 @@
 class Stream:
     
     def __init__(self, AppKey: str, AppSecret: str):
         self.AppKey = AppKey
         self.AppSecret = AppSecret
 
 
+class CustomStreamConnect:
+    
+    def __init__(self, StreamUrl: str, SignHandler: Union[str, Callable] = None, ExtraHeaders: dict = None):
+        if ExtraHeaders is None:
+            self.ExtraHeaders = {}
+        self.StreamUrl = StreamUrl
+        self.SignHandler = SignHandler
+
+
 class Config:
     
     def __init__(self,
                  event_callback: CallBack = None,
                  bot: Bot = None,
                  stream: List[Stream] = None,
                  *,
+                 customStreamConnect: CustomStreamConnect = None,
                  autoBotConfig: bool = True,
                  useDatabase: bool = True
                  ):
         """初始化Config
         
         Notes:
             在 `autoBotConfig` 启用且 `Stream` 启用时会自动替换 `Bot` 的值
@@ -53,13 +63,14 @@
             event_callback:
             bot:
             stream:
             autoBotConfig: 是否自动替换Bot的值
         """
         self.useDatabase = useDatabase
         self.event_callback = event_callback
+        self.customStreamConnect = customStreamConnect
         self.bot: Union[Bot, None] = bot
         self.stream: Union[List[Stream], None] = stream
         if not isinstance(self.stream, list):
             self.stream = [self.stream]
         if len(self.stream) == 1 and autoBotConfig:
             self.bot = Bot(stream[0].AppKey, stream[0].AppSecret, stream[0].AppKey)
```

### Comparing `dingraia-2.0.6/dingraia/element.py` & `dingraia-2.0.8/dingraia/element.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,7 +105,32 @@
         return json.loads(self.text)
     
     def __bool__(self) -> bool:
         return True if self.ok else False
     
     def __repr__(self):
         return f"<Response [{self.ok}]>"
+
+
+class UrlBuilder:
+    """抽象builder"""
+    
+    def __init__(self, base_url: str = ""):
+        self.url = base_url
+    
+    def __getattr__(self, u):
+        self.url += "." + str(u)
+        return self
+    
+    def __floordiv__(self, other):
+        self.url += "://" + str(other)
+        return self
+    
+    def __truediv__(self, other):
+        self.url += "/" + str(other)
+        return self
+    
+    def __str__(self) -> str:
+        return self.url
+    
+    def __repr__(self):
+        return self.url
```

### Comparing `dingraia-2.0.6/dingraia/event/event.py` & `dingraia-2.0.8/dingraia/event/event.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/exceptions.py` & `dingraia-2.0.8/dingraia/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """
 错误合集，用于提示
 """
 
 
+class DingtalkAPIError(Exception):
+    code = -1
+
+
 class ConfigError(Exception):
     pass
 
 
 class UnsupportedRecallType(Exception):
     pass
 
@@ -15,62 +19,67 @@
     pass
 
 
 class UploadFileError(Exception):
     pass
 
 
-class DownloadFileError(Exception):
+class DownloadFileError(DingtalkAPIError):
     ...
 
 
 class UploadFileSizeError(Exception):
     ...
 
 
-class DingtalkAPIError(Exception):
-    code = -1
+class SQLError(Exception):
+    ...
 
 
-class ResourceNotFoundError(Exception):
+class ResourceNotFoundError(DingtalkAPIError):
     code = "resource.not.found"
 
 
-class WrongParameterError(Exception):
+class WrongParameterError(DingtalkAPIError):
     code = 400002
 
 
-class InvalidParameterError(Exception):
+class InvalidParameterError(DingtalkAPIError):
     code = 40035
 
 
-class InvalidUserIdError(Exception):
+class InvalidFileTypeError(DingtalkAPIError):
+    code = 40005
+
+
+class InvalidUserIdError(DingtalkAPIError):
     code = 33012
 
 
-class ApiPermissionDeniedError(Exception):
+class ApiPermissionDeniedError(DingtalkAPIError):
     code = 60011
 
 
-class IPNotInWhitelistError(Exception):
+class IPNotInWhitelistError(DingtalkAPIError):
     code = 60020
 
 
-class UserNotFoundError(Exception):
+class UserNotFoundError(DingtalkAPIError):
     code = 60121
 
 
-class APIRateLimitedError(Exception):
+class APIRateLimitedError(DingtalkAPIError):
     code = 90002
     code2 = 90018
 
 
 err_code_map = {
     -1                                                  : DingtalkAPIError,
     "resource.not.found"                                : ResourceNotFoundError,
+    40005: InvalidFileTypeError,
     40035                                               : InvalidParameterError,
     "param.invalid"                                     : InvalidParameterError,
     33012                                               : InvalidUserIdError,
     60011                                               : ApiPermissionDeniedError,
     "Forbidden.AccessDenied.AccessTokenPermissionDenied": ApiPermissionDeniedError,
     60020                                               : IPNotInWhitelistError,
     60121                                               : UserNotFoundError,
@@ -83,9 +92,9 @@
 class ErrorReason:
     
     def __init__(self):
         self.err_map = err_code_map
     
     def __getitem__(self, item):
         if item in self.err_map:
-            return self.err_map
+            return self.err_map[item]
         return DingtalkAPIError
```

### Comparing `dingraia-2.0.6/dingraia/message/chain.py` & `dingraia-2.0.8/dingraia/message/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-﻿from typing import Any
+﻿from typing import Any, TypeVar
 
 from typing_extensions import Self
 
 from .element import At
 
+_T = TypeVar('_T')
+
 
 class MessageChain:
     
     def __init__(self, *elements, at: list = None):
         self.mes = [s for s in list(elements)]
         self.display = ''.join([str(x) for x in self.mes])
         if at is not None:
             self.mes += [At(at_id) for at_id in at]
     
     def include(self, __obj: type) -> Self:
         return self.get(__obj)  # __class__([i for i in self.mes if isinstance(i, __obj)])
     
-    def get_first(self, __obj: type) -> Self:
+    def get_first(self, __obj: _T) -> _T:
         return self.get(__obj)[0]
     
     def get(self, element_class: type, count: int = -1) -> list:
         """
         获取消息链中所有特定类型的消息元素
 
         Args:
```

### Comparing `dingraia-2.0.6/dingraia/message/element.py` & `dingraia-2.0.8/dingraia/message/element.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import hashlib
 import json
 import os
 from pathlib import Path
-from typing import Union, BinaryIO
+from typing import Union, BinaryIO, List
 
 from ..model import Member
 
 
 class File:
     type: "File"
     
@@ -17,25 +17,28 @@
     
     fileType: str
     
     mediaId = None
     
     downloadCode: str = None
     
-    def __init__(self, file: Union[Path, BinaryIO, str] = None):
+    def __init__(self, file: Union[Path, BinaryIO, bytes, str] = None):
         if file:
-            if not isinstance(file, BinaryIO):
+            if isinstance(file, (Path, str)):
                 f = open(file, 'rb')
                 self.file = f
                 f.seek(0, os.SEEK_END)
                 self.size = f.tell()
                 f.seek(0)
             else:
                 self.file = file
-                self.size = len(self.file.read())
+                if isinstance(self.file, BinaryIO):
+                    self.size = len(self.file.read())
+                elif isinstance(self.file, bytes):
+                    self.size = len(self.file)
         self.mediaId = None
         self.fileName = None
         self.fileType = 'file'
     
     @property
     def template(self):
         return {
@@ -94,28 +97,17 @@
     
     def __str__(self):
         return f"[Link]({self.url})"
 
 
 class Image(File):
     
-    def __init__(self, file: Union[Path, BinaryIO, str] = None):
+    def __init__(self, file: Union[Path, BinaryIO, bytes, str] = None):
         super().__init__(file)
-        if file:
-            if not isinstance(file, BinaryIO):
-                f = open(file, 'rb')
-                self.file = f
-                f.seek(0, os.SEEK_END)
-                self.size = f.tell()
-                f.seek(0)
-            else:
-                self.file = file
-                self.size = len(self.file.read())
         self.fileType = 'image'
-        self.mediaId = None
     
     @property
     def template(self):
         return {
             'msgKey'  : "sampleImageMsg",
             'msgParam': json.dumps({
                 'photoURL': self.mediaId
@@ -130,26 +122,15 @@
         return f"[图片]({self.downloadCode} {self.mediaId})"
 
 
 class Audio(File):
     
     def __init__(self, file: Union[Path, BinaryIO, str] = None):
         super().__init__(file)
-        if file:
-            if not isinstance(file, BinaryIO):
-                f = open(file, 'rb')
-                self.file = f
-                f.seek(0, os.SEEK_END)
-                self.size = f.tell()
-                f.seek(0)
-            else:
-                self.file = file
-                self.size = len(self.file.read())
         self.fileType = 'voice'
-        self.mediaId = None
         self.duration = None
     
     @property
     def template(self):
         return {
             'msgKey'  : "sampleAudio",
             'msgParam': json.dumps({
@@ -166,26 +147,15 @@
         return f"[音频]({self.downloadCode} {self.mediaId})"
 
 
 class Video(File):
     
     def __init__(self, file: Union[Path, BinaryIO, str] = None):
         super().__init__(file)
-        if file:
-            if not isinstance(file, BinaryIO):
-                f = open(file, 'rb')
-                self.file = f
-                f.seek(0, os.SEEK_END)
-                self.size = f.tell()
-                f.seek(0)
-            else:
-                self.file = file
-                self.size = len(self.file.read())
         self.fileType = 'video'
-        self.mediaId = None
         self.videoMediaId = None
         self.videoType = 'mp4'
         self.duration = None
         self.picMediaId = None
     
     @property
     def template(self):
@@ -232,15 +202,15 @@
     
     def __str__(self):
         return "[Markdown]"
 
 
 class ActionCard(BaseElement):
     
-    def __init__(self, text: str, button: list, title: str = "[ActionCard]", orientation: int = 0):
+    def __init__(self, text: str, button: List[List[str]], title: str = "[ActionCard]", orientation: int = 0):
         """发送ActionCard消息
 
         Args:
             title: 标题(似乎没啥用)
             text: Markdown文本
             button: 按钮列表，即使只有一个也要使用[[title, url], ...]的格式
             orientation: 排列方向，0为竖向，1为横向，建议横向不超过5个字
@@ -352,15 +322,15 @@
     
     def __str__(self):
         return "[ActionCard]"
 
 
 class FeedCard(BaseElement):
     
-    def __init__(self, links: list):
+    def __init__(self, links: List[List[str]]):
         """发送FeedCard消息
 
         Args:
             links: 链接列表，格式：[[title, msgURL, picURL], ...]
         """
         self.links = links
         self.data = {
@@ -377,14 +347,16 @@
                 })
     
     def __str__(self):
         return "[FeedCard]"
 
 
 class At:
+    id: str
+    target: str
     
     def __init__(self, target: Union[tuple, Member], display: str = ""):
         if isinstance(target, Member):
             self.id = (int(hashlib.sha1(str(target.id)[str(target.id).rfind("$"):].encode('utf-8')).hexdigest(), 16)) % \
                       (10 ** 10) + 1000
             self.target = str(target.staffid)
         else:
```

### Comparing `dingraia-2.0.6/dingraia/model/__init__.py` & `dingraia-2.0.8/dingraia/model/__init__.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/saya/__init__.py` & `dingraia-2.0.8/dingraia/saya/__init__.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/saya/builtins/broadcast/schema.py` & `dingraia-2.0.8/dingraia/saya/builtins/broadcast/schema.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/saya/channel.py` & `dingraia-2.0.8/dingraia/saya/channel.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/signer.py` & `dingraia-2.0.8/dingraia/signer.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/tools/color_text.py` & `dingraia-2.0.8/dingraia/tools/color_text.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/tools/debug.py` & `dingraia-2.0.8/dingraia/tools/debug.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia/verify.py` & `dingraia-2.0.8/dingraia/verify.py`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/dingraia.egg-info/SOURCES.txt` & `dingraia-2.0.8/dingraia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingraia-2.0.6/setup.py` & `dingraia-2.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿from setuptools import setup, find_packages
-# from dingraia.VERSION import VERSION
+from dingraia.VERSION import VERSION
 
 setup(
     name='dingraia',
-    version="2.0.6",
+    version=VERSION,
     packages=find_packages(),
     url='https://github.com/MeiHuaGuangShuo/Dingraia',
     author='MeiHuaGuangShuo',
     author_email='meihuaguangshuo@gmail.com',
     description='A Dingtalk robot framework based on Python, supported http and stream mode.',
     long_description='A Dingtalk robot framework, easier to use.',
     install_requires=[
```

