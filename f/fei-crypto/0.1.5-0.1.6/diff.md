# Comparing `tmp/fei_crypto-0.1.5.tar.gz` & `tmp/fei_crypto-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fei_crypto-0.1.5.tar", max compression
+gzip compressed data, was "fei_crypto-0.1.6.tar", max compression
```

## Comparing `fei_crypto-0.1.5.tar` & `fei_crypto-0.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      140 2023-12-20 05:11:49.661668 fei_crypto-0.1.5/fei_crypto/__init__.py
--rw-r--r--   0        0        0      887 2024-03-21 05:14:18.936639 fei_crypto-0.1.5/fei_crypto/captcha.py
--rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.5/fei_crypto/crypto.py
--rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.5/fei_crypto/discordwebhook.py
--rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.5/fei_crypto/env.py
--rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.5/fei_crypto/md5.py
--rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.5/fei_crypto/os.py
--rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.5/fei_crypto/rmw.py
--rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.5/fei_crypto/rnd_emoj.py
--rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.5/fei_crypto/t2m.py
--rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.5/fei_crypto/time.py
--rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.5/LICENSE
--rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.5/main/__init__.py
--rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.5/main/btc_eth.py
--rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.5/main/captcha.py
--rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.5/main/dc_webhook_send.py
--rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.5/main/emoj.py
--rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.5/main/env.py
--rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.5/main/main.py
--rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.5/main/os.py
--rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.5/main/rmw.py
--rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.5/main/say.py
--rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.5/main/t2m.py
--rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.5/main/tg_forward.py
--rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.5/main/tg_login.py
--rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.5/main/ts.py
--rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.5/main/uu_id.py
--rw-r--r--   0        0        0     1453 2024-04-03 08:51:31.022597 fei_crypto-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3309 2024-04-03 08:49:10.430965 fei_crypto-0.1.5/README.md
--rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.5/tg/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.5/tg/bot/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-03 08:01:55.185079 fei_crypto-0.1.5/tg/bot/live_bot.py
--rw-r--r--   0        0        0     1908 2024-04-02 17:24:42.314843 fei_crypto-0.1.5/tg/bot/utils.py
--rw-r--r--   0        0        0     3966 2024-04-03 08:28:04.109210 fei_crypto-0.1.5/tg/cli_forward.py
--rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.5/tg/cli_login.py
--rw-r--r--   0        0        0     6472 2024-04-03 08:27:32.982473 fei_crypto-0.1.5/tg/config.py
--rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.5/tg/const.py
--rw-r--r--   0        0        0     3903 2024-04-03 08:01:55.176079 fei_crypto-0.1.5/tg/live.py
--rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.5/tg/login.py
--rw-r--r--   0        0        0     2274 2024-04-03 08:01:56.268330 fei_crypto-0.1.5/tg/message.py
--rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.5/tg/parse.py
--rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.5/tg/past.py
--rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.5/tg/plugin_models.py
--rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.5/tg/plugins/__init__.py
--rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.5/tg/plugins/caption.py
--rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.5/tg/plugins/filter.py
--rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.5/tg/plugins/fmt.py
--rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.5/tg/plugins/replace.py
--rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.5/tg/storage.py
--rw-r--r--   0        0        0     1779 2024-04-02 18:16:11.762778 fei_crypto-0.1.5/tg/utils.py
--rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 fei_crypto-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      140 2023-12-20 05:11:49.661668 fei_crypto-0.1.6/fei_crypto/__init__.py
+-rw-r--r--   0        0        0      887 2024-03-21 05:14:18.936639 fei_crypto-0.1.6/fei_crypto/captcha.py
+-rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.6/fei_crypto/crypto.py
+-rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.6/fei_crypto/discordwebhook.py
+-rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.6/fei_crypto/env.py
+-rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.6/fei_crypto/md5.py
+-rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.6/fei_crypto/os.py
+-rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.6/fei_crypto/rmw.py
+-rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.6/fei_crypto/rnd_emoj.py
+-rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.6/fei_crypto/t2m.py
+-rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.6/fei_crypto/time.py
+-rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.6/LICENSE
+-rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.6/main/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.6/main/btc_eth.py
+-rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.6/main/captcha.py
+-rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.6/main/dc_webhook_send.py
+-rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.6/main/emoj.py
+-rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.6/main/env.py
+-rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.6/main/main.py
+-rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.6/main/os.py
+-rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.6/main/rmw.py
+-rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.6/main/say.py
+-rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.6/main/t2m.py
+-rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.6/main/tg_forward.py
+-rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.6/main/tg_login.py
+-rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.6/main/ts.py
+-rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.6/main/uu_id.py
+-rw-r--r--   0        0        0     1453 2024-04-04 11:07:03.897698 fei_crypto-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3597 2024-04-04 09:38:32.012308 fei_crypto-0.1.6/README.md
+-rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.6/tg/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.6/tg/bot/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-03 08:01:55.185079 fei_crypto-0.1.6/tg/bot/live_bot.py
+-rw-r--r--   0        0        0     1908 2024-04-02 17:24:42.314843 fei_crypto-0.1.6/tg/bot/utils.py
+-rw-r--r--   0        0        0     3966 2024-04-03 08:28:04.109210 fei_crypto-0.1.6/tg/cli_forward.py
+-rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.6/tg/cli_login.py
+-rw-r--r--   0        0        0     6472 2024-04-03 08:27:32.982473 fei_crypto-0.1.6/tg/config.py
+-rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.6/tg/const.py
+-rw-r--r--   0        0        0     3903 2024-04-03 08:01:55.176079 fei_crypto-0.1.6/tg/live.py
+-rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.6/tg/login.py
+-rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.1.6/tg/message.py
+-rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.6/tg/parse.py
+-rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.6/tg/past.py
+-rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.6/tg/plugin_models.py
+-rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.6/tg/plugins/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.6/tg/plugins/caption.py
+-rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.6/tg/plugins/filter.py
+-rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.6/tg/plugins/fmt.py
+-rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.6/tg/plugins/replace.py
+-rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.6/tg/storage.py
+-rw-r--r--   0        0        0     1779 2024-04-02 18:16:11.762778 fei_crypto-0.1.6/tg/utils.py
+-rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 fei_crypto-0.1.6/PKG-INFO
```

### Comparing `fei_crypto-0.1.5/fei_crypto/captcha.py` & `fei_crypto-0.1.6/fei_crypto/captcha.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/fei_crypto/discordwebhook.py` & `fei_crypto-0.1.6/fei_crypto/discordwebhook.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/fei_crypto/rmw.py` & `fei_crypto-0.1.6/fei_crypto/rmw.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/fei_crypto/rnd_emoj.py` & `fei_crypto-0.1.6/fei_crypto/rnd_emoj.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/fei_crypto/t2m.py` & `fei_crypto-0.1.6/fei_crypto/t2m.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/LICENSE` & `fei_crypto-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/pyproject.toml` & `fei_crypto-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 name = "fei-crypto"
 packages = [
     { include = "fei_crypto" },
     { include = "tg" },
     { include = "main" },
 ]
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 cowsay = "^6.1"
 filestools = "^0.2.1"
 pillow = "^9.5.0"
 python = "<3.12,>=3.10"
 #python = "~3.11"
```

### Comparing `fei_crypto-0.1.5/README.md` & `fei_crypto-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -49,20 +49,23 @@
 14. dcw # 使用discord webhook send发送消息
     - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
-15. tgf # 转发telegram group或channel,支持用户转发和机器人转发
+15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
+    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`
     - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
-    - 示例:`run tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
+    - 机器人转发需在配置文件中填写`BOT_TOKEN`
+    - 代理配置,在配置文件login下配置`"PROXY": "socks5://127.0.0.1:7890"`
+    - 示例:`tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
     - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
-    - --config-path,-c: 配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
+    - --config-path,-c: 可传入任意配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
     - --version,-v: 查看版本信息
     - --help:帮助文档
     
 # dev
 
 ```shell
 poetry shell
```

### Comparing `fei_crypto-0.1.5/tg/bot/live_bot.py` & `fei_crypto-0.1.6/tg/bot/live_bot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/bot/utils.py` & `fei_crypto-0.1.6/tg/bot/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/cli_forward.py` & `fei_crypto-0.1.6/tg/cli_forward.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/cli_login.py` & `fei_crypto-0.1.6/tg/cli_login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/config.py` & `fei_crypto-0.1.6/tg/config.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/live.py` & `fei_crypto-0.1.6/tg/live.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/login.py` & `fei_crypto-0.1.6/tg/login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/message.py` & `fei_crypto-0.1.6/tg/message.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,15 +47,18 @@
 
 async def send_message(recipient: EntityLike, tm: TgMessage) -> Sequence[Message] | Message:
     """Forward or send a copy, depending on config."""
     client: TelegramClient = tm.message.client
     sender = await tm.message.get_sender()
 
     if tm.message.is_group:
-        from_user = f'【{sender.first_name} {sender.last_name}】'
+        last_name = ''
+        if sender.last_name is not None and sender.last_name != '':
+            last_name = ' ' + sender.last_name
+        from_user = f'【{sender.first_name}{last_name}】'
         tm.text = from_user + tm.text
 
     if CONFIG.show_forwarded_from:
         return await client.forward_messages(recipient, tm.message)
     if tm.new_file:
         message = await client.send_file(
             recipient, tm.new_file, caption=tm.text, reply_to=tm.reply_to
```

### Comparing `fei_crypto-0.1.5/tg/past.py` & `fei_crypto-0.1.6/tg/past.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/plugin_models.py` & `fei_crypto-0.1.6/tg/plugin_models.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/plugins/__init__.py` & `fei_crypto-0.1.6/tg/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/plugins/filter.py` & `fei_crypto-0.1.6/tg/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/plugins/fmt.py` & `fei_crypto-0.1.6/tg/plugins/fmt.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/plugins/replace.py` & `fei_crypto-0.1.6/tg/plugins/replace.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/storage.py` & `fei_crypto-0.1.6/tg/storage.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/tg/utils.py` & `fei_crypto-0.1.6/tg/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.5/PKG-INFO` & `fei_crypto-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fei-crypto
-Version: 0.1.5
+Version: 0.1.6
 Summary: fei crypto command utils
 License: MIT
 Author: feicrypto
 Author-email: feicrypto@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -78,20 +78,23 @@
 14. dcw # 使用discord webhook send发送消息
     - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
-15. tgf # 转发telegram group或channel,支持用户转发和机器人转发
+15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
+    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`
     - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
-    - 示例:`run tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
+    - 机器人转发需在配置文件中填写`BOT_TOKEN`
+    - 代理配置,在配置文件login下配置`"PROXY": "socks5://127.0.0.1:7890"`
+    - 示例:`tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
     - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
-    - --config-path,-c: 配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
+    - --config-path,-c: 可传入任意配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
     - --version,-v: 查看版本信息
     - --help:帮助文档
     
 # dev
 
 ```shell
 poetry shell
```

