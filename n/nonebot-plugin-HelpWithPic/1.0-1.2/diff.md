# Comparing `tmp/nonebot-plugin-HelpWithPic-1.0.tar.gz` & `tmp/nonebot-plugin-HelpWithPic-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-HelpWithPic-1.0.tar", last modified: Wed Mar 20 13:33:23 2024, max compression
+gzip compressed data, was "nonebot-plugin-HelpWithPic-1.2.tar", last modified: Thu Apr  4 13:41:56 2024, max compression
```

## Comparing `nonebot-plugin-HelpWithPic-1.0.tar` & `nonebot-plugin-HelpWithPic-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:33:23.428067 nonebot-plugin-HelpWithPic-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-20 13:33:15.000000 nonebot-plugin-HelpWithPic-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44058 2024-03-20 13:33:23.428067 nonebot-plugin-HelpWithPic-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-20 13:33:15.000000 nonebot-plugin-HelpWithPic-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:33:23.428067 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44058 2024-03-20 13:33:23.000000 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-20 13:33:23.000000 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:33:23.000000 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-20 13:33:23.000000 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:33:23.000000 nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-20 13:33:15.000000 nonebot-plugin-HelpWithPic-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:33:23.428067 nonebot-plugin-HelpWithPic-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44126 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44126 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:41:56.000000 nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 13:41:52.000000 nonebot-plugin-HelpWithPic-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:41:56.148584 nonebot-plugin-HelpWithPic-1.2/setup.cfg
```

### Comparing `nonebot-plugin-HelpWithPic-1.0/LICENSE` & `nonebot-plugin-HelpWithPic-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-HelpWithPic-1.0/PKG-INFO` & `nonebot-plugin-HelpWithPic-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-HelpWithPic
-Version: 1.0
+Version: 1.2
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,15 +683,15 @@
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
-Requires-Dist: nonebot_plugin_saa
+Requires-Dist: nonebot_plugin_send_anything_anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -719,23 +719,22 @@
 
 
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
 此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
+目前只支持 onebotV11 !!!!
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
-暂时未完成上传PYPI，目前只能下载源码使用。
-
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-HelpWithPic
 
 </details>
@@ -770,23 +769,24 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+大小写不影响配置)
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| ps_font | 否 | None | 配置说明 |
-| ps_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png'] |
+| HWP_font | 否 | None | 使用的字体文件 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| plugin_version | 否 | "HelpWithPic-Beta1.0"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

### Comparing `nonebot-plugin-HelpWithPic-1.0/README.md` & `nonebot-plugin-HelpWithPic-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,22 @@
 
 
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
 此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
+目前只支持 onebotV11 !!!!
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
-暂时未完成上传PYPI，目前只能下载源码使用。
-
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-HelpWithPic
 
 </details>
@@ -77,23 +76,24 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+大小写不影响配置)
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| ps_font | 否 | None | 配置说明 |
-| ps_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png'] |
+| HWP_font | 否 | None | 使用的字体文件 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| plugin_version | 否 | "HelpWithPic-Beta1.0"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-HelpWithPic _â¨ nonebotæä»¶-å¨æå¸®å©å¾çå¶ä½ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## â  æ³¨æ
 å ä¸ºææ¯å°ç½,æåªè½ä»¥æèªå·±çæ¹å¼åæè§å¾å¯è½æºå¥½ç¨çæä»¶
 () æä»¥é¨åä»£ç é»è¾å¯è½ä¸æ¯å¾å¥½ æ­¤æä»¶é¨åä»£ç åè
-nonebot-plugin-picstatus (å¶å¾ä¸é¨åèµæºè·å) ## ð ä»ç»
-è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿ å®è£
-ææ¶æªå®æä¸ä¼ PYPIï¼ç®ååªè½ä¸è½½æºç ä½¿ç¨ã ä½¿ç¨ nb-cli
-å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+nonebot-plugin-picstatus (å¶å¾ä¸é¨åèµæºè·å) ç®ååªæ¯æ
+onebotV11 !!!! ## ð ä»ç» è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿
+å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-HelpWithPic
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-HelpWithPic pdm pdm add nonebot-plugin-
 HelpWithPic poetry poetry add nonebot-plugin-HelpWithPic conda conda install
 nonebot-plugin-HelpWithPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_HelpWithPic"] ## âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | ps_font | å¦ | None |
-éç½®è¯´æ | | ps_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///
-å¼å¤´,æ¯å¦['file:///./data/draw/default_bg1.png'] | | version | å¦ |
-"Unknow" | å¯ä»¥å¡«ä½ çbotçæ¬ | | HWP_commandstart | å¦ | "#" |
-èªå®ä¹å½ä»¤å¤´ | | HWP_nickname | å¦ | "æ¬botçå¸®å©ææ¡£" | æ é¢ |
-| HWP_text | å¦ | "ä½ æ³è¦ç,æä»¬é½æ²¡æ(ä¸æ¯\nè¿æ¯æè¿°" | æè¿°
-| | plugin_version | å¦ | "HelpWithPic-Beta1.0" | æä»¶çæ¬ | ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:----:|:----:| | #help | user | å¦ | ç¾¤è/ç§è |
-è¯·æ ¹æ®HWP_commandstartä½¿ç¨ |
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
+å¤§å°åä¸å½±åéç½®) | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:
+|:----:|:----:|:----:| | HWP_font | å¦ | None | ä½¿ç¨çå­ä½æä»¶ | |
+HWP_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///å¼å¤´,æ¯å¦['file://
+/./data/draw/default_bg1.png']æ­¤å¤ä½¿ç¨ç¸å¯¹è·¯å¾,é»è®¤ä½¿ç¨bingå£çº¸ |
+| version | å¦ | "Unknow" | å¯ä»¥å¡«ä½ çbotçæ¬ | | HWP_commandstart |
+å¦ | "#" | èªå®ä¹å½ä»¤å¤´ | | HWP_nickname | å¦ | "æ¬botçå¸®å©ææ¡£"
+| æ é¢ | | HWP_text | å¦ | "ä½ æ³è¦ç,æä»¬é½æ²¡æ
+(ä¸æ¯\nè¿æ¯æè¿°" | æè¿° | | HWP_version | å¦ | "HelpWithPic-Beta1.2" |
+æä»¶çæ¬ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ |
+èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | #help | user | å¦ |
+ç¾¤è/ç§è | è¯·æ ¹æ®HWP_commandstartä½¿ç¨ |
```

### Comparing `nonebot-plugin-HelpWithPic-1.0/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO` & `nonebot-plugin-HelpWithPic-1.2/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-HelpWithPic
-Version: 1.0
+Version: 1.2
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,15 +683,15 @@
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
-Requires-Dist: nonebot_plugin_saa
+Requires-Dist: nonebot_plugin_send_anything_anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -719,23 +719,22 @@
 
 
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
 此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
+目前只支持 onebotV11 !!!!
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
-暂时未完成上传PYPI，目前只能下载源码使用。
-
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-HelpWithPic
 
 </details>
@@ -770,23 +769,24 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+大小写不影响配置)
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| ps_font | 否 | None | 配置说明 |
-| ps_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png'] |
+| HWP_font | 否 | None | 使用的字体文件 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
-| plugin_version | 否 | "HelpWithPic-Beta1.0"  | 插件版本 |
+| HWP_version | 否 | "HelpWithPic-Beta1.2"  | 插件版本 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

