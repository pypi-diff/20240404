# Comparing `tmp/nonebot-plugin-HelpWithPic-1.2.tar.gz` & `tmp/nonebot-plugin-HelpWithPic-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-HelpWithPic-1.2.tar", last modified: Thu Apr  4 13:41:56 2024, max compression
+gzip compressed data, was "nonebot-plugin-HelpWithPic-1.2.1.tar", last modified: Thu Apr  4 13:54:54 2024, max compression
```

## Comparing `nonebot-plugin-HelpWithPic-1.2.tar` & `nonebot-plugin-HelpWithPic-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44126 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44126 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44128 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44128 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/setup.cfg
```

### Comparing `nonebot-plugin-HelpWithPic-1.2/LICENSE` & `nonebot-plugin-HelpWithPic-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-HelpWithPic-1.2/PKG-INFO` & `nonebot-plugin-HelpWithPic-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-HelpWithPic
-Version: 1.2
+Version: 1.2.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -779,14 +779,14 @@
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

### Comparing `nonebot-plugin-HelpWithPic-1.2/README.md` & `nonebot-plugin-HelpWithPic-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,14 @@
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

#### html2text {}

```diff
@@ -20,11 +20,11 @@
 å¤§å°åä¸å½±åéç½®) | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:
 |:----:|:----:|:----:| | HWP_font | å¦ | None | ä½¿ç¨çå­ä½æä»¶ | |
 HWP_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///å¼å¤´,æ¯å¦['file://
 /./data/draw/default_bg1.png']æ­¤å¤ä½¿ç¨ç¸å¯¹è·¯å¾,é»è®¤ä½¿ç¨bingå£çº¸ |
 | version | å¦ | "Unknow" | å¯ä»¥å¡«ä½ çbotçæ¬ | | HWP_commandstart |
 å¦ | "#" | èªå®ä¹å½ä»¤å¤´ | | HWP_nickname | å¦ | "æ¬botçå¸®å©ææ¡£"
 | æ é¢ | | HWP_text | å¦ | "ä½ æ³è¦ç,æä»¬é½æ²¡æ
-(ä¸æ¯\nè¿æ¯æè¿°" | æè¿° | | HWP_version | å¦ | "HelpWithPic-Beta1.2" |
+(ä¸æ¯\nè¿æ¯æè¿°" | æè¿° | | HWP_version | å¦ | "HelpWithPic-Betaxxx" |
 æä»¶çæ¬ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ |
 èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | #help | user | å¦ |
 ç¾¤è/ç§è | è¯·æ ¹æ®HWP_commandstartä½¿ç¨ |
```

### Comparing `nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO` & `nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-HelpWithPic
-Version: 1.2
+Version: 1.2.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -779,14 +779,14 @@
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

### Comparing `nonebot-plugin-HelpWithPic-1.2/pyproject.toml` & `nonebot-plugin-HelpWithPic-1.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-HelpWithPic"
-version = "1.2"
+version = "1.2.1"
 description = "nonebot插件-动态帮助图片制作"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

