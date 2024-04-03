# Comparing `tmp/tooldelta-0.4.8.tar.gz` & `tmp/tooldelta-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.4.8.tar", max compression
+gzip compressed data, was "tooldelta-0.4.9.tar", max compression
```

## Comparing `tooldelta-0.4.8.tar` & `tooldelta-0.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1497 2024-03-19 09:29:46.412079 tooldelta-0.4.8/LICENSE
--rwxr-xr-x   0        0        0     4376 2024-03-19 09:29:46.412079 tooldelta-0.4.8/README.md
--rwxr-xr-x   0        0        0      885 2024-03-19 09:29:55.132230 tooldelta-0.4.8/pyproject.toml
--rwxr-xr-x   0        0        0      290 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/__init__.py
--rwxr-xr-x   0        0        0     1564 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/basic_mods.py
--rwxr-xr-x   0        0        0    13640 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/builtins.py
--rwxr-xr-x   0        0        0     9338 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/cfg.py
--rwxr-xr-x   0        0        0     7848 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/color_print.py
--rw-r--r--   0        0        0     1945 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    38821 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/frame.py
--rwxr-xr-x   0        0        0     3367 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0     1663 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/get_python_libs.py
--rwxr-xr-x   0        0        0      338 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    25909 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1054 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2138 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/logger.py
--rwxr-xr-x   0        0        0    33949 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     9089 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/old_dotcs_env.py
--rwxr-xr-x   0        0        0     1143 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/packets.py
--rwxr-xr-x   0        0        0    11936 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     2177 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     6359 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0     7579 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/dotcs_plugin/__init__.py
--rwxr-xr-x   0        0        0      345 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     6914 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9279 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    14849 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    12409 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1822 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/starter.py
--rwxr-xr-x   0        0        0      639 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     6602 2024-03-19 09:29:46.416079 tooldelta-0.4.8/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 tooldelta-0.4.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-03-20 04:18:37.807537 tooldelta-0.4.9/LICENSE
+-rwxr-xr-x   0        0        0     4376 2024-03-20 04:18:37.807537 tooldelta-0.4.9/README.md
+-rwxr-xr-x   0        0        0      885 2024-03-20 04:18:46.263443 tooldelta-0.4.9/pyproject.toml
+-rwxr-xr-x   0        0        0      290 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/__init__.py
+-rwxr-xr-x   0        0        0     1591 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/basic_mods.py
+-rwxr-xr-x   0        0        0    13640 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0     9338 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0     7848 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1945 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    38486 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     3367 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0     1663 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/get_python_libs.py
+-rwxr-xr-x   0        0        0      338 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    25909 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1054 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2138 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/logger.py
+-rwxr-xr-x   0        0        0    33949 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/neo_libs/neo_conn.py
+-rwxr-xr-x   0        0        0     9089 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/old_dotcs_env.py
+-rwxr-xr-x   0        0        0     1143 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    11936 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     2177 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     6359 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0     7579 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/dotcs_plugin/__init__.py
+-rwxr-xr-x   0        0        0      345 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     6914 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9235 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    14849 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    12409 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1822 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      639 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     6602 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 tooldelta-0.4.9/PKG-INFO
```

### Comparing `tooldelta-0.4.8/LICENSE` & `tooldelta-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/README.md` & `tooldelta-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/pyproject.toml` & `tooldelta-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.4.8" # This field is automatically set to the value in the version file
+version = "0.4.9" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.4.8/tooldelta/basic_mods.py` & `tooldelta-0.4.9/tooldelta/basic_mods.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     import datetime
     import platform
     import subprocess
     import socket
     import logging
     import ctypes
     import asyncio
+    import multiprocessing
     import copy
     import math
     import random
     import psutil
     import pyspeedtest
     import requests
     import nbt
```

### Comparing `tooldelta-0.4.8/tooldelta/builtins.py` & `tooldelta-0.4.9/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/cfg.py` & `tooldelta-0.4.9/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/color_print.py` & `tooldelta-0.4.9/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/constants.py` & `tooldelta-0.4.9/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.4.9/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/frame.py` & `tooldelta-0.4.9/tooldelta/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -754,14 +754,18 @@
             isJoining = bool(player["Skin"]["SkinData"])
             playername = player["Username"]
             if isJoining:
                 Print.print_inf(f"§e{playername} 加入了游戏")
                 if playername not in self.allplayers and not res:
                     self.allplayers.append(playername)
                     return
+                plugin_group.execute_player_join(
+                    playername, self.linked_frame.on_plugin_err
+                )
+                asyncio.run(execute_player_join(player))
             else:
                 playername = next(
                     (k for k, v in self.players_uuid.items() if v == player["UUID"]),
                     None,
                 )
                 if playername is None:
                     Print.print_war("无法获取PlayerList中玩家名字")
@@ -780,23 +784,14 @@
             case 2:
                 if pkt["Message"] == "§e%multiplayer.player.joined":
                     player = pkt["Parameters"][0]
                     plugin_grp.execute_player_prejoin(
                         player, self.linked_frame.on_plugin_err
                     )
                     asyncio.run(execute_player_prejoin(player))
-                if pkt["Message"] == "§e%multiplayer.player.join":
-                    player = pkt["Parameters"][0]
-                    plugin_grp.execute_player_join(
-                        player, self.linked_frame.on_plugin_err
-                    )
-                    asyncio.run(execute_player_join(player))
-
-                elif pkt["Message"] == "§e%multiplayer.player.left":
-                    player = pkt["Parameters"][0]
                 elif pkt["Message"].startswith("death."):
                     death_message = self.Game_Data.get(pkt["Message"])
                     if death_message:
                         filled_parameters = [
                             self.Game_Data.get(param.replace("%", ""), param)
                             for param in pkt["Parameters"]
                         ]
@@ -878,21 +873,16 @@
         Print.print_suc(
             "初始化完成, 在线玩家: "
             + ", ".join(self.allplayers)
             + ", 机器人ID: "
             + self.bot_name
         )
         time.sleep(0.5)
-        self.say_to("@a", "§l§7[§f!§7] §r§fToolDelta Enabled!")
-        self.say_to(
-            "@a",
-            "§l§7[§f!§7] §r§f北京时间 "
-            + datetime.datetime.now().strftime("§a%H§f : §a%M"),
-        )
-        self.say_to("@a", "§l§7[§f!§7] §r§f输入.help获取更多帮助哦")
+        self.say_to("@a", "§l§7[§f!§7] §r§fToolDelta Enabled!\n§l§7[§f!§7] §r§f北京时间 "
+            + datetime.datetime.now().strftime("§a%H§f : §a%M") + "\n§l§7[§f!§7] §r§f输入.help获取更多帮助哦")
         self.sendcmd("/tag @s add robot")
         Print.print_suc("§f在控制台输入 §ahelp / ?§f可查看控制台命令")
 
     def say_to(self, target: str, msg: str):
         """
         向玩家发送聊天栏信息
```

### Comparing `tooldelta-0.4.8/tooldelta/game_texts.py` & `tooldelta-0.4.9/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/get_python_libs.py` & `tooldelta-0.4.9/tooldelta/get_python_libs.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/launch_cli.py` & `tooldelta-0.4.9/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/launch_options.py` & `tooldelta-0.4.9/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/logger.py` & `tooldelta-0.4.9/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/neo_libs/neo_conn.py` & `tooldelta-0.4.9/tooldelta/neo_libs/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/old_dotcs_env.py` & `tooldelta-0.4.9/tooldelta/old_dotcs_env.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/packets.py` & `tooldelta-0.4.9/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.4.9/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/__init__.py` & `tooldelta-0.4.9/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.4.9/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/dotcs_plugin/__init__.py` & `tooldelta-0.4.9/tooldelta/plugin_load/dotcs_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,14 @@
         x: X坐标
         y: Y坐标
         z: Z坐标
     """
     res = sendwscmd(f"/testforblock {x} {y} {z} air", True)
     if res.SuccessCount:
         return "air"
-    print(res.OutputMessages[0].Parameters)
     return res.OutputMessages[0].Parameters[4].strip("%tile.").strip(".name")
 
 
 def getTickingAreaList() -> dict | AttributeError:
     """
     获取 tickingarea 列表
```

### Comparing `tooldelta-0.4.8/tooldelta/plugin_manager.py` & `tooldelta-0.4.9/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/plugin_market.py` & `tooldelta-0.4.9/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/starter.py` & `tooldelta-0.4.9/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/sys_args.py` & `tooldelta-0.4.9/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/tooldelta/urlmethod.py` & `tooldelta-0.4.9/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.8/PKG-INFO` & `tooldelta-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.4.8
+Version: 0.4.9
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.4.8 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.4.9 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: nbt (==1.5.1) Requires-Dist: pillow
```

