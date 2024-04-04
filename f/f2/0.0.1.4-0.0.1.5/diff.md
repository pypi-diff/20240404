# Comparing `tmp/f2-0.0.1.4.tar.gz` & `tmp/f2-0.0.1.5.tar.gz`

## Comparing `f2-0.0.1.4.tar` & `f2-0.0.1.5.tar`

### file list

```diff
@@ -1,69 +1,65 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/__main__.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/helps.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/__apps__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/api.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/cli.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/crawler.py
--rw-r--r--   0        0        0    10693 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/db.py
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/dl.py
--rw-r--r--   0        0        0    37332 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/filter.py
--rw-r--r--   0        0        0    35108 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/handler.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/help.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/model.py
--rw-r--r--   0        0        0    24408 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_apps_model.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_aweme_id.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_crawler.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_handler.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_room_id.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_sec_user_id.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_sso_login.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/douyin/test/test_webcast_id.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/api.py
--rw-r--r--   0        0        0    15483 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/cli.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/crawler.py
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/db.py
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/dl.py
--rw-r--r--   0        0        0    19343 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/filter.py
--rw-r--r--   0        0        0    25067 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/handler.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/help.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/model.py
--rw-r--r--   0        0        0    23775 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/tiktok/utils.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/twitter/__init__.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/apps/twitter/help.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/cli/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/cli/cli_commands.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/cli/cli_console.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/conf/app.yaml
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/conf/conf.yaml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/conf/defaults.yaml
--rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/crawlers/base_crawler.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/db/base_db.py
--rw-r--r--   0        0        0    19266 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/dl/base_downloader.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/exceptions/__init__.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/exceptions/api_exceptions.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/exceptions/db_exceptions.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/exceptions/file_exceptions.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/i18n/translator.py
--rw-r--r--   0        0        0    29107 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/languages/en_US/LC_MESSAGES/en_US.mo
--rw-r--r--   0        0        0    27692 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/languages/zh_CN/LC_MESSAGES/zh_CN.mo
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/log/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/__init__.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/__version__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/_dl.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/_signal.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/_singleton.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/conf_manager.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/json_filter.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/mode_handler.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/utils.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 f2-0.0.1.4/f2/utils/xbogus.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 f2-0.0.1.4/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 f2-0.0.1.4/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 f2-0.0.1.4/README.md
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 f2-0.0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 f2-0.0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/__main__.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/helps.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/__apps__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/__init__.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/api.py
+-rw-r--r--   0        0        0    13947 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/cli.py
+-rw-r--r--   0        0        0    10358 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/crawler.py
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/db.py
+-rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/dl.py
+-rw-r--r--   0        0        0    50773 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/filter.py
+-rw-r--r--   0        0        0    57839 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/handler.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/help.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/model.py
+-rw-r--r--   0        0        0    28213 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_apps_model.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_aweme_id.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_crawler.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_handler.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_lrc.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_room_id.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_sec_user_id.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_sso_login.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/douyin/test/test_webcast_id.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/api.py
+-rw-r--r--   0        0        0    12655 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/cli.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/crawler.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/db.py
+-rw-r--r--   0        0        0    11320 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/dl.py
+-rw-r--r--   0        0        0    21009 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/filter.py
+-rw-r--r--   0        0        0    25947 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/handler.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/help.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/model.py
+-rw-r--r--   0        0        0    26297 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/apps/tiktok/utils.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/cli/__init__.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/cli/cli_commands.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/cli/cli_console.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/conf/app.yaml
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/conf/conf.yaml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/conf/defaults.yaml
+-rw-r--r--   0        0        0    11369 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/crawlers/base_crawler.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/db/base_db.py
+-rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/dl/base_downloader.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/exceptions/__init__.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/exceptions/api_exceptions.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/exceptions/db_exceptions.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/exceptions/file_exceptions.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/i18n/translator.py
+-rw-r--r--   0        0        0    34741 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/languages/en_US/LC_MESSAGES/en_US.mo
+-rw-r--r--   0        0        0    32992 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/languages/zh_CN/LC_MESSAGES/zh_CN.mo
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/log/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/__init__.py
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/_dl.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/_signal.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/_singleton.py
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/conf_manager.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/json_filter.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/mode_handler.py
+-rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/utils.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 f2-0.0.1.5/f2/utils/xbogus.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 f2-0.0.1.5/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 f2-0.0.1.5/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 f2-0.0.1.5/README.md
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 f2-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 f2-0.0.1.5/PKG-INFO
```

### Comparing `f2-0.0.1.4/f2/helps.py` & `f2-0.0.1.5/f2/helps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,109 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @Description:helps.py
 @Date       :2023/02/06 17:36:41
 @Author     :JohnserfSeed
-@version    :0.0.1.4
+@version    :0.0.1.5
 @License    :Apache License 2.0
 @Github     :https://github.com/johnserf-seed
 @Mail       :johnserf-seed@foxmail.com
 -------------------------------------------------
 Change Log  :
 2023/02/06 17:36:41 - create output help
+2024/03/11 18:23:30 - change get_help @ importlib path
 -------------------------------------------------
 """
 
+import f2
 import importlib
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from f2.i18n.translator import _
-from f2.utils import __version__
 
 
 def get_help(app_name: str) -> None:
     try:
-        module = importlib.import_module(f"f2.apps.{app_name}")
+        module = importlib.import_module(f"f2.apps.{app_name}.help")
         if hasattr(module, "help"):
             module.help()
         else:
             print(_("在 {0} 应用里没有找到帮助文件").format(app_name))
     except ImportError:
         print(_("没有找到 {0} 应用").format(app_name))
 
 
-def f2() -> None:
+def main() -> None:
     # 真彩
     console = Console(color_system="truecolor")
-    console.print(
-        f"\n:rocket: [bold]f2 {__version__._version} :rocket:", justify="center"
-    )
-    console.print(f"\n[i]{__version__._description_cn}", justify="center")
-    console.print(f"[i]{__version__._description_en}", justify="center")
-    console.print(f"[i]GitHub {__version__._repourl}\n", justify="center")
-
-    table = Table.grid(padding=1, pad_edge=True, expand=True)
-    table.add_column("Website", no_wrap=True, justify="left", style="bold")
-    table.add_column("Description", no_wrap=True, justify="left", style="bold")
-
-    # 分割
-    # console.rule("[b]已适配[/b]", align="center")
-    # table.add_row(
-    #     _("抖音"), _("  单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，原声。后续更新：推荐作品，朋友作品，好友作品，搜索作品")
-    # )
-    # table.add_row(
-    #     _("TikTok"), _("  单个作品，主页作品，点赞作品，收藏作品，播放列表（合辑）作品，原声。后续更新：推荐作品，朋友作品，好友作品，搜索作品")
-    # )
-    # # 待适配
-    # console.print(table)
-    # 分割
-    # console.rule()
+    console.print(f"\n:rocket: [bold]f2 {f2.__version__} :rocket:", justify="center")
+    console.print(f"\n[i]{f2.__description_cn__}", justify="center")
+    console.print(f"[i]{f2.__description_en__}", justify="center")
+    console.print(f"[i]GitHub {f2.__repourl__}\n", justify="center")
 
     # 使用方法
     table = Table.grid(padding=1, pad_edge=True)
     table.add_column("Usage", no_wrap=True, justify="left", style="bold")
     table.add_row("[b]f2[/b] [magenta]<apps> [/magenta][cyan][COMMAND]")
-    table.add_row(_("例： f2 dy -h 来获取douyin的命令帮助"))
+    table.add_row(_("例：f2 dy -h/--help 获取douyin的命令帮助"))
+    table.add_row(
+        "[b]f2[/b] [magenta][Option] [/magenta][cyan][Args][/cyan] [magenta]<apps> [/magenta][cyan][COMMAND]"
+    )
+    table.add_row(_("例：f2 -d DEBUG dy 日志级别为调试运行"))
     console.print(
         Panel(table, border_style="bold", title="使用方法 | Usage", title_align="left")
     )
 
-    table = Table.grid(padding=1, pad_edge=True, expand=True)
+    # 应用列表
     table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("Parameter", no_wrap=True, justify="left", style="bold")
-    table.add_column("Description", no_wrap=True, style="bold")
-    table.add_column("Status", no_wrap=True, justify="left", style="bold")
+    table.add_column(_("参数"), no_wrap=True, justify="left", style="bold")
+    table.add_column(_("描述"), no_wrap=True, style="bold")
+    table.add_column(_("状态"), no_wrap=True, justify="left", style="bold")
 
     table.add_row(_("weibo 或 wb"), _("- 获取微博"))
     table.add_row(
-        _("douyin 或 dy"), _("- 单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，文案，封面，直播，原声。"), _("✔")
+        _("douyin 或 dy"),
+        _(
+            "- 单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，文案，封面，直播，原声。"
+        ),
+        _("✔"),
     )
     table.add_row(
-        _("tiktok 或 tk"), _("- 单个作品，主页作品，点赞作品，收藏作品，播放列表（合辑）作品，文案，封面，原声。"), _("✔")
+        _("tiktok 或 tk"),
+        _(
+            "- 单个作品，主页作品，点赞作品，收藏作品，播放列表（合辑）作品，文案，封面，原声。"
+        ),
+        _("✔"),
     )
     table.add_row(_("instagram 或 ig"), _("- 获取ig的作品"), _("⏳"))
     table.add_row(_("twitch 或 tv"), _("- 获取Twitch直播"))
     table.add_row(_("twitter 或 x"), _("- 获取Twitter作品"), _("⏳"))
     table.add_row(_("youtube 或 ytb"), _("- 获取YouTube的作品"))
     table.add_row(_("bilibili 或 bili"), _("- 获取BiliBili的作品"))
     table.add_row(_("neteasy_music 或 nem"), _("- 获取网易云音乐作品"))
     table.add_row(_("little_red_book 或 lrb"), _("- 获取小红书的作品"))
     table.add_row("\n")
     table.add_row(
-        "f2 -d [magenta]<apps> [/magenta][cyan][COMMAND]",
-        _("- 记录app的debug到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏感信息[/red]"),
+        "f2 -d DEBUG",
+        _(
+            "- 记录app的调试日志到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏感信息[/red]"
+        ),
         _("⚠"),
     )
     table.add_row(
         "Issues❓", "[link=https://github.com/Johnserf-Seed/f2/issues]Click Here[/]"
     ),
     table.add_row(
         "Document📕", "[link=https://johnserf-seed.github.io/f2/]Click Here[/]"
     )
     console.print(
         Panel(
             table,
             border_style="bold",
-            title="<apps>",
+            title="应用 | apps",
             title_align="left",
             subtitle=_("欢迎提交PR适配更多网站"),
         )
     )
```

### Comparing `f2-0.0.1.4/f2/apps/__apps__.py` & `f2-0.0.1.5/f2/apps/__apps__.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/api.py` & `f2-0.0.1.5/f2/apps/douyin/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,23 +50,38 @@
 
     # 用户喜欢A (User Like A)
     USER_FAVORITE_A = f"{DOUYIN_DOMAIN}/aweme/v1/web/aweme/favorite/"
 
     # 用户喜欢B (User Like B)
     USER_FAVORITE_B = f"{IESDOUYIN_DOMAIN}/web/api/v2/aweme/like/"
 
+    # 关注用户(User Following)
+    USER_FOLLOWING = f"{DOUYIN_DOMAIN}/aweme/v1/web/user/following/list/"
+
+    # 粉丝用户 (User Follower)
+    USER_FOLLOWER = f"{DOUYIN_DOMAIN}/aweme/v1/web/user/follower/list/"
+
     # 合集作品
     MIX_AWEME = f"{DOUYIN_DOMAIN}/aweme/v1/web/mix/aweme/"
 
     # 用户历史 (User History)
     USER_HISTORY = f"{DOUYIN_DOMAIN}/aweme/v1/web/history/read/"
 
     # 用户收藏 (User Collection)
     USER_COLLECTION = f"{DOUYIN_DOMAIN}/aweme/v1/web/aweme/listcollection/"
 
+    # 用户收藏夹 (User Collects)
+    USER_COLLECTS = f"{DOUYIN_DOMAIN}/aweme/v1/web/collects/list/"
+
+    # 用户收藏夹作品 (User Collects Posts)
+    USER_COLLECTS_VIDEO = f"{DOUYIN_DOMAIN}/aweme/v1/web/collects/video/list/"
+
+    # 用户音乐收藏 (User Music Collection)
+    USER_MUSIC_COLLECTION = f"{DOUYIN_DOMAIN}/aweme/v1/web/music/listcollection/"
+
     # 首页朋友作品 (Friend Feed)
     FRIEND_FEED = f"{DOUYIN_DOMAIN}/aweme/v1/web/familiar/feed/"
 
     # 关注用户作品 (Follow Feed)
     FOLLOW_FEED = f"{DOUYIN_DOMAIN}/aweme/v1/web/follow/feed/"
 
     # 相关推荐 (Related Feed)
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/cli.py` & `f2-0.0.1.5/f2/apps/douyin/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # path: f2/apps/douyin/cli.py
 
 import f2
 import click
 import typing
 import asyncio
-import browser_cookie3
 
 from pathlib import Path
 
 from f2 import helps
 from f2.cli.cli_commands import set_cli_config
 from f2.log.logger import logger
-from f2.utils.utils import split_dict_cookie, get_resource_path
+from f2.utils.utils import (
+    split_dict_cookie,
+    get_resource_path,
+    get_cookie_from_browser,
+    check_invalid_naming,
+    merge_config,
+)
 from f2.utils.conf_manager import ConfigManager
 from f2.i18n.translator import TranslationManager, _
 from f2.apps.douyin.handler import handle_sso_login
 
 
-def handle_help(
+def handler_help(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> None:
     """
     处理帮助信息 (Handle help messages)
 
@@ -49,78 +54,53 @@
     用于自动从浏览器获取cookie (Used to automatically get cookies from the browser)
 
     Args:
         ctx: click的上下文对象 (Click's context object)
         param: 提供的参数或选项 (The provided parameter or option)
         value: 参数或选项的值 (The value of the parameter or option)
     """
-    if not value or ctx.resilient_parsing:
-        return
-
-    # 如果用户明确设置了 --cookie，那么跳过自动获取过程
-    if ctx.params.get("cookie"):
+    # 如果没有提供值或者用户已经设置了 resilient_parsing 或者提供了 --cookie 参数则跳过
+    if not value or ctx.resilient_parsing or ctx.params.get("cookie"):
         return
 
     # 根据浏览器选择获取cookie
-    if value in ["chrome", "firefox", "edge", "opera"]:
-        try:
-            cookie_value = split_dict_cookie(get_cookie_from_browser(value))
-            manager = ConfigManager(ctx.params.get("config", "conf/app.yaml"))
-            manager.update_config_with_args("douyin", cookie=cookie_value)
-        except PermissionError:
-            message = _("请关闭所有已打开的浏览器重试, 并且你有适当的权限访问浏览器 !")
-            logger.error(message)
-            click.echo(message)
-            ctx.abort()
-        except Exception as e:
-            message = _("自动获取Cookie失败: {0}".format(str(e)))
-            logger.error(message)
-            click.echo(message)
-            ctx.abort()
+    try:
+        cookie_value = split_dict_cookie(get_cookie_from_browser(value, "douyin.com"))
 
+        if not cookie_value:
+            raise ValueError(_("无法从 {0} 浏览器中获取cookie").format(value))
 
-def get_cookie_from_browser(browser_choice: str):
-    """
-    根据用户选择的浏览器获取douyin.com的cookie。
-
-    Args:
-        browser_choice (str): 用户选择的浏览器名称
-
-    Returns:
-        str: *.douyin.com的cookie值
-    """
-
-    BROWSER_FUNCTIONS = {
-        "chrome": browser_cookie3.chrome,
-        "firefox": browser_cookie3.firefox,
-        "edge": browser_cookie3.edge,
-        "opera": browser_cookie3.opera,
-    }
-    cj_function = BROWSER_FUNCTIONS.get(browser_choice)
-    if not cj_function:
-        raise ValueError(_("不支持的浏览器选项, 输入f2 dy --help查看更多帮助!"))
-
-    cj = cj_function(domain_name="douyin.com")
-
-    # cookie_value = next((c.value for c in cj if c.name == 'ttwid'), None)
-    cookie_value = {c.name: c.value for c in cj if c.domain.endswith("douyin.com")}
-
-    if not cookie_value:
-        raise ValueError(_("无法从 {0} 浏览器中获取cookie").format(browser_choice))
-
-    return cookie_value
+        # 如果没有提供配置文件，那么使用高频配置文件
+        manager = ConfigManager(
+            ctx.params.get("config", get_resource_path(f2.APP_CONFIG_FILE_PATH))
+        )
+        manager.update_config_with_args("douyin", cookie=cookie_value)
+    except PermissionError:
+        logger.error(_("请关闭所有已打开的浏览器重试，并且你有适当的权限访问浏览器！"))
+        ctx.abort()
+    except Exception as e:
+        logger.error(_("自动获取Cookie失败：{0}").format(str(e)))
+        ctx.abort()
 
 
 def handler_language(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> typing.Any:
-    """用于设置语言 (For setting the language)"""
+    """用于设置语言 (For setting the language)
 
+    Args:
+        ctx: click的上下文对象 (Click's context object)
+        param: 提供的参数或选项 (The provided parameter or option)
+        value: 参数或选项的值 (The value of the parameter or option)
+    """
+
+    if not value or ctx.resilient_parsing:
+        return
     TranslationManager.get_instance().set_language(value)
     global _
     _ = TranslationManager.get_instance().gettext
     return value
 
 
 def handler_naming(
@@ -138,50 +118,28 @@
     Raises:
         click.BadParameter: 如果命名模式无效 (If the naming pattern is invalid)
 
     Returns:
         value: 命名模式模板 (Naming pattern template)
     """
     # 避免和配置文件参数冲突
-    if value is None:
+    if not value or ctx.resilient_parsing:
         return
 
     # 允许的模式和分隔符
-    ALLOWED_PATTERNS = ["{nickname}", "{create}", "{aid}", "{desc}"]
+    ALLOWED_PATTERNS = ["{nickname}", "{create}", "{aweme_id}", "{desc}", "{uid}"]
     ALLOWED_SEPARATORS = ["-", "_"]
 
-    temp_naming = value
-    invalid_patterns = []
-
-    # 检查提供的模式是否有效
-    for pattern in ALLOWED_PATTERNS:
-        if pattern in temp_naming:
-            temp_naming = temp_naming.replace(pattern, "")
-
-    # 此时，temp_naming应只包含分隔符
-    for char in temp_naming:
-        if char not in ALLOWED_SEPARATORS:
-            invalid_patterns.append(char)
-
-    # 检查连续的无效模式或分隔符
-    for pattern in ALLOWED_PATTERNS:
-        # 检查像"{aid}{aid}"这样的模式
-        if pattern + pattern in value:
-            invalid_patterns.append(pattern + pattern)
-        for sep in ALLOWED_SEPARATORS:
-            # 检查像"{aid}-{aid}"这样的模式
-            if pattern + sep + pattern in value:
-                invalid_patterns.append(pattern + sep + pattern)
+    # 检查命名是否符合命名规范
+    invalid_patterns = check_invalid_naming(value, ALLOWED_PATTERNS, ALLOWED_SEPARATORS)
 
     if invalid_patterns:
         raise click.BadParameter(
-            _(
-                "`{0}` 中的 `{1}` 不符合命名模式".format(
-                    value, "".join(invalid_patterns)
-                )
+            _("`{0}` 中的 `{1}` 不符合命名模式").format(
+                value, "".join(invalid_patterns)
             )
         )
 
     return value
 
 
 def handler_sso_login(
@@ -215,43 +173,14 @@
             ctx.params.get("config", get_resource_path(f2.APP_CONFIG_FILE_PATH))
         )
         manager.update_config_with_args("douyin", cookie=login_cookie)
     else:
         raise click.UsageError(_("SSO登录失败，请重试！"))
 
 
-def merge_config(main_conf, custom_conf, **kwargs):
-    """
-    合并配置参数，使 CLI 参数优先级高于自定义配置，自定义配置优先级高于主配置，最终生成完整配置参数字典。
-    Args:
-        main_conf (dict): 主配置参数字典
-        custom_conf (dict): 自定义配置参数字典
-        **kwargs: CLI 参数和其他额外的配置参数
-
-    Returns:
-        dict: 合并后的配置参数字典
-    """
-    # 合并主配置和自定义配置
-    merged_conf = {}
-    for key, value in main_conf.items():
-        merged_conf[key] = value  # 将主配置复制到合并后的配置中
-    for key, value in custom_conf.items():
-        if value is not None and value != "":  # 只有值不为 None 和 空值，才进行合并
-            merged_conf[key] = value  # 自定义配置参数会覆盖主配置中的同名参数
-
-    # 合并 CLI 参数与合并后的配置，确保 CLI 参数的优先级最高
-    for key, value in kwargs.items():
-        if key not in merged_conf:  # 如果合并后的配置中没有这个键，则直接添加
-            merged_conf[key] = value
-        elif value is not None and value != "":  # 如果值不为 None 和 空值，则进行合并
-            merged_conf[key] = value  # CLI 参数会覆盖自定义配置和主配置中的同名参数
-
-    return merged_conf
-
-
 @click.command(name="douyin", help=_("抖音无水印解析"))
 @click.option(
     "--config",
     "-c",
     type=click.Path(file_okay=True, dir_okay=False, readable=True),  # exists=True
     help=_("配置文件的路径，最低优先"),
 )
@@ -265,52 +194,52 @@
     ),
 )
 @click.option(
     "--music",
     "-m",
     type=bool,
     # default="yes",
-    help=_("是否保存视频原声。可选：'yes'、'no'"),
+    help=_("是否保存视频原声"),
 )
 @click.option(
     "--cover",
     "-v",
     type=bool,
     # default="yes",
-    help=_("是否保存视频封面。可选：'yes'、'no'"),
+    help=_("是否保存视频封面"),
 )
 @click.option(
     "--desc",
     "-d",
     type=bool,
     # default="yes",
-    help=_("是否保存视频文案。可选：'yes'、'no'"),
+    help=_("是否保存视频文案"),
 )
 @click.option(
     "--path",
     "-p",
     type=str,
     # default="Download",
-    help=_("作品保存位置，支持绝对与相对路径。"),
+    help=_("作品保存位置，支持绝对与相对路径"),
 )
 @click.option(
     "--folderize",
     "-f",
     type=bool,
     # default="yes",
-    help=_("是否将作品保存到单独的文件夹。可选：'yes'、'no'"),
+    help=_("是否将作品保存到单独的文件夹"),
 )
 @click.option(
     "--mode",
     "-M",
-    type=click.Choice(["one", "post", "like", "collect", "mix", "live"]),
+    type=click.Choice(f2.DOUYIN_MODE_LIST),
     # default="post",
     # required=True,
     help=_(
-        "下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collect)，合辑(mix)，直播(live)"
+        "下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collection)，收藏夹作品(collects)，收藏音乐(music)，合辑(mix)，直播(live)"
     ),
 )
 @click.option(
     "--naming",
     "-n",
     type=str,
     # default="{create}_{desc}",
@@ -332,102 +261,107 @@
     help=_("下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"),
 )
 @click.option(
     "--timeout",
     "-e",
     type=int,
     # default=10,
-    help=_("网络请求超时时间。"),
+    help=_("网络请求超时时间"),
 )
 @click.option(
     "--max_retries",
     "-r",
     type=int,
     # default=5,
-    help=_("网络请求超时重试数。"),
+    help=_("网络请求超时重试数"),
 )
 @click.option(
     "--max-connections",
     "-x",
     type=int,
     # default=5,
-    help=_("网络请求并发连接数。"),
+    help=_("网络请求并发连接数"),
 )
 @click.option(
     "--max-tasks",
     "-t",
     type=int,
     # default=10,
-    help=_("异步的任务数。"),
+    help=_("异步的任务数"),
 )
 @click.option(
     "--max-counts",
     "-o",
     type=int,
     # default=0,
     help=_("最大作品下载数。0 表示无限制"),
 )
 @click.option(
     "--page-counts",
     "-s",
     type=int,
     # default=20,
-    help=_("从接口每页可获取作品数，不建议超过20。"),
+    help=_("从接口每页可获取作品数，不建议超过20"),
 )
 @click.option(
     "--languages",
     "-l",
     type=click.Choice(["zh_CN", "en_US"]),
     default="zh_CN",
-    help=_("显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'。不支持配置文件修改。"),
+    help=_("显示语言。默认为 'zh_CN'，可选：'zh_CN'、'en_US'，不支持配置文件修改"),
     callback=handler_language,
 )
 @click.option(
     "--proxies",
     "-P",
     type=str,
     nargs=2,
     help=_(
         "代理服务器，最多 2 个参数，http与https。空格区分 2 个参数 http://x.x.x.x https://x.x.x.x"
     ),
 )
+@click.option("--lyric", "-L", type=bool, help=_("是否保存原声歌词"))
 @click.option(
     "--update-config",
     type=bool,
     is_flag=True,
     help=_("使用命令行选项更新配置文件。需要先使用'-c'选项提供一个配置文件路径"),
 )
 @click.option(
     "--init-config", type=str, help=_("初始化配置文件。不能同时初始化和更新配置文件")
 )
 @click.option(
     "--auto-cookie",
-    type=click.Choice(["none", "chrome", "firefox", "edge", "opera"]),
+    type=click.Choice(f2.BROWSER_LIST),
     # default="none",
-    help=_(
-        "自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、opera。使用该命令前请确保关闭所选的浏览器"
-    ),
+    help=_("自动从浏览器获取cookie，使用该命令前请确保关闭所选的浏览器"),
     callback=handler_auto_cookie,
 )
 @click.option(
     "--sso-login",
     is_flag=True,
-    help=_("使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"),
+    help=_("使用SSO扫码登录获取cookie，保存低频主配置文件"),
     callback=handler_sso_login,
 )
 @click.option(
     "-h",
     is_flag=True,
     is_eager=True,
     expose_value=False,
     help=_("显示富文本帮助"),
-    callback=handle_help,
+    callback=handler_help,
 )
 @click.pass_context
-def douyin(ctx, config, init_config, update_config, **kwargs):
+def douyin(
+    ctx: click.Context,
+    config: str,
+    init_config: str,
+    update_config: bool,
+    **kwargs,
+):
     ##################
     # f2 存在2个主配置文件，分别是app低频配置(app.yaml)和f2低频配置(conf.yaml)
     # app低频配置存放app相关的参数
     # f2低频配置存放计算值所需的参数
 
     # 其中cli参数具有最高优先，cli >= 自定义 >= 低频
     # 在f2低频配置中设置代理参数
@@ -463,15 +397,15 @@
         main_manager.generate_config("douyin", init_config)
         # return
     elif init_config:
         raise click.UsageError(_("不能同时初始化和更新配置文件"))
     # 如果没有初始化配置文件，但是更新配置文件，则需要提供配置文件路径
     elif update_config and not config:
         raise click.UsageError(
-            _("要更新配置, 首先需要使用'-c'选项提供一个自定义配置文件路径")
+            _("要更新配置，首先需要使用'-c'选项提供一个自定义配置文件路径")
         )
 
     # 读取自定义配置文件
     if config:
         custom_manager = ConfigManager(config)
     else:
         custom_manager = main_manager
@@ -489,21 +423,21 @@
             "http": kwargs["proxies"][0],
             "https": kwargs["proxies"][1],
         }
 
     # 从低频配置开始到高频配置再到cli参数，逐级覆盖，如果键值不存在使用父级的键值
     kwargs = merge_config(main_conf, custom_conf, **kwargs)
 
-    logger.info(_("主配置路径： {0}".format(main_conf_path)))
-    logger.info(_("自定义配置路径： {0}".format(Path.cwd() / config)))
-    logger.debug(_("主配置参数：{0}".format(main_conf)))
-    logger.debug(_("自定义配置参数：{0}".format(custom_conf)))
-    logger.debug(_("CLI参数：{0}".format(kwargs)))
+    logger.info(_("主配置路径：{0}").format(main_conf_path))
+    logger.info(_("自定义配置路径：{0}").format(Path.cwd() / config))
+    logger.debug(_("主配置参数：{0}").format(main_conf))
+    logger.debug(_("自定义配置参数：{0}").format(custom_conf))
+    logger.debug(_("CLI参数：{0}").format(kwargs))
 
     # 尝试从命令行参数或kwargs中获取URL
     if not kwargs.get("url"):
         logger.error("缺乏URL参数，详情看命令帮助")
-        handle_help(ctx, None, True)
+        handler_help(ctx, None, True)
 
     # 添加app_name到kwargs
     kwargs["app_name"] = "douyin"
     ctx.invoke(set_cli_config, **kwargs)
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/crawler.py` & `f2-0.0.1.5/f2/apps/tiktok/crawler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# path: f2/apps/douyin/crawler.py
+# path: f2/apps/tiktok/crawler.py
 
 import f2
 
 from f2.log.logger import logger
 from f2.i18n.translator import _
 from f2.utils.conf_manager import ConfigManager
 from f2.crawlers.base_crawler import BaseCrawler
-from f2.apps.douyin.api import DouyinAPIEndpoints as dyendpoint
-from f2.apps.douyin.model import (
+from f2.apps.tiktok.api import TiktokAPIEndpoints as tkendpoint
+from f2.apps.tiktok.model import (
     UserProfile,
     UserPost,
     UserLike,
+    UserMix,
     UserCollect,
     PostDetail,
-    UserMix,
-    UserLive,
-    UserLive2,
-    FollowUserLive,
-    LoginGetQr,
-    LoginCheckQr,
+    UserPlayList,
+    PostComment,
 )
-from f2.apps.douyin.utils import XBogusManager
+from f2.apps.tiktok.utils import XBogusManager
 
 
-class DouyinCrawler(BaseCrawler):
-    def __init__(self, kwargs: dict = {}):
+class TiktokCrawler(BaseCrawler):
+    def __init__(
+        self,
+        kwargs: dict = ...,
+    ):
         f2_manager = ConfigManager(f2.F2_CONFIG_FILE_PATH)
-        f2_conf = f2_manager.get_config("f2").get("douyin")
+        f2_conf = f2_manager.get_config("f2").get("tiktok")
         proxies_conf = kwargs.get("proxies", {"http": None, "https": None})
         proxies = {
             "http://": proxies_conf.get("http", None),
             "https://": proxies_conf.get("https", None),
         }
 
         self.headers = {
@@ -39,142 +39,91 @@
             "Cookie": kwargs["cookie"],
         }
 
         super().__init__(proxies=proxies, crawler_headers=self.headers)
 
     async def fetch_user_profile(self, params: UserProfile):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.USER_DETAIL, params.dict()
-        )  # fmt: off
-        logger.debug(_("用户信息接口地址:" + endpoint))
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_DETAIL,
+            params.dict(),
+        )
+        logger.debug(_("用户信息接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
     async def fetch_user_post(self, params: UserPost):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.USER_POST, params.dict()
-        )  # fmt: off
-        logger.debug(_("主页作品接口地址:" + endpoint))
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_POST,
+            params.dict(),
+        )
+        logger.debug(_("主页作品接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
     async def fetch_user_like(self, params: UserLike):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.USER_FAVORITE_A, params.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_LIKE,
+            params.dict(),
         )
-        logger.debug(_("喜欢作品接口地址:" + endpoint))
+        logger.debug(_("喜欢作品接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
     async def fetch_user_collect(self, params: UserCollect):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.USER_COLLECTION, params.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_COLLECT,
+            params.dict(),
         )
-        logger.debug(_("收藏作品接口地址:" + endpoint))
-        return await self._fetch_post_json(endpoint, params.dict())
-
-    async def fetch_user_mix(self, params: UserMix):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.MIX_AWEME, params.dict()
-        )  # fmt: off
-        logger.debug(_("合集作品接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_post_detail(self, params: PostDetail):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.POST_DETAIL, params.dict()
-        )  # fmt: off
-        logger.debug(_("作品详情接口地址:" + endpoint))
+        logger.debug(_("收藏作品接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
-    async def fetch_post_comment(self, params: PostDetail):
+    async def fetch_user_play_list(self, params: UserPlayList):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.POST_COMMENT, params.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_PLAY_LIST,
+            params.dict(),
         )
-        logger.debug(_("作品评论接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_post_feed(self, params: PostDetail):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.TAB_FEED, params.dict()
-        )  # fmt: off
-        logger.debug(_("首页推荐作品接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_follow_feed(self, params: PostDetail):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.FOLLOW_FEED, params.dict()
-        )  # fmt: off
-        logger.debug(_("关注作品接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_friend_feed(self, params: PostDetail):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.FRIEND_FEED, params.dict()
-        )  # fmt: off
-        logger.debug(_("朋友作品接口地址:" + endpoint))
+        logger.debug(_("合辑列表接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
-    async def fetch_post_related(self, params: PostDetail):
+    async def fetch_user_mix(self, params: UserMix):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.POST_RELATED, params.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.USER_MIX,
+            params.dict(),
         )
-        logger.debug(_("相关推荐作品接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_live(self, params: UserLive):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.LIVE_INFO, params.dict()
-        )  # fmt: off
-        logger.debug(_("直播接口地址:" + endpoint))
+        logger.debug(_("合辑作品接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
-    async def fetch_live_room_id(self, params: UserLive2):
-        original_headers = self.aclient.headers.copy()
-        try:
-            # 避免invalid session
-            self.aclient.headers.update({"Cookie": ""})
-            endpoint = XBogusManager.model_2_endpoint(
-                dyendpoint.LIVE_INFO_ROOM_ID, params.dict()
-            )
-            logger.debug(_("直播接口地址（room_id）:" + endpoint))
-            return await self._fetch_get_json(endpoint)
-        finally:
-            self.aclient.headers = original_headers
-
-    async def fetch_follow_live(self, params: FollowUserLive):
+    async def fetch_post_detail(self, params: PostDetail):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.FOLLOW_USER_LIVE, params.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.AWEME_DETAIL,
+            params.dict(),
         )
-        logger.debug(_("关注用户直播接口地址:" + endpoint))
-        return await self._fetch_get_json(endpoint)
-
-    async def fetch_locate_post(self, params: UserPost):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.LOCATE_POST, params.dict()
-        )  # fmt: off
-        logger.debug(_("定位上一次作品接口地址:" + endpoint))
+        logger.debug(_("作品详情接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
-    async def fetch_login_qrcode(self, parms: LoginGetQr):
+    async def fetch_post_comment(self, params: PostComment):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.SSO_LOGIN_GET_QR, parms.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.POST_COMMENT,
+            params.dict(),
         )
-        logger.debug(_("SSO获取二维码接口地址:" + endpoint))
+        logger.debug(_("作品评论接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
-    async def fetch_check_qrcode(self, parms: LoginCheckQr):
-        endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.SSO_LOGIN_CHECK_QR, parms.dict()
-        )
-        logger.debug(_("SSO检查扫码状态接口地址:" + endpoint))
-        return await self._fetch_response(endpoint)
-
-    async def fetch_check_login(self, parms: LoginCheckQr):
+    async def fetch_post_recommend(self, params: PostDetail):
         endpoint = XBogusManager.model_2_endpoint(
-            dyendpoint.SSO_LOGIN_CHECK_LOGIN, parms.dict()
+            self.headers.get("User-Agent"),
+            tkendpoint.HOME_RECOMMEND,
+            params.dict(),
         )
-        logger.debug(_("SSO检查登录状态接口地址:" + endpoint))
+        logger.debug(_("首页推荐接口地址：{0}").format(endpoint))
         return await self._fetch_get_json(endpoint)
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/db.py` & `f2-0.0.1.5/f2/apps/douyin/db.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # path: f2/apps/douyin/db.py
 
-import aiosqlite
 from f2.db.base_db import BaseDB
 
 
 class AsyncUserDB(BaseDB):
     TABLE_NAME = "user_info_web"
 
     async def _create_table(self) -> None:
@@ -28,18 +27,20 @@
             "is_block BOOLEAN",
             "is_blocked BOOLEAN",
             "is_star BOOLEAN",
             "live_status INTEGER",
             "mix_count INTEGER",
             "mplatform_followers_count INTEGER",
             "nickname TEXT",
+            "nickname_raw TEXT",
             "room_id TEXT",
             "school_name TEXT",
             "short_id TEXT",
             "signature TEXT",
+            "signature_raw TEXT",
             "total_favorited INTEGER",
             "uid TEXT",
             "unique_id TEXT",
             "user_age INTEGER",
             "last_aweme_id TEXT",
         ]
 
@@ -73,15 +74,15 @@
         await self.execute(
             f"INSERT OR REPLACE INTO {self.TABLE_NAME} ({keys}) VALUES ({placeholders})",
             values,
         )
         # VALUES (?, {placeholders})', (kwargs.get('sec_user_id'), *values))
         await self.commit()
 
-    async def update_user_info(self, sec_user_id, **kwargs) -> None:
+    async def update_user_info(self, sec_user_id: str, **kwargs) -> None:
         """
         更新用户信息
 
         Args:
             sec_user_id (str): 用户唯一标识
             **kwargs: 用户的其他字段键值对
         """
@@ -143,25 +144,27 @@
         """
         await super()._create_table()
         fields = [
             "api_status_code TEXT",
             "aweme_id TEXT PRIMARY KEY",
             "aweme_type TEXT",
             "nickname TEXT",
+            "nickname_raw TEXT",
             "sec_user_id TEXT",
             "short_id TEXT",
             "uid TEXT",
             "unique_id TEXT",
             "can_comment TEXT",
             "can_forward TEXT",
             "can_share TEXT",
             "can_show_comment TEXT",
             "comment_gid TEXT",
             "create_time TEXT",
             "desc TEXT",
+            "desc_raw TEXT",
             "duration TEXT",
             "is_ads TEXT",
             "is_story TEXT",
             "is_top TEXT",
             "video_bit_rate JSON",
             "video_play_addr TEXT",
             "images JSON",
@@ -170,37 +173,43 @@
             "part_see TEXT",
             "private_status TEXT",
             "is_delete TEXT",
             "is_prohibited TEXT",
             "is_long_video TEXT",
             "media_type TEXT",
             "mix_desc TEXT",
+            "mix_desc_raw TEXT",
             "mix_create_time TEXT",
             "mix_id TEXT",
             "mix_name TEXT",
             "mix_pic_type TEXT",
             "mix_type TEXT",
             "mix_share_url TEXT",
             "mix_update_time TEXT",
             "is_commerce_music TEXT",
             "is_original TEXT",
             "is_original_sound TEXT",
             "is_pgc TEXT",
             "music_author TEXT",
+            "music_author_raw TEXT",
             "music_author_deleted TEXT",
             "music_duration TEXT",
             "music_id TEXT",
             "music_mid TEXT",
             "pgc_author TEXT",
+            "pgc_author_raw TEXT",
             "pgc_author_title TEXT",
+            "pgc_author_title_raw TEXT",
             "pgc_music_type TEXT",
             "music_status TEXT",
             "music_owner_handle TEXT",
+            "music_owner_handle_raw TEXT",
             "music_owner_id TEXT",
             "music_owner_nickname TEXT",
+            "music_owner_nickname_raw TEXT",
             "music_play_url TEXT",
             "position TEXT",
             "region TEXT",
             "seo_ocr_content TEXT",
             "allow_douplus TEXT",
             "download_setting TEXT",
             "allow_share TEXT",
@@ -251,37 +260,34 @@
         """
         批量添加视频信息
 
         Args:
             video_data_list (list): 视频信息列表
             ignore_fields (list): 要忽略的字段列表，例如 ["field1", "field2"]
         """
-        try:
-            # 如果 ignore_fields 未提供或者为 None，将其设置为空列表
-            ignore_fields = ignore_fields or []
-
-            # 删除要忽略的字段
-            for field in ignore_fields:
-                for video_data in video_data_list:
-                    if field in video_data:
-                        del video_data[field]
+        # 如果 ignore_fields 未提供或者为 None，将其设置为空列表
+        ignore_fields = ignore_fields or []
 
-            keys = ", ".join(video_data_list[0].keys())
-            placeholders = ", ".join(["?" for _ in range(len(video_data_list[0]))])
+        # 删除要忽略的字段
+        for field in ignore_fields:
+            for video_data in video_data_list:
+                if field in video_data:
+                    del video_data[field]
 
-            # 构建插入数据的元组列表
-            values = [tuple(video_data.values()) for video_data in video_data_list]
+        keys = ", ".join(video_data_list[0].keys())
+        placeholders = ", ".join(["?" for _ in range(len(video_data_list[0]))])
 
-            await self.execute(
-                f"INSERT OR REPLACE INTO {self.TABLE_NAME} ({keys}) VALUES ({placeholders})",
-                values,
-            )
-            await self.commit()
-        except aiosqlite.Error as e:
-            print(f"Error batch inserting videos: {e}")
+        # 构建插入数据的元组列表
+        values = [tuple(video_data.values()) for video_data in video_data_list]
+
+        await self.execute(
+            f"INSERT OR REPLACE INTO {self.TABLE_NAME} ({keys}) VALUES ({placeholders})",
+            values,
+        )
+        await self.commit()
 
     async def get_video_info(self, aweme_id: str) -> dict:
         """
         获取特定视频的信息
 
         Args:
             aweme_id (str): 视频ID
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/dl.py` & `f2-0.0.1.5/f2/apps/tiktok/dl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# path: f2/apps/douyin/dl.py
+# path: f2/apps/tiktok/dl.py
 
 import sys
 from datetime import datetime
 from typing import Any, Union
 
 from f2.i18n.translator import _
 from f2.log.logger import logger
 from f2.dl.base_downloader import BaseDownloader
 from f2.utils.utils import get_timestamp, timestamp_2_str
-from f2.apps.douyin.db import AsyncUserDB
-from f2.apps.douyin.utils import format_file_name
+from f2.apps.tiktok.db import AsyncUserDB
+from f2.apps.tiktok.utils import format_file_name
 
 
-class DouyinDownloader(BaseDownloader):
+class TiktokDownloader(BaseDownloader):
     def __init__(self, kwargs: dict = {}):
         if kwargs["cookie"] is None:
             raise ValueError(
                 _(
-                    "cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取 f2 -d dy --help，如扫码登录请保留双引号cookie: "
-                    "，再使用--sso-login命令。"
+                    "cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取。如 `--auto-cookie edge`"
                 )
             )
 
         super().__init__(kwargs)
 
-    async def save_last_aweme_id(self, sec_user_id: str, aweme_id: int) -> None:
+    async def save_last_aweme_id(self, secUid: str, aweme_id: str) -> None:
         """
         保存最后一个请求的aweme_id
         (Save the last requested aweme_id)
 
         Args:
-            aweme_id (int): 作品id (aweme_id)
+            aweme_id (str): 作品id (aweme_id)
         """
 
-        async with AsyncUserDB("douyin_users.db") as db:
-            await db.update_user_info(sec_user_id=sec_user_id, last_aweme_id=aweme_id)
+        async with AsyncUserDB("tiktok_users.db") as db:
+            await db.update_user_info(secUid=secUid, last_aweme_id=aweme_id)
 
     async def filter_aweme_datas_by_interval(
         self, aweme_datas: Union[list, dict], interval: str
     ) -> Union[list[dict], dict, None]:
         """
         筛选指定日期区间内的作品
 
@@ -59,16 +58,18 @@
             start_date = datetime.strptime(start_str + " 00-00-00", "%Y-%m-%d %H-%M-%S")
             end_date = datetime.strptime(end_str + " 23-59-59", "%Y-%m-%d %H-%M-%S")
             logger.info(_("筛选日期区间：{0} 至 {1}").format(start_date, end_date))
         except ValueError:
             logger.error(_("日期区间参数格式错误，请查阅文档后重试"))
             return None
 
+        logger.info(aweme_datas)
+
         if isinstance(aweme_datas, dict):
-            aweme_date_str = aweme_datas.get("create_time")
+            aweme_date_str = aweme_datas.get("createTime")
             try:
                 aweme_date = datetime.strptime(aweme_date_str, "%Y-%m-%d %H-%M-%S")
             except ValueError:
                 logger.warning(_("无法解析作品发布时间：{0}").format(aweme_date_str))
                 return None
 
             # 检查作品发布时间是否在指定区间内
@@ -144,78 +145,84 @@
         self, kwargs: dict, aweme_data_dict: dict, user_path: Any
     ) -> None:
         """
         处理下载任务
 
         Args:
             kwargs (dict): 命令行参数
-            aweme_data_dict (dict): 作品数据字典
-            user_path (Any): 用户目录路径
         """
 
         # 构建文件夹路径
         base_path = (
             user_path
             / format_file_name(kwargs.get("naming", "{create}_{desc}"), aweme_data_dict)
             if kwargs.get("folderize")
             else user_path
         )
 
-        sec_user_id = str(aweme_data_dict.get("sec_user_id"))  # 用户ID
-        aweme_prohibited = aweme_data_dict.get("is_prohibited")  # 作品状态 0正常, 1屏蔽
-        aweme_part_see = aweme_data_dict.get(
-            "part_see"
-        )  # 部分可见 part_see 1, private_status 1
-        aweme_status = aweme_data_dict.get(
-            "private_status"
-        )  # 视频权限 0公开或不给谁看, 1私密, 2互关朋友
-        aweme_type = aweme_data_dict.get(
-            "aweme_type"
-        )  # 视频类型 0视频, 55动图或关闭下载, 61挑战， 109日常, 68图集
+        secUid = str(aweme_data_dict.get("secUid"))  # 用户ID
+        aweme_privateItem = aweme_data_dict.get(
+            "privateItem"
+        )  # 作品权限 false公开, true私密
+        aweme_secret = aweme_data_dict.get("secret")  # 作品权限 false公开, true私密
         aweme_id = str(aweme_data_dict.get("aweme_id"))  # 视频ID
 
         logger.debug(f"========{aweme_id}========")
         logger.debug(aweme_data_dict)
-        logger.debug("================")
+        logger.debug("===================================")
 
         # 检查作品是否被屏蔽
-        if aweme_prohibited:
-            logger.warning(_("{0} 该作品已被屏蔽，无法下载").format(aweme_id))
+        if aweme_privateItem:
+            logger.warning(_("该 {0} 作品已被屏蔽，无法下载").format(aweme_id))
             return
 
         # 检查作品是否可见
-        if aweme_status in [0, 1, 2]:
+        if not aweme_secret:
+            video_name = (
+                format_file_name(
+                    kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
+                )
+                + "_video"
+            )
+
+            video_url = aweme_data_dict.get("video_playAddr")
+            if video_url != None:
+                await self.initiate_download(
+                    _("视频"), video_url, base_path, video_name, ".mp4"
+                )
+            else:
+                logger.warning(_("{0} 该作品没有视频链接，无法下载").format(aweme_id))
+
             # 处理音乐下载任务
             if kwargs.get("music"):
-                if aweme_data_dict.get("music_status") == 1:  # 原声状态 1 正常 0 失效
-                    music_name = (
-                        format_file_name(
-                            kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
-                        )
-                        + "_music"
+                music_name = (
+                    format_file_name(
+                        kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
                     )
+                    + "_music"
+                )
 
-                    music_url = aweme_data_dict.get("music_play_url")
-                    if music_url != None:
-                        await self.initiate_download(
-                            _("原声"), music_url, base_path, music_name, ".mp3"
-                        )
+                music_url = aweme_data_dict.get("music_playUrl")
+                if music_url != None:
+                    await self.initiate_download(
+                        _("原声"), music_url, base_path, music_name, ".mp3"
+                    )
                 else:
                     logger.warning(_("{0} 该原声已被屏蔽，无法下载").format(aweme_id))
 
             # 处理封面下载任务
             if kwargs.get("cover"):
                 cover_name = (
                     format_file_name(
                         kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
                     )
                     + "_cover"
                 )
-                animated_cover_url = aweme_data_dict.get("animated_cover")
-                cover_url = aweme_data_dict.get("cover")
+                animated_cover_url = aweme_data_dict.get("video_dynamicCover")
+                cover_url = aweme_data_dict.get("video_cover")
                 if animated_cover_url != None:
                     await self.initiate_download(
                         _("封面"), animated_cover_url, base_path, cover_name, ".webp"
                     )
                 elif cover_url != None:
                     logger.warning(_("{0} 该作品没有动态封面").format(aweme_id))
                     await self.initiate_download(
@@ -233,58 +240,27 @@
                     + "_desc"
                 )
                 desc_content = aweme_data_dict.get("desc")
                 await self.initiate_static_download(
                     _("文案"), desc_content, base_path, desc_name, ".txt"
                 )
 
-            # 处理不同类型的作品下载任务
-            if aweme_type in [0, 55, 61, 109]:
-                video_name = (
-                    format_file_name(
-                        kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
-                    )
-                    + "_video"
-                )
-
-                video_url = aweme_data_dict.get("video_play_addr")
-                if video_url != None:
-                    await self.initiate_download(
-                        _("视频"), video_url, base_path, video_name, ".mp4"
-                    )
-                else:
-                    logger.warning(
-                        _("{0} 该作品没有视频链接，无法下载").format(aweme_id)
-                    )
-
-            elif aweme_type in [68]:
-                for i, image_url in enumerate(aweme_data_dict.get("images", None)):
-                    image_name = f"{format_file_name(kwargs.get('naming'), aweme_data_dict)}_image_{i + 1}"
-                    if image_url != None:
-                        await self.initiate_download(
-                            _("图集"), image_url, base_path, image_name, ".jpg"
-                        )
-                    else:
-                        logger.warning(
-                            _("{0} 该图集没有图片链接，无法下载").format(aweme_id)
-                        )
-
         # 保存最后一个aweme_id
-        await self.save_last_aweme_id(sec_user_id, aweme_id)
+        await self.save_last_aweme_id(secUid, aweme_id)
 
     async def create_stream_tasks(
         self, kwargs: dict, webcast_datas: Union[list, dict], user_path: Any
     ) -> None:
         """
         创建视频流下载任务
 
         Args:
             kwargs (dict): 命令行参数
             aweme_datas (list, dict): 作品数据列表或字典
-            user_path (Any): 用户目录路径
+            user_path (str): 用户目录路径
         """
 
         if (
             not kwargs
             or not webcast_datas
             or not isinstance(webcast_datas, (list, dict))
             or not user_path
@@ -304,16 +280,14 @@
         self, kwargs: dict, webcast_data_dict: dict, user_path: Any
     ) -> None:
         """
         处理视频流下载任务
 
         Args:
             kwargs (dict): 命令行参数
-            aweme_data_dict (dict): 直播数据字典
-            user_path (Any): 用户目录路径
         """
         custom_fields = {
             "create": timestamp_2_str(timestamp=get_timestamp(unit="sec")),
             "nickname": webcast_data_dict.get("nickname", ""),
             "aweme_id": webcast_data_dict.get("room_id", ""),
             "desc": webcast_data_dict.get("live_title", ""),
             "uid": webcast_data_dict.get("user_id", ""),
@@ -324,13 +298,13 @@
             / format_file_name(
                 kwargs.get("naming", "{create}_{desc}"), custom_fields=custom_fields
             )
             if kwargs.get("folderize")
             else user_path
         )
 
-        webcast_name = f"{format_file_name(kwargs.get('naming'), custom_fields=custom_fields)}_live"
-        webcast_url = webcast_data_dict.get("m3u8_pull_url").get("FULL_HD1")
+        webcast_name = f"{format_file_name(kwargs.get('naming', '{create}_{desc}'), custom_fields=custom_fields)}_live"
+        webcast_url = webcast_data_dict.get("m3u8_pull_url", None).get("FULL_HD1")
 
         await self.initiate_m3u8_download(
             _("直播"), webcast_url, base_path, webcast_name, ".mp4"
         )
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/filter.py` & `f2-0.0.1.5/f2/apps/douyin/filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# path: f2/apps/douyin/filter.py
+
 from f2.utils.json_filter import JSONModel
 from f2.utils.utils import _get_first_item_from_list, timestamp_2_str, replaceT
 
 # Filter
 
 
 class UserProfileFilter(JSONModel):
@@ -70,14 +72,18 @@
         return self._get_attr_value("$.user.mplatform_followers_count")
 
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.user.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.user.nickname")
+
+    @property
     def room_id(self):
         return self._get_attr_value("$.user.room_id")
 
     @property
     def school_name(self):
         return self._get_attr_value("$.user.school_name")
 
@@ -90,14 +96,18 @@
         return self._get_attr_value("$.user.short_id")
 
     @property
     def signature(self):
         return replaceT(self._get_attr_value("$.user.signature"))
 
     @property
+    def signature_raw(self):
+        return self._get_attr_value("$.user.signature")
+
+    @property
     def total_favorited(self):
         return self._get_attr_value("$.user.total_favorited")
 
     @property
     def uid(self):
         return self._get_attr_value("$.user.uid")
 
@@ -105,14 +115,17 @@
     def unique_id(self):
         return self._get_attr_value("$.user.unique_id")
 
     @property
     def user_age(self):
         return self._get_attr_value("$.user.user_age")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -137,69 +150,81 @@
     def aweme_type(self):
         return self._get_list_attr_value("$.aweme_list[*].aweme_type")
 
     @property
     def create_time(self):
         create_times = self._get_list_attr_value("$.aweme_list[*].create_time")
         return (
-            [timestamp_2_str(ct) for ct in create_times]
+            [timestamp_2_str(str(ct)) for ct in create_times]
             if isinstance(create_times, list)
-            else timestamp_2_str(create_times)
+            else timestamp_2_str(str(create_times))
         )
 
     @property
     def desc(self):
         return replaceT(self._get_list_attr_value("$.aweme_list[*].desc"))
 
     @property
+    def desc_raw(self):
+        return self._get_list_attr_value("$.aweme_list[*].desc")
+
+    @property
     def uid(self):
         return self._get_list_attr_value("$.aweme_list[*].author.uid")
 
     @property
     def sec_user_id(self):
         return self._get_list_attr_value("$.aweme_list[*].author.sec_uid")
 
     @property
     def nickname(self):
         return replaceT(self._get_list_attr_value("$.aweme_list[*].author.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_list_attr_value("$.aweme_list[*].author.nickname")
+
+    @property
     def author_avatar_thumb(self):
         return self._get_list_attr_value(
             "$.aweme_list[*].author.avatar_thumb.url_list[0]"
         )
 
     @property
     def images(self):
         images_list = self._get_list_attr_value("$.aweme_list[*].images")
 
         return [
-            [
-                img["url_list"][0]
-                for img in images
-                if isinstance(img, dict) and "url_list" in img and img["url_list"]
-            ]
-            if images
-            else None
+            (
+                [
+                    img["url_list"][0]
+                    for img in images
+                    if isinstance(img, dict) and "url_list" in img and img["url_list"]
+                ]
+                if images
+                else None
+            )
             for images in images_list
         ]
 
     @property
     def animated_cover(self):
         # 临时办法
         # https://github.com/h2non/jsonpath-ng/issues/82
 
         # 获取所有视频
         videos = self._get_list_attr_value("$.aweme_list[*].video")
 
         # 逐个视频判断是否存在animated_cover
         animated_covers = [
-            video.get("animated_cover", {}).get("url_list", [None])[0]
-            if video.get("animated_cover")
-            else None
+            (
+                video.get("animated_cover", {}).get("url_list", [None])[0]
+                if video.get("animated_cover")
+                else None
+            )
             for video in videos
         ]
 
         return animated_covers
 
     @property
     def cover(self):
@@ -212,19 +237,23 @@
         return self._get_list_attr_value("$.aweme_list[*].video.play_addr.url_list[0]")
 
     @property
     def video_bit_rate(self):
         bit_rate_data = self._get_list_attr_value("$.aweme_list[*].video.bit_rate")
 
         return [
-            [aweme["bit_rate"]]
-            if isinstance(aweme, dict)
-            else [aweme[0]["bit_rate"]]
-            if len(aweme) == 1
-            else [item["bit_rate"] for item in aweme]
+            (
+                [aweme["bit_rate"]]
+                if isinstance(aweme, dict)
+                else (
+                    [aweme[0]["bit_rate"]]
+                    if len(aweme) == 1
+                    else [item["bit_rate"] for item in aweme]
+                )
+            )
             for aweme in bit_rate_data
         ]
 
     @property
     def video_duration(self):
         return self._get_list_attr_value("$.aweme_list[*].video.duration")
 
@@ -252,14 +281,18 @@
         return self._get_list_attr_value("$.aweme_list[*].music.status")
 
     @property
     def music_title(self):
         return replaceT(self._get_list_attr_value("$.aweme_list[*].music.title"))
 
     @property
+    def music_title_raw(self):
+        return self._get_list_attr_value("$.aweme_list[*].music.title")
+
+    @property
     def music_play_url(self):
         url_list = self._get_list_attr_value("$.aweme_list[*].music.play_url.url_list")
         return _get_first_item_from_list(url_list)
 
     @property
     def has_more(self) -> bool:
         return bool(self._get_attr_value("$.has_more"))
@@ -268,14 +301,17 @@
     def max_cursor(self):
         return self._get_attr_value("$.max_cursor")
 
     @property
     def min_cursor(self):
         return self._get_attr_value("$.min_cursor")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -309,123 +345,715 @@
                 attr_values = getattr(self, key)
                 index = aweme_entries.index(entry)
                 d[key] = attr_values[index] if index < len(attr_values) else None
             list_dicts.append(d)
         return list_dicts
 
 
-class UserCollectFilter(UserPostFilter):
+class UserCollectionFilter(UserPostFilter):
     def __init__(self, data):
         super().__init__(data)
 
     @property
     def max_cursor(self):
         return self._get_attr_value("$.cursor")
 
 
+class UserCollectsFilter(JSONModel):
+
+    @property
+    def max_cursor(self):
+        return self._get_attr_value("$.cursor")
+
+    @property
+    def status_code(self):
+        return self._get_attr_value("$.status_code")
+
+    @property
+    def total_number(self):
+        return self._get_attr_value("$.total_number")
+
+    @property
+    def has_more(self):
+        return bool(self._get_attr_value("$.has_more"))
+
+    @property
+    def app_id(self):
+        return self._get_list_attr_value("$.collects_list[*].app_id")
+
+    @property
+    def collects_cover(self):
+        return self._get_list_attr_value(
+            "$.collects_list[*].collects_cover.url_list[0]"
+        )
+
+    @property
+    def collects_id(self):
+        return self._get_list_attr_value("$.collects_list[*].collects_id")
+
+    @property
+    def collects_name(self):
+        return replaceT(self._get_list_attr_value("$.collects_list[*].collects_name"))
+
+    @property
+    def collects_name_raw(self):
+        return self._get_list_attr_value("$.collects_list[*].collects_name")
+
+    @property
+    def create_time(self):
+        create_times = self._get_list_attr_value("$.collects_list[*].create_time")
+        return (
+            [timestamp_2_str(str(ct)) for ct in create_times]
+            if isinstance(create_times, list)
+            else timestamp_2_str(str(create_times))
+        )
+
+    @property
+    def follow_status(self):
+        return self._get_list_attr_value("$.collects_list[*].follow_status")
+
+    @property
+    def followed_count(self):
+        return self._get_list_attr_value("$.collects_list[*].followed_count")
+
+    @property
+    def is_normal_status(self):
+        return self._get_list_attr_value("$.collects_list[*].is_normal_status")
+
+    @property
+    def item_type(self):
+        return self._get_list_attr_value("$.collects_list[*].item_type")
+
+    @property
+    def last_collect_time(self):
+        create_times = self._get_list_attr_value("$.collects_list[*].last_collect_time")
+        return (
+            [timestamp_2_str(str(ct)) for ct in create_times]
+            if isinstance(create_times, list)
+            else timestamp_2_str(str(create_times))
+        )
+
+    @property
+    def play_count(self):
+        return self._get_list_attr_value("$.collects_list[*].play_count")
+
+    @property
+    def states(self):
+        return self._get_list_attr_value("$.collects_list[*].states")
+
+    @property
+    def status(self):
+        return self._get_list_attr_value("$.collects_list[*].status")
+
+    @property
+    def system_type(self):
+        return self._get_list_attr_value("$.collects_list[*].system_type")
+
+    @property
+    def total_number(self):
+        return self._get_list_attr_value("$.collects_list[*].total_number")
+
+    @property
+    def user_id(self):
+        return self._get_list_attr_value("$.collects_list[*].user_id")
+
+    # user_info
+    @property
+    def nickname(self):
+        return replaceT(
+            self._get_list_attr_value("$.collects_list[*].user_info.nickname")
+        )
+
+    @property
+    def nickname_raw(self):
+        return self._get_list_attr_value("$.collects_list[*].user_info.nickname")
+
+    @property
+    def uid(self):
+        return self._get_list_attr_value("$.collects_list[*].user_info.uid")
+
+    def _to_raw(self) -> dict:
+        return self._data
+
+    def _to_dict(self) -> dict:
+        return {
+            prop_name: getattr(self, prop_name)
+            for prop_name in dir(self)
+            if not prop_name.startswith("__") and not prop_name.startswith("_")
+        }
+
+
+class UserMusicCollectionFilter(JSONModel):
+
+    @property
+    def max_cursor(self):
+        return self._get_attr_value("$.cursor")
+
+    @property
+    def has_more(self):
+        return self._get_attr_value("$.has_more")
+
+    @property
+    def status_code(self):
+        return self._get_attr_value("$.status_code")
+
+    @property
+    def msg(self):
+        return self._get_attr_value("$.msg")
+
+    @property
+    def album(self):
+        return self._get_list_attr_value("$.mc_list[*].album")
+
+    @property
+    def audition_duration(self):
+        return self._get_list_attr_value("$.mc_list[*].audition_duration")
+
+    @property
+    def duration(self):
+        return self._get_list_attr_value("$.mc_list[*].duration")
+
+    @property
+    def author(self):
+        return replaceT(self._get_list_attr_value("$.mc_list[*].author"))
+
+    @property
+    def author_raw(self):
+        return self._get_list_attr_value("$.mc_list[*].author")
+
+    @property
+    def collect_status(self):
+        return self._get_list_attr_value("$.mc_list[*].collect_stat")
+
+    @property
+    def music_status(self):
+        return self._get_list_attr_value("$.mc_list[*].music_status")
+
+    @property
+    def cover_hd(self):
+        return self._get_list_attr_value("$.mc_list[*].cover_hd.url_list[0]")
+
+    @property
+    def music_id(self):
+        return self._get_list_attr_value("$.mc_list[*].id")
+
+    @property
+    def mid(self):
+        return self._get_list_attr_value("$.mc_list[*].mid")
+
+    @property
+    def is_commerce_music(self):
+        return self._get_list_attr_value("$.mc_list[*].is_commerce_music")
+
+    @property
+    def is_original(self):
+        return self._get_list_attr_value("$.mc_list[*].is_original")
+
+    @property
+    def is_original_sound(self):
+        return self._get_list_attr_value("$.mc_list[*].is_original_sound")
+
+    @property
+    def lyric_type(self):
+        return self._get_list_attr_value("$.mc_list[*].lyric_type")
+
+    @property
+    def lyric_url(self):
+        # 不是每个作品都有 lyric_url，如果不存在则为 None
+        lyric_urls = []
+        for item in self._data.get("mc_list"):
+            lyric_urls.append(item.get("lyric_url", None))
+
+        return lyric_urls
+
+    @property
+    def play_url(self):
+        return self._get_list_attr_value("$.mc_list[*].play_url.url_list[0]")
+
+    @property
+    def title(self):
+        return replaceT(self._get_list_attr_value("$.mc_list[*].title"))
+
+    @property
+    def title_raw(self):
+        return self._get_list_attr_value("$.mc_list[*].title")
+
+    @property
+    def strong_beat_url(self):
+        return self._get_list_attr_value("$.mc_list[*].strong_beat_url.url_list[0]")
+
+    @property
+    def owner_nickname(self):
+        return replaceT(self._get_list_attr_value("$.mc_list[*].owner_nickname"))
+
+    @property
+    def owner_nickname_raw(self):
+        return self._get_list_attr_value("$.mc_list[*].owner_nickname")
+
+    @property
+    def owner_id(self):
+        return self._get_list_attr_value("$.mc_list[*].owner_id")
+
+    @property
+    def sec_uid(self):
+        return self._get_list_attr_value("$.mc_list[*].sec_uid")
+
+    def _to_raw(self) -> dict:
+        return self._data
+
+    def _to_dict(self) -> dict:
+        return {
+            prop_name: getattr(self, prop_name)
+            for prop_name in dir(self)
+            if not prop_name.startswith("__") and not prop_name.startswith("_")
+        }
+
+    def _to_list(self):
+        exclude_list = ["has_more", "max_cursor", "status_code", "msg"]
+
+        keys = [
+            prop_name
+            for prop_name in dir(self)
+            if not prop_name.startswith("__")
+            and not prop_name.startswith("_")
+            and prop_name not in exclude_list
+        ]
+
+        aweme_entries = self._get_attr_value("$.mc_list") or []
+
+        list_dicts = []
+        for entry in aweme_entries:
+            d = {
+                "has_more": self.has_more,
+                "max_cursor": self.max_cursor,
+                "status_code": self.status_code,
+                "msg": self.msg,
+            }
+            for key in keys:
+                attr_values = getattr(self, key)
+                index = aweme_entries.index(entry)
+                d[key] = attr_values[index] if index < len(attr_values) else None
+            list_dicts.append(d)
+        return list_dicts
+
+
 class UserMixFilter(UserPostFilter):
     def __init__(self, data):
         super().__init__(data)
 
     @property
     def max_cursor(self):
         return self._get_attr_value("$.cursor")
 
 
 class UserLikeFilter(UserPostFilter):
     def __init__(self, data):
         super().__init__(data)
 
 
-class PostDetailFilter(JSONModel):
-    # api_status_code = property(lambda self: self._get_attr_value("$.status_code"))
-    # # author
-    # nickname = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.author.nickname")))
-    # sec_user_id = property(lambda self: self._get_attr_value("$.aweme_detail.author.sec_uid"))
-    # short_id = property(lambda self: self._get_attr_value("$.aweme_detail.author.short_id"))
-    # uid = property(lambda self: self._get_attr_value("$.aweme_detail.author.uid"))
-    # unique_id = property(lambda self: self._get_attr_value("$.aweme_detail.author.unique_id"))
-
-    # can_comment = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_control.can_comment"))
-    # can_forward = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_control.can_forward"))
-    # can_share = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_control.can_share"))
-    # can_show_comment = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_control.can_show_comment"))
-    # aweme_type = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_control.aweme_type"))
-    # aweme_id = property(lambda self: self._get_attr_value("$.aweme_detail.aweme_id"))
-    # comment_gid = property(lambda self: self._get_attr_value("$.aweme_detail.comment_gid"))
-    # create_time = property(lambda self: timestamp_2_str(self._get_attr_value("$.aweme_detail.create_time")))
-    # desc = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.desc")))
-    # duration = property(lambda self: self._get_attr_value("$.aweme_detail.duration"))
-    # is_ads = property(lambda self: self._get_attr_value("$.aweme_detail.is_ads"))
-    # is_story = property(lambda self: self._get_attr_value("$.aweme_detail.is_story"))
-    # is_top = property(lambda self: self._get_attr_value("$.aweme_detail.is_top"))
-    # video_bit_rate = property(lambda self: [
-    #     [aweme['bit_rate']] if isinstance(aweme, dict)
-    #     else [aweme[0]['bit_rate']] if len(aweme) == 1
-    #     else [item['bit_rate'] for item in aweme]
-    #     for aweme in self._get_list_attr_value("$.aweme_detail.video.bit_rate")
-    # ])
-    # video_play_addr = property(lambda self: self._get_attr_value("$.aweme_detail.video.play_addr.url_list[0]"))
-    # images = property(lambda self: [
-    #     [img['url_list'][0] for img in images if isinstance(img, dict) and 'url_list' in img and img['url_list']]
-    #     if images else None
-    #     for images in self._get_list_attr_value("$.aweme_detail.images")
-    # ])
-
-    # # aweme status
-    # is_delete = property(lambda self: self._get_attr_value("$.aweme_detail.status.is_delete"))
-    # is_prohibited = property(lambda self: self._get_attr_value("$.aweme_detail.status.is_prohibited"))
-
-    # is_long_video = property(lambda self: self._get_attr_value("$.aweme_detail.long_video"))
-    # media_type = property(lambda self: self._get_attr_value("$.aweme_detail.media_type"))
-    # # mix
-    # mix_desc = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.mix_info.mix_desc")))
-    # mix_create_time = property(lambda self: timestamp_2_str(self._get_attr_value("$.aweme_detail.mix_info.mix_create_time")))
-    # mix_id = property(lambda self: self._get_attr_value("$.aweme_detail.mix_info.mix_id"))
-    # mix_name = property(lambda self: self._get_attr_value("$.aweme_detail.mix_info.mix_name"))
-    # mix_pic_type = property(lambda self: self._get_attr_value("$.aweme_detail.mix_info.mix_pic_type"))
-    # mix_type = property(lambda self: self._get_attr_value("$.aweme_detail.mix_info.mix_type"))
-    # mix_share_url = property(lambda self: self._get_attr_value("$.aweme_detail.mix_info.mix_share_url"))
-    # mix_update_time = property(lambda self: timestamp_2_str(self._get_attr_value("$.aweme_detail.mix_info.mix_update_time")))
-    # # music
-    # is_commerce_music = property(lambda self: self._get_attr_value("$.aweme_detail.music.is_commerce_music"))
-    # is_original = property(lambda self: self._get_attr_value("$.aweme_detail.music.is_original"))
-    # is_original_sound = property(lambda self: self._get_attr_value("$.aweme_detail.music.is_original_sound"))
-    # is_pgc = property(lambda self: self._get_attr_value("$.aweme_detail.music.is_pgc"))
-    # music_author = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.music.author")))
-    # music_author_deleted = property(lambda self: self._get_attr_value("$.aweme_detail.music.author_deleted"))
-    # music_duration = property(lambda self: self._get_attr_value("$.aweme_detail.music.duration"))
-    # music_id = property(lambda self: self._get_attr_value("$.aweme_detail.music.id"))
-    # music_id_str = property(lambda self: self._get_attr_value("$.aweme_detail.music.id_str"))
-    # music_mid = property(lambda self: self._get_attr_value("$.aweme_detail.music.mid"))
-    # pgc_author = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.music.matched_pgc_sound.pgc_author")))
-    # pgc_author_title = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.music.matched_pgc_sound.pgc_author_title")))
-    # pgc_music_type = property(lambda self: self._get_attr_value("$.aweme_detail.music.matched_pgc_sound.pgc_music_type"))
-    # music_status = property(lambda self: self._get_attr_value("$.aweme_detail.music.status"))
-    # music_owner_handle = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.music.owner_handle")))
-    # music_owner_id = property(lambda self: self._get_attr_value("$.aweme_detail.music.owner_id"))
-    # music_owner_nickname = property(lambda self: replaceT(self._get_attr_value("$.aweme_detail.music.owner_nickname")))
-    # music_play_url = property(lambda self: self._get_attr_value("$.aweme_detail.music.play_url.url_list[0]"))
-
-    # # position
-    # position = property(lambda self: self._get_attr_value("$.aweme_detail.position"))
-    # # region = property(lambda self: self._get_attr_value("$.aweme_detail.region"))
-
-    # # seo_ocr_content
-    # seo_ocr_content = property(lambda self: self._get_attr_value("$.aweme_detail.seo_info.seo_ocr_content"))
-
-    # admire_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.admire_count"))
-    # collect_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.collect_count"))
-    # comment_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.comment_count"))
-    # digg_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.digg_count"))
-    # # play_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.play_count"))
-    # share_count = property(lambda self: self._get_attr_value("$.aweme_detail.statistics.share_count"))
+class UserFollowingFilter(JSONModel):
+
+    @property
+    def status_code(self):  # 1 正常，2096 用户隐私设置不允许查看
+        return self._get_attr_value("$.status_code")
+
+    @property
+    def status_msg(self):
+        return self._get_attr_value("$.status_msg")
+
+    @property
+    def has_more(self):
+        return self._get_attr_value("$.has_more")
+
+    @property
+    def total(self):
+        return self._get_attr_value("$.total")
+
+    @property
+    def mix_count(self):
+        return self._get_attr_value("$.mix_count")
+
+    @property
+    def offset(self):
+        return self._get_attr_value("$.offset")
+
+    @property
+    def myself_user_id(self):
+        return self._get_attr_value("$.myself_user_id")
+
+    @property
+    def max_time(self):
+        return self._get_attr_value("$.max_time")
+
+    @property
+    def min_time(self):
+        return self._get_attr_value("$.min_time")
+
+    # following_list
+    @property
+    def avatar_larger(self):
+        return self._get_list_attr_value("$.followings[*].avatar_larger.url_list[0]")
+
+    @property
+    def can_comment(self):
+        return self._get_list_attr_value("$.followings[*].aweme_control.can_comment")
+
+    @property
+    def can_forward(self):
+        return self._get_list_attr_value("$.followings[*].aweme_control.can_forward")
+
+    @property
+    def can_share(self):
+        return self._get_list_attr_value("$.followings[*].aweme_control.can_share")
+
+    @property
+    def can_show_comment(self):
+        return self._get_list_attr_value(
+            "$.followings[*].aweme_control.can_show_comment"
+        )
+
+    @property
+    def aweme_count(self):
+        return self._get_list_attr_value("$.followings[*].aweme_count")
+
+    @property
+    def back_cover(self):
+        return self._get_list_attr_value("$.followings[*].cover_url[0].url_list[0]")
+
+    @property
+    def register_time(self):
+        return self._get_list_attr_value("$.followings[*].create_time")
+
+    @property
+    def secondary_priority(self):
+        # secondary_priority 6 代表未看过的作品数量 1 代表正在直播 7 代表简介内容
+        return self._get_list_attr_value(
+            "$.followings[*].following_list_secondary_information_struct.secondary_information_priority"
+        )
+
+    @property
+    def secondary_text(self):
+        return replaceT(
+            self._get_list_attr_value(
+                "$.followings[*].following_list_secondary_information_struct.secondary_information_text"
+            )
+        )
+
+    @property
+    def secondary_text_raw(self):
+        return self._get_list_attr_value(
+            "$.followings[*].following_list_secondary_information_struct.secondary_information_text"
+        )
+
+    @property
+    def is_block(self):
+        return self._get_list_attr_value("$.followings[*].is_block")
+
+    @property
+    def is_blocked(self):
+        return self._get_list_attr_value("$.followings[*].is_blocked")
+
+    @property
+    def is_gov_media_vip(self):
+        return self._get_list_attr_value("$.followings[*].is_gov_media_vip")
 
-    # hashtag_ids = property(lambda self: self._get_list_attr_value("$.aweme_detail.text_extra[*].hashtag_id"))
-    # hashtag_names = property(lambda self: self._get_list_attr_value("$.aweme_detail.text_extra[*].hashtag_name"))
+    @property
+    def is_mix_user(self):
+        return self._get_list_attr_value("$.followings[*].is_mix_user")
+
+    @property
+    def is_phone_binded(self):
+        return self._get_list_attr_value("$.followings[*].is_phone_binded")
+
+    @property
+    def is_star(self):
+        return self._get_list_attr_value("$.followings[*].is_star")
+
+    @property
+    def is_top(self):
+        # 超粉?
+        return self._get_list_attr_value("$.followings[*].is_top")
+
+    @property
+    def is_verified(self):
+        # 实名?
+        return self._get_list_attr_value("$.followings[*].is_verified")
+
+    @property
+    def language(self):
+        return self._get_list_attr_value("$.followings[*].language")
+
+    @property
+    def nickname(self):
+        return replaceT(self._get_list_attr_value("$.followings[*].nickname"))
+
+    @property
+    def nickname_raw(self):
+        return self._get_list_attr_value("$.followings[*].nickname")
+
+    @property
+    def relation_label(self):
+        return self._get_list_attr_value("$.followings[*].relation_label")
+
+    @property
+    def room_id(self):
+        return self._get_list_attr_value("$.followings[*].room_id")
+
+    @property
+    def sec_uid(self):
+        return self._get_list_attr_value("$.followings[*].sec_uid")
+
+    @property
+    def secret(self):
+        # 私密?
+        return self._get_list_attr_value("$.followings[*].secret")
+
+    @property
+    def short_id(self):
+        return self._get_list_attr_value("$.followings[*].short_id")
+
+    @property
+    def signature(self):
+        return replaceT(self._get_list_attr_value("$.followings[*].signature"))
+
+    @property
+    def signature_raw(self):
+        return self._get_list_attr_value("$.followings[*].signature")
+
+    @property
+    def uid(self):
+        return self._get_list_attr_value("$.followings[*].uid")
+
+    @property
+    def unique_id(self):
+        return self._get_list_attr_value("$.followings[*].unique_id")
+
+    def _to_raw(self) -> dict:
+        return self._data
+
+    def _to_dict(self) -> dict:
+        return {
+            prop_name: getattr(self, prop_name)
+            for prop_name in dir(self)
+            if not prop_name.startswith("__") and not prop_name.startswith("_")
+        }
+
+    def _to_list(self):
+        exclude_list = [
+            "status_code",
+            "status_msg",
+            "has_more",
+            "total",
+            "mix_count",
+            "offset",
+            "myself_user_id",
+            "max_time",
+            "min_time",
+        ]
+
+        keys = [
+            prop_name
+            for prop_name in dir(self)
+            if not prop_name.startswith("__")
+            and not prop_name.startswith("_")
+            and prop_name not in exclude_list
+        ]
+
+        following_entries = self._get_attr_value("$.followings") or []
+
+        list_dicts = []
+        for entry in following_entries:
+            d = {
+                "has_more": self.has_more,
+                "total": self.total,
+                "mix_count": self.mix_count,
+                "offset": self.offset,
+                "myself_user_id": self.myself_user_id,
+                "max_time": self.max_time,
+                "min_time": self.min_time,
+            }
+            for key in keys:
+                attr_values = getattr(self, key)
+                index = following_entries.index(entry)
+                d[key] = attr_values[index] if index < len(attr_values) else None
+            list_dicts.append(d)
+        return list_dicts
+
+
+class UserFollowerFilter(UserFollowingFilter):
+    def __init__(self, data):
+        super().__init__(data)
+
+    @property
+    def total(self):
+        return self._get_attr_value("$.total")
+
+    # followers
+    @property
+    def avatar_larger(self):
+        return self._get_list_attr_value("$.followers[*].avatar_larger.url_list[0]")
+
+    @property
+    def can_comment(self):
+        return self._get_list_attr_value("$.followers[*].aweme_control.can_comment")
+
+    @property
+    def can_forward(self):
+        return self._get_list_attr_value("$.followers[*].aweme_control.can_forward")
+
+    @property
+    def can_share(self):
+        return self._get_list_attr_value(
+            "$.followersfollowers[*].aweme_control.can_share"
+        )
+
+    @property
+    def can_show_comment(self):
+        return self._get_list_attr_value(
+            "$.followers[*].aweme_control.can_show_comment"
+        )
+
+    @property
+    def aweme_count(self):
+        return self._get_list_attr_value("$.followers[*].aweme_count")
+
+    @property
+    def back_cover(self):
+        return self._get_list_attr_value("$.followers[*].cover_url[0].url_list[0]")
+
+    @property
+    def register_time(self):
+        return self._get_list_attr_value("$.followers[*].create_time")
+
+    @property
+    def is_block(self):
+        return self._get_list_attr_value("$.followers[*].is_block")
+
+    @property
+    def is_blocked(self):
+        return self._get_list_attr_value("$.followers[*].is_blocked")
+
+    @property
+    def is_gov_media_vip(self):
+        return self._get_list_attr_value("$.followers[*].is_gov_media_vip")
+
+    @property
+    def is_mix_user(self):
+        return self._get_list_attr_value("$.followers[*].is_mix_user")
+
+    @property
+    def is_phone_binded(self):
+        return self._get_list_attr_value("$.followers[*].is_phone_binded")
+
+    @property
+    def is_star(self):
+        return self._get_list_attr_value("$.followers[*].is_star")
+
+    @property
+    def is_top(self):
+        # 超粉?
+        return self._get_list_attr_value("$.followers[*].is_top")
+
+    @property
+    def is_verified(self):
+        # 实名?
+        return self._get_list_attr_value("$.followers[*].is_verified")
+
+    @property
+    def language(self):
+        return self._get_list_attr_value("$.followers[*].language")
+
+    @property
+    def nickname(self):
+        return replaceT(self._get_list_attr_value("$.followers[*].nickname"))
+
+    @property
+    def nickname_raw(self):
+        return self._get_list_attr_value("$.followers[*].nickname")
+
+    @property
+    def relation_label(self):
+        return self._get_list_attr_value("$.followers[*].relation_label")
+
+    @property
+    def room_id(self):
+        return self._get_list_attr_value("$.followers[*].room_id")
+
+    @property
+    def sec_uid(self):
+        return self._get_list_attr_value("$.followers[*].sec_uid")
+
+    @property
+    def secret(self):
+        # 私密?
+        return self._get_list_attr_value("$.followers[*].secret")
+
+    @property
+    def short_id(self):
+        return self._get_list_attr_value("$.followers[*].short_id")
+
+    @property
+    def signature(self):
+        return replaceT(self._get_list_attr_value("$.followers[*].signature"))
+
+    @property
+    def signature_raw(self):
+        return self._get_list_attr_value("$.followers[*].signature")
+
+    @property
+    def uid(self):
+        return self._get_list_attr_value("$.followers[*].uid")
+
+    @property
+    def unique_id(self):
+        return self._get_list_attr_value("$.followers[*].unique_id")
+
+    def _to_list(self):
+        exclude_list = [
+            "status_code",
+            "status_msg",
+            "has_more",
+            "total",
+            "mix_count",
+            "offset",
+            "myself_user_id",
+            "max_time",
+            "min_time",
+        ]
+
+        keys = [
+            prop_name
+            for prop_name in dir(self)
+            if not prop_name.startswith("__")
+            and not prop_name.startswith("_")
+            and prop_name not in exclude_list
+        ]
+
+        following_entries = self._get_attr_value("$.followers") or []
+
+        list_dicts = []
+        for entry in following_entries:
+            d = {
+                "has_more": self.has_more,
+                "total": self.total,
+                "mix_count": self.mix_count,
+                "offset": self.offset,
+                "myself_user_id": self.myself_user_id,
+                "max_time": self.max_time,
+                "min_time": self.min_time,
+            }
+            for key in keys:
+                attr_values = getattr(self, key)
+                index = following_entries.index(entry)
+                d[key] = attr_values[index] if index < len(attr_values) else None
+            list_dicts.append(d)
+        return list_dicts
+
+
+class PostDetailFilter(JSONModel):
 
     @property
     def api_status_code(self):
         return self._get_attr_value("$.status_code")
 
     @property
     def aweme_type(self):
@@ -437,14 +1065,18 @@
 
     # author
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.aweme_detail.author.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.aweme_detail.author.nickname")
+
+    @property
     def sec_user_id(self):
         return self._get_attr_value("$.aweme_detail.author.sec_uid")
 
     @property
     def short_id(self):
         return self._get_attr_value("$.aweme_detail.author.short_id")
 
@@ -483,14 +1115,18 @@
         return timestamp_2_str(str(self._get_attr_value("$.aweme_detail.create_time")))
 
     @property
     def desc(self):
         return replaceT(self._get_attr_value("$.aweme_detail.desc"))
 
     @property
+    def desc_raw(self):
+        return self._get_attr_value("$.aweme_detail.desc")
+
+    @property
     def duration(self):
         return self._get_attr_value("$.aweme_detail.duration")
 
     @property
     def is_ads(self):
         return self._get_attr_value("$.aweme_detail.is_ads")
 
@@ -530,14 +1166,18 @@
 
     # mix
     @property
     def mix_desc(self):
         return replaceT(self._get_attr_value("$.aweme_detail.mix_info.mix_desc"))
 
     @property
+    def mix_desc_raw(self):
+        return self._get_attr_value("$.aweme_detail.mix_info.mix_desc")
+
+    @property
     def mix_create_time(self):
         return timestamp_2_str(
             str(self._get_attr_value("$.aweme_detail.mix_info.mix_create_time"))
         )
 
     @property
     def mix_id(self):
@@ -583,14 +1223,18 @@
         return self._get_attr_value("$.aweme_detail.music.is_pgc")
 
     @property
     def music_author(self):
         return replaceT(self._get_attr_value("$.aweme_detail.music.author"))
 
     @property
+    def music_author_raw(self):
+        return self._get_attr_value("$.aweme_detail.music.author")
+
+    @property
     def music_author_deleted(self):
         return self._get_attr_value("$.aweme_detail.music.author_deleted")
 
     @property
     def music_duration(self):
         return self._get_attr_value("$.aweme_detail.music.duration")
 
@@ -605,44 +1249,62 @@
     @property
     def pgc_author(self):
         return replaceT(
             self._get_attr_value("$.aweme_detail.music.matched_pgc_sound.pgc_author")
         )
 
     @property
+    def pgc_author_raw(self):
+        return self._get_attr_value("$.aweme_detail.music.matched_pgc_sound.pgc_author")
+
+    @property
     def pgc_author_title(self):
         return replaceT(
             self._get_attr_value(
                 "$.aweme_detail.music.matched_pgc_sound.pgc_author_title"
             )
         )
 
     @property
+    def pgc_author_title_raw(self):
+        return self._get_attr_value(
+            "$.aweme_detail.music.matched_pgc_sound.pgc_author_title"
+        )
+
+    @property
     def pgc_music_type(self):
         return self._get_attr_value(
             "$.aweme_detail.music.matched_pgc_sound.pgc_music_type"
         )
 
     @property
     def music_status(self):
         return self._get_attr_value("$.aweme_detail.music.status")
 
     @property
     def music_owner_handle(self):
         return replaceT(self._get_attr_value("$.aweme_detail.music.owner_handle"))
 
     @property
+    def music_owner_handle_raw(self):
+        return self._get_attr_value("$.aweme_detail.music.owner_handle")
+
+    @property
     def music_owner_id(self):
         return self._get_attr_value("$.aweme_detail.music.owner_id")
 
     @property
     def music_owner_nickname(self):
         return replaceT(self._get_attr_value("$.aweme_detail.music.owner_nickname"))
 
     @property
+    def music_owner_nickname_raw(self):
+        return self._get_attr_value("$.aweme_detail.music.owner_nickname")
+
+    @property
     def music_play_url(self):
         return self._get_attr_value("$.aweme_detail.music.play_url.url_list[0]")
 
     # position
     @property
     def position(self):
         return self._get_attr_value("$.aweme_detail.position")
@@ -720,67 +1382,45 @@
     @property
     def video_bit_rate(self):
         bit_rate_data = self._get_list_attr_value(
             "$.aweme_detail.video.bit_rate",
         )
 
         return [
-            [aweme["bit_rate"]]
-            if isinstance(aweme, dict)
-            else [aweme[0]["bit_rate"]]
-            if len(aweme) == 1
-            else [item["bit_rate"] for item in aweme]
+            (
+                [aweme["bit_rate"]]
+                if isinstance(aweme, dict)
+                else (
+                    [aweme[0]["bit_rate"]]
+                    if len(aweme) == 1
+                    else [item["bit_rate"] for item in aweme]
+                )
+            )
             for aweme in bit_rate_data
         ]
 
     @property
     def video_play_addr(self):
-        return self._get_attr_value("$.aweme_detail.video.play_addr.url_list[0]")
+        return self._get_attr_value("$.aweme_detail.video.play_addr.url_list")
 
     # images
     @property
     def images(self):
         return self._get_list_attr_value("$.aweme_detail.images[*].url_list[0]")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
-    def _to_list(self):
-        # 不需要的属性列表
-        exclude_list = ["has_more", "max_cursor", "min_cursor"]
-        # 生成属性名称列表，然后过滤掉不需要的属性
-        keys = [
-            prop_name
-            for prop_name in dir(self)
-            if not prop_name.startswith("__")
-            and not prop_name.startswith("_")
-            and prop_name not in exclude_list
-        ]
-
-        aweme_entries = self._get_attr_value("$.aweme_detail") or []
-
-        list_dicts = []
-        # 遍历每个条目并创建一个字典
-        # (Iterate through each entry and create a dict)
-        for entry in aweme_entries:
-            d = {}
-            for key in keys:
-                attr_values = getattr(self, key)
-                # 当前aweme_entry在属性列表中的索引
-                index = aweme_entries.index(entry)
-                # 如果属性值的长度足够则赋值，否则赋None
-                # (Assign value if the length of the attribute value is sufficient, otherwise assign None)
-                d[key] = attr_values[index] if index < len(attr_values) else None
-            list_dicts.append(d)
-        return list_dicts
-
 
 class UserLiveFilter(JSONModel):
     # live
     @property
     def api_status_code(self):
         return self._get_attr_value("$.status_code")
 
@@ -793,14 +1433,18 @@
         return self._get_attr_value("$.data.data[0].status")
 
     @property
     def live_title(self):
         return replaceT(self._get_attr_value("$.data.data[0].title"))
 
     @property
+    def live_title_raw(self):
+        return self._get_attr_value("$.data.data[0].title")
+
+    @property
     def cover(self):
         return self._get_attr_value("$.data.data[0].cover.url_list[0]")
 
     @property
     def user_count(self):
         return self._get_attr_value("$.data.data[0].stats.user_count_str")
 
@@ -830,14 +1474,18 @@
         return self._get_attr_value("$.data.data[0].owner.sec_uid")
 
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.data.data[0].owner.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.data.data[0].owner.nickname")
+
+    @property
     def avatar_thumb(self):
         return self._get_attr_value("$.data.data[0].owner.avatar_thumb.url_list[0]")
 
     @property
     def follow_status(self):
         return self._get_attr_value("$.data.data[0].owner.follow_info.follow_status")
 
@@ -877,50 +1525,24 @@
     def DiggAuth(self):
         return self._get_attr_value("$.data.data[0].room_auth.Digg")
 
     @property
     def ShareAuth(self):
         return self._get_attr_value("$.data.data[0].room_auth.Share")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
-    def _to_list(self):
-        # 不需要的属性列表
-        exclude_list = []
-        # 生成属性名称列表，然后过滤掉不需要的属性
-        keys = [
-            prop_name
-            for prop_name in dir(self)
-            if not prop_name.startswith("__")
-            and not prop_name.startswith("_")
-            and prop_name not in exclude_list
-        ]
-
-        aweme_entries = self._get_attr_value("$.aweme_list") or []
-
-        list_dicts = []
-        # 遍历每个条目并创建一个字典
-        # (Iterate through each entry and create a dict)
-        for entry in aweme_entries:
-            d = {}
-            for key in keys:
-                attr_values = getattr(self, key)
-                # 当前aweme_entry在属性列表中的索引
-                index = aweme_entries.index(entry)
-                # 如果属性值的长度足够则赋值，否则赋None
-                # (Assign value if the length of the attribute value is sufficient, otherwise assign None)
-                d[key] = attr_values[index] if index < len(attr_values) else None
-            list_dicts.append(d)
-        return list_dicts
-
 
 class UserLive2Filter(JSONModel):
     # live
     @property
     def api_status_code(self):
         return self._get_attr_value("$.status_code")
 
@@ -937,24 +1559,28 @@
         return self._get_attr_value("$.data.room.status")
 
     @property
     def live_title(self):
         return replaceT(self._get_attr_value("$.data.room.title"))
 
     @property
+    def live_title_raw(self):
+        return self._get_attr_value("$.data.room.title")
+
+    @property
     def user_count(self):
         return self._get_attr_value("$.data.room.user_count")
 
     @property
     def create_time(self):
-        return timestamp_2_str(self._get_attr_value("$.data.room.create_time"))
+        return timestamp_2_str(str(self._get_attr_value("$.data.room.create_time")))
 
     @property
     def finish_time(self):
-        return timestamp_2_str(self._get_attr_value("$.data.room.finish_time"))
+        return timestamp_2_str(str(self._get_attr_value("$.data.room.finish_time")))
 
     @property
     def cover(self):
         return self._get_attr_value("$.data.room.cover.url_list[0]")
 
     @property
     def stream_id(self):
@@ -974,22 +1600,34 @@
 
     # user
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.data.room.owner.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.data.room.owner.nickname")
+
+    @property
     def gender(self):
         return replaceT(self._get_attr_value("$.data.room.owner.gender"))
 
     @property
+    def gender_raw(self):
+        return self._get_attr_value("$.data.room.owner.gender")
+
+    @property
     def signature(self):
         return replaceT(self._get_attr_value("$.data.room.owner.signature"))
 
     @property
+    def signature_raw(self):
+        return self._get_attr_value("$.data.room.owner.signature")
+
+    @property
     def avatar_large(self):
         return self._get_attr_value("$.data.room.owner.avatar_large.url_list[0]")
 
     @property
     def verified(self):
         return self._get_attr_value("$.data.room.owner.verified")
 
@@ -1005,14 +1643,17 @@
     def follower_count(self):
         return self._get_attr_value("$.data.room.owner.follow_info.follower_count")
 
     @property
     def sec_uid(self):
         return self._get_attr_value("$.data.room.owner.sec_uid")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -1070,14 +1711,17 @@
     def error_code(self):
         return self._get_attr_value("$.error_code")
 
     @property
     def message(self):
         return self._get_attr_value("$.message")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -1107,13 +1751,16 @@
     def message(self):
         return self._get_attr_value("$.message")
 
     @property
     def verify_ticket(self):
         return self._get_attr_value("$.verify_ticket")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/handler.py` & `f2-0.0.1.5/f2/apps/tiktok/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,925 +1,695 @@
-# path: f2/apps/douyin/handler.py
+# path: f2/apps/tiktok/handler.py
 
-import asyncio
-from typing import AsyncGenerator, Dict, Any, List
+import sys
+
+from pathlib import Path
+from typing import AsyncGenerator, Union, List, Any
 
-from f2.log.logger import logger
 from f2.i18n.translator import _
+from f2.log.logger import logger
 from f2.utils.mode_handler import mode_handler, mode_function_map
-from f2.utils.utils import split_set_cookie
-from f2.apps.douyin.db import AsyncUserDB, AsyncVideoDB
-from f2.apps.douyin.crawler import DouyinCrawler
-from f2.apps.douyin.dl import DouyinDownloader
-from f2.apps.douyin.model import (
-    UserPost,
+from f2.apps.tiktok.db import AsyncUserDB, AsyncVideoDB
+from f2.apps.tiktok.crawler import TiktokCrawler
+from f2.apps.tiktok.dl import TiktokDownloader
+from f2.apps.tiktok.model import (
     UserProfile,
+    UserPost,
     UserLike,
     UserCollect,
     UserMix,
+    UserPlayList,
     PostDetail,
-    UserLive,
-    UserLive2,
-    LoginGetQr,
-    LoginCheckQr,
 )
-from f2.apps.douyin.filter import (
-    UserPostFilter,
+from f2.apps.tiktok.filter import (
     UserProfileFilter,
-    UserCollectFilter,
-    UserMixFilter,
+    UserPostFilter,
     PostDetailFilter,
-    UserLiveFilter,
-    UserLive2Filter,
-    GetQrcodeFilter,
-    CheckQrcodeFilter,
+    UserMixFilter,
+    UserPlayListFilter,
 )
-from f2.apps.douyin.utils import (
+from f2.apps.tiktok.utils import (
     SecUserIdFetcher,
     AwemeIdFetcher,
-    WebCastIdFetcher,
-    VerifyFpManager,
     create_or_rename_user_folder,
-    show_qrcode,
 )
 from f2.cli.cli_console import RichConsoleManager
+from f2.exceptions.api_exceptions import APIResponseError
 
 rich_console = RichConsoleManager().rich_console
 rich_prompt = RichConsoleManager().rich_prompt
 
 
-class DouyinHandler:
+class TiktokHandler:
 
     # 需要忽略的字段（需过滤掉有时效性的字段）
     ignore_fields = ["video_play_addr", "images", "video_bit_rate", "cover"]
 
-    def __init__(self, kwargs) -> None:
+    def __init__(self, kwargs: dict = ...) -> None:
         self.kwargs = kwargs
-        self.downloader = DouyinDownloader(kwargs)
+        self.downloader = TiktokDownloader(kwargs)
 
-    async def handler_user_profile(self, sec_user_id: str) -> UserProfileFilter:
+    async def handler_user_profile(
+        self,
+        secUid: str = "",
+        uniqueId: str = "",
+    ) -> UserProfileFilter:
         """
         用于获取指定用户的个人信息
         (Used to get personal info of specified users)
 
         Args:
-            sec_user_id: str: 用户ID (User ID)
+            secUid: str: 用户ID (User ID)
+            uniqueId: str: 用户唯一ID (User unique ID)
 
         Return:
             user: UserProfileFilter: 用户信息过滤器 (User info filter)
         """
 
-        async with DouyinCrawler(self.kwargs) as crawler:
-            params = UserProfile(sec_user_id=sec_user_id)
+        if not secUid and not uniqueId:
+            raise ValueError(_("至少提供 secUid 或 uniqueId 中的一个参数"))
+
+        async with TiktokCrawler(self.kwargs) as crawler:
+            params = UserProfile(secUid=secUid, uniqueId=uniqueId)
             response = await crawler.fetch_user_profile(params)
+            user = UserProfileFilter(response)
+            if user.nickname is None:
+                raise APIResponseError(_("API内容请求失败，请更换新cookie后再试"))
             return UserProfileFilter(response)
 
-    async def get_user_nickname(self, sec_user_id: str, db: AsyncUserDB) -> str:
+    async def get_user_nickname(
+        self,
+        secUid: str,
+        db: AsyncUserDB,
+    ) -> str:
         """
-        获取指定用户的昵称，如果不存在，则从服务器获取并存储到数据库中
-        (Used to get personal info of specified users)
+        用于获取指定用户的昵称
+        (Used to get nickname of specified users)
 
         Args:
-            sec_user_id (str): 用户ID (User ID)
-            db (AsyncUserDB): 用户数据库 (User database)
+            secUid: str: 用户ID (User ID)
+            db: AsyncUserDB: 用户数据库 (User database)
 
-        Returns:
-            user_nickname: (str): 用户昵称 (User nickname)
+        Return:
+            nick_name: str: 用户昵称 (User nickname)
         """
 
-        user_dict = await db.get_user_info(sec_user_id)
+        user_dict = await db.get_user_info(secUid)
         if not user_dict:
-            user_dict = await self.handler_user_profile(sec_user_id)
+            user_dict = await self.handler_user_profile(secUid)
             await db.add_user_info(**user_dict._to_dict())
-        return user_dict.get("nickname")
+        return user_dict.get("nickname", "")
 
     async def get_or_add_user_data(
-        self, kwargs: dict, sec_user_id: str, db: AsyncUserDB
-    ) -> Any:
+        self,
+        secUid: str,
+        db: AsyncUserDB,
+    ) -> Path:
         """
         获取或创建用户数据同时创建用户目录
         (Get or create user data and create user directory)
 
         Args:
             kwargs (dict): 配置参数 (Conf parameters)
-            sec_user_id (str): 用户ID (User ID)
+            secUid (str): 用户ID (User ID)
             db (AsyncUserDB): 用户数据库 (User database)
 
         Returns:
             user_path (Path): 用户目录路径 (User directory path)
         """
 
         # 尝试从数据库中获取用户数据
-        local_user_data = await db.get_user_info(sec_user_id)
+        local_user_data = await db.get_user_info(secUid)
 
         # 从服务器获取当前用户最新数据
-        current_user_data = await self.handler_user_profile(sec_user_id)
+        current_user_data = await self.handler_user_profile(secUid)
 
         # 获取当前用户最新昵称
         current_nickname = current_user_data._to_dict().get("nickname")
 
         # 设置用户目录
         user_path = create_or_rename_user_folder(
-            kwargs, local_user_data, current_nickname
+            self.kwargs, local_user_data, current_nickname
         )
 
         # 如果用户不在数据库中，将其添加到数据库
         if not local_user_data:
             await db.add_user_info(**current_user_data._to_dict())
 
         return user_path
 
     @classmethod
     async def get_or_add_video_data(
-        cls, aweme_data: dict, db: AsyncVideoDB, ignore_fields: list = None
+        cls,
+        aweme_data: dict,
+        db: AsyncVideoDB,
+        ignore_fields: list = None,
     ):
         """
-        获取或创建作品数据库数据
+        获取或创建作品数据同时创建用户目录
         (Get or create user data and create user directory)
 
         Args:
             aweme_data (dict): 作品数据 (User data)
             db (AsyncVideoDB): 作品数据库 (User database)
             ignore_fields (list): 剔除的字段
         """
 
         # 尝试从数据库中获取作品数据
-        local_video_data = await db.get_video_info(aweme_data.get("aweme_id"))
+        local_video_data = await db.get_video_info(aweme_data.get("aweme_id", None))
 
         # 如果作品不在数据库中，将其添加到数据库
         if not local_video_data:
             # 从服务器获取当前作品最新数据
             # current_video_data = await fetch_one_video(aweme_data.get("aweme_id"))
             await db.add_video_info(ignore_fields=ignore_fields, **aweme_data)
 
+    async def fetch_play_list(
+        self,
+        secUid: str,
+        cursor: int,
+        page_counts: int,
+    ) -> UserPlayListFilter:
+        """
+        用于获取指定用户的作品合集列表
+        (Used to get video mix list of specified user)
+
+        Args:
+            secUid: str: 用户ID (User ID)
+            cursor: int: 分页游标 (Page cursor)
+            page_counts: int: 分页数量 (Page counts)
+
+        Return:
+            playlist: UserPlayListFilter: 作品合集列表 (Video mix list)
+        """
+
+        logger.debug(_("开始爬取用户：{0} 的作品合集列表").format(secUid))
+
+        async with TiktokCrawler(self.kwargs) as crawler:
+            params = UserPlayList(secUid=secUid, cursor=cursor, count=page_counts)
+            response = await crawler.fetch_user_play_list(params)
+            playlist = UserPlayListFilter(response)
+
+        if not playlist.hasPlayList:
+            logger.info(_("用户：{0} 没有作品合集").format(secUid))
+            return {}
+
+        logger.debug(_("当前请求的cursor：{0}").format(cursor))
+        logger.debug(
+            _("作品合集ID：{0} 作品合集标题：{1}").format(
+                playlist.mixId, playlist.mixName
+            )
+        )
+        logger.debug("===================================")
+        return playlist
+
+    async def select_playlist(
+        self, playlists: Union[dict, UserPlayListFilter]
+    ) -> Union[str, List[str]]:
+        """
+        用于选择要下载的作品合辑
+        (Used to select the video mix to download)
+
+        Args:
+            playlists: Union[dict, UserPlayListFilter]: 作品合辑列表 (Video mix list)
+
+        Return:
+            selected_index: Union[str, List[str]]: 选择的作品合辑序号 (Selected video mix index)
+        """
+
+        if playlists == {}:
+            sys.exit(_("用户没有作品合辑"))
+
+        rich_console.print("[bold]请选择要下载的合辑：[/bold]")
+        rich_console.print("0: [bold]全部下载[/bold]")
+
+        for i in range(len(playlists.mixId)):
+            rich_console.print(
+                _("{0}: {1} (包含 {2} 个作品，收藏夹ID {3})").format(
+                    i + 1,
+                    playlists.mixName[i],
+                    playlists.videoCount[i],
+                    playlists.mixId[i],
+                )
+            )
+
+        # rich_prompt 会有字符刷新问题，暂时使用rich_print
+        rich_console.print(_("[bold yellow]请输入希望下载的合辑序号：[/bold yellow]"))
+        selected_index = int(
+            rich_prompt.ask(
+                # _("[bold yellow]请输入希望下载的合辑序号:[/bold yellow]"),
+                choices=[str(i) for i in range(len(playlists) + 1)],
+            )
+        )
+
+        if selected_index == 0:
+            return playlists.mixId
+        else:
+            return playlists.mixId[selected_index - 1]
+
     @mode_handler("one")
-    async def handle_one_video(self):
+    async def handler_one_video(self):
         """
-        用于处理单个视频。
-        (Used to process a single video.)
+        用于获取指定作品的信息
+        (Used to get video info of specified video)
 
         Args:
             kwargs: dict: 参数字典 (Parameter dictionary)
         """
 
         aweme_id = await AwemeIdFetcher.get_aweme_id(self.kwargs.get("url"))
 
         aweme_data = await self.fetch_one_video(aweme_id)
 
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(
-                self.kwargs, aweme_data.get("sec_user_id"), db
+        async with AsyncUserDB("tiktok_users.db") as udb:
+            user_path = await self.get_or_add_user_data(aweme_data.secUid, udb)
+
+        async with AsyncVideoDB("tiktok_videos.db") as vdb:
+            await self.get_or_add_video_data(
+                aweme_data._to_dict(), vdb, self.ignore_fields
             )
 
-        async with AsyncVideoDB("douyin_videos.db") as db:
-            await self.get_or_add_video_data(aweme_data, db, self.ignore_fields)
+        logger.debug(_("单个作品数据：{0}").format(aweme_data._to_dict()))
 
-        logger.debug(_("单个视频数据: {0}".format(aweme_data)))
-        await self.downloader.create_download_tasks(self.kwargs, aweme_data, user_path)
+        # 创建下载任务
+        await self.downloader.create_download_tasks(
+            self.kwargs, aweme_data._to_dict(), user_path
+        )
 
-    async def fetch_one_video(self, aweme_id: str) -> dict:
+    async def fetch_one_video(self, itemId: str) -> PostDetailFilter:
         """
-        用于获取单个视频。
+        用于获取指定作品的详细信息
+        (Used to get detailed information of specified video)
 
         Args:
-            aweme_id: str: 视频ID
+            itemId: str: 作品ID (Video ID)
 
         Return:
-            video_data: dict: 视频数据字典，包含视频ID、视频文案、作者昵称
+            video: PostDetailFilter: 作品信息过滤器 (Video info filter)
         """
 
-        logger.debug(_("开始爬取视频: {0}").format(aweme_id))
-        async with DouyinCrawler(self.kwargs) as crawler:
-            params = PostDetail(aweme_id=aweme_id)
+        logger.debug(_("开始爬取作品：{0}").format(itemId))
+        async with TiktokCrawler(self.kwargs) as crawler:
+            params = PostDetail(itemId=itemId)
             response = await crawler.fetch_post_detail(params)
             video = PostDetailFilter(response)
 
         logger.debug(
-            _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
+            _("作品ID：{0} 作品文案：{1} 作者：{2}").format(
                 video.aweme_id, video.desc, video.nickname
             )
         )
 
-        return video._to_dict()
+        return video
 
     @mode_handler("post")
-    async def handle_user_post(self):
+    async def handler_user_post(self):
         """
-        用于处理用户发布的视频。
-        (Used to process videos published by users.)
+        用于获取指定用户的作品信息
+        (Used to get video info of specified user)
 
         Args:
             kwargs: dict: 参数字典 (Parameter dictionary)
         """
 
-        max_cursor = self.kwargs.get("max_cursor", 0)
-        page_counts = self.kwargs.get("page_counts", 20)
+        cursor = self.kwargs.get("cursor", 0)
+        page_counts = self.kwargs.get("page_counts", 35)
         max_counts = self.kwargs.get("max_counts")
 
-        # 获取用户数据并返回创建用户目录
-        sec_user_id = await SecUserIdFetcher.get_sec_user_id(self.kwargs.get("url"))
-        async with AsyncUserDB("douyin_users.db") as udb:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, udb)
+        secUid = await SecUserIdFetcher.get_secuid(self.kwargs.get("url"))
+
+        async with AsyncUserDB("tiktok_users.db") as udb:
+            user_path = await self.get_or_add_user_data(secUid, udb)
 
         async for aweme_data_list in self.fetch_user_post_videos(
-            sec_user_id, max_cursor, page_counts, max_counts
+            secUid, cursor, page_counts, max_counts
         ):
             # 创建下载任务
             await self.downloader.create_download_tasks(
-                self.kwargs, aweme_data_list, user_path
+                self.kwargs, aweme_data_list._to_list(), user_path
             )
 
-            # # 一次性批量插入视频数据到数据库
-            # async with AsyncVideoDB("douyin_videos.db") as db:
-            #     await db.batch_insert_videos(aweme_data_list, ignore_fields)
-
     async def fetch_user_post_videos(
-        self,
-        sec_user_id: str,
-        max_cursor: int = 0,
-        page_counts: int = 20,
-        max_counts: int = None,
-    ):
+        self, secUid: str, cursor: int, page_counts: int, max_counts: float
+    ) -> AsyncGenerator[UserPostFilter, Any]:
         """
-        用于获取指定用户发布的视频列表。
+        用于获取指定用户发布的作品列表
+        (Used to get video list of specified user)
 
         Args:
-            sec_user_id: str: 用户ID
-            max_cursor: int: 起始页
-            page_counts: int: 每页视频数
-            max_counts: int: 最大视频数
+            secUid: str: 用户ID (User ID)
+            cursor: int: 分页游标 (Page cursor)
+            page_counts: int: 分页数量 (Page counts)
+            max_counts: float: 最大数量 (Max counts)
 
         Return:
-            aweme_data: dict: 视频数据字典，包含视频ID列表、视频文案、作者昵称、起始页
+            video: AsyncGenerator[UserPostFilter, Any]: 用户发布作品信息过滤器 (Video info filter)
         """
 
         max_counts = max_counts or float("inf")
         videos_collected = 0
 
-        logger.debug(_("开始爬取用户: {0} 发布的视频").format(sec_user_id))
+        logger.debug(_("开始爬取用户：{0} 发布的作品").format(secUid))
 
         while videos_collected < max_counts:
             current_request_size = min(page_counts, max_counts - videos_collected)
 
-            logger.debug("=====================================")
+            logger.debug("===================================")
             logger.debug(
                 _("最大数量: {0} 每次请求数量: {1}").format(
                     max_counts, current_request_size
                 )
             )
-            logger.debug(_("开始爬取第 {0} 页").format(max_cursor))
+            logger.debug(_("开始爬取第 {0} 页").format(cursor))
 
-            async with DouyinCrawler(self.kwargs) as crawler:
-                params = UserPost(
-                    max_cursor=max_cursor,
-                    count=current_request_size,
-                    sec_user_id=sec_user_id,
-                )
+            async with TiktokCrawler(self.kwargs) as crawler:
+                params = UserPost(secUid=secUid, cursor=cursor, count=page_counts)
                 response = await crawler.fetch_user_post(params)
                 video = UserPostFilter(response)
 
             if not video.has_aweme:
-                logger.debug(_("{0} 页没有找到作品".format(max_cursor)))
-                if not video.has_more:
-                    logger.debug(_("用户: {0} 所有作品采集完毕".format(sec_user_id)))
+                logger.debug(_("第 {0} 页没有找到作品").format(cursor))
+                if not video.hasMore and str(video.api_status_code) == "0":
+                    logger.debug(_("用户：{0} 所有作品采集完毕").format(secUid))
                     break
+                else:
+                    cursor = video.cursor
+                    continue
 
-                max_cursor = video.max_cursor
-                continue
-
-            logger.debug(_("当前请求的max_cursor: {0}").format(max_cursor))
+            logger.debug(_("当前请求的cursor：{0}").format(cursor))
             logger.debug(
-                _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
+                _("作品ID：{0} 作品文案：{1} 作者：{2}").format(
                     video.aweme_id, video.desc, video.nickname
                 )
             )
-            logger.debug("=====================================")
+            logger.debug("===================================")
 
-            aweme_data_list = video._to_list()
-            yield aweme_data_list
+            yield video
 
-            # 更新已经处理的视频数量 (Update the number of videos processed)
+            # 更新已经处理的作品数量 (Update the number of videos processed)
             videos_collected += len(video.aweme_id)
-            max_cursor = video.max_cursor
+            cursor = video.cursor
 
-        logger.debug(_("爬取结束，共爬取{0}个视频").format(videos_collected))
+        logger.debug(_("爬取结束，共爬取 {0} 个作品").format(videos_collected))
 
     @mode_handler("like")
-    async def handle_user_like(self):
+    async def handler_user_like(self):
         """
-        用于处理用户喜欢的视频 (Used to process videos liked by users)
+        用于获取指定用户的点赞作品信息
+        (Used to get liked video info of specified user)
 
         Args:
             kwargs: dict: 参数字典 (Parameter dictionary)
         """
 
-        max_cursor = self.kwargs.get("max_cursor", 0)
-        page_counts = self.kwargs.get("page_counts", 20)
+        cursor = self.kwargs.get("cursor", 0)
+        page_counts = self.kwargs.get("page_counts", 30)
         max_counts = self.kwargs.get("max_counts")
 
-        # 获取用户数据并返回创建用户目录
-        sec_user_id = await SecUserIdFetcher.get_sec_user_id(self.kwargs.get("url"))
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, db)
+        secUid = await SecUserIdFetcher.get_secuid(self.kwargs.get("url"))
+
+        async with AsyncUserDB("tiktok_users.db") as udb:
+            user_path = await self.get_or_add_user_data(secUid, udb)
 
         async for aweme_data_list in self.fetch_user_like_videos(
-            sec_user_id, max_cursor, page_counts, max_counts
+            secUid, cursor, page_counts, max_counts
         ):
             # 创建下载任务
             await self.downloader.create_download_tasks(
-                self.kwargs, aweme_data_list, user_path
+                self.kwargs, aweme_data_list._to_list(), user_path
             )
 
-            # async with AsyncVideoDB("douyin_videos.db") as db:
-            #     for aweme_data in aweme_data_list:
-            #         await get_or_add_video_data(aweme_data, db, ignore_fields)
-
-            # # 一次性批量插入视频数据到数据库
-            # async with AsyncVideoDB("douyin_videos.db") as db:
-            #     await db.batch_insert_videos(aweme_data_list, ignore_fields)
-
     async def fetch_user_like_videos(
-        self,
-        sec_user_id: str,
-        max_cursor: int = 0,
-        page_counts: int = 20,
-        max_counts: int = None,
-    ) -> AsyncGenerator[List[Dict[str, Any]], None]:
-        """
-        用于获取指定用户喜欢的视频列表。
+        self, secUid: str, cursor: int, page_counts: int, max_counts: float
+    ) -> AsyncGenerator[UserPostFilter, Any]:
+        """
+        用于获取指定用户点赞的作品列表
+        (Used to get liked video list of specified user)
 
         Args:
-            sec_user_id: str: 用户ID
-            max_cursor: int: 起始页
-            page_counts: int: 每页视频数
-            max_counts: int: 最大视频数
+            secUid: str: 用户ID (User ID)
+            cursor: int: 分页游标 (Page cursor)
+            page_counts: int: 分页数量 (Page counts)
+            max_counts: float: 最大数量 (Max counts)
 
         Return:
-            aweme_data: dict: 视频数据字典，包含视频ID列表、视频文案、作者昵称、起始页
+            like: AsyncGenerator[UserPostFilter, Any]: 用户点赞作品信息过滤器 (Video info filter)
         """
 
         max_counts = max_counts or float("inf")
         videos_collected = 0
 
-        logger.debug(_("开始爬取用户: {0} 喜欢的视频").format(sec_user_id))
+        logger.debug(_("开始爬取用户：{0} 点赞的作品").format(secUid))
 
         while videos_collected < max_counts:
             current_request_size = min(page_counts, max_counts - videos_collected)
 
-            logger.debug("=====================================")
+            logger.debug("===================================")
             logger.debug(
-                _("最大数量: {0} 每次请求数量: {1}").format(
+                _("最大数量：{0} 每次请求数量：{1}").format(
                     max_counts, current_request_size
                 )
             )
-            logger.debug(_("开始爬取第 {0} 页").format(max_cursor))
+            logger.debug(_("开始爬取第 {0} 页").format(cursor))
 
-            async with DouyinCrawler(self.kwargs) as crawler:
-                params = UserLike(
-                    max_cursor=max_cursor,
-                    count=current_request_size,
-                    sec_user_id=sec_user_id,
-                )
+            async with TiktokCrawler(self.kwargs) as crawler:
+                params = UserLike(secUid=secUid, cursor=cursor, count=page_counts)
                 response = await crawler.fetch_user_like(params)
-                video = UserPostFilter(response)
+                like = UserPostFilter(response)
 
-            if not video.has_aweme:
-                logger.debug(_("{0} 页没有找到作品".format(max_cursor)))
-                if not video.has_more:
-                    logger.debug(_("用户: {0} 所有作品采集完毕".format(sec_user_id)))
-                    break
+            if like.has_aweme:
+                logger.debug(_("当前请求的cursor：{0}").format(cursor))
+                logger.debug(
+                    _("作品ID：{0} 作品文案：{1} 作者：{2}").format(
+                        like.aweme_id, like.desc, like.nickname
+                    )
+                )
+                logger.debug("===================================")
 
-                max_cursor = video.max_cursor
-                continue
+                yield like
 
-            logger.debug(_("当前请求的max_cursor: {0}").format(max_cursor))
-            logger.debug(
-                _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
-                    video.aweme_id, video.desc, video.nickname
-                )
-            )
-            logger.debug("=====================================")
+                # 更新已经处理的作品数量 (Update the number of videos processed)
+                videos_collected += len(like.aweme_id)
 
-            aweme_data_list = video._to_list()
-            yield aweme_data_list
+                if not like.hasMore and str(like.api_status_code) == "0":
+                    logger.debug(_("用户：{0} 所有作品采集完毕").format(secUid))
+                    break
 
-            # 更新已经处理的视频数量 (Update the number of videos processed)
-            videos_collected += len(aweme_data_list)
-            max_cursor = video.max_cursor
+            else:
+                logger.debug(_("第 {0} 页没有找到作品").format(cursor))
 
-        logger.debug(_("爬取结束，共爬取{0}个视频").format(videos_collected))
+                if not like.hasMore and str(like.api_status_code) == "0":
+                    logger.debug(_("用户：{0} 所有作品采集完毕").format(secUid))
+                    break
+
+            # 更新已经处理的作品数量 (Update the number of videos processed)
+            videos_collected += len(like.aweme_id)
+            cursor = like.cursor
+
+        logger.debug(_("爬取结束，共爬取 {0} 个作品").format(videos_collected))
 
     @mode_handler("collect")
-    async def handle_user_collect(self):
+    async def handler_user_collect(self):
         """
-        用于处理用户收藏的视频 (Used to process videos collected by users)
+        用于获取指定用户的收藏作品信息
+        (Used to get collected video info of specified user)
 
         Args:
             kwargs: dict: 参数字典 (Parameter dictionary)
         """
 
-        max_cursor = self.kwargs.get("max_cursor", 0)
-        page_counts = self.kwargs.get("page_counts", 20)
+        cursor = self.kwargs.get("cursor", 0)
+        page_counts = self.kwargs.get("page_counts", 30)
         max_counts = self.kwargs.get("max_counts")
 
-        sec_user_id = await SecUserIdFetcher.get_sec_user_id(self.kwargs.get("url"))
+        secUid = await SecUserIdFetcher.get_secuid(self.kwargs.get("url"))
 
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, db)
+        async with AsyncUserDB("tiktok_users.db") as udb:
+            user_path = await self.get_or_add_user_data(secUid, udb)
 
         async for aweme_data_list in self.fetch_user_collect_videos(
-            max_cursor, page_counts, max_counts
+            secUid, cursor, page_counts, max_counts
         ):
+            # 创建下载任务
             await self.downloader.create_download_tasks(
-                self.kwargs, aweme_data_list, user_path
+                self.kwargs, aweme_data_list._to_list(), user_path
             )
 
     async def fetch_user_collect_videos(
-        self, max_cursor: int = 0, page_counts: int = 20, max_counts: int = None
-    ) -> AsyncGenerator[List[Dict[str, Any]], None]:
+        self, secUid: str, cursor: int, page_counts: int, max_counts: float
+    ) -> AsyncGenerator[UserPostFilter, Any]:
         """
-        用于获取指定用户收藏的视频列表。
-        (Used to get the list of videos collected by the specified user.)
-        该接口需要用POST且只靠cookie来获取数据。
-        (This interface needs to be POST and only relies on cookies to get data.)
+        用于获取指定用户收藏的作品列表
+        (Used to get collected video list of specified user)
 
         Args:
-            max_cursor: int: 起始页 (Start page)
-            page_counts: int: 每页视频数 (Number of videos per page)
-            max_counts: int: 最大视频数 (Maximum number of videos)
+            secUid: str: 用户ID (User ID)
+            cursor: int: 分页游标 (Page cursor)
+            page_counts: int: 分页数量 (Page counts)
+            max_counts: float: 最大数量 (Max counts)
 
         Return:
-            aweme_data: dict: 视频数据字典, 包含视频ID列表、视频文案、作者昵称、起始页
-            (Video data dictionary, including video ID list, video description,
-            author nickname, start page)
+            collect: AsyncGenerator[UserPostFilter, Any]: 收藏作品信息过滤器 (Video info filter)
         """
 
         max_counts = max_counts or float("inf")
         videos_collected = 0
 
-        logger.debug(_("开始爬取用户收藏的视频"))
+        logger.debug(_("开始爬取用户：{0} 收藏的作品").format(secUid))
 
         while videos_collected < max_counts:
             current_request_size = min(page_counts, max_counts - videos_collected)
 
-            logger.debug("=====================================")
+            logger.debug("===================================")
             logger.debug(
-                _("最大数量: {0} 每次请求数量: {1}").format(
+                _("最大数量：{0} 每次请求数量：{1}").format(
                     max_counts, current_request_size
                 )
             )
-            logger.debug(_("开始爬取第 {0} 页").format(max_cursor))
+            logger.debug(_("开始爬取第 {0} 页").format(cursor))
 
-            async with DouyinCrawler(self.kwargs) as crawler:
-                params = UserCollect(cursor=max_cursor, count=current_request_size)
+            async with TiktokCrawler(self.kwargs) as crawler:
+                params = UserCollect(secUid=secUid, cursor=cursor, count=page_counts)
                 response = await crawler.fetch_user_collect(params)
-                video = UserCollectFilter(response)
-
-            logger.debug(_("当前请求的max_cursor: {0}").format(max_cursor))
-            logger.debug(
-                _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
-                    video.aweme_id, video.desc, video.nickname
-                )
-            )
-            logger.debug("=====================================")
-
-            aweme_data_list = video._to_list()
-            yield aweme_data_list
-
-            if not video.has_more:
-                logger.debug(_("用户收藏的视频采集完毕"))
-                break
-
-            # 更新已经处理的视频数量 (Update the number of videos processed)
-            videos_collected += len(aweme_data_list)
-            max_cursor = video.max_cursor
-
-    @mode_handler("mix")
-    async def handle_user_mix(self):
-        """
-        用于处理用户合集的视频 (Used to process videos of users' collections)
-
-        Args:
-            kwargs: dict: 参数字典 (Parameter dictionary)
-        """
-
-        max_cursor = self.kwargs.get("max_cursor", 0)
-        page_counts = self.kwargs.get("page_counts", 20)
-        max_counts = self.kwargs.get("max_counts")
-
-        aweme_id = await AwemeIdFetcher.get_aweme_id(self.kwargs.get("url"))
-        mix_data = await self.fetch_one_video(aweme_id)
-        sec_user_id = mix_data.get("sec_user_id")
-        mix_id = mix_data.get("mix_id")
-
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, db)
-
-        async for aweme_data_list in self.fetch_user_mix_videos(
-            mix_id, max_cursor, page_counts, max_counts
-        ):
-            # 创建下载任务
-            await self.downloader.create_download_tasks(
-                self.kwargs, aweme_data_list, user_path
-            )
-
-        # async with AsyncVideoDB("douyin_videos.db") as db:
-        #     for aweme_data in aweme_data_list:
-        #         await get_or_add_video_data(aweme_data, db, ignore_fields)
-
-    async def fetch_user_mix_videos(
-        self,
-        mix_id: str,
-        max_cursor: int = 0,
-        page_counts: int = 20,
-        max_counts: int = None,
-    ) -> AsyncGenerator[List[Dict[str, Any]], None]:
-        """
-        用于获取指定用户合集的视频列表。
-
-        Args:
-            mix_id: str: 合集ID
-            max_cursor: int: 起始页
-            page_counts: int: 每页视频数
-            max_counts: int: 最大视频数
-
-        Return:
-            aweme_data: dict: 视频数据字典，包含视频ID列表、视频文案、作者昵称、起始页
-        """
-
-        max_counts = max_counts or float("inf")
-        videos_collected = 0
-
-        logger.debug(_("开始爬取合集: {0} 的视频").format(mix_id))
-
-        while videos_collected < max_counts:
-            current_request_size = min(page_counts, max_counts - videos_collected)
-
-            logger.debug("=====================================")
-            logger.debug(
-                _("最大数量: {0} 每次请求数量: {1}").format(
-                    max_counts, current_request_size
-                )
-            )
-            logger.debug(_("开始爬取第 {0} 页").format(max_cursor))
-
-            async with DouyinCrawler(self.kwargs) as crawler:
-                params = UserMix(
-                    cursor=max_cursor, count=current_request_size, mix_id=mix_id
-                )
-                response = await crawler.fetch_user_mix(params)
-                video = UserMixFilter(response)
+                collect = UserPostFilter(response)
 
-            logger.debug(_("当前请求的max_cursor: {0}").format(max_cursor))
-            logger.debug(
-                _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
-                    video.aweme_id, video.desc, video.nickname
+            if collect.has_aweme:
+                logger.debug(_("当前请求的cursor：{0}").format(cursor))
+                logger.debug(
+                    _("作品ID：{0} 作品文案：{1} 作者：{2}").format(
+                        collect.aweme_id, collect.desc, collect.nickname
+                    )
                 )
-            )
-            logger.debug("=====================================")
-
-            aweme_data_list = video._to_list()
-            yield aweme_data_list
-
-            # 更新已经处理的视频数量 (Update the number of videos processed)
-            videos_collected += len(aweme_data_list)
-            max_cursor = video.max_cursor
-
-            if not video.has_more:
-                logger.debug(_("合集: {0} 所有作品采集完毕").format(mix_id))
-                break
-
-        logger.debug(_("爬取结束，共爬取{0}个视频").format(videos_collected))
-
-    @mode_handler("live")
-    async def handle_user_live(self):
-        """
-        用于处理用户直播 (Used to process user live)
-
-        Args:
-            kwargs: dict: 参数字典 (Parameter dictionary)
-        """
+                logger.debug("===================================")
 
-        # 获取直播相关信息与主播信息
-        webcast_id = await WebCastIdFetcher.get_webcast_id(self.kwargs.get("url"))
+                yield collect
 
-        # 然后下载直播推流
-        webcast_data = await self.fetch_user_live_videos(webcast_id)
-        live_status = webcast_data.get("live_status")
-        # 是否正在直播
-        if live_status != 2:
-            logger.debug(_("直播已结束"))
-            return
-        sec_user_id = webcast_data.get("sec_user_id")
+                # 更新已经处理的作品数量 (Update the number of videos processed)
+                videos_collected += len(collect.aweme_id)
 
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, db)
-        await self.downloader.create_stream_tasks(self.kwargs, webcast_data, user_path)
-
-    async def fetch_user_live_videos(self, webcast_id: str):
-        """
-        用于获取指定用户直播列表。
-        (Used to get the list of videos collected by the specified user.)
-
-        Args:
-            webcast_id: str: 直播ID (Live ID)
-
-        Return:
-            webcast_data: dict: 直播数据字典，包含直播ID、直播标题、直播状态、观看人数、子分区、主播昵称
-            (Live data dict, including live ID, live title, live status, number of viewers,
-            sub-partition, anchor nickname)
-        """
-
-        logger.debug(_("开始爬取直播: {0} 的数据").format(webcast_id))
-        logger.debug("=====================================")
-
-        async with DouyinCrawler(self.kwargs) as crawler:
-            params = UserLive(web_rid=webcast_id, room_id_str="")
-            response = await crawler.fetch_live(params)
-            live = UserLiveFilter(response)
-
-        logger.debug(
-            _("直播ID: {0} 直播标题: {1} 直播状态: {2} 观看人数: {3}").format(
-                live.room_id, live.live_title, live.live_status, live.user_count
-            )
-        )
-        logger.debug(
-            _("子分区: {0} 主播昵称: {1}").format(
-                live.sub_partition_title, live.nickname
-            )
-        )
-        logger.debug("=====================================")
-        logger.debug(_("直播信息爬取结束"))
-
-        webcast_data = live._to_dict()
-        return webcast_data
-
-    async def fetch_user_live_videos_by_room_id(self, room_id: str):
-        """
-        使用room_id获取指定用户直播列表。
-        (Used to get the list of videos collected by the specified user)
-
-        Args:
-            room_id: str: 直播ID (Live ID)
+                if not collect.hasMore and str(collect.api_status_code) == "0":
+                    logger.debug(_("用户：{0} 所有作品采集完毕").format(secUid))
+                    break
 
-        Return:
-            webcast_data: dict: 直播数据字典，包含直播ID、直播标题、直播状态、观看人数、主播昵称
-            (Live data dict, including live ID, live title, live status, number of viewers,
-            anchor nickname)
-        """
+            else:
+                logger.debug(_("第 {0} 页没有找到作品").format(cursor))
 
-        logger.debug(_("开始爬取房间号: {0} 的数据").format(room_id))
-        logger.debug("=====================================")
-
-        async with DouyinCrawler(self.kwargs) as crawler:
-            params = UserLive2(room_id=room_id)
-            response = await crawler.fetch_live_room_id(params)
-            live = UserLive2Filter(response)
+                if not collect.hasMore and str(collect.api_status_code) == "0":
+                    logger.debug(_("用户：{0} 所有作品采集完毕").format(secUid))
+                    break
 
-        logger.debug(
-            _("直播ID: {0} 直播标题: {1} 直播状态: {2} 观看人数: {3}").format(
-                live.web_rid, live.live_title, live.live_status, live.user_count
-            )
-        )
-        logger.debug(
-            _("主播昵称: {0} 开播时间: {1} 直播流清晰度: {2}").format(
-                live.nickname,
-                live.create_time,
-                "、".join(
-                    [f"{key}: {value}" for key, value in live.resolution_name.items()]
-                ),
-            )
-        )
-        logger.debug("=====================================")
-        logger.debug(_("直播信息爬取结束"))
+            # 更新已经处理的作品数量 (Update the number of videos processed)
+            videos_collected += len(collect.aweme_id)
+            cursor = collect.cursor
 
-        webcast_data = live._to_dict()
-        return webcast_data
+        logger.debug(_("爬取结束，共爬取 {0} 个作品").format(videos_collected))
 
-    @mode_handler("feed")
-    async def handle_user_feed(self):
+    @mode_handler("mix")
+    async def handler_user_mix(self):
         """
-        用于处理用户feed (Used to process user feed)
+        用于获取指定用户的合集作品信息
+        (Used to get mix video info of specified user)
 
         Args:
             kwargs: dict: 参数字典 (Parameter dictionary)
         """
 
-        max_cursor = self.kwargs.get("max_cursor", 0)
-        page_counts = self.kwargs.get("page_counts", 20)
+        cursor = self.kwargs.get("cursor", 0)
+        page_counts = self.kwargs.get("page_counts", 30)
         max_counts = self.kwargs.get("max_counts")
 
-        sec_user_id = await SecUserIdFetcher.get_sec_user_id(self.kwargs.get("url"))
-
-        async with AsyncUserDB("douyin_users.db") as db:
-            user_path = await self.get_or_add_user_data(self.kwargs, sec_user_id, db)
-
-        async for aweme_data_list in self.fetch_user_feed_videos(
-            sec_user_id, max_cursor, page_counts, max_counts
-        ):
-            # 创建下载任务
-            await self.downloader.create_download_tasks(
-                self.kwargs, aweme_data_list, user_path
-            )
+        secUid = await SecUserIdFetcher.get_secuid(self.kwargs.get("url"))
+        playlist = await self.fetch_play_list(secUid, cursor, page_counts)
+        mixId = await self.select_playlist(playlist)
+
+        async with AsyncUserDB("tiktok_users.db") as audb:
+            user_path = await self.get_or_add_user_data(secUid, audb)
+
+        if isinstance(mixId, str):
+            mixId = [mixId]
+
+        for mixId in playlist.get("mixId", []):
+            async for aweme_data_list in self.fetch_user_mix_videos(
+                mixId, cursor, page_counts, max_counts
+            ):
+                # 创建下载任务
+                await self.downloader.create_download_tasks(
+                    self.kwargs, aweme_data_list._to_list(), user_path
+                )
 
-    async def fetch_user_feed_videos(
-        self,
-        sec_user_id: str,
-        max_cursor: int = 0,
-        page_counts: int = 20,
-        max_counts: int = None,
-    ) -> AsyncGenerator[List[Dict[str, Any]], None]:
-        """
-        用于获取指定用户feed的视频列表。
+    async def fetch_user_mix_videos(
+        self, mixId: str, cursor: int, page_counts: int, max_counts: float
+    ) -> AsyncGenerator[UserMixFilter, Any]:
+        """
+        用于获取指定用户合集的作品列表
+        (Used to get mix video list of specified user)
 
         Args:
-            sec_user_id: str: 用户ID
-            max_cursor: int: 起始页
-            page_counts: int: 每页视频数
-            max_counts: int: 最大视频数
+            mixId: str: 合集ID (Mix ID)
+            cursor: int: 分页游标 (Page cursor)
+            page_counts: int: 分页数量 (Page counts)
+            max_counts: float: 最大数量 (Max counts)
 
         Return:
-            aweme_data: dict: 视频数据字典，包含视频ID列表、视频文案、作者昵称、起始页
+            mix: AsyncGenerator[UserMixFilter, Any]: 合集作品信息过滤器 (Video info filter)
         """
 
         max_counts = max_counts or float("inf")
         videos_collected = 0
 
-        logger.debug(_("开始爬取用户: {0} feed的视频").format(sec_user_id))
+        logger.debug(_("开始爬取用户: {0} 合集的作品").format(mixId))
 
         while videos_collected < max_counts:
             current_request_size = min(page_counts, max_counts - videos_collected)
 
-            logger.debug("=====================================")
+            logger.debug("===================================")
             logger.debug(
                 _("最大数量: {0} 每次请求数量: {1}").format(
                     max_counts, current_request_size
                 )
             )
-            logger.debug(_("开始爬取第 {0} 页").format(max_cursor))
+            logger.debug(_("开始爬取第 {0} 页").format(cursor))
 
-            async with DouyinCrawler(self.kwargs) as crawler:
-                params = UserPost(
-                    max_cursor=max_cursor,
-                    count=current_request_size,
-                    sec_user_id=sec_user_id,
-                )
-                response = await crawler.fetch_user_post(params)
-                video = UserPostFilter(response)
-
-            if not video.has_aweme:
-                logger.debug(_("{0} 页没有找到作品".format(max_cursor)))
-                if not video.has_more:
-                    logger.debug(_("用户: {0} 所有作品采集完毕".format(sec_user_id)))
-                    break
-
-                max_cursor = video.max_cursor
-                continue
+            async with TiktokCrawler(self.kwargs) as crawler:
+                params = UserMix(mixId=mixId, cursor=cursor, count=page_counts)
+                response = await crawler.fetch_user_mix(params)
+                mix = UserMixFilter(response)
 
-            logger.debug(_("当前请求的max_cursor: {0}").format(max_cursor))
-            logger.debug(
-                _("视频ID: {0} 视频文案: {1} 作者: {2}").format(
-                    video.aweme_id, video.desc, video.nickname
+            if mix.has_aweme:
+                logger.debug(_("当前请求的cursor: {0}").format(cursor))
+                logger.debug(
+                    _("作品ID: {0} 作品文案: {1} 作者: {2}").format(
+                        mix.aweme_id, mix.desc, mix.nickname
+                    )
                 )
-            )
-            logger.debug("=====================================")
-
-            aweme_data_list = video._to_list()
-            yield aweme_data_list
-
-            # 更新已经处理的视频数量 (Update the number of videos processed)
-            videos_collected += len(video.aweme_id)
-            max_cursor = video.max_cursor
+                logger.debug("===================================")
 
-        logger.debug(_("爬取结束，共爬取{0}个视频").format(videos_collected))
+                yield mix
 
+                # 更新已经处理的作品数量 (Update the number of videos processed)
+                videos_collected += len(mix.aweme_id)
 
-async def handle_sso_login():
-    """
-    用于处理用户登录 (Used to process user login)
-    """
-
-    kwargs = {
-        "proxies": {"http": None, "https": None},
-        "cookie": "",
-        "headers": {
-            "Referer": "https://www.douyin.com/",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML,like Gecko) Chrome/104.0.0.0 Safari/537.36",
-        },
-    }
-
-    async def get_qrcode() -> str:
-        params = LoginGetQr(verifyFp=verify_fp, fp=verify_fp)
-        async with DouyinCrawler(kwargs) as crawler:
-            response = await crawler.fetch_login_qrcode(params)
-            sso = GetQrcodeFilter(response)
-            show_qrcode(sso.qrcode_index_url)
-            return await check_qrcode(sso.token, crawler)
-
-    async def check_qrcode(token: str, crawler) -> bool:
-        """
-        检查二维码状态
-
-        Args:
-            token (str): 二维码token
-
-        Returns:
-            bool: 是否成功登录
-        """
-        logger.debug(f"check_qrcode token:{token}")
-
-        status_mapping = {
-            "1": {"message": _("[  登录  ]:等待二维码扫描！"), "log": logger.info},
-            "2": {"message": _("[  登录  ]:扫描二维码成功！"), "log": logger.info},
-            "3": {"message": _("[  登录  ]:确认二维码登录！"), "log": logger.info},
-            "4": {
-                "message": _("[  登录  ]:访问频繁，请检查参数！"),
-                "log": logger.warning,
-            },
-            "5": {
-                "message": _("[  登录  ]:二维码过期，重新获取！"),
-                "log": logger.warning,
-            },
-            "2046": {
-                "messages": _("[  登录  ]:扫码环境异常，请前往app验证！"),
-                "log": logger.warning,
-            },
-        }
-
-        while True:
-            params = LoginCheckQr(token=token, verifyFp=verify_fp, fp=verify_fp)
-            check_response = await crawler.fetch_check_qrcode(params)
-            check = CheckQrcodeFilter(check_response.json())
-            check_status = check.status
-            check_status = "2046" if check_status is None else check_status
-
-            status_info = status_mapping.get(check_status, {})
-            message = status_info.get("message", "")
-            log_func = status_info.get("log", logger.info)
-            logger.info(message)
-            log_func(message)
-
-            if check_status == "3":
-                login_cookies = split_set_cookie(
-                    check_response.headers.get("set-cookie", "")
-                )
-                is_login, login_cookie = await login_redirect(
-                    check.redirect_url, login_cookies, crawler
-                )
-                return is_login, login_cookie
-            elif check_status == "5":
-                get_qrcode()
-                break
-            elif check_status is None:
-                break
-
-            await asyncio.sleep(5)
-
-    async def login_redirect(redirect_url: str, login_cookies: str, crawler):
-        """
-        登录重定向，获取登录后Cookie
+                if not mix.hasMore and str(mix.api_status_code) == "0":
+                    logger.debug(_("合辑: {0} 所有作品采集完毕").format(mixId))
+                    break
 
-        Args:
-            redirect_url (str): 重定向url
-            login_cookies (str): 登录cookie
+            else:
+                logger.debug(_("第 {0} 页没有找到作品").format(cursor))
 
-        Returns:
-            is_login (bool): 是否成功登录
-            login_cookie (str): 登录cookie
-        """
-        crawler.headers["Cookie"] = login_cookies
-        redirect_response = await crawler.get_fetch_data(redirect_url)
+                if not mix.hasMore and str(mix.api_status_code) == "0":
+                    logger.debug(_("合辑: {0} 所有作品采集完毕").format(mixId))
+                    break
 
-        if redirect_response.history and len(redirect_response.history) > 1:
-            logger.debug(f"login_redirect headers:{redirect_response.headers}")
-            logger.debug(f"login_redirect history:{redirect_response.history}")
-            logger.debug(
-                f"login_redirect history[0] headers:{redirect_response.history[0].headers}"
-            )
-            logger.debug(
-                f"login_redirect history[1] headers:{redirect_response.history[1].headers}"
-            )
-            # 获取重最后一个重定向里的Cookie
-            login_cookie = split_set_cookie(
-                redirect_response.history[1].headers.get("set-cookie", "")
-            )
-            logger.debug(f"login_cookie:{login_cookie}")
-            return True, login_cookie
-        else:
-            logger.warning("[  登录  ]:自动重定向登录失败")
-            if redirect_response:
-                error_message = f"网络异常: 自动重定向登录失败。 状态码: {redirect_response.status_code}, 响应体: {redirect_response.text}"
-            else:
-                error_message = f"网络异常: 自动重定向登录失败。 无法连接到服务器。"
-            logger.warning(error_message)
-            return False, ""
+            # 更新已经处理的作品数量 (Update the number of videos processed)
+            videos_collected += len(mix.aweme_id)
+            cursor = mix.cursor
 
-    verify_fp = VerifyFpManager.gen_verify_fp()
-    return await get_qrcode()
+        logger.debug(_("爬取结束，共爬取 {0} 个作品").format(videos_collected))
 
 
 async def main(kwargs):
     mode = kwargs.get("mode")
     if mode in mode_function_map:
-        await mode_function_map[mode](DouyinHandler(kwargs))
+        await mode_function_map[mode](TiktokHandler(kwargs))
     else:
         logger.error(_("不存在该模式: {0}").format(mode))
+        rich_console.print(_("不存在该模式: {0}").format(mode))
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/help.py` & `f2-0.0.1.5/f2/apps/tiktok/help.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# path: f2/apps/douyin/help.py
+# path: f2/apps/tiktok/help.py
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from f2.i18n.translator import _
 
@@ -33,15 +33,15 @@
             "[dark_cyan]Choice",
             _("是否将作品保存到单独的文件夹。可选：'yes'、'no'"),
         ),
         (
             "-M --mode",
             "[dark_cyan]Choice",
             _(
-                "下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collect)，合辑(mix)，直播(live)"
+                "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑播放列表(mix)"
             ),
         ),
         (
             "-n --naming",
             "[dark_cyan]str",
             _("全局作品文件命名方式，前往文档查看更多帮助"),
         ),
@@ -59,15 +59,19 @@
                 "下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"
             ),
         ),
         ("-e --timeout", "[dark_cyan]int", _("网络请求超时时间。")),
         ("-r --max-retries", "[dark_cyan]int", _("网络请求超时重试数。")),
         ("-x --max-connections", "[dark_cyan]int", _("网络请求并发连接数。")),
         ("-t --max-tasks", "[dark_cyan]int", _("异步的任务数。")),
-        ("-o --max-counts", "[dark_cyan]int", _("最大作品下载数。0 表示无限制")),
+        (
+            "-o --max-counts",
+            "[dark_cyan]int",
+            _("最大作品下载数。0 表示无限制"),
+        ),
         (
             "-s --page-counts",
             "[dark_cyan]int",
             _("从接口每页可获取作品数，不建议超过20。"),
         ),
         (
             "-l --languages",
@@ -91,31 +95,26 @@
             "[dark_cyan]Flag",
             _("初始化配置文件。不能同时初始化和更新配置文件"),
         ),
         (
             "--auto-cookie",
             "[dark_cyan]Choice",
             _(
-                "自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、opera。使用该命令前请确保关闭所选的浏览器"
+                "自动从浏览器获取[yellow]cookie[/yellow]，使用该命令前请确保关闭所选的浏览器"
             ),
         ),
-        (
-            "--sso-login",
-            "[dark_cyan]Flag",
-            _("使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"),
-        ),
         ("--help", "[dark_cyan]Flag", _("显示经典帮助信息")),
         (
             "",
             "",
             _(
                 "更加详细的参数说明请点击[link=https://johnserf-seed.github.io/f2/site-config.html][dark_violet]前往文档[/dark_violet][/]查看"
             ),
         ),
     ]
 
     for option in options:
         table.add_row(*option)
 
     console.print(
-        Panel(table, border_style="bold", title="[DouYin]", title_align="left")
+        Panel(table, border_style="bold", title="[TikTok]", title_align="left")
     )
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/model.py` & `f2-0.0.1.5/f2/apps/douyin/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 # Base Model
 class BaseRequestModel(BaseModel):
     device_platform: str = "webapp"
     aid: str = "6383"
     channel: str = "channel_pc_web"
     pc_client_type: int = 1
-    version_code: str = "170400"
-    version_name: str = "17.4.0"
+    version_code: str = "190500"
+    version_name: str = "19.5.0"
     cookie_enabled: str = "true"
     screen_width: int = 1920
     screen_height: int = 1080
     browser_language: str = "zh-CN"
     browser_platform: str = "Win32"
     browser_name: str = "Edge"
-    browser_version: str = "117.0.2045.47"
+    browser_version: str = "122.0.0.0"
     browser_online: str = "true"
     engine_name: str = "Blink"
-    engine_version: str = "117.0.0.0"
+    engine_version: str = "122.0.0.0"
     os_name: str = "Windows"
     os_version: str = "10"
     cpu_core_num: int = 12
     device_memory: int = 8
     platform: str = "PC"
     downlink: int = 10
     effective_type: str = "4g"
@@ -59,14 +59,15 @@
     type_id: str = "0"
     live_id: str = "1"
     sec_user_id: str = ""
     version_code: str = "99.99.99"
     app_id: str = "1128"
     msToken: str = TokenManager.gen_real_msToken()
 
+
 class BaseLoginModel(BaseModel):
     service: str = "https://www.douyin.com"
     need_logo: str = "false"
     need_short_url: str = "true"
     device_platform: str = "web_app"
     aid: str = "6383"
     account_sdk_source: str = "sso"
@@ -87,20 +88,39 @@
 
 class UserLike(BaseRequestModel):
     max_cursor: int
     count: int
     sec_user_id: str
 
 
-class UserCollect(BaseRequestModel):
+class UserCollection(BaseRequestModel):
     # POST
     cursor: int
     count: int
 
 
+class UserCollects(BaseRequestModel):
+    # GET
+    cursor: int
+    count: int
+
+
+class UserCollectsVideo(BaseRequestModel):
+    # GET
+    cursor: int
+    count: int
+    collects_id: str
+
+
+class UserMusicCollection(BaseRequestModel):
+    # GET
+    cursor: int
+    count: int
+
+
 class UserMix(BaseRequestModel):
     cursor: int
     count: int
     mix_id: str
 
 
 class FriendFeed(BaseRequestModel):
@@ -171,14 +191,15 @@
     publish_video_strategy_type: int = 2
 
 
 class UserLive(BaseLiveModel):
     web_rid: str
     room_id_str: str
 
+
 class UserLive2(BaseLiveModel2):
     room_id: str
 
 
 class FollowUserLive(BaseRequestModel):
     scene: str = "aweme_pc_follow_top"
 
@@ -206,12 +227,41 @@
 
 
 class LoginGetQr(BaseLoginModel):
     verifyFp: str = ""
     fp: str = ""
     # msToken: str = TokenManager.gen_real_msToken()
 
+
 class LoginCheckQr(BaseLoginModel):
     token: str = ""
     verifyFp: str = ""
     fp: str = ""
-    # msToken: str = TokenManager.gen_real_msToken()
+    # msToken: str = TokenManager.gen_real_msToken()
+
+
+class UserFollowing(BaseRequestModel):
+    user_id: str = ""
+    sec_user_id: str = ""
+    offset: int = 0  # 相当于cursor
+    min_time: int = 0
+    max_time: int = 0
+    count: int = 20
+    # source_type = 1: 最近关注 需要指定max_time(s) 3: 最早关注 需要指定min_time(s) 4: 综合排序
+    source_type: int = 4
+    gps_access: int = 0
+    address_book_access: int = 0
+    is_top: int = 1
+
+
+class UserFollower(BaseRequestModel):
+    user_id: str
+    sec_user_id: str
+    offset: int = 0  # 相当于cursor 但只对source_type: = 2 有效，其他情况为 0 即可
+    min_time: int = 0
+    max_time: int = 0
+    count: int = 20
+    # source_type = 1: 最近关注 需要指定max_time(s) 2: 综合关注(意义不明)
+    source_type: int = 1
+    gps_access: int = 0
+    address_book_access: int = 0
+    is_top: int = 1
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/utils.py` & `f2-0.0.1.5/f2/apps/tiktok/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# path: f2/apps/douyin/utils.py
+# path: f2/apps/tiktok/utils.py
 
 import f2
 import re
 import json
-import time
 import httpx
-import qrcode
-import random
 import asyncio
 
 from typing import Union
 from pathlib import Path
 
 from f2.i18n.translator import _
 from f2.log.logger import logger
@@ -22,24 +19,24 @@
     extract_valid_urls,
     split_filename,
 )
 from f2.exceptions.api_exceptions import (
     APIError,
     APIConnectionError,
     APIResponseError,
-    APIUnavailableError,
     APIUnauthorizedError,
     APINotFoundError,
 )
 
 
 class TokenManager:
-    f2_manager = ConfigManager(f2.F2_CONFIG_FILE_PATH).get_config("f2").get("douyin")
+    f2_manager = ConfigManager(f2.F2_CONFIG_FILE_PATH).get_config("f2").get("tiktok")
     token_conf = f2_manager.get("msToken", None)
     ttwid_conf = f2_manager.get("ttwid", None)
+    odin_tt_conf = f2_manager.get("odin_tt", None)
     proxies_conf = f2_manager.get("proxies", None)
     proxies = {
         "http://": proxies_conf.get("http", None),
         "https://": proxies_conf.get("https", None),
     }
 
     @classmethod
@@ -54,467 +51,506 @@
                 "magic": cls.token_conf["magic"],
                 "version": cls.token_conf["version"],
                 "dataType": cls.token_conf["dataType"],
                 "strData": cls.token_conf["strData"],
                 "tspFromClient": get_timestamp(),
             }
         )
+
         headers = {
             "User-Agent": cls.token_conf["User-Agent"],
             "Content-Type": "application/json",
         }
 
         transport = httpx.HTTPTransport(retries=5)
         with httpx.Client(transport=transport, proxies=cls.proxies) as client:
             try:
                 response = client.post(
                     cls.token_conf["url"], headers=headers, content=payload
                 )
-
-                if response.status_code == 401:
-                    raise APIUnauthorizedError(_("由于某些错误, 无法获取msToken"))
-                elif response.status_code == 404:
-                    raise APINotFoundError(_("无法找到API端点"))
+                response.raise_for_status()
 
                 msToken = str(httpx.Cookies(response.cookies).get("msToken"))
 
-                if len(msToken) not in [120, 128]:
-                    raise APIResponseError(
-                        _(
-                            "msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 douyin 新规则。"
-                        )
-                    )
+                if len(msToken) not in [148]:
+                    raise APIResponseError(_("{0} 内容不符合要求").format("msToken"))
 
                 return msToken
 
-            except httpx.RequestError:
+            except httpx.RequestError as exc:
                 # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
                 raise APIConnectionError(
                     _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(cls.token_conf["url"], cls.proxies, cls.__name__)
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(cls.token_conf["url"], cls.proxies, cls.__name__, exc)
                 )
 
             except httpx.HTTPStatusError as e:
                 # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
-                raise APIResponseError(
-                    f"HTTP Status Code {e.response.status_code}: {e.response.text}"
-                )
+                if response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _(
+                            "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+                        ).format("msToken", "tiktok")
+                    )
+
+                elif response.status_code == 404:
+                    raise APINotFoundError(_("{0} 无法找到API端点").format("msToken"))
+                else:
+                    raise APIResponseError(
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            e.response.url, e.response.status_code, e.response.text
+                        )
+                    )
 
             except APIError as e:
+                # 返回虚假的msToken (Return a fake msToken)
+                logger.error(_("msToken API错误：{0}").format(e))
                 logger.info(_("生成虚假的msToken"))
                 return cls.gen_false_msToken()
 
     @classmethod
     def gen_false_msToken(cls) -> str:
         """生成随机msToken (Generate random msToken)"""
-        return gen_random_str(126) + "=="
+        return gen_random_str(146) + "=="
 
     @classmethod
     def gen_ttwid(cls) -> str:
         """
-        生成请求必带的ttwid
-        (Generate the essential ttwid for requests)
+        生成请求必带的ttwid (Generate the essential ttwid for requests)
         """
-
         transport = httpx.HTTPTransport(retries=5)
-        with httpx.Client(transport=transport) as client:
+        with httpx.Client(transport=transport, proxies=cls.proxies) as client:
             try:
                 response = client.post(
-                    cls.ttwid_conf["url"], content=cls.ttwid_conf["data"]
+                    cls.ttwid_conf["url"],
+                    content=cls.ttwid_conf["data"],
+                    headers={
+                        "Cookie": cls.ttwid_conf.get("cookie"),
+                        "Content-Type": "text/plain",
+                    },
                 )
+                response.raise_for_status()
 
-                if response.status_code == 401:
-                    raise APIUnauthorizedError(_("由于某些错误, 无法获取ttwid"))
-                elif response.status_code == 404:
-                    raise APINotFoundError(_("无法找到API端点"))
+                ttwid = httpx.Cookies(response.cookies).get("ttwid")
+
+                if ttwid is None:
+                    raise APIResponseError(
+                        _("ttwid: 检查没有通过, 请更新配置文件中的ttwid")
+                    )
 
-                ttwid = str(httpx.Cookies(response.cookies).get("ttwid"))
                 return ttwid
 
-            except httpx.RequestError:
+            except httpx.RequestError as exc:
                 # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
                 raise APIConnectionError(
                     _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(cls.ttwid_conf["url"], cls.proxies, cls.__name__)
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(cls.ttwid_conf["url"], cls.proxies, cls.__name__, exc)
                 )
 
             except httpx.HTTPStatusError as e:
                 # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
-                raise APIResponseError(
-                    f"HTTP Status Code {e.response.status_code}: {e.response.text}"
-                )
+                if response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _(
+                            "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+                        ).format("ttwid", "tiktok")
+                    )
 
+                elif response.status_code == 404:
+                    raise APINotFoundError(_("{0} 无法找到API端点").format("ttwid"))
+                else:
+                    raise APIResponseError(
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            e.response.url, e.response.status_code, e.response.text
+                        )
+                    )
 
-class VerifyFpManager:
     @classmethod
-    def gen_verify_fp(cls) -> str:
+    def gen_odin_tt(cls):
         """
-        生成verifyFp 与 s_v_web_id (Generate verifyFp)
+        生成请求必带的odin_tt (Generate the essential odin_tt for requests)
         """
-        base_str = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
-        t = len(base_str)
-        milliseconds = int(round(time.time() * 1000))
-        base36 = ""
-        while milliseconds > 0:
-            remainder = milliseconds % 36
-            if remainder < 10:
-                base36 = str(remainder) + base36
-            else:
-                base36 = chr(ord("a") + remainder - 10) + base36
-            milliseconds = int(milliseconds / 36)
-        r = base36
-        o = [""] * 36
-        o[8] = o[13] = o[18] = o[23] = "_"
-        o[14] = "4"
+        transport = httpx.HTTPTransport(retries=5)
+        with httpx.Client(transport=transport, proxies=cls.proxies) as client:
+            try:
+                response = client.get(cls.odin_tt_conf["url"])
+                response.raise_for_status()
 
-        for i in range(36):
-            if not o[i]:
-                n = 0 or int(random.random() * t)
-                if i == 19:
-                    n = 3 & n | 8
-                o[i] = base_str[n]
+                odin_tt = httpx.Cookies(response.cookies).get("odin_tt")
 
-        return "verify_" + r + "_" + "".join(o)
+                if odin_tt is None:
+                    raise APIResponseError(_("{0} 内容不符合要求").format("odin_tt"))
 
-    @classmethod
-    def gen_s_v_web_id(cls) -> str:
-        return cls.gen_verify_fp()
+                return odin_tt
+
+            except httpx.RequestError as exc:
+                # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
+                raise APIConnectionError(
+                    _(
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(cls.odin_tt_conf["url"], cls.proxies, cls.__name__, exc)
+                )
+
+            except httpx.HTTPStatusError as e:
+                # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
+                if response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _(
+                            "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+                        ).format("odin_tt", "tiktok")
+                    )
+
+                elif response.status_code == 404:
+                    raise APINotFoundError(_("{0} 无法找到API端点").format("odin_tt"))
+                else:
+                    raise APIResponseError(
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            e.response.url, e.response.status_code, e.response.text
+                        )
+                    )
 
 
 class XBogusManager:
     @classmethod
-    def str_2_endpoint(cls, endpoint: str) -> str:
+    def str_2_endpoint(
+        cls,
+        user_agent: str,
+        endpoint: str,
+    ) -> str:
         try:
-            final_endpoint = XB().getXBogus(endpoint)
+            final_endpoint = XB(user_agent).getXBogus(endpoint)
         except Exception as e:
             raise RuntimeError(_("生成X-Bogus失败: {0})").format(e))
 
         return final_endpoint[0]
 
     @classmethod
-    def model_2_endpoint(cls, base_endpoint: str, params: dict) -> str:
+    def model_2_endpoint(
+        cls,
+        user_agent: str,
+        base_endpoint: str,
+        params: dict,
+    ) -> str:
+        # 检查params是否是一个字典 (Check if params is a dict)
         if not isinstance(params, dict):
             raise TypeError(_("参数必须是字典类型"))
 
         param_str = "&".join([f"{k}={v}" for k, v in params.items()])
 
         try:
-            xb_value = XB().getXBogus(param_str)
+            xb_value = XB(user_agent).getXBogus(param_str)
         except Exception as e:
             raise RuntimeError(_("生成X-Bogus失败: {0})").format(e))
 
         # 检查base_endpoint是否已有查询参数 (Check if base_endpoint already has query parameters)
         separator = "&" if "?" in base_endpoint else "?"
 
         final_endpoint = f"{base_endpoint}{separator}{param_str}&X-Bogus={xb_value[1]}"
 
         return final_endpoint
 
 
 class SecUserIdFetcher:
     # 预编译正则表达式
-    _DOUYIN_URL_PATTERN = re.compile(r"user/([^/?]*)")
-    _REDIRECT_URL_PATTERN = re.compile(r"sec_uid=([^&]*)")
+    _TIKTOK_SECUID_PARREN = re.compile(
+        r"<script id=\"__UNIVERSAL_DATA_FOR_REHYDRATION__\" type=\"application/json\">(.*?)</script>"
+    )
+    _TIKTOK_UNIQUEID_PARREN = re.compile(r"/@([^/?]*)")
+    _TIKTOK_NOTFOUND_PARREN = re.compile(r"notfound")
 
     @classmethod
-    async def get_sec_user_id(cls, url: str) -> str:
+    async def get_secuid(cls, url: str) -> str:
         """
-        从单个url中获取sec_user_id (Get sec_user_id from a single url)
-
+        获取TikTok用户sec_uid
         Args:
-            url (str): 输入的url (Input url)
-
-        Returns:
-            str: 匹配到的sec_user_id (Matched sec_user_id)。
+            url: 用户主页链接
+        Return:
+            sec_uid: 用户唯一标识
         """
 
+        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError(_("参数必须是字符串类型"))
+            raise TypeError("输入参数必须是字符串")
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
 
-        pattern = (
-            cls._REDIRECT_URL_PATTERN
-            if "v.douyin.com" in url
-            else cls._DOUYIN_URL_PATTERN
-        )
-
-        try:
-            transport = httpx.AsyncHTTPTransport(retries=5)
-            async with httpx.AsyncClient(
-                transport=transport, proxies=TokenManager.proxies, timeout=10
-            ) as client:
+        transport = httpx.AsyncHTTPTransport(retries=5)
+        async with httpx.AsyncClient(
+            transport=transport, proxies=TokenManager.proxies, timeout=10
+        ) as client:
+            try:
                 response = await client.get(url, follow_redirects=True)
-
+                # 444一般为Nginx拦截，不返回状态 (444 is generally intercepted by Nginx and does not return status)
                 if response.status_code in {200, 444}:
-                    match = pattern.search(str(response.url))
-                    if match:
-                        return match.group(1)
-                    else:
+                    if cls._TIKTOK_NOTFOUND_PARREN.search(str(response.url)):
+                        raise APINotFoundError(
+                            _(
+                                "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
+                            ).format(cls.__name__)
+                        )
+
+                    match = cls._TIKTOK_SECUID_PARREN.search(str(response.text))
+                    if not match:
                         raise APIResponseError(
                             _(
-                                "未在响应的地址中找到sec_user_id, 检查链接是否为用户主页类名: {0}".format(
-                                    cls.__name__
-                                )
-                            )
+                                "未在响应中找到 {0}，检查链接是否为用户主页。类名: {1}"
+                            ).format("sec_uid", cls.__name__)
                         )
 
-                elif response.status_code == 401:
-                    raise APIUnauthorizedError(
-                        _("未授权的请求。类名: {0}".format(cls.__name__))
-                    )
-                elif response.status_code == 404:
-                    raise APINotFoundError(
-                        _("未找到API端点。类名: {0}".format(cls.__name__))
-                    )
-                elif response.status_code == 503:
-                    raise APIUnavailableError(
-                        _("API服务不可用。类名: {0}".format(cls.__name__))
-                    )
-                else:
-                    raise APIError(
-                        _("API错误码：{0}。类名: {1}").format(
-                            response.status_code, cls.__name__
+                    # 提取SIGI_STATE对象中的sec_uid
+                    data = json.loads(match.group(1))
+                    default_scope = data.get("__DEFAULT_SCOPE__", {})
+                    user_detail = default_scope.get("webapp.user-detail", {})
+                    user_info = user_detail.get("userInfo", {}).get("user", {})
+                    sec_uid = user_info.get("secUid")
+
+                    if sec_uid is None:
+                        raise RuntimeError(
+                            _("获取 {0} 失败，{1}").format(sec_uid, user_info)
                         )
-                    )
 
-        except httpx.RequestError:
-            raise APIConnectionError(
-                _(
-                    "连接到API时发生错误，请检查URL或网络情况。类名: {0}".format(
-                        cls.__name__
-                    )
-                ),
-                url,
-            )
+                    return sec_uid
+                else:
+                    raise ConnectionError(_("接口状态码异常, 请检查重试"))
+
+            except httpx.RequestError as exc:
+                # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
+                raise APIConnectionError(
+                    _(
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(url, TokenManager.proxies, cls.__name__, exc)
+                )
 
     @classmethod
-    async def get_all_sec_user_id(cls, urls: list) -> list:
+    async def get_all_secuid(cls, urls: list) -> list:
         """
-        获取列表sec_user_id列表 (Get list sec_user_id list)
+        获取列表secuid列表 (Get list sec_user_id list)
 
         Args:
             urls: list: 用户url列表 (User url list)
 
         Return:
-            sec_user_ids: list: 用户sec_user_id列表 (User sec_user_id list)
+            secuids: list: 用户secuid列表 (User secuid list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        sec_user_ids = [cls.get_sec_user_id(url) for url in urls]
-        return await asyncio.gather(*sec_user_ids)
-
-
-class AwemeIdFetcher:
-    # 预编译正则表达式
-    _DOUYIN_VIDEO_URL_PATTERN = re.compile(r"video/([^/?]*)")
-    _DOUYIN_NOTE_URL_PATTERN = re.compile(r"note/([^/?]*)")
+        secuids = [cls.get_secuid(url) for url in urls]
+        return await asyncio.gather(*secuids)
 
     @classmethod
-    async def get_aweme_id(cls, url: str) -> str:
+    async def get_uniqueid(cls, url: str) -> str:
         """
-        从单个url中获取aweme_id (Get aweme_id from a single url)
-
+        获取TikTok用户unique_id
         Args:
-            url (str): 输入的url (Input url)
-
-        Returns:
-            str: 匹配到的aweme_id (Matched aweme_id)。
+            url: 用户主页链接
+        Return:
+            unique_id: 用户唯一id
         """
 
+        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError(_("参数必须是字符串类型"))
+            raise TypeError("输入参数必须是字符串")
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
 
-        # 重定向到完整链接
         transport = httpx.AsyncHTTPTransport(retries=5)
         async with httpx.AsyncClient(
             transport=transport, proxies=TokenManager.proxies, timeout=10
         ) as client:
             try:
                 response = await client.get(url, follow_redirects=True)
 
-                video_pattern = cls._DOUYIN_VIDEO_URL_PATTERN
-                note_pattern = cls._DOUYIN_NOTE_URL_PATTERN
+                if response.status_code in {200, 444}:
+                    if cls._TIKTOK_NOTFOUND_PARREN.search(str(response.url)):
+                        raise APINotFoundError(
+                            _(
+                                "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
+                            ).format(cls.__name__)
+                        )
 
-                match = video_pattern.search(str(response.url))
-                if match:
-                    aweme_id = match.group(1)
-                else:
-                    match = note_pattern.search(str(response.url))
-                    if match:
-                        aweme_id = match.group(1)
-                    else:
+                    match = cls._TIKTOK_UNIQUEID_PARREN.search(str(response.url))
+                    if not match:
                         raise APIResponseError(
-                            _("未在响应的地址中找到aweme_id, 检查链接是否为作品页")
+                            _("未在响应中找到 {0}").format("unique_id")
                         )
-                return aweme_id
+
+                    unique_id = match.group(1)
+
+                    if unique_id is None:
+                        raise RuntimeError(
+                            _("获取 {0} 失败，{1}").format("unique_id", response.url)
+                        )
+
+                    return unique_id
+                else:
+                    raise ConnectionError(
+                        _("接口状态码异常 {0}, 请检查重试").format(response.status_code)
+                    )
 
             except httpx.RequestError:
                 raise APIConnectionError(
                     _(
                         "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(
-                        url,
-                        TokenManager.proxies,
-                        cls.__name__,
-                    )
+                    ).format(url, TokenManager.proxies, cls.__name__),
                 )
 
     @classmethod
-    async def get_all_aweme_id(cls, urls: list) -> list:
+    async def get_all_uniqueid(cls, urls: list) -> list:
         """
-        获取视频aweme_id,传入列表url都可以解析出aweme_id (Get video aweme_id, pass in the list url can parse out aweme_id)
+        获取列表unique_id列表 (Get list sec_user_id list)
 
         Args:
-            urls: list: 列表url (list url)
+            urls: list: 用户url列表 (User url list)
 
         Return:
-            aweme_ids: list: 视频的唯一标识，返回列表 (The unique identifier of the video, return list)
+            unique_ids: list: 用户unique_id列表 (User unique_id list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        aweme_ids = [cls.get_aweme_id(url) for url in urls]
-        return await asyncio.gather(*aweme_ids)
-
+        unique_ids = [cls.get_uniqueid(url) for url in urls]
+        return await asyncio.gather(*unique_ids)
 
-class MixIdFetcher:
-    @classmethod
-    async def get_mix_id(cls, url: str) -> str:
-        return
 
+class AwemeIdFetcher:
+    # https://www.tiktok.com/@scarlettjonesuk/video/7255716763118226715
+    # https://www.tiktok.com/@scarlettjonesuk/video/7255716763118226715?is_from_webapp=1&sender_device=pc&web_id=7306060721837852167
 
-class WebCastIdFetcher:
     # 预编译正则表达式
-    _DOUYIN_LIVE_URL_PATTERN = re.compile(r"live/([^/?]*)")
-    # https://live.douyin.com/766545142636?cover_type=0&enter_from_merge=web_live&enter_method=web_card&game_name=&is_recommend=1&live_type=game&more_detail=&request_id=20231110224012D47CD00C18B4AE4BFF9B&room_id=7299828646049827596&stream_type=vertical&title_type=1&web_live_page=hot_live&web_live_tab=all
-    # https://live.douyin.com/766545142636
-    _DOUYIN_LIVE_URL_PATTERN2 = re.compile(r"https://live.douyin.com/(\d+)")
-    # https://webcast.amemv.com/douyin/webcast/reflow/7318296342189919011?u_code=l1j9bkbd&did=MS4wLjABAAAAEs86TBQPNwAo-RGrcxWyCdwKhI66AK3Pqf3ieo6HaxI&iid=MS4wLjABAAAA0ptpM-zzoliLEeyvWOCUt-_dQza4uSjlIvbtIazXnCY&with_sec_did=1&use_link_command=1&ecom_share_track_params=&extra_params={"from_request_id":"20231230162057EC005772A8EAA0199906","im_channel_invite_id":"0"}&user_id=3644207898042206&liveId=7318296342189919011&from=share&style=share&enter_method=click_share&roomId=7318296342189919011&activity_info={}
-    _DOUYIN_LIVE_URL_PATTERN3 = re.compile(r"reflow/([^/?]*)")
+    _TIKTOK_AWEMEID_PARREN = re.compile(r"video/(\d*)")
+    _TIKTOK_NOTFOUND_PARREN = re.compile(r"notfound")
 
     @classmethod
-    async def get_webcast_id(cls, url: str) -> str:
+    async def get_aweme_id(cls, url: str) -> str:
         """
-        从单个url中获取webcast_id (Get webcast_id from a single url)
-
+        获取TikTok作品aweme_id
         Args:
-            url (str): 输入的url (Input url)
-
-        Returns:
-            str: 匹配到的webcast_id (Matched webcast_id)。
+            url: 作品链接
+        Return:
+            aweme_id: 作品唯一标识
         """
 
+        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError(_("参数必须是字符串类型"))
+            raise TypeError("输入参数必须是字符串")
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
 
-        # 重定向到完整链接
         transport = httpx.AsyncHTTPTransport(retries=5)
         async with httpx.AsyncClient(
             transport=transport, proxies=TokenManager.proxies, timeout=10
         ) as client:
-            response = await client.get(url, follow_redirects=True)
-            url = str(response.url)
+            try:
+                response = await client.get(url, follow_redirects=True)
 
-        live_pattern = cls._DOUYIN_LIVE_URL_PATTERN
-        live_pattern2 = cls._DOUYIN_LIVE_URL_PATTERN2
-        live_pattern3 = cls._DOUYIN_LIVE_URL_PATTERN3
-
-        if live_pattern.search(url):
-            match = live_pattern.search(url)
-        elif live_pattern2.search(url):
-            match = live_pattern2.search(url)
-        elif live_pattern3.search(url):
-            match = live_pattern3.search(url)
-            logger.debug(
-                _(
-                    "该链接返回的是room_id，请使用`fetch_user_live_videos_by_room_id`接口"
-                )
-            )
-        else:
-            raise APIResponseError(
-                _("未在响应的地址中找到webcast_id, 检查链接是否为直播页")
-            )
+                if response.status_code in {200, 444}:
+                    if cls._TIKTOK_NOTFOUND_PARREN.search(str(response.url)):
+                        raise APINotFoundError(
+                            _(
+                                "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
+                            ).format(cls.__name__)
+                        )
+
+                    match = cls._TIKTOK_AWEMEID_PARREN.search(str(response.url))
+                    if not match:
+                        raise APIResponseError(
+                            _("未在响应中找到 {0}").format("aweme_id")
+                        )
+
+                    aweme_id = match.group(1)
 
-        return match.group(1)
+                    if aweme_id is None:
+                        raise RuntimeError(
+                            _("获取 {0} 失败，{1}").format("aweme_id", response.url)
+                        )
+
+                    return aweme_id
+                else:
+                    raise ConnectionError(
+                        _("接口状态码异常 {0}，请检查重试").format(response.status_code)
+                    )
+
+            except httpx.RequestError as exc:
+                # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
+                raise APIConnectionError(
+                    _(
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(url, TokenManager.proxies, cls.__name__, exc)
+                )
 
     @classmethod
-    async def get_all_webcast_id(cls, urls: list) -> list:
+    async def get_all_aweme_id(cls, urls: list) -> list:
         """
-        获取直播webcast_id,传入列表url都可以解析出webcast_id (Get live webcast_id, pass in the list url can parse out webcast_id)
+        获取视频aweme_id,传入列表url都可以解析出aweme_id (Get video aweme_id, pass in the list url can parse out aweme_id)
 
         Args:
             urls: list: 列表url (list url)
 
         Return:
-            webcast_ids: list: 直播的唯一标识，返回列表 (The unique identifier of the live, return list)
+            aweme_ids: list: 视频的唯一标识，返回列表 (The unique identifier of the video, return list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        webcast_ids = [cls.get_webcast_id(url) for url in urls]
-        return await asyncio.gather(*webcast_ids)
+        aweme_ids = [cls.get_aweme_id(url) for url in urls]
+        return await asyncio.gather(*aweme_ids)
 
 
 def format_file_name(
     naming_template: str,
     aweme_data: dict = {},
     custom_fields: dict = {},
 ) -> str:
@@ -546,45 +582,45 @@
         "win32": 200,
         "cygwin": 60,
         "darwin": 60,
         "linux": 60,
     }
 
     fields = {
-        "create": aweme_data.get("create_time", ""),  # 长度固定19
+        "create": aweme_data.get("createTime", ""),  # 长度固定19
         "nickname": aweme_data.get("nickname", ""),  # 最长30
         "aweme_id": aweme_data.get("aweme_id", ""),  # 长度固定19
         "desc": split_filename(aweme_data.get("desc", ""), os_limit),
         "uid": aweme_data.get("uid", ""),  # 固定11
     }
 
     if custom_fields:
         # 更新自定义字段
         fields.update(custom_fields)
 
     try:
         return naming_template.format(**fields)
     except KeyError as e:
-        raise KeyError(_("文件名模板字段 {0} 不存在，请检查".format(e)))
+        raise KeyError(_("文件名模板字段 {0} 不存在，请检查").format(e))
 
 
 def create_user_folder(kwargs: dict, nickname: Union[str, int]) -> Path:
     """
     根据提供的配置文件和昵称，创建对应的保存目录。
     (Create the corresponding save directory according to the provided conf file and nickname.)
 
     Args:
         kwargs (dict): 配置文件，字典格式。(Conf file, dict format)
         nickname (Union[str, int]): 用户的昵称，允许字符串或整数。  (User nickname, allow strings or integers)
 
     Note:
         如果未在配置文件中指定路径，则默认为 "Download"。
         (If the path is not specified in the conf file, it defaults to "Download".)
-        支持绝对与相对路径。
-        (Support absolute and relative paths)
+        仅支持相对路径。
+        (Only relative paths are supported.)
 
     Raises:
         TypeError: 如果 kwargs 不是字典格式，将引发 TypeError。
         (If kwargs is not in dict format, TypeError will be raised.)
     """
 
     # 确定函数参数是否正确
@@ -592,15 +628,15 @@
         raise TypeError("kwargs 参数必须是字典")
 
     # 创建基础路径
     base_path = Path(kwargs.get("path", "Download"))
 
     # 添加下载模式和用户名
     user_path = (
-        base_path / "douyin" / kwargs.get("mode", "PLEASE_SETUP_MODE") / str(nickname)
+        base_path / "tiktok" / kwargs.get("mode", "PLEASE_SETUP_MODE") / str(nickname)
     )
 
     # 获取绝对路径并确保它存在
     resolve_user_path = user_path.resolve()
 
     # 创建目录
     resolve_user_path.mkdir(parents=True, exist_ok=True)
@@ -648,28 +684,7 @@
         return user_path
 
     if local_user_data.get("nickname") != current_nickname:
         # 昵称不一致，触发目录更新操作
         user_path = rename_user_folder(user_path, current_nickname)
 
     return user_path
-
-
-def show_qrcode(qrcode_url: str, show_image: bool = False) -> None:
-    """
-    显示二维码
-
-    Args:
-        qrcode_url (str): 登录二维码链接
-        show_image (bool): 是否显示图像，True 表示显示，False 表示在控制台显示
-    """
-    if show_image:
-        # 创建并显示QR码图像
-        qr_code_img = qrcode.make(qrcode_url)
-        qr_code_img.show()
-    else:
-        # 在控制台以 ASCII 形式打印二维码
-        qr = qrcode.QRCode()
-        qr.add_data(qrcode_url)
-        qr.make(fit=True)
-        # 在控制台以 ASCII 形式打印二维码
-        qr.print_ascii(invert=True)
```

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_apps_model.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_apps_model.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_aweme_id.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_aweme_id.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_crawler.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_crawler.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_handler.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_room_id.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_room_id.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_sec_user_id.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_sec_user_id.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/douyin/test/test_webcast_id.py` & `f2-0.0.1.5/f2/apps/douyin/test/test_webcast_id.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/tiktok/api.py` & `f2-0.0.1.5/f2/apps/tiktok/api.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/tiktok/cli.py` & `f2-0.0.1.5/f2/apps/tiktok/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # path: f2/apps/tiktok/cli.py
 
 import f2
 import click
 import typing
-import browser_cookie3
 
 from pathlib import Path
 
 from f2 import helps
 from f2.cli.cli_commands import set_cli_config
 from f2.log.logger import logger
-from f2.utils.utils import split_dict_cookie, get_resource_path
+from f2.utils.utils import (
+    split_dict_cookie,
+    get_resource_path,
+    get_cookie_from_browser,
+    check_invalid_naming,
+    merge_config,
+)
 from f2.utils.conf_manager import ConfigManager
 from f2.i18n.translator import TranslationManager, _
 
 
-def handle_help(
+def handler_help(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> None:
     """
     处理帮助信息 (Handle help messages)
 
@@ -46,78 +51,53 @@
     用于自动从浏览器获取cookie (Used to automatically get cookies from the browser)
 
     Args:
         ctx: click的上下文对象 (Click's context object)
         param: 提供的参数或选项 (The provided parameter or option)
         value: 参数或选项的值 (The value of the parameter or option)
     """
-    if not value or ctx.resilient_parsing:
-        return
-
-    # 如果用户明确设置了 --cookie，那么跳过自动获取过程
-    if ctx.params.get("cookie"):
+    # 如果用户没有提供值或者设置了 resilient_parsing 或者设置了 --cookie，那么跳过自动获取过程
+    if not value or ctx.resilient_parsing or ctx.params.get("cookie"):
         return
 
     # 根据浏览器选择获取cookie
-    if value in ["chrome", "firefox", "edge", "opera"]:
-        try:
-            cookie_value = split_dict_cookie(get_cookie_from_browser(value))
-            manager = ConfigManager(ctx.params.get("config", "conf/app.yaml"))
-            manager.update_config_with_args("tiktok", cookie=cookie_value)
-        except PermissionError:
-            message = _("请关闭所有已打开的浏览器重试, 并且你有适当的权限访问浏览器 !")
-            logger.error(message)
-            click.echo(message)
-            ctx.abort()
-        except Exception as e:
-            message = _("自动获取Cookie失败: {0}".format(str(e)))
-            logger.error(message)
-            click.echo(message)
-            ctx.abort()
-
-
-def get_cookie_from_browser(browser_choice: str):
-    """
-    根据用户选择的浏览器获取tiktok.com的cookie。
-
-    Args:
-        browser_choice (str): 用户选择的浏览器名称
-
-    Returns:
-        str: *.tiktok.com的cookie值
-    """
-
-    BROWSER_FUNCTIONS = {
-        "chrome": browser_cookie3.chrome,
-        "firefox": browser_cookie3.firefox,
-        "edge": browser_cookie3.edge,
-        "opera": browser_cookie3.opera,
-    }
-    cj_function = BROWSER_FUNCTIONS.get(browser_choice)
-    if not cj_function:
-        raise ValueError(_("不支持的浏览器选项, 输入f2 dy --help查看更多帮助!"))
-
-    cj = cj_function(domain_name="tiktok.com")
+    try:
+        cookie_value = split_dict_cookie(get_cookie_from_browser(value, "tiktok.com"))
 
-    # cookie_value = next((c.value for c in cj if c.name == 'ttwid'), None)
-    cookie_value = {c.name: c.value for c in cj if c.domain.endswith("tiktok.com")}
+        if not cookie_value:
+            raise ValueError(_("无法从 {0} 浏览器中获取cookie").format(value))
 
-    if not cookie_value:
-        raise ValueError(_("无法从{0}浏览器中获取cookie").format(browser_choice))
-
-    return cookie_value
+        # 如果没有提供配置文件，那么使用高频配置文件
+        manager = ConfigManager(
+            ctx.params.get("config", get_resource_path(f2.APP_CONFIG_FILE_PATH))
+        )
+        manager.update_config_with_args("tiktok", cookie=cookie_value)
+    except PermissionError:
+        logger.error(_("请关闭所有已打开的浏览器重试，并且你有适当的权限访问浏览器！"))
+        ctx.abort()
+    except Exception as e:
+        logger.error(_("自动获取Cookie失败：{0}").format(str(e)))
+        ctx.abort()
 
 
 def handler_language(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> typing.Any:
-    """用于设置语言 (For setting the language)"""
+    """用于设置语言 (For setting the language)
 
+    Args:
+        ctx: click的上下文对象 (Click's context object)
+        param: 提供的参数或选项 (The provided parameter or option)
+        value: 参数或选项的值 (The value of the parameter or option)
+    """
+
+    if not value or ctx.resilient_parsing:
+        return
     TranslationManager.get_instance().set_language(value)
     global _
     _ = TranslationManager.get_instance().gettext
     return value
 
 
 def handler_naming(
@@ -135,85 +115,34 @@
     Raises:
         click.BadParameter: 如果命名模式无效 (If the naming pattern is invalid)
 
     Returns:
         value: 命名模式模板 (Naming pattern template)
     """
     # 避免和配置文件参数冲突
-    if value is None:
+    if not value or ctx.resilient_parsing:
         return
 
     # 允许的模式和分隔符
-    ALLOWED_PATTERNS = ["{nickname}", "{create}", "{aid}", "{desc}"]
+    ALLOWED_PATTERNS = ["{nickname}", "{create}", "{aweme_id}", "{desc}", "{uid}"]
     ALLOWED_SEPARATORS = ["-", "_"]
 
-    temp_naming = value
-    invalid_patterns = []
-
-    # 检查提供的模式是否有效
-    for pattern in ALLOWED_PATTERNS:
-        if pattern in temp_naming:
-            temp_naming = temp_naming.replace(pattern, "")
-
-    # 此时，temp_naming应只包含分隔符
-    for char in temp_naming:
-        if char not in ALLOWED_SEPARATORS:
-            invalid_patterns.append(char)
-
-    # 检查连续的无效模式或分隔符
-    for pattern in ALLOWED_PATTERNS:
-        # 检查像"{aid}{aid}"这样的模式
-        if pattern + pattern in value:
-            invalid_patterns.append(pattern + pattern)
-        for sep in ALLOWED_SEPARATORS:
-            # 检查像"{aid}-{aid}"这样的模式
-            if pattern + sep + pattern in value:
-                invalid_patterns.append(pattern + sep + pattern)
+    # 检查命名是否符合命名规范
+    invalid_patterns = check_invalid_naming(value, ALLOWED_PATTERNS, ALLOWED_SEPARATORS)
 
     if invalid_patterns:
         raise click.BadParameter(
-            _(
-                "`{0}` 中的 `{1}` 不符合命名模式".format(
-                    value, "".join(invalid_patterns)
-                )
+            _("`{0}` 中的 `{1}` 不符合命名模式").format(
+                value, "".join(invalid_patterns)
             )
         )
 
     return value
 
 
-def merge_config(main_conf, custom_conf, **kwargs):
-    """
-    合并配置参数，使 CLI 参数优先级高于自定义配置，自定义配置优先级高于主配置，最终生成完整配置参数字典。
-    Args:
-        main_conf (dict): 主配置参数字典
-        custom_conf (dict): 自定义配置参数字典
-        **kwargs: CLI 参数和其他额外的配置参数
-
-    Returns:
-        dict: 合并后的配置参数字典
-    """
-    # 合并主配置和自定义配置
-    merged_conf = {}
-    for key, value in main_conf.items():
-        merged_conf[key] = value  # 将主配置复制到合并后的配置中
-    for key, value in custom_conf.items():
-        if value is not None and value != "":  # 只有值不为 None 和 空值，才进行合并
-            merged_conf[key] = value  # 自定义配置参数会覆盖主配置中的同名参数
-
-    # 合并 CLI 参数与合并后的配置，确保 CLI 参数的优先级最高
-    for key, value in kwargs.items():
-        if key not in merged_conf:  # 如果合并后的配置中没有这个键，则直接添加
-            merged_conf[key] = value
-        elif value is not None and value != "":  # 如果值不为 None 和 空值，则进行合并
-            merged_conf[key] = value  # CLI 参数会覆盖自定义配置和主配置中的同名参数
-
-    return merged_conf
-
-
 @click.command(name="tiktok", help=_("TikTok无水印解析"))
 @click.option(
     "--config",
     "-c",
     type=click.Path(file_okay=True, dir_okay=False, readable=True),  # exists=True
     help=_("配置文件的路径，最低优先"),
 )
@@ -227,48 +156,48 @@
     ),
 )
 @click.option(
     "--music",
     "-m",
     type=bool,
     # default="yes",
-    help=_("是否保存视频原声。可选：'yes'、'no'"),
+    help=_("是否保存视频原声"),
 )
 @click.option(
     "--cover",
     "-v",
     type=bool,
     # default="yes",
-    help=_("是否保存视频封面。可选：'yes'、'no'"),
+    help=_("是否保存视频封面"),
 )
 @click.option(
     "--desc",
     "-d",
     type=bool,
     # default="yes",
-    help=_("是否保存视频文案。可选：'yes'、'no'"),
+    help=_("是否保存视频文案"),
 )
 @click.option(
     "--path",
     "-p",
     type=str,
     # default="Download",
-    help=_("作品保存位置，支持绝对与相对路径。"),
+    help=_("作品保存位置，支持绝对与相对路径"),
 )
 @click.option(
     "--folderize",
     "-f",
     type=bool,
     # default="yes",
-    help=_("是否将作品保存到单独的文件夹。可选：'yes'、'no'"),
+    help=_("是否将作品保存到单独的文件夹"),
 )
 @click.option(
     "--mode",
     "-M",
-    type=click.Choice(["one", "post", "like", "collect", "mix"]),
+    type=click.Choice(f2.TIKTOK_MODE_LIST),
     # default="post",
     # required=True,
     help=_(
         "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑播放列表(mix)"
     ),
 )
 @click.option(
@@ -363,31 +292,35 @@
 )
 @click.option(
     "--init-config", type=str, help=_("初始化配置文件。不能同时初始化和更新配置文件")
 )
 # @click.confirmation_option(prompt='是否要使用命令行的参数更新配置文件?')
 @click.option(
     "--auto-cookie",
-    type=click.Choice(["none", "chrome", "firefox", "edge", "opera"]),
+    type=click.Choice(f2.BROWSER_LIST),
     # default="none",
-    help=_(
-        "自动从浏览器获取cookie。可选项：chrome、firefox、edge、opera。使用该命令前请确保关闭所选的浏览器"
-    ),
+    help=_("自动从浏览器获取cookie，使用该命令前请确保关闭所选的浏览器"),
     callback=handler_auto_cookie,
 )
 @click.option(
     "-h",
     is_flag=True,
     is_eager=True,
     expose_value=False,
-    help="显示富文本帮助",
-    callback=handle_help,
+    help=_("显示富文本帮助"),
+    callback=handler_help,
 )
 @click.pass_context
-def tiktok(ctx, config, init_config, update_config, **kwargs):
+def tiktok(
+    ctx: click.Context,
+    config: str,
+    init_config: str,
+    update_config: bool,
+    **kwargs,
+) -> None:
     ##################
     # f2 存在2个主配置文件，分别是app低频配置(app.yaml)和f2低频配置(conf.yaml)
     # app低频配置存放app相关的参数
     # f2低频配置存放计算值所需的参数
 
     # 其中cli参数具有最高优先，cli >= 自定义 >= 低频
     # 在f2低频配置中设置代理参数
@@ -449,21 +382,21 @@
             "http": kwargs["proxies"][0],
             "https": kwargs["proxies"][1],
         }
 
     # 从低频配置开始到高频配置再到cli参数，逐级覆盖，如果键值不存在使用父级的键值
     kwargs = merge_config(main_conf, custom_conf, **kwargs)
 
-    logger.info(_("主配置路径： {0}".format(main_conf_path)))
-    logger.info(_("自定义配置路径： {0}".format(Path.cwd() / config)))
-    logger.debug(_("主配置参数：{0}".format(main_conf)))
-    logger.debug(_("自定义配置参数：{0}".format(custom_conf)))
-    logger.debug(_("CLI参数：{0}".format(kwargs)))
+    logger.info(_("主配置路径：{0}").format(main_conf_path))
+    logger.info(_("自定义配置路径：{0}").format(Path.cwd() / config))
+    logger.debug(_("主配置参数：{0}").format(main_conf))
+    logger.debug(_("自定义配置参数：{0}").format(custom_conf))
+    logger.debug(_("CLI参数：{0}").format(kwargs))
 
     # 尝试从命令行参数或kwargs中获取URL
     if not kwargs.get("url"):
         logger.error("缺乏URL参数，详情看命令帮助")
-        handle_help(ctx, None, True)
+        handler_help(ctx, None, True)
 
     # 添加app_name到kwargs
     kwargs["app_name"] = "tiktok"
     ctx.invoke(set_cli_config, **kwargs)
```

### Comparing `f2-0.0.1.4/f2/apps/tiktok/db.py` & `f2-0.0.1.5/f2/apps/tiktok/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # path: f2/apps/tiktok/db.py
 
-import aiosqlite
 from f2.db.base_db import BaseDB
 
 
 class AsyncUserDB(BaseDB):
     TABLE_NAME = "user_info_web"
 
     async def _create_table(self) -> None:
@@ -20,22 +19,24 @@
             "followerCount INTEGER",
             "followingCount INTEGER",
             "friendCount INTEGER",
             "heartCount INTEGER",
             "videoCount INTEGER",
             "uid TEXT",
             "nickname TEXT",
+            "nickname_raw TEXT",
             "uniqueId TEXT",
             "commentSetting BOOLEAN",
             "followingVisibility BOOLEAN",
             "openFavorite BOOLEAN",
             "privateAccount BOOLEAN",
             "showPlayListTab BOOLEAN",
             "relation BOOLEAN",
             "signature TEXT",
+            "signature_raw TEXT",
             "ttSeller BOOLEAN",
             "verified BOOLEAN",
             "last_aweme_id TEXT",
             "api_status_code TEXT",
         ]
 
         fields_sql = ", ".join(fields)
```

### Comparing `f2-0.0.1.4/f2/apps/tiktok/dl.py` & `f2-0.0.1.5/f2/apps/douyin/dl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# path: f2/apps/tiktok/dl.py
+# path: f2/apps/douyin/dl.py
 
 import sys
 from datetime import datetime
 from typing import Any, Union
 
 from f2.i18n.translator import _
 from f2.log.logger import logger
 from f2.dl.base_downloader import BaseDownloader
 from f2.utils.utils import get_timestamp, timestamp_2_str
-from f2.apps.tiktok.db import AsyncUserDB
-from f2.apps.tiktok.utils import format_file_name
+from f2.apps.douyin.db import AsyncUserDB
+from f2.apps.douyin.utils import format_file_name, json_2_lrc
 
 
-class TiktokDownloader(BaseDownloader):
+class DouyinDownloader(BaseDownloader):
     def __init__(self, kwargs: dict = {}):
         if kwargs["cookie"] is None:
             raise ValueError(
                 _(
-                    "cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取 f2 -d dy --help，如扫码登录请保留双引号cookie: "
-                    "，再使用--sso-login命令。"
+                    "cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取。如 `--auto-cookie edge`"
                 )
             )
 
         super().__init__(kwargs)
 
-    async def save_last_aweme_id(self, secUid: str, aweme_id: str) -> None:
+    async def save_last_aweme_id(self, sec_user_id: str, aweme_id: int) -> None:
         """
         保存最后一个请求的aweme_id
         (Save the last requested aweme_id)
 
         Args:
-            aweme_id (str): 作品id (aweme_id)
+            aweme_id (int): 作品id (aweme_id)
         """
 
-        async with AsyncUserDB("tiktok_users.db") as db:
-            await db.update_user_info(secUid=secUid, last_aweme_id=aweme_id)
+        async with AsyncUserDB("douyin_users.db") as db:
+            await db.update_user_info(sec_user_id=sec_user_id, last_aweme_id=aweme_id)
 
     async def filter_aweme_datas_by_interval(
         self, aweme_datas: Union[list, dict], interval: str
     ) -> Union[list[dict], dict, None]:
         """
         筛选指定日期区间内的作品
 
@@ -59,18 +58,16 @@
             start_date = datetime.strptime(start_str + " 00-00-00", "%Y-%m-%d %H-%M-%S")
             end_date = datetime.strptime(end_str + " 23-59-59", "%Y-%m-%d %H-%M-%S")
             logger.info(_("筛选日期区间：{0} 至 {1}").format(start_date, end_date))
         except ValueError:
             logger.error(_("日期区间参数格式错误，请查阅文档后重试"))
             return None
 
-        logger.info(aweme_datas)
-
         if isinstance(aweme_datas, dict):
-            aweme_date_str = aweme_datas.get("createTime")
+            aweme_date_str = aweme_datas.get("create_time")
             try:
                 aweme_date = datetime.strptime(aweme_date_str, "%Y-%m-%d %H-%M-%S")
             except ValueError:
                 logger.warning(_("无法解析作品发布时间：{0}").format(aweme_date_str))
                 return None
 
             # 检查作品发布时间是否在指定区间内
@@ -78,15 +75,17 @@
                 logger.info(
                     _("作品发布时间在指定区间内：作品id {0} 发布时间 {1}").format(
                         aweme_datas.get("aweme_id"), aweme_date_str
                     )
                 )
                 return aweme_datas
             else:
-                logger.warning(_("作品发布时间不在指定区间内：{0}").format(aweme_date_str))
+                logger.warning(
+                    _("作品发布时间不在指定区间内：{0}").format(aweme_date_str)
+                )
                 return None
 
         elif isinstance(aweme_datas, list):
             # 遍历列表中的每个字典
             filtered_list = []
             for aweme_data in aweme_datas:
                 filtered_data = await self.filter_aweme_datas_by_interval(
@@ -144,82 +143,78 @@
         self, kwargs: dict, aweme_data_dict: dict, user_path: Any
     ) -> None:
         """
         处理下载任务
 
         Args:
             kwargs (dict): 命令行参数
+            aweme_data_dict (dict): 作品数据字典
+            user_path (Any): 用户目录路径
         """
 
         # 构建文件夹路径
         base_path = (
             user_path
             / format_file_name(kwargs.get("naming", "{create}_{desc}"), aweme_data_dict)
             if kwargs.get("folderize")
             else user_path
         )
 
-        secUid = str(aweme_data_dict.get("secUid"))  # 用户ID
-        aweme_privateItem = aweme_data_dict.get("privateItem")  # 作品权限 false公开, true私密
-        aweme_secret = aweme_data_dict.get("secret")  # 作品权限 false公开, true私密
+        sec_user_id = str(aweme_data_dict.get("sec_user_id"))  # 用户ID
+        aweme_prohibited = aweme_data_dict.get("is_prohibited")  # 作品状态 0正常, 1屏蔽
+        aweme_part_see = aweme_data_dict.get(
+            "part_see"
+        )  # 部分可见 part_see 1, private_status 1
+        aweme_status = aweme_data_dict.get(
+            "private_status"
+        )  # 视频权限 0公开或不给谁看, 1私密, 2互关朋友
+        aweme_type = aweme_data_dict.get(
+            "aweme_type"
+        )  # 视频类型 0视频, 55动图或关闭下载, 61挑战， 109日常, 68图集
         aweme_id = str(aweme_data_dict.get("aweme_id"))  # 视频ID
 
         logger.debug(f"========{aweme_id}========")
         logger.debug(aweme_data_dict)
-        logger.debug("================")
+        logger.debug("===================================")
 
         # 检查作品是否被屏蔽
-        if aweme_privateItem:
-            logger.warning(_("{0} 该作品已被屏蔽，无法下载").format(aweme_id))
+        if aweme_prohibited:
+            logger.warning(_("该 {0} 作品已被屏蔽，无法下载").format(aweme_id))
             return
 
         # 检查作品是否可见
-        if not aweme_secret:
-            video_name = (
-                format_file_name(
-                    kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
-                )
-                + "_video"
-            )
-
-            video_url = aweme_data_dict.get("video_playAddr")
-            if video_url != None:
-                await self.initiate_download(
-                    _("视频"), video_url, base_path, video_name, ".mp4"
-                )
-            else:
-                logger.warning(_("{0} 该作品没有视频链接，无法下载").format(aweme_id))
-
+        if aweme_status in [0, 1, 2]:
             # 处理音乐下载任务
             if kwargs.get("music"):
-                music_name = (
-                    format_file_name(
-                        kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
+                if aweme_data_dict.get("music_status") == 1:  # 原声状态 1 正常 0 失效
+                    music_name = (
+                        format_file_name(
+                            kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
+                        )
+                        + "_music"
                     )
-                    + "_music"
-                )
 
-                music_url = aweme_data_dict.get("music_playUrl")
-                if music_url != None:
-                    await self.initiate_download(
-                        _("原声"), music_url, base_path, music_name, ".mp3"
-                    )
+                    music_url = aweme_data_dict.get("music_play_url")
+                    if music_url != None:
+                        await self.initiate_download(
+                            _("原声"), music_url, base_path, music_name, ".mp3"
+                        )
                 else:
                     logger.warning(_("{0} 该原声已被屏蔽，无法下载").format(aweme_id))
 
             # 处理封面下载任务
             if kwargs.get("cover"):
                 cover_name = (
                     format_file_name(
                         kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
                     )
                     + "_cover"
                 )
-                animated_cover_url = aweme_data_dict.get("video_dynamicCover")
-                cover_url = aweme_data_dict.get("video_cover")
+                animated_cover_url = aweme_data_dict.get("animated_cover")
+                cover_url = aweme_data_dict.get("cover")
                 if animated_cover_url != None:
                     await self.initiate_download(
                         _("封面"), animated_cover_url, base_path, cover_name, ".webp"
                     )
                 elif cover_url != None:
                     logger.warning(_("{0} 该作品没有动态封面").format(aweme_id))
                     await self.initiate_download(
@@ -237,27 +232,131 @@
                     + "_desc"
                 )
                 desc_content = aweme_data_dict.get("desc")
                 await self.initiate_static_download(
                     _("文案"), desc_content, base_path, desc_name, ".txt"
                 )
 
+            # 处理不同类型的作品下载任务
+            if aweme_type in [0, 55, 61, 109]:
+                video_name = (
+                    format_file_name(
+                        kwargs.get("naming", "{create}_{desc}"), aweme_data_dict
+                    )
+                    + "_video"
+                )
+                # video_play_addr 现在为一个list，第一个链接下载失败，则下载第二个链接
+                video_url = aweme_data_dict.get("video_play_addr")
+                if video_url != None:
+                    await self.initiate_download(
+                        _("视频"), video_url, base_path, video_name, ".mp4"
+                    )
+                else:
+                    logger.warning(
+                        _("{0} 该作品没有视频链接，无法下载").format(aweme_id)
+                    )
+
+            elif aweme_type in [68]:
+                for i, image_url in enumerate(aweme_data_dict.get("images", None)):
+                    image_name = f"{format_file_name(kwargs.get('naming'), aweme_data_dict)}_image_{i + 1}"
+                    if image_url != None:
+                        await self.initiate_download(
+                            _("图集"), image_url, base_path, image_name, ".jpg"
+                        )
+                    else:
+                        logger.warning(
+                            _("{0} 该图集没有图片链接，无法下载").format(aweme_id)
+                        )
+
         # 保存最后一个aweme_id
-        await self.save_last_aweme_id(secUid, aweme_id)
+        await self.save_last_aweme_id(sec_user_id, aweme_id)
+
+    async def create_music_download_tasks(
+        self, kwargs: dict, music_datas: Union[list, dict], user_path: Any
+    ) -> None:
+        """
+        创建音乐下载任务
+
+        Args:
+            kwargs (dict): 命令行参数
+            music_datas (list, dict): 音乐数据列表或字典
+            user_path (Any): 用户目录路径
+        """
+
+        if (
+            not kwargs
+            or not music_datas
+            or not isinstance(music_datas, (list, dict))
+            or not user_path
+        ):
+            return
+
+        if isinstance(music_datas, dict):
+            await self.handler_music_download(kwargs, music_datas, user_path)
+        else:
+            for music_data in music_datas:
+                await self.handler_music_download(kwargs, music_data, user_path)
+
+        # 执行下载任务
+        await self.execute_tasks()
+
+    async def handler_music_download(
+        self, kwargs: dict, music_data_dict: dict, user_path: Any
+    ) -> None:
+        """
+        处理音乐下载任务
+
+        Args:
+            kwargs (dict): 命令行参数
+            music_data_dict (dict): 音乐数据字典
+            user_path (Any): 用户目录路径
+        """
+
+        # 构建文件夹路径
+        base_path = (
+            user_path / music_data_dict.get("title")
+            if kwargs.get("folderize")
+            else user_path
+        )
+        music_name = music_data_dict.get("title") + "_music"
+        music_url = music_data_dict.get("play_url")
+        lyric_name = music_data_dict.get("title") + "_lyric"
+        lyric_url = music_data_dict.get("lyric_url")
+
+        if music_url != None:
+            await self.initiate_download(
+                _("音乐"), music_url, base_path, music_name, ".mp3"
+            )
+
+        if kwargs.get("lyric"):
+            if lyric_url is None:
+                return
+
+            # 下载str格式的json歌词文件
+            lyric = await self.get_fetch_data(lyric_url)
+
+            # 如果json歌词文件下载成功，则读取并处理成lrc格式
+            if lyric.status_code != 200:
+                return
+
+            lrc_content = json_2_lrc(lyric.json())
+            await self.initiate_static_download(
+                _("歌词"), lrc_content, base_path, lyric_name, ".lrc"
+            )
 
     async def create_stream_tasks(
         self, kwargs: dict, webcast_datas: Union[list, dict], user_path: Any
     ) -> None:
         """
         创建视频流下载任务
 
         Args:
             kwargs (dict): 命令行参数
             aweme_datas (list, dict): 作品数据列表或字典
-            user_path (str): 用户目录路径
+            user_path (Any): 用户目录路径
         """
 
         if (
             not kwargs
             or not webcast_datas
             or not isinstance(webcast_datas, (list, dict))
             or not user_path
@@ -277,14 +376,16 @@
         self, kwargs: dict, webcast_data_dict: dict, user_path: Any
     ) -> None:
         """
         处理视频流下载任务
 
         Args:
             kwargs (dict): 命令行参数
+            aweme_data_dict (dict): 直播数据字典
+            user_path (Any): 用户目录路径
         """
         custom_fields = {
             "create": timestamp_2_str(timestamp=get_timestamp(unit="sec")),
             "nickname": webcast_data_dict.get("nickname", ""),
             "aweme_id": webcast_data_dict.get("room_id", ""),
             "desc": webcast_data_dict.get("live_title", ""),
             "uid": webcast_data_dict.get("user_id", ""),
@@ -295,13 +396,13 @@
             / format_file_name(
                 kwargs.get("naming", "{create}_{desc}"), custom_fields=custom_fields
             )
             if kwargs.get("folderize")
             else user_path
         )
 
-        webcast_name = f"{format_file_name(kwargs.get('naming', '{create}_{desc}'), custom_fields=custom_fields)}_live"
-        webcast_url = webcast_data_dict.get("m3u8_pull_url", None).get("FULL_HD1")
+        webcast_name = f"{format_file_name(kwargs.get('naming'), custom_fields=custom_fields)}_live"
+        webcast_url = webcast_data_dict.get("m3u8_pull_url").get("FULL_HD1")
 
         await self.initiate_m3u8_download(
             _("直播"), webcast_url, base_path, webcast_name, ".mp4"
         )
```

### Comparing `f2-0.0.1.4/f2/apps/tiktok/filter.py` & `f2-0.0.1.5/f2/apps/tiktok/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # path: f2/apps/tiktok/filter.py
 
-from typing import List, Union
-
 from f2.utils.json_filter import JSONModel
 from f2.utils.utils import _get_first_item_from_list, timestamp_2_str, replaceT
 
 
 class UserProfileFilter(JSONModel):
     @property
     def api_status_code(self):
@@ -42,14 +40,18 @@
         return self._get_attr_value("$.userInfo.user.id")
 
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.userInfo.user.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.userInfo.user.nickname")
+
+    @property
     def secUid(self):
         return self._get_attr_value("$.userInfo.user.secUid")
 
     @property
     def uniqueId(self):
         return self._get_attr_value("$.userInfo.user.uniqueId")
 
@@ -78,21 +80,28 @@
         return bool(self._get_attr_value("$.userInfo.user.relation"))
 
     @property
     def signature(self):
         return replaceT(self._get_attr_value("$.userInfo.user.signature"))
 
     @property
+    def signature_raw(self):
+        return self._get_attr_value("$.userInfo.user.signature")
+
+    @property
     def ttSeller(self) -> bool:
         return bool(self._get_attr_value("$.userInfo.user.ttSeller"))
 
     @property
     def verified(self) -> bool:
         return bool(self._get_attr_value("$.userInfo.user.verified"))
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -129,24 +138,32 @@
         )
 
     @property
     def desc(self):
         return replaceT(self._get_list_attr_value("$.itemList[*].desc"))
 
     @property
+    def desc_raw(self):
+        return self._get_list_attr_value("$.itemList[*].desc")
+
+    @property
     def textExtra(self):
         return self._get_list_attr_value("$.itemList[*].textExtra")
 
     # author
 
     @property
     def nickname(self):
         return replaceT(self._get_list_attr_value("$.itemList[*].author.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_list_attr_value("$.itemList[*].author.nickname")
+
+    @property
     def uid(self):
         return self._get_list_attr_value("$.itemList[*].author.id")
 
     @property
     def secUid(self):
         return self._get_list_attr_value("$.itemList[*].author.secUid")
 
@@ -218,14 +235,18 @@
         return self._get_list_attr_value("$.itemList[*].music.album")
 
     @property
     def music_authorName(self):
         return replaceT(self._get_list_attr_value("$.itemList[*].music.authorName"))
 
     @property
+    def music_authorName_raw(self):
+        return self._get_list_attr_value("$.itemList[*].music.authorName")
+
+    @property
     def music_coverLarge(self):
         return self._get_list_attr_value("$.itemList[*].music.coverLarge")
 
     @property
     def music_duration(self):
         return self._get_list_attr_value("$.itemList[*].music.duration")
 
@@ -241,14 +262,18 @@
     def music_playUrl(self):
         return self._get_list_attr_value("$.itemList[*].music.playUrl")
 
     @property
     def music_title(self):
         return replaceT(self._get_list_attr_value("$.itemList[*].music.title"))
 
+    @property
+    def music_title_raw(self):
+        return self._get_list_attr_value("$.itemList[*].music.title")
+
     # video
     @property
     def video_bitrate(self):
         return self._get_list_attr_value("$.itemList[*].video.bitrate")
 
     # @property
     # def video_bitrateInfo(self):
@@ -262,19 +287,25 @@
     #         for aweme in bit_rate_data
     #     ]
 
     @property
     def video_bitrateInfo(self):
         bit_rate_data = self._get_list_attr_value("$.itemList[*].video.bitrateInfo")
         return [
-            [aweme.get("Bitrate", "")]  # 使用 get 方法以处理字典中没有 "Bitrate" 键的情况
-            if isinstance(aweme, dict)
-            else [aweme[0].get("Bitrate", "")]
-            if len(aweme) == 1
-            else [item.get("Bitrate", "") for item in aweme]
+            (
+                [
+                    aweme.get("Bitrate", "")
+                ]  # 使用 get 方法以处理字典中没有 "Bitrate" 键的情况
+                if isinstance(aweme, dict)
+                else (
+                    [aweme[0].get("Bitrate", "")]
+                    if len(aweme) == 1
+                    else [item.get("Bitrate", "") for item in aweme]
+                )
+            )
             for aweme in bit_rate_data
         ]
 
     @property
     def video_codecType(self):
         return self._get_list_attr_value("$.itemList[*].video.codecType")
 
@@ -302,14 +333,17 @@
     def video_height(self):
         return self._get_list_attr_value("$.itemList[*].video.height")
 
     @property
     def video_width(self):
         return self._get_list_attr_value("$.itemList[*].video.width")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -379,14 +413,17 @@
     def mixName(self):
         return self._get_attr_value("$.playList[*].mixName")
 
     @property
     def videoCount(self):
         return self._get_attr_value("$.playList[*].videoCount")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
 
@@ -414,26 +451,34 @@
         return self._get_attr_value("$.itemInfo.itemStruct.author.id")
 
     @property
     def nickname(self):
         return replaceT(self._get_attr_value("$.itemInfo.itemStruct.author.nickname"))
 
     @property
+    def nickname_raw(self):
+        return self._get_attr_value("$.itemInfo.itemStruct.author.nickname")
+
+    @property
     def secUid(self):
         return self._get_attr_value("$.itemInfo.itemStruct.author.secUid")
 
     @property
     def uniqueId(self):
         return self._get_attr_value("$.itemInfo.itemStruct.author.uniqueId")
 
     @property
     def signature(self):
         return replaceT(self._get_attr_value("$.itemInfo.itemStruct.author.signature"))
 
     @property
+    def signature_raw(self):
+        return self._get_attr_value("$.itemInfo.itemStruct.author.signature")
+
+    @property
     def openFavorite(self):
         return self._get_attr_value("$.itemInfo.itemStruct.author.openFavorite")
 
     @property
     def privateAccount(self):
         return self._get_attr_value("$.itemInfo.itemStruct.author.privateAccount")
 
@@ -458,14 +503,18 @@
         )
 
     @property
     def desc(self):
         return replaceT(self._get_attr_value("$.itemInfo.itemStruct.desc"))
 
     @property
+    def desc_raw(self):
+        return self._get_attr_value("$.itemInfo.itemStruct.desc")
+
+    @property
     def textExtra(self):
         return self._get_attr_value("$.itemInfo.itemStruct.textExtra")
 
     @property
     def aweme_id(self):
         return self._get_attr_value("$.itemInfo.itemStruct.id")
 
@@ -528,14 +577,18 @@
 
     # music
     @property
     def music_authorName(self):
         return replaceT(self._get_attr_value("$.itemInfo.itemStruct.music.authorName"))
 
     @property
+    def music_authorName_raw(self):
+        return self._get_attr_value("$.itemInfo.itemStruct.music.authorName")
+
+    @property
     def music_coverLarge(self):
         return self._get_attr_value("$.itemInfo.itemStruct.music.coverLarge")
 
     @property
     def music_duration(self):
         return self._get_attr_value("$.itemInfo.itemStruct.music.duration")
 
@@ -551,14 +604,18 @@
     def music_playUrl(self):
         return self._get_attr_value("$.itemInfo.itemStruct.music.playUrl")
 
     @property
     def music_title(self):
         return replaceT(self._get_attr_value("$.itemInfo.itemStruct.music.title"))
 
+    @property
+    def music_title_raw(self):
+        return self._get_attr_value("$.itemInfo.itemStruct.music.title")
+
     # video
     @property
     def video_bitrate(self):
         return self._get_attr_value("$.itemInfo.itemStruct.video.bitrate")
 
     @property
     def video_bitrateInfo(self):
@@ -595,14 +652,17 @@
     def video_height(self):
         return self._get_attr_value("$.itemInfo.itemStruct.video.height")
 
     @property
     def video_width(self):
         return self._get_attr_value("$.itemInfo.itemStruct.video.width")
 
+    def _to_raw(self) -> dict:
+        return self._data
+
     def _to_dict(self) -> dict:
         return {
             prop_name: getattr(self, prop_name)
             for prop_name in dir(self)
             if not prop_name.startswith("__") and not prop_name.startswith("_")
         }
```

### Comparing `f2-0.0.1.4/f2/apps/tiktok/help.py` & `f2-0.0.1.5/f2/apps/douyin/help.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# path: f2/apps/tiktok/help.py
+# path: f2/apps/douyin/help.py
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from f2.i18n.translator import _
 
@@ -20,28 +20,28 @@
         (
             "-u --url",
             "[dark_cyan]str",
             _(
                 "根据模式提供相应的链接。例如：主页、点赞、收藏作品填入主页链接，单作品填入作品链接，合辑与直播同上"
             ),
         ),
-        ("-m --music", "[dark_cyan]Choice", _("是否保存视频原声。可选：'yes'、'no'")),
-        ("-v --cover", "[dark_cyan]Choice", _("是否保存视频封面。可选：'yes'、'no'")),
-        ("-d --desc", "[dark_cyan]Choice", _("是否保存视频文案。可选：'yes'、'no'")),
+        ("-m --music", "[dark_cyan]Bool", _("是否保存视频原声")),
+        ("-v --cover", "[dark_cyan]Bool", _("是否保存视频封面")),
+        ("-d --desc", "[dark_cyan]Bool", _("是否保存视频文案")),
         ("-p --path", "[dark_cyan]str", _("作品保存位置，支持绝对与相对路径。")),
         (
             "-f --folderize",
-            "[dark_cyan]Choice",
-            _("是否将作品保存到单独的文件夹。可选：'yes'、'no'"),
+            "[dark_cyan]Bool",
+            _("是否将作品保存到单独的文件夹"),
         ),
         (
             "-M --mode",
             "[dark_cyan]Choice",
             _(
-                "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑播放列表(mix)"
+                "下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collection)，收藏夹作品(collects)，合辑(mix)，直播(live)"
             ),
         ),
         (
             "-n --naming",
             "[dark_cyan]str",
             _("全局作品文件命名方式，前往文档查看更多帮助"),
         ),
@@ -55,66 +55,68 @@
         (
             "-i --interval",
             "[dark_cyan]str",
             _(
                 "下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"
             ),
         ),
-        ("-e --timeout", "[dark_cyan]int", _("网络请求超时时间。")),
-        ("-r --max-retries", "[dark_cyan]int", _("网络请求超时重试数。")),
-        ("-x --max-connections", "[dark_cyan]int", _("网络请求并发连接数。")),
-        ("-t --max-tasks", "[dark_cyan]int", _("异步的任务数。")),
-        (
-            "-o --max-counts",
-            "[dark_cyan]int",
-            _("最大作品下载数。0 表示无限制"),
-        ),
+        ("-e --timeout", "[dark_cyan]int", _("网络请求超时时间")),
+        ("-r --max-retries", "[dark_cyan]int", _("网络请求超时重试数")),
+        ("-x --max-connections", "[dark_cyan]int", _("网络请求并发连接数")),
+        ("-t --max-tasks", "[dark_cyan]int", _("异步的任务数")),
+        ("-o --max-counts", "[dark_cyan]int", _("最大作品下载数。0 表示无限制")),
         (
             "-s --page-counts",
             "[dark_cyan]int",
-            _("从接口每页可获取作品数，不建议超过20。"),
+            _("从接口每页可获取作品数，不建议超过20"),
         ),
         (
             "-l --languages",
             "[dark_cyan]Choice",
             _("显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'"),
         ),
         (
             "-P --proxies",
             "[dark_cyan]str",
             _(
                 "代理服务器，最多 2 个参数，http与https。空格区分 2 个参数 http://x.x.x.x https://x.x.x.x"
             ),
         ),
+        ("-L --lyric", "[dark_cyan]Bool", _("是否保存视频歌词")),
         (
             "--update-config",
             "[dark_cyan]Flag",
             _("使用命令行选项更新配置文件。需要先使用'-c'选项提供一个配置文件路径"),
         ),
         (
             "--init-config",
             "[dark_cyan]Flag",
             _("初始化配置文件。不能同时初始化和更新配置文件"),
         ),
         (
             "--auto-cookie",
             "[dark_cyan]Choice",
             _(
-                "自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、opera。使用该命令前请确保关闭所选的浏览器"
+                "自动从浏览器获取[yellow]cookie[/yellow]，使用该命令前请确保关闭所选的浏览器"
             ),
         ),
+        (
+            "--sso-login",
+            "[dark_cyan]Flag",
+            _("使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"),
+        ),
         ("--help", "[dark_cyan]Flag", _("显示经典帮助信息")),
         (
             "",
             "",
             _(
                 "更加详细的参数说明请点击[link=https://johnserf-seed.github.io/f2/site-config.html][dark_violet]前往文档[/dark_violet][/]查看"
             ),
         ),
     ]
 
     for option in options:
         table.add_row(*option)
 
     console.print(
-        Panel(table, border_style="bold", title="[TikTok]", title_align="left")
+        Panel(table, border_style="bold", title="[DouYin]", title_align="left")
     )
```

### Comparing `f2-0.0.1.4/f2/apps/tiktok/model.py` & `f2-0.0.1.5/f2/apps/tiktok/model.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/apps/tiktok/utils.py` & `f2-0.0.1.5/f2/apps/douyin/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-# path: f2/apps/tiktok/utils.py
+# path: f2/apps/douyin/utils.py
 
 import f2
 import re
 import json
+import time
 import httpx
+import qrcode
+import random
 import asyncio
 
 from typing import Union
 from pathlib import Path
 
 from f2.i18n.translator import _
 from f2.log.logger import logger
@@ -19,24 +22,24 @@
     extract_valid_urls,
     split_filename,
 )
 from f2.exceptions.api_exceptions import (
     APIError,
     APIConnectionError,
     APIResponseError,
+    APIUnavailableError,
     APIUnauthorizedError,
     APINotFoundError,
 )
 
 
 class TokenManager:
-    f2_manager = ConfigManager(f2.F2_CONFIG_FILE_PATH).get_config("f2").get("tiktok")
+    f2_manager = ConfigManager(f2.F2_CONFIG_FILE_PATH).get_config("f2").get("douyin")
     token_conf = f2_manager.get("msToken", None)
     ttwid_conf = f2_manager.get("ttwid", None)
-    odin_tt_conf = f2_manager.get("odin_tt", None)
     proxies_conf = f2_manager.get("proxies", None)
     proxies = {
         "http://": proxies_conf.get("http", None),
         "https://": proxies_conf.get("https", None),
     }
 
     @classmethod
@@ -51,461 +54,506 @@
                 "magic": cls.token_conf["magic"],
                 "version": cls.token_conf["version"],
                 "dataType": cls.token_conf["dataType"],
                 "strData": cls.token_conf["strData"],
                 "tspFromClient": get_timestamp(),
             }
         )
-
         headers = {
             "User-Agent": cls.token_conf["User-Agent"],
             "Content-Type": "application/json",
         }
 
         transport = httpx.HTTPTransport(retries=5)
         with httpx.Client(transport=transport, proxies=cls.proxies) as client:
             try:
                 response = client.post(
-                    cls.token_conf["url"], headers=headers, content=payload
+                    cls.token_conf["url"], content=payload, headers=headers
                 )
-
-                if response.status_code == 401:
-                    raise APIUnauthorizedError(_("由于某些错误, 无法获取msToken"))
-                elif response.status_code == 404:
-                    raise APINotFoundError(_("无法找到API端点"))
+                response.raise_for_status()
 
                 msToken = str(httpx.Cookies(response.cookies).get("msToken"))
-
-                if len(msToken) not in [148]:
-                    raise APIResponseError(
-                        _(
-                            "msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 tiktok 新规则。"
-                        )
-                    )
+                if len(msToken) not in [120, 128]:
+                    raise APIResponseError(_("{0} 内容不符合要求").format("msToken"))
 
                 return msToken
 
-            except httpx.RequestError:
+            except httpx.RequestError as exc:
                 # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
                 raise APIConnectionError(
                     _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(cls.token_conf["url"], cls.proxies, cls.__name__)
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(cls.token_conf["url"], cls.proxies, cls.__name__, exc)
                 )
 
             except httpx.HTTPStatusError as e:
                 # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
-                raise APIResponseError(
-                    f"HTTP Status Code {e.response.status_code}: {e.response.text}"
-                )
+                if e.response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _(
+                            "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+                        ).format("msToken", "douyin")
+                    )
+
+                elif e.response.status_code == 404:
+                    raise APINotFoundError(_("{0} 无法找到API端点").format("msToken"))
+                else:
+                    raise APIResponseError(
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            e.response.url, e.response.status_code, e.response.text
+                        )
+                    )
 
             except APIError as e:
                 # 返回虚假的msToken (Return a fake msToken)
+                logger.error(_("msToken API错误：{0}").format(e))
                 logger.info(_("生成虚假的msToken"))
                 return cls.gen_false_msToken()
 
     @classmethod
     def gen_false_msToken(cls) -> str:
         """生成随机msToken (Generate random msToken)"""
-        return gen_random_str(146) + "=="
+        return gen_random_str(126) + "=="
 
     @classmethod
     def gen_ttwid(cls) -> str:
         """
-        生成请求必带的ttwid (Generate the essential ttwid for requests)
+        生成请求必带的ttwid
+        (Generate the essential ttwid for requests)
         """
+
         transport = httpx.HTTPTransport(retries=5)
-        with httpx.Client(transport=transport, proxies=cls.proxies) as client:
+        with httpx.Client(transport=transport) as client:
             try:
                 response = client.post(
-                    cls.ttwid_conf["url"],
-                    headers={
-                        "Cookie": cls.ttwid_conf.get("cookie"),
-                        "Content-Type": "text/plain",
-                    },
-                    content=cls.ttwid_conf["data"],
+                    cls.ttwid_conf["url"], content=cls.ttwid_conf["data"]
                 )
+                response.raise_for_status()
 
-                if response.status_code == 401:
-                    raise APIUnauthorizedError(_("401 由于某些错误, 无法获取ttwid"))
-                elif response.status_code == 404:
-                    raise APINotFoundError(_("404 无法找到API端点"))
-
-                ttwid = httpx.Cookies(response.cookies).get("ttwid")
-
-                if ttwid is None:
-                    raise APIResponseError(
-                        _("ttwid: 检查没有通过, 请更新配置文件中的ttwid")
-                    )
-
+                ttwid = str(httpx.Cookies(response.cookies).get("ttwid"))
                 return ttwid
 
-            except httpx.RequestError:
+            except httpx.RequestError as exc:
                 # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
                 raise APIConnectionError(
                     _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(cls.ttwid_conf["url"], cls.proxies, cls.__name__)
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(cls.ttwid_conf["url"], cls.proxies, cls.__name__, exc)
                 )
 
             except httpx.HTTPStatusError as e:
                 # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
-                raise APIResponseError(
-                    f"HTTP Status Code {e.response.status_code}: {e.response.text}"
-                )
-
-    @classmethod
-    def gen_odin_tt(cls):
-        """
-        生成请求必带的odin_tt (Generate the essential odin_tt for requests)
-        """
-        transport = httpx.HTTPTransport(retries=5)
-        with httpx.Client(transport=transport, proxies=cls.proxies) as client:
-            try:
-                response = client.get(cls.odin_tt_conf["url"])
-
-                if response.status_code == 401:
-                    raise APIUnauthorizedError(_("401 由于某些错误, 无法获取ttwid"))
-                elif response.status_code == 404:
-                    raise APINotFoundError(_("404 无法找到API端点"))
-
-                odin_tt = httpx.Cookies(response.cookies).get("odin_tt")
+                if e.response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _(
+                            "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+                        ).format("ttwid", "douyin")
+                    )
 
-                if odin_tt is None:
+                elif e.response.status_code == 404:
+                    raise APINotFoundError(_("ttwid无法找到API端点"))
+                else:
                     raise APIResponseError(
-                        _("odin_tt: 检查没有通过, 请更新配置文件中的odin_tt")
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            e.response.url, e.response.status_code, e.response.text
+                        )
                     )
 
-                return odin_tt
 
-            except httpx.RequestError:
-                # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
-                raise APIConnectionError(
-                    _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(cls.odin_tt_conf["url"], cls.proxies, cls.__name__)
-                )
+class VerifyFpManager:
+    @classmethod
+    def gen_verify_fp(cls) -> str:
+        """
+        生成verifyFp 与 s_v_web_id (Generate verifyFp)
+        """
+        base_str = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
+        t = len(base_str)
+        milliseconds = int(round(time.time() * 1000))
+        base36 = ""
+        while milliseconds > 0:
+            remainder = milliseconds % 36
+            if remainder < 10:
+                base36 = str(remainder) + base36
+            else:
+                base36 = chr(ord("a") + remainder - 10) + base36
+            milliseconds = int(milliseconds / 36)
+        r = base36
+        o = [""] * 36
+        o[8] = o[13] = o[18] = o[23] = "_"
+        o[14] = "4"
+
+        for i in range(36):
+            if not o[i]:
+                n = 0 or int(random.random() * t)
+                if i == 19:
+                    n = 3 & n | 8
+                o[i] = base_str[n]
 
-            except httpx.HTTPStatusError as e:
-                # 捕获 httpx 的状态代码错误 (captures specific status code errors from httpx)
-                raise APIResponseError(
-                    f"HTTP Status Code {e.response.status_code}: {e.response.text}"
-                )
+        return "verify_" + r + "_" + "".join(o)
+
+    @classmethod
+    def gen_s_v_web_id(cls) -> str:
+        return cls.gen_verify_fp()
 
 
 class XBogusManager:
     @classmethod
-    def str_2_endpoint(cls, endpoint: str) -> str:
+    def str_2_endpoint(
+        cls,
+        user_agent: str,
+        endpoint: str,
+    ) -> str:
         try:
-            final_endpoint = XB().getXBogus(endpoint)
+            final_endpoint = XB(user_agent).getXBogus(endpoint)
         except Exception as e:
             raise RuntimeError(_("生成X-Bogus失败: {0})").format(e))
 
         return final_endpoint[0]
 
     @classmethod
-    def model_2_endpoint(cls, base_endpoint: str, params: dict) -> str:
-        # 检查params是否是一个字典 (Check if params is a dict)
+    def model_2_endpoint(
+        cls,
+        user_agent: str,
+        base_endpoint: str,
+        params: dict,
+    ) -> str:
         if not isinstance(params, dict):
             raise TypeError(_("参数必须是字典类型"))
 
         param_str = "&".join([f"{k}={v}" for k, v in params.items()])
 
         try:
-            xb_value = XB().getXBogus(param_str)
+            xb_value = XB(user_agent).getXBogus(param_str)
         except Exception as e:
             raise RuntimeError(_("生成X-Bogus失败: {0})").format(e))
 
         # 检查base_endpoint是否已有查询参数 (Check if base_endpoint already has query parameters)
         separator = "&" if "?" in base_endpoint else "?"
 
         final_endpoint = f"{base_endpoint}{separator}{param_str}&X-Bogus={xb_value[1]}"
 
         return final_endpoint
 
 
 class SecUserIdFetcher:
-    _TIKTOK_SECUID_PARREN = re.compile(
-        r"<script id=\"__UNIVERSAL_DATA_FOR_REHYDRATION__\" type=\"application/json\">(.*?)</script>"
-    )
-    _TIKTOK_UNIQUEID_PARREN = re.compile(r"/@([^/?]*)")
-    _TIKTOK_NOTFOUND_PARREN = re.compile(r"notfound")
+    # 预编译正则表达式
+    _DOUYIN_URL_PATTERN = re.compile(r"user/([^/?]*)")
+    _REDIRECT_URL_PATTERN = re.compile(r"sec_uid=([^&]*)")
 
     @classmethod
-    async def get_secuid(cls, url: str) -> str:
+    async def get_sec_user_id(cls, url: str) -> str:
         """
-        获取TikTok用户sec_uid
+        从单个url中获取sec_user_id (Get sec_user_id from a single url)
+
         Args:
-            url: 用户主页链接
-        Return:
-            sec_uid: 用户唯一标识
+            url (str): 输入的url (Input url)
+
+        Returns:
+            str: 匹配到的sec_user_id (Matched sec_user_id)。
         """
 
-        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError("输入参数必须是字符串")
+            raise TypeError(_("参数必须是字符串类型"))
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
 
-        transport = httpx.AsyncHTTPTransport(retries=5)
-        async with httpx.AsyncClient(
-            transport=transport, proxies=TokenManager.proxies, timeout=10
-        ) as client:
-            try:
-                response = await client.get(url, follow_redirects=True)
+        pattern = (
+            cls._REDIRECT_URL_PATTERN
+            if "v.douyin.com" in url
+            else cls._DOUYIN_URL_PATTERN
+        )
 
+        try:
+            transport = httpx.AsyncHTTPTransport(retries=5)
+            async with httpx.AsyncClient(
+                transport=transport, proxies=TokenManager.proxies, timeout=10
+            ) as client:
+                response = await client.get(url, follow_redirects=True)
+                # 444一般为Nginx拦截，不返回状态 (444 is generally intercepted by Nginx and does not return status)
                 if response.status_code in {200, 444}:
-                    if cls._TIKTOK_NOTFOUND_PARREN.search(str(response.url)):
-                        raise APINotFoundError(
-                            _(
-                                "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}".format(
-                                    cls.__name__
-                                )
-                            )
-                        )
-                    match = cls._TIKTOK_SECUID_PARREN.search(str(response.text))
-                    if not match:
+                    match = pattern.search(str(response.url))
+                    if match:
+                        return match.group(1)
+                    else:
                         raise APIResponseError(
                             _(
-                                "未在响应的地址中找到sec_uid, 检查链接是否为用户主页类名: {0}".format(
-                                    cls.__name__
-                                )
-                            )
+                                "未在响应的地址中找到sec_user_id，检查链接是否为用户主页类名：{0}"
+                            ).format(cls.__name__)
                         )
 
-                    # 提取SIGI_STATE对象中的sec_uid
-                    data = json.loads(match.group(1))
-                    default_scope = data.get("__DEFAULT_SCOPE__", {})
-                    user_detail = default_scope.get("webapp.user-detail", {})
-                    user_info = user_detail.get("userInfo", {}).get("user", {})
-                    sec_uid = user_info.get("secUid")
-
-                    if sec_uid is None:
-                        raise RuntimeError(_("获取sec_uid失败, {0}".format(user_info)))
-
-                    return sec_uid
+                elif response.status_code == 401:
+                    raise APIUnauthorizedError(
+                        _("未授权的请求。类名：{0}").format(cls.__name__)
+                    )
+                elif response.status_code == 404:
+                    raise APINotFoundError(
+                        _("未找到API端点。类名：{0}").format(cls.__name__)
+                    )
+                elif response.status_code == 503:
+                    raise APIUnavailableError(
+                        _("API服务不可用。类名：{0}").format(cls.__name__)
+                    )
                 else:
-                    raise ConnectionError(_("接口状态码异常, 请检查重试"))
+                    raise APIResponseError(
+                        _("链接：{0}，状态码 {1}：{2} ").format(
+                            response.url, response.status_code, response.text
+                        )
+                    )
 
-            except httpx.RequestError:
-                raise APIConnectionError(
-                    _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(url, TokenManager.proxies, cls.__name__)
-                )
+        except httpx.RequestError as exc:
+            raise APIConnectionError(
+                _(
+                    "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                ).format(url, TokenManager.proxies, cls.__name__, exc)
+            )
 
     @classmethod
-    async def get_all_secuid(cls, urls: list) -> list:
+    async def get_all_sec_user_id(cls, urls: list) -> list:
         """
-        获取列表secuid列表 (Get list sec_user_id list)
+        获取列表sec_user_id列表 (Get list sec_user_id list)
 
         Args:
             urls: list: 用户url列表 (User url list)
 
         Return:
-            secuids: list: 用户secuid列表 (User secuid list)
+            sec_user_ids: list: 用户sec_user_id列表 (User sec_user_id list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        secuids = [cls.get_secuid(url) for url in urls]
-        return await asyncio.gather(*secuids)
+        sec_user_ids = [cls.get_sec_user_id(url) for url in urls]
+        return await asyncio.gather(*sec_user_ids)
+
+
+class AwemeIdFetcher:
+    # 预编译正则表达式
+    _DOUYIN_VIDEO_URL_PATTERN = re.compile(r"video/([^/?]*)")
+    _DOUYIN_NOTE_URL_PATTERN = re.compile(r"note/([^/?]*)")
 
     @classmethod
-    async def get_uniqueid(cls, url: str) -> str:
+    async def get_aweme_id(cls, url: str) -> str:
         """
-        获取TikTok用户unique_id
+        从单个url中获取aweme_id (Get aweme_id from a single url)
+
         Args:
-            url: 用户主页链接
-        Return:
-            unique_id: 用户唯一id
+            url (str): 输入的url (Input url)
+
+        Returns:
+            str: 匹配到的aweme_id (Matched aweme_id)。
         """
 
-        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError("输入参数必须是字符串")
+            raise TypeError(_("参数必须是字符串类型"))
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
 
+        # 重定向到完整链接
         transport = httpx.AsyncHTTPTransport(retries=5)
         async with httpx.AsyncClient(
             transport=transport, proxies=TokenManager.proxies, timeout=10
         ) as client:
             try:
                 response = await client.get(url, follow_redirects=True)
+                response.raise_for_status()
 
-                if response.status_code in {200, 444}:
-                    match = cls._TIKTOK_UNIQUEID_PARREN.search(str(response.url))
-                    if not match:
-                        raise APIResponseError(_("未在响应中找到unique_id"))
-
-                    unique_id = match.group(1)
-
-                    if unique_id is None:
-                        raise RuntimeError(
-                            _("获取unique_id失败, {0}".format(response.url))
-                        )
+                video_pattern = cls._DOUYIN_VIDEO_URL_PATTERN
+                note_pattern = cls._DOUYIN_NOTE_URL_PATTERN
 
-                    return unique_id
+                match = video_pattern.search(str(response.url))
+                if match:
+                    aweme_id = match.group(1)
                 else:
-                    raise ConnectionError(
-                        _("接口状态码异常 {0}, 请检查重试").format(response.status_code)
-                    )
+                    match = note_pattern.search(str(response.url))
+                    if match:
+                        aweme_id = match.group(1)
+                    else:
+                        raise APIResponseError(
+                            _("未在响应的地址中找到aweme_id，检查链接是否为作品页")
+                        )
+                return aweme_id
 
-            except httpx.RequestError:
+            except httpx.RequestError as exc:
+                # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
                 raise APIConnectionError(
                     _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(url, TokenManager.proxies, cls.__name__),
+                        "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                    ).format(url, TokenManager.proxies, cls.__name__, exc)
+                )
+
+            except httpx.HTTPStatusError as e:
+                raise APIResponseError(
+                    _("链接：{0}，状态码 {1}：{2} ").format(
+                        e.response.url, e.response.status_code, e.response.text
+                    )
                 )
 
     @classmethod
-    async def get_all_uniqueid(cls, urls: list) -> list:
+    async def get_all_aweme_id(cls, urls: list) -> list:
         """
-        获取列表unique_id列表 (Get list sec_user_id list)
+        获取视频aweme_id,传入列表url都可以解析出aweme_id (Get video aweme_id, pass in the list url can parse out aweme_id)
 
         Args:
-            urls: list: 用户url列表 (User url list)
+            urls: list: 列表url (list url)
 
         Return:
-            unique_ids: list: 用户unique_id列表 (User unique_id list)
+            aweme_ids: list: 视频的唯一标识，返回列表 (The unique identifier of the video, return list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        unique_ids = [cls.get_uniqueid(url) for url in urls]
-        return await asyncio.gather(*unique_ids)
+        aweme_ids = [cls.get_aweme_id(url) for url in urls]
+        return await asyncio.gather(*aweme_ids)
+
 
+class MixIdFetcher:
+    # 获取方法同AwemeIdFetcher
+    @classmethod
+    async def get_mix_id(cls, url: str) -> str:
+        return
 
-class AwemeIdFetcher:
-    # https://www.tiktok.com/@scarlettjonesuk/video/7255716763118226715
-    # https://www.tiktok.com/@scarlettjonesuk/video/7255716763118226715?is_from_webapp=1&sender_device=pc&web_id=7306060721837852167
 
+class WebCastIdFetcher:
     # 预编译正则表达式
-    _TIKTOK_AWEMEID_PARREN = re.compile(r"video/(\d*)")
+    _DOUYIN_LIVE_URL_PATTERN = re.compile(r"live/([^/?]*)")
+    # https://live.douyin.com/766545142636?cover_type=0&enter_from_merge=web_live&enter_method=web_card&game_name=&is_recommend=1&live_type=game&more_detail=&request_id=20231110224012D47CD00C18B4AE4BFF9B&room_id=7299828646049827596&stream_type=vertical&title_type=1&web_live_page=hot_live&web_live_tab=all
+    # https://live.douyin.com/766545142636
+    _DOUYIN_LIVE_URL_PATTERN2 = re.compile(r"http[s]?://live.douyin.com/(\d+)")
+    # https://webcast.amemv.com/douyin/webcast/reflow/7318296342189919011?u_code=l1j9bkbd&did=MS4wLjABAAAAEs86TBQPNwAo-RGrcxWyCdwKhI66AK3Pqf3ieo6HaxI&iid=MS4wLjABAAAA0ptpM-zzoliLEeyvWOCUt-_dQza4uSjlIvbtIazXnCY&with_sec_did=1&use_link_command=1&ecom_share_track_params=&extra_params={"from_request_id":"20231230162057EC005772A8EAA0199906","im_channel_invite_id":"0"}&user_id=3644207898042206&liveId=7318296342189919011&from=share&style=share&enter_method=click_share&roomId=7318296342189919011&activity_info={}
+    _DOUYIN_LIVE_URL_PATTERN3 = re.compile(r"reflow/([^/?]*)")
 
     @classmethod
-    async def get_aweme_id(cls, url: str) -> str:
+    async def get_webcast_id(cls, url: str) -> str:
         """
-        获取TikTok作品aweme_id
+        从单个url中获取webcast_id (Get webcast_id from a single url)
+
         Args:
-            url: 作品链接
-        Return:
-            aweme_id: 作品唯一标识
+            url (str): 输入的url (Input url)
+
+        Returns:
+            str: 匹配到的webcast_id (Matched webcast_id)。
         """
 
-        # 进行参数检查
         if not isinstance(url, str):
-            raise TypeError("输入参数必须是字符串")
+            raise TypeError(_("参数必须是字符串类型"))
 
         # 提取有效URL
         url = extract_valid_urls(url)
 
         if url is None:
             raise (
-                APINotFoundError(_("输入的URL不合法。类名：{0}".format(cls.__name__)))
+                APINotFoundError(_("输入的URL不合法。类名：{0}").format(cls.__name__))
             )
-
-        transport = httpx.AsyncHTTPTransport(retries=5)
-        async with httpx.AsyncClient(
-            transport=transport, proxies=TokenManager.proxies, timeout=10
-        ) as client:
-            try:
+        try:
+            # 重定向到完整链接
+            transport = httpx.AsyncHTTPTransport(retries=5)
+            async with httpx.AsyncClient(
+                transport=transport, proxies=TokenManager.proxies, timeout=10
+            ) as client:
                 response = await client.get(url, follow_redirects=True)
+                response.raise_for_status()
+                url = str(response.url)
 
-                if response.status_code in {200, 444}:
-                    match = cls._TIKTOK_AWEMEID_PARREN.search(str(response.url))
-                    if not match:
-                        raise APIResponseError(_("未在响应中找到aweme_id"))
-
-                    aweme_id = match.group(1)
-
-                    if aweme_id is None:
-                        raise RuntimeError(
-                            _("获取aweme_id失败, {0}".format(response.url))
+                live_pattern = cls._DOUYIN_LIVE_URL_PATTERN
+                live_pattern2 = cls._DOUYIN_LIVE_URL_PATTERN2
+                live_pattern3 = cls._DOUYIN_LIVE_URL_PATTERN3
+
+                if live_pattern.search(url):
+                    match = live_pattern.search(url)
+                elif live_pattern2.search(url):
+                    match = live_pattern2.search(url)
+                elif live_pattern3.search(url):
+                    match = live_pattern3.search(url)
+                    logger.warning(
+                        _(
+                            "该链接返回的是room_id，请使用`fetch_user_live_videos_by_room_id`接口"
                         )
-
-                    return aweme_id
+                    )
                 else:
-                    raise ConnectionError(
-                        _("接口状态码异常 {0}, 请检查重试").format(response.status_code)
+                    raise APIResponseError(
+                        _("未在响应的地址中找到webcast_id，检查链接是否为直播页")
                     )
 
-            except httpx.RequestError:
-                raise APIConnectionError(
-                    _(
-                        "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
-                    ).format(
-                        url,
-                        TokenManager.proxies,
-                        cls.__name__,
-                    )
+                return match.group(1)
+
+        except httpx.RequestError as exc:
+            # 捕获所有与 httpx 请求相关的异常情况 (Captures all httpx request-related exceptions)
+            raise APIConnectionError(
+                _(
+                    "请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常详细信息：{3}"
+                ).format(url, TokenManager.proxies, cls.__name__, exc)
+            )
+
+        except httpx.HTTPStatusError as e:
+            raise APIResponseError(
+                _("链接：{0}，状态码 {1}：{2} ").format(
+                    e.response.url, e.response.status_code, e.response.text
                 )
+            )
 
     @classmethod
-    async def get_all_aweme_id(cls, urls: list) -> list:
+    async def get_all_webcast_id(cls, urls: list) -> list:
         """
-        获取视频aweme_id,传入列表url都可以解析出aweme_id (Get video aweme_id, pass in the list url can parse out aweme_id)
+        获取直播webcast_id,传入列表url都可以解析出webcast_id (Get live webcast_id, pass in the list url can parse out webcast_id)
 
         Args:
             urls: list: 列表url (list url)
 
         Return:
-            aweme_ids: list: 视频的唯一标识，返回列表 (The unique identifier of the video, return list)
+            webcast_ids: list: 直播的唯一标识，返回列表 (The unique identifier of the live, return list)
         """
 
         if not isinstance(urls, list):
             raise TypeError(_("参数必须是列表类型"))
 
         # 提取有效URL
         urls = extract_valid_urls(urls)
 
         if urls == []:
             raise (
                 APINotFoundError(
-                    _("输入的URL List不合法。类名：{0}".format(cls.__name__))
+                    _("输入的URL List不合法。类名：{0}").format(cls.__name__)
                 )
             )
 
-        aweme_ids = [cls.get_aweme_id(url) for url in urls]
-        return await asyncio.gather(*aweme_ids)
+        webcast_ids = [cls.get_webcast_id(url) for url in urls]
+        return await asyncio.gather(*webcast_ids)
 
 
 def format_file_name(
     naming_template: str,
     aweme_data: dict = {},
     custom_fields: dict = {},
 ) -> str:
@@ -537,45 +585,45 @@
         "win32": 200,
         "cygwin": 60,
         "darwin": 60,
         "linux": 60,
     }
 
     fields = {
-        "create": aweme_data.get("createTime", ""),  # 长度固定19
+        "create": aweme_data.get("create_time", ""),  # 长度固定19
         "nickname": aweme_data.get("nickname", ""),  # 最长30
         "aweme_id": aweme_data.get("aweme_id", ""),  # 长度固定19
         "desc": split_filename(aweme_data.get("desc", ""), os_limit),
         "uid": aweme_data.get("uid", ""),  # 固定11
     }
 
     if custom_fields:
         # 更新自定义字段
         fields.update(custom_fields)
 
     try:
         return naming_template.format(**fields)
     except KeyError as e:
-        raise KeyError(_("文件名模板字段 {0} 不存在，请检查".format(e)))
+        raise KeyError(_("文件名模板字段 {0} 不存在，请检查").format(e))
 
 
 def create_user_folder(kwargs: dict, nickname: Union[str, int]) -> Path:
     """
     根据提供的配置文件和昵称，创建对应的保存目录。
     (Create the corresponding save directory according to the provided conf file and nickname.)
 
     Args:
         kwargs (dict): 配置文件，字典格式。(Conf file, dict format)
         nickname (Union[str, int]): 用户的昵称，允许字符串或整数。  (User nickname, allow strings or integers)
 
     Note:
         如果未在配置文件中指定路径，则默认为 "Download"。
         (If the path is not specified in the conf file, it defaults to "Download".)
-        仅支持相对路径。
-        (Only relative paths are supported.)
+        支持绝对与相对路径。
+        (Support absolute and relative paths)
 
     Raises:
         TypeError: 如果 kwargs 不是字典格式，将引发 TypeError。
         (If kwargs is not in dict format, TypeError will be raised.)
     """
 
     # 确定函数参数是否正确
@@ -583,15 +631,15 @@
         raise TypeError("kwargs 参数必须是字典")
 
     # 创建基础路径
     base_path = Path(kwargs.get("path", "Download"))
 
     # 添加下载模式和用户名
     user_path = (
-        base_path / "tiktok" / kwargs.get("mode", "PLEASE_SETUP_MODE") / str(nickname)
+        base_path / "douyin" / kwargs.get("mode", "PLEASE_SETUP_MODE") / str(nickname)
     )
 
     # 获取绝对路径并确保它存在
     resolve_user_path = user_path.resolve()
 
     # 创建目录
     resolve_user_path.mkdir(parents=True, exist_ok=True)
@@ -639,7 +687,59 @@
         return user_path
 
     if local_user_data.get("nickname") != current_nickname:
         # 昵称不一致，触发目录更新操作
         user_path = rename_user_folder(user_path, current_nickname)
 
     return user_path
+
+
+def show_qrcode(qrcode_url: str, show_image: bool = False) -> None:
+    """
+    显示二维码 (Show QR code)
+
+    Args:
+        qrcode_url (str): 登录二维码链接 (Login QR code link)
+        show_image (bool): 是否显示图像，True 表示显示，False 表示在控制台显示
+        (Whether to display the image, True means display, False means display in the console)
+    """
+    if show_image:
+        # 创建并显示QR码图像
+        qr_code_img = qrcode.make(qrcode_url)
+        qr_code_img.show()
+    else:
+        # 在控制台以 ASCII 形式打印二维码
+        qr = qrcode.QRCode()
+        qr.add_data(qrcode_url)
+        qr.make(fit=True)
+        # 在控制台以 ASCII 形式打印二维码
+        qr.print_ascii(invert=True)
+
+
+def json_2_lrc(data: Union[str, list, dict]) -> str:
+    """
+    从抖音原声json格式歌词生成lrc格式歌词
+    (Generate lrc lyrics format from Douyin original json lyrics format)
+
+    Args:
+        data (Union[str, list, dict]): 抖音原声json格式歌词 (Douyin original json lyrics format)
+
+    Returns:
+        str: 生成的lrc格式歌词 (Generated lrc format lyrics)
+    """
+    try:
+        lrc_lines = []
+        for item in data:
+            text = item["text"]
+            time_seconds = float(item["timeId"])
+            minutes = int(time_seconds // 60)
+            seconds = int(time_seconds % 60)
+            milliseconds = int((time_seconds % 1) * 1000)
+            time_str = f"{minutes:02}:{seconds:02}.{milliseconds:03}"
+            lrc_lines.append(f"[{time_str}] {text}")
+    except KeyError as e:
+        raise KeyError(_("歌词数据字段错误：{0}").format(e))
+    except RuntimeError as e:
+        raise RuntimeError(_("生成歌词文件失败：{0}，请检查歌词 `data` 内容").format(e))
+    except TypeError as e:
+        raise TypeError(_("歌词数据类型错误：{0}").format(e))
+    return "\n".join(lrc_lines)
```

### Comparing `f2-0.0.1.4/f2/cli/cli_commands.py` & `f2-0.0.1.5/f2/cli/cli_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # path: f2/cli/cli_command.py
 
+import f2
 import click
 import typing
 import asyncio
 import importlib
 
 from f2 import helps
 from f2.apps import __apps__ as apps_module
-from f2.utils import __version__
 from f2.exceptions import APIError
 from f2.cli.cli_console import RichConsoleManager
 from f2.utils._signal import SignalManager
 from f2.i18n.translator import _
 from f2.log.logger import logger
 
 
@@ -19,28 +19,28 @@
 def handle_help(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
-    helps.f2()
+    helps.main()
     ctx.exit()
 
 
 # 处理版本号
 def handle_version(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
     value: typing.Any,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
-    logger.debug(f"Version {__version__._version}")
-    print(f"Version {__version__._version}")
+
+    click.echo(f"Version {f2.__version__}")
     ctx.exit()
 
 
 # 处理debug
 def handle_debug(
     ctx: click.Context,
     param: typing.Union[click.Option, click.Parameter],
@@ -130,18 +130,19 @@
 
     SignalManager().register_shutdown_signal()
 
     with RichConsoleManager().progress:
         try:
             asyncio.run(run_app(kwargs))
         except APIError as e:
-            logger.error(e.display_error())
+            logger.error(e)
 
 
 async def run_app(kwargs):
+    logger.info(f"Version {f2.__version__}")
     app_name = kwargs["app_name"]
     app_module = importlib.import_module(f"f2.apps.{app_name}.handler")
     await app_module.main(kwargs)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `f2-0.0.1.4/f2/cli/cli_console.py` & `f2-0.0.1.5/f2/cli/cli_console.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/conf/conf.yaml` & `f2-0.0.1.5/f2/conf/conf.yaml`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/crawlers/base_crawler.py` & `f2-0.0.1.5/f2/crawlers/base_crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,15 +146,14 @@
             try:
                 response = await self.aclient.get(url, follow_redirects=True)
                 if not response.text.strip() or not response.content:
                     error_message = _(
                         "第 {0} 次响应内容为空, 状态码: {1}, URL:{2}"
                     ).format(attempt + 1, response.status_code, response.url)
 
-                    print(error_message)
                     logger.warning(error_message)
 
                     if attempt == self._max_retries - 1:
                         raise APIRetryExhaustedError(
                             _("获取端点数据失败, 次数达到上限")
                         )
 
@@ -172,15 +171,15 @@
                     ).format(url, self.proxies, self.__class__.__name__)
                 )
 
             except httpx.HTTPStatusError as http_error:
                 self.handle_http_status_error(http_error, url, attempt + 1)
 
             except APIError as e:
-                e.display_error()
+                logger.error(e)
 
     async def post_fetch_data(self, url: str, params: dict = {}):
         """
         获取POST端点数据 (Get POST endpoint data)
 
         Args:
             url (str): 端点URL (Endpoint URL)
@@ -195,15 +194,14 @@
                     url, json=dict(params), follow_redirects=True
                 )
                 if not response.text.strip() or not response.content:
                     error_message = _(
                         "第 {0} 次响应内容为空, 状态码: {1}, URL:{2}"
                     ).format(attempt + 1, response.status_code, response.url)
 
-                    print(error_message)
                     logger.warning(error_message)
 
                     if attempt == self._max_retries - 1:
                         raise APIRetryExhaustedError(
                             _("获取端点数据失败, 次数达到上限")
                         )
 
@@ -221,15 +219,15 @@
                     ).format(url, self.proxies, self.__class__.__name__)
                 )
 
             except httpx.HTTPStatusError as http_error:
                 self.handle_http_status_error(http_error, url, attempt + 1)
 
             except APIError as e:
-                e.display_error()
+                logger.error(e)
 
     async def head_fetch_data(self, url: str):
         """
         获取HEAD端点数据 (Get HEAD endpoint data)
 
         Args:
             url (str): 端点URL (Endpoint URL)
@@ -250,15 +248,15 @@
                 )
             )
 
         except httpx.HTTPStatusError as http_error:
             self.handle_http_status_error(http_error, url, 1)
 
         except APIError as e:
-            e.display_error()
+            logger.error(e)
 
     def handle_http_status_error(self, http_error, url: str, attempt):
         """
         处理HTTP状态错误 (Handle HTTP status error)
 
         Args:
             http_error: HTTP状态错误 (HTTP status error)
@@ -275,39 +273,41 @@
             APIRetryExhaustedError: 重试次数达到上限 (The number of retries has reached the upper limit)
         """
         response = getattr(http_error, "response", None)
         status_code = getattr(response, "status_code", None)
 
         if response is None or status_code is None:
             logger.error(
-                _("HTTP状态错误: {0}, URL: {1}, 尝试次数: {2}").format(
+                _("HTTP状态错误：{0}, URL：{1}, 尝试次数：{2}").format(
                     http_error, url, attempt
                 )
             )
-            raise APIResponseError(f"处理HTTP错误时遇到意外情况: {http_error}")
+            raise APIResponseError(
+                _("处理HTTP错误时遇到意外情况：{0}").format(http_error)
+            )
 
         if status_code == 302:
             pass
         elif status_code == 404:
-            raise APINotFoundError(f"HTTP Status Code {status_code}")
+            raise APINotFoundError(_("HTTP状态码错误："), status_code)
         elif status_code == 503:
-            raise APIUnavailableError(f"HTTP Status Code {status_code}")
+            raise APIUnavailableError(_("HTTP状态码错误："), status_code)
         elif status_code == 408:
-            raise APITimeoutError(f"HTTP Status Code {status_code}")
+            raise APITimeoutError(_("HTTP状态码错误："), status_code)
         elif status_code == 401:
-            raise APIUnauthorizedError(f"HTTP Status Code {status_code}")
+            raise APIUnauthorizedError(_("HTTP状态码错误："), status_code)
         elif status_code == 429:
-            raise APIRateLimitError(f"HTTP Status Code {status_code}")
+            raise APIRateLimitError(_("HTTP状态码错误："), status_code)
         else:
             logger.error(
-                _("HTTP状态错误: {0}, URL: {1}, 尝试次数: {2}").format(
-                    status_code, url, attempt
+                _("HTTP状态错误：{0}, URL：{1}, 尝试次数：{2}").format(
+                    http_error, url, attempt
                 )
             )
-            raise APIResponseError(f"HTTP状态错误: {status_code}")
+            raise APIResponseError(_("HTTP状态码错误："), status_code)
 
     async def close(self):
         await self.aclient.aclose()
 
     async def __aenter__(self):
         return self
```

### Comparing `f2-0.0.1.4/f2/db/base_db.py` & `f2-0.0.1.5/f2/db/base_db.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/dl/base_downloader.py` & `f2-0.0.1.5/f2/dl/base_downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import httpx
 import asyncio
 import aiofiles
 import traceback
 from pathlib import Path
 from rich.progress import TaskID
-from typing import Union, Optional, Any
+from typing import Union, Optional, Any, List
 
 from f2.log.logger import logger
 from f2.i18n.translator import _
 from f2.cli.cli_console import RichConsoleManager
 from f2.crawlers.base_crawler import BaseCrawler
 from f2.utils._signal import SignalManager
 from f2.utils.utils import ensure_path
@@ -22,15 +22,15 @@
     get_segments_from_m3u8,
 )
 
 
 class BaseDownloader(BaseCrawler):
     """基础下载器 (Base Downloader Class)"""
 
-    def __init__(self, kwargs: dict = {}):
+    def __init__(self, kwargs: dict = ...):
         proxies_conf = kwargs.get("proxies", {"http": None, "https": None})
         proxies = {
             "http://": proxies_conf.get("http", None),
             "https://": proxies_conf.get("https", None),
         }
 
         self.headers = {
@@ -38,15 +38,14 @@
             "Referer": kwargs["headers"]["Referer"],
             "Cookie": kwargs["cookie"],
         }
 
         super().__init__(proxies=proxies, crawler_headers=self.headers)
         self.progress = RichConsoleManager().progress
         self.download_tasks = []
-        logger.debug(_("BaseDownloader 请求头headers:{0}".format(self.headers)))
 
     @staticmethod
     def _ensure_path(path: Union[str, Path]) -> Path:
         return ensure_path(path)
 
     async def _download_chunks(
         self,
@@ -73,97 +72,151 @@
                 if SignalManager.is_shutdown_signaled():
                     break
                 await file.write(chunk)
                 await self.progress.update(
                     task_id, advance=len(chunk), total=int(content_length)
                 )
         except httpx.ReadTimeout as e:
-            logger.warning(_("文件区块下载超时: {0}".format(e)))
+            logger.warning(_("文件区块下载超时：{0}").format(e))
         except Exception as e:
-            logger.error(_("文件区块下载失败: {0}".format(e)))
+            logger.error(_("文件区块下载失败：{0}").format(e))
 
     async def download_file(
-        self, task_id: TaskID, url: str, full_path: Union[str, Path]
+        self,
+        task_id: TaskID,
+        urls: Union[str, List[str]],
+        full_path: Union[str, Path],
     ) -> None:
         """
         下载文件 (Download file)
 
         Args:
             task_id (TaskID): 任务ID (Task ID)
-            url (str): 文件URL (File URL)
+            urls (Union[str, List[str]]): 文件URL (File URL)
             full_path (Union[str, Path]): 保存路径 (Save path)
+
+        Note:
+            url仅代表一个文件的链接，当url为列表时，表示该文件的多个链接
+            (url represents only a link to a file, when url is a list,
+                it represents multiple links to the file)
         """
         async with self.semaphore:
+            # 如果urls是单个链接，则转换为列表以便统一处理
+            if isinstance(urls, str):
+                urls = [urls]
+
             # 确保目标路径存在 (Ensure target path exists)
             full_path = self._ensure_path(full_path)
-            # 获取文件内容大小 (Get the size of the file content)
-            content_length = await get_content_length(url, self.headers, self.proxies)
 
-            logger.debug(
-                _("{0}在服务器上的总内容长度为：{1} 字节".format(url, content_length))
-            )
+            # 遍历所有链接 (Iterate over all links)
+            for link in urls:
+                # 获取文件内容大小 (Get the size of the file content)
+                content_length = await get_content_length(
+                    link, self.headers, self.proxies
+                )
 
-            # 如果文件内容大小为0, 则不下载 (If file content size is 0, skip download)
-            if content_length == 0:
-                logger.warning(_("内容长度为0，跳过下载"))
-                await self.progress.update(
-                    task_id,
-                    description=_("[  丢失  ]:"),
-                    filename=trim_filename(full_path.name, 45),
-                    state="completed",
+                logger.debug(
+                    _("{0} 在服务器上的总内容长度为：{1} 字节").format(
+                        link, content_length
+                    )
                 )
-                return
 
-            # 确保目标路径存在 (Ensure target path exists)
-            full_path.parent.mkdir(parents=True, exist_ok=True)
-            # 寻找未下载完的临时文件 (Find unfinished temporary files)
-            tmp_path = full_path.with_suffix(".tmp")
-            # 获取临时文件的大小 (Get the size of the temporary file)
-            start_byte = 0 if not tmp_path.exists() else tmp_path.stat().st_size
-
-            logger.debug(
-                _(
-                    "找到了未下载完的文件 {0}, 大小为 {1} 字节".format(
+                # 如果文件内容大小为0, 则尝试下一个链接 (If file content size is 0, try the next link)
+                if content_length == 0:
+                    logger.warning(
+                        _("链接 {0} 内容长度为0，尝试下一个链接是否可用").format(link)
+                    )
+                    continue
+
+                # 确保目标路径存在 (Ensure target path exists)
+                full_path.parent.mkdir(parents=True, exist_ok=True)
+                # 寻找未下载完的临时文件 (Find unfinished temporary files)
+                tmp_path = full_path.with_suffix(".tmp")
+                # 获取临时文件的大小 (Get the size of the temporary file)
+                start_byte = 0 if not tmp_path.exists() else tmp_path.stat().st_size
+
+                logger.debug(
+                    _("找到了未下载完的文件 {0}, 大小为 {1} 字节").format(
                         tmp_path, start_byte
                     )
                 )
-            )
 
-            if start_byte in [0, content_length]:
-                if start_byte:
+                if start_byte in [0, content_length]:
+                    if start_byte:
+                        tmp_path.rename(full_path)
+                        logger.debug(_("临时文件已完全下载"))
+                        return
+
+                # 构建range请求头 (Build range request header)
+                range_headers = (
+                    {"Range": "bytes={}-".format(start_byte)} if start_byte else {}
+                )
+                range_headers.update(self.headers)
+                range_request = self.aclient.build_request(
+                    "GET", link, headers=range_headers
+                )
+                async with aiofiles.open(
+                    tmp_path, "ab" if start_byte else "wb"
+                ) as file:
+                    await self._download_chunks(
+                        self.aclient, range_request, file, content_length, task_id
+                    )
+
+                # 下载完成后重命名文件 (Rename file after download is complete)
+                try:
                     tmp_path.rename(full_path)
-                    logger.debug(_("临时文件已完全下载"))
-                    return
+                except FileExistsError:
+                    logger.warning(_("{0} 已存在，将覆盖").format(full_path))
+                    tmp_path.replace(full_path)
+                except PermissionError:
+                    logger.error(
+                        _(
+                            "另一个程序正在使用此文件或受异步调度影响，该任务需要重新下载"
+                        )
+                    )
+                    # 尝试删除临时文件 (Try to delete the temporary file)
+                    try:
+                        tmp_path.unlink()
+                        tmp_path.rename(full_path)
+                    except Exception as e:
+                        logger.error(_("尝试删除临时文件失败：{0}").format(e))
 
-            # 构建range请求头 (Build range request header)
-            range_headers = (
-                {"Range": "bytes={}-".format(start_byte)} if start_byte else {}
-            )
-            range_headers.update(self.headers)
-            range_request = self.aclient.build_request(
-                "GET", url, headers=range_headers
-            )
-            async with aiofiles.open(tmp_path, "ab" if start_byte else "wb") as file:
-                await self._download_chunks(
-                    self.aclient, range_request, file, content_length, task_id
+                    await self.progress.update(
+                        task_id,
+                        description=_("[  失败  ]："),
+                        filename=trim_filename(full_path.name, 45),
+                        state="error",
+                    )
+
+                await self.progress.update(
+                    task_id,
+                    description=_("[  完成  ]："),
+                    filename=trim_filename(full_path.name, 45),
+                    state="completed",
                 )
+                logger.debug(_("下载完成, 文件已保存为 {0}").format(full_path))
 
-            # 下载完成后重命名文件 (Rename file after download is complete)
-            tmp_path.rename(full_path)
+                # 如果下载成功，则跳出循环 (If download is successful, break the loop)
+                break
 
-            await self.progress.update(
-                task_id,
-                description=_("[  完成  ]:"),
-                filename=trim_filename(full_path.name, 45),
-                state="completed",
-            )
-            logger.debug(_("下载完成, 文件已保存为 {0}".format(full_path)))
+            else:
+                # 如果遍历完所有链接仍然无法成功下载，则记录警告
+                logger.warning("所有链接都无法下载")
+                await self.progress.update(
+                    task_id,
+                    description=_("[  丢失  ]：所有链接都无法下载"),
+                    filename=trim_filename(full_path.name, 45),
+                    state="error",
+                )
 
     async def save_file(
-        self, task_id: TaskID, content: Any, full_path: Union[str, Path]
+        self,
+        task_id: TaskID,
+        content: Any,
+        full_path: Union[str, Path],
     ):
         """
         保存文件 (Save file)
 
         Args:
             task_id (TaskID): 任务ID (Task ID)
             content (Any): 文件内容 (File content)
@@ -184,18 +237,21 @@
 
         await self.progress.update(
             task_id,
             description=_("[  完成  ]:"),
             filename=trim_filename(full_path.name, 45),
             state="completed",
         )
-        logger.debug(_("下载完成, 文件已保存为 {0}".format(full_path)))
+        logger.debug(_("下载完成, 文件已保存为 {0}").format(full_path))
 
     async def download_m3u8_stream(
-        self, task_id: TaskID, url: str, full_path: Union[str, Path]
+        self,
+        task_id: TaskID,
+        url: str,
+        full_path: Union[str, Path],
     ) -> None:
         """
         下载m3u8流视频 (Download m3u8 stream video)
 
         Args:
             task_id (TaskID): 任务ID (Task ID)
             url (str): m3u8文件的URL (m3u8 file URL)
@@ -259,17 +315,17 @@
                                     await self.progress.update(
                                         task_id,
                                         advance=len(chunk),
                                         total=total_downloaded,
                                     )
 
                             except httpx.ReadTimeout as e:
-                                logger.warning(_("TS文件下载超时: {0}".format(e)))
+                                logger.warning(_("TS文件下载超时: {0}").format(e))
                             except Exception as e:
-                                logger.error(_("TS文件下载失败: {0}".format(e)))
+                                logger.error(_("TS文件下载失败: {0}").format(e))
                                 logger.error(traceback.format_exc())
                             finally:
                                 await ts_response.aclose()
                     # 等待一段时间后再次请求更新 (Request update again after waiting for a while)
                     await asyncio.sleep(5)
 
                 except httpx.HTTPStatusError as e:
@@ -279,53 +335,58 @@
                             task_id,
                             description=_("[  丢失  ]:"),
                             filename=trim_filename(full_path.name, 45),
                             state="completed",
                         )
                         return
                     else:
-                        logger.error(_("HTTP错误: {0}".format(e)))
+                        logger.error(_("HTTP错误: {0}").format(e))
                         await self.progress.update(
                             task_id,
                             description=_("[  失败  ]:"),
                             filename=trim_filename(full_path.name, 45),
                             state="completed",
                         )
                         return
 
                 except Exception as e:
-                    logger.error(_("m3u8文件解析失败: {0}".format(e)))
+                    logger.error(_("m3u8文件解析失败: {0}").format(e))
                     logger.error(traceback.format_exc())
                     await self.progress.update(
                         task_id,
                         description=_("[  失败  ]:"),
                         filename=trim_filename(full_path.name, 45),
                         state="completed",
                     )
                     return
 
     async def initiate_download(
         self,
         file_type: str,
-        file_url: str,
+        file_url: Union[str, List[str]],
         base_path: Union[str, Path],
         file_name: str,
         file_suffix: Optional[str],
     ) -> None:
         """
         初始化下载任务。如果文件已经存在，则跳过下载。否则，创建一个新的异步下载任务。
         (Initiate a download task. If file already exists,
         skip the download. Otherwise, create a new async download task)
 
         Args:
             file_type (str): 文件类型描述 (File type description)
-            file_url (str): 文件URL (File URL)
+            file_url (Union[str, List[str]]): 文件URL (File URL)
             file_name (str): 文件名称 (File name)
             base_path (Union[str, Path]): 基础路径 (Base path)
             file_suffix (Optional[str]): 文件后缀 (File suffix)
+
+        Note:
+            file_url仅代表一个文件的链接，当file_url为列表时，表示该文件的多个链接
+            (file_url represents only a link to a file, when file_url is a list,
+                it represents multiple links to the file)
         """
 
         # 文件路径
         file_path = f"{file_name}{file_suffix}"
         # 文件全路径
         full_path = self._ensure_path(base_path) / file_path
 
@@ -336,15 +397,15 @@
                 start=True,
                 total=1,
                 completed=1,
             )
             await self.progress.update(task_id, state="completed")
         else:
             task_id = await self.progress.add_task(
-                description=_("[  {0}  ]:".format(file_type)),
+                description=_("[  {0}  ]:").format(file_type),
                 filename=trim_filename(file_path, 45),
                 start=True,
             )
             await self.progress.update(task_id, state="starting")
             download_task = asyncio.create_task(
                 self.download_file(task_id, file_url, full_path)
             )
@@ -383,15 +444,15 @@
                 start=True,
                 total=1,
                 completed=1,
             )
             await self.progress.update(task_id, state="completed")
         else:
             task_id = await self.progress.add_task(
-                description=_("[  {0}  ]:".format(file_type)),
+                description=_("[  {0}  ]:").format(file_type),
                 filename=trim_filename(file_path, 45),
                 start=True,
             )
             await self.progress.update(task_id, state="starting")
             download_task = asyncio.create_task(
                 self.save_file(task_id, content, full_path)
             )
@@ -429,28 +490,28 @@
                 start=True,
                 total=1,
                 completed=1,
             )
             await self.progress.update(task_id, state="completed")
         else:
             task_id = await self.progress.add_task(
-                description=_("[  {0}  ]:".format(file_type)),
+                description=_("[  {0}  ]:").format(file_type),
                 filename=trim_filename(file_path, 45),
                 start=True,
             )
             await self.progress.update(task_id, state="starting")
             download_task = asyncio.create_task(
                 self.download_m3u8_stream(task_id, m3u8_url, full_path)
             )
             self.download_tasks.append(download_task)
 
     async def execute_tasks(self):
         """执行所有下载任务 (Execute all download tasks)"""
         logger.debug(
-            _("开始执行下载任务，本次共有 {0} 个任务".format(len(self.download_tasks)))
+            _("开始执行下载任务，本次共有 {0} 个任务").format(len(self.download_tasks))
         )
         await asyncio.gather(*self.download_tasks)
         self.download_tasks.clear()
 
     async def close(self) -> None:
         """关闭下载器 (Close the downloader)"""
         await self.aclient.aclose()
```

### Comparing `f2-0.0.1.4/f2/exceptions/__init__.py` & `f2-0.0.1.5/f2/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/exceptions/api_exceptions.py` & `f2-0.0.1.5/f2/exceptions/api_exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,74 +4,75 @@
 
 exception_console = RichConsoleManager().exception_console
 
 
 class APIError(Exception):
     """基本API异常类，其他API异常都会继承这个类"""
 
-    def __init__(self, status_code=None):
-        self.status_code = status_code
+    def __init__(self, message=None, status_code=None):
         exception_console.print(
             "请前往QA文档 https://johnserf-seed.github.io/f2/question-answer/qa.html 查看相关帮助"
         )
+        self.status_code = status_code
+        super().__init__(message)
 
-    def display_error(self):
-        """显示错误信息和状态码（如果有的话）"""
-        return f"Error: {self.args[0]}." + (
-            f" Status Code: {self.status_code}." if self.status_code else ""
+    def __str__(self):
+        """返回错误信息和文件路径（如果有的话）"""
+        return f"{super().__str__()}" + (
+            f" Status Code: {self.status_code}" if self.status_code else ""
         )
 
 
 class APIConnectionError(APIError):
     """当与API的连接出现问题时抛出"""
 
-    def display_error(self):
-        return f"API Connection Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APIUnavailableError(APIError):
     """当API服务不可用时抛出，例如维护或超时"""
 
-    def display_error(self):
-        return f"API Unavailable Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APINotFoundError(APIError):
     """当API端点不存在时抛出"""
 
-    def display_error(self):
-        return f"API Not Found Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APIResponseError(APIError):
     """当API返回的响应与预期不符时抛出"""
 
-    def display_error(self):
-        return f"API Response Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APIRateLimitError(APIError):
     """当达到API的请求速率限制时抛出"""
 
-    def display_error(self):
-        return f"API Rate Limit Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APITimeoutError(APIError):
     """当API请求超时时抛出"""
 
-    def display_error(self):
-        return f"API Timeout Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APIUnauthorizedError(APIError):
     """当API请求由于授权失败而被拒绝时抛出"""
 
-    def display_error(self):
-        return f"API Unauthorized Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
 
 
 class APIRetryExhaustedError(APIError):
     """当API请求重试次数用尽时抛出"""
 
-    def display_error(self):
-        return f"API Retry Exhausted Error: {self.args[0]}."
+    def __init__(self, message=None, status_code=None):
+        super().__init__(message, status_code)
```

### Comparing `f2-0.0.1.4/f2/exceptions/file_exceptions.py` & `f2-0.0.1.5/f2/exceptions/file_exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,54 +4,45 @@
 
 exception_console = RichConsoleManager().exception_console
 
 
 class FileError(Exception):
     """基本的文件错误异常类，其他文件异常都会继承这个类"""
 
-    def __init__(self, filepath=None):
-        self.filepath = filepath
+    def __init__(self, message, filepath=None):
         exception_console.print(
             "请前往QA文档 https://johnserf-seed.github.io/f2/question-answer/qa.html 查看相关帮助"
         )
+        self.filepath = filepath
+        super().__init__(message)
 
-    def display_error(self):
-        """显示错误信息和文件路径（如果有的话）"""
-        return f"File Error: {self.args[0]}." + (
-            f" Filepath: {self.filepath}." if self.filepath else ""
-        )
+    def __str__(self):
+        """返回错误信息和文件路径（如果有的话）"""
+        return f"{super().__str__()} Filepath: {self.filepath}" if self.filepath else ""
 
 
-class FileNotFound(FileError, FileNotFoundError):
+class FileNotFound(FileError):
     """文件不存在错误"""
 
-    def display_error(self):
-        return f"File Not Found Error: {self.args[0]}." + (
-            f" Filepath: {self.filepath}." if self.filepath else ""
-        )
+    def __init__(self, message=None, filepath=None):
+        super().__init__(message, filepath)
 
 
-class FilePermissionError(FileError, PermissionError):
+class FilePermissionError(FileError):
     """文件权限错误"""
 
-    def display_error(self):
-        return f"File Permission Error: {self.args[0]}." + (
-            f" Filepath: {self.filepath}." if self.filepath else ""
-        )
+    def __init__(self, message, filepath=None):
+        super().__init__(message, filepath)
 
 
 class FileReadError(FileError):
     """文件读取错误"""
 
-    def display_error(self):
-        return f"File Read Error: {self.args[0]}." + (
-            f" Filepath: {self.filepath}." if self.filepath else ""
-        )
+    def __init__(self, message, filepath=None):
+        super().__init__(message, filepath)
 
 
 class FileWriteError(FileError):
     """文件写入错误"""
 
-    def display_error(self):
-        return f"File Write Error: {self.args[0]}." + (
-            f" Filepath: {self.filepath}." if self.filepath else ""
-        )
+    def __init__(self, message, filepath=None):
+        super().__init__(message, filepath)
```

### Comparing `f2-0.0.1.4/f2/i18n/translator.py` & `f2-0.0.1.5/f2/i18n/translator.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/languages/en_US/LC_MESSAGES/en_US.mo` & `f2-0.0.1.5/f2/languages/en_US/LC_MESSAGES/en_US.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: f2-translate\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"PO-Revision-Date: 2024-02-15 23:31+0800\n"
+"PO-Revision-Date: 2024-04-05 00:24+0800\n"
 "Last-Translator: JohnserfSeed <johnserf-seed@foxmail.com>\n"
 "Language-Team: English, United States\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -14,20 +14,14 @@
 "X-Crowdin-Project: f2-translate\n"
 "X-Crowdin-Project-ID: 631650\n"
 "X-Crowdin-Language: en-US\n"
 "X-Crowdin-File: messages.pot\n"
 "X-Crowdin-File-ID: 2\n"
 "X-Generator: Poedit 3.3.2\n"
 
-msgid "'{0}' 配置文件路径不存在"
-msgstr "'{0}' Configuration file path does not exist"
-
-msgid "'{0}' 配置文件路径无写权限"
-msgstr "'{0}' Configuration file path has no write permissions"
-
 msgid ""
 "- 单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，文案，封面，直播，"
 "原声。"
 msgstr ""
 "- one video, user post, liked post, collect post, mix post, note, desc, "
 "cover, live, original sound。"
 
@@ -59,65 +53,62 @@
 msgid "- 获取微博"
 msgstr "- Get Weibo"
 
 msgid "- 获取网易云音乐作品"
 msgstr "- Get music from NetEase Cloud Music"
 
 msgid ""
-"- 记录app的debug到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏感"
-"信息[/red]"
+"- 记录app的调试日志到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏"
+"感信息[/red]"
 msgstr ""
-"- Record the app's debug to /logs, in case of a bug when submitting an "
-"Issue, please attach the file and [red]delete personal sensitive "
-"information[/red]"
+"- Record the app's debug logs to /logs, such as bugs submit Issue when the "
+"attached file and [red]delete personal sensitive information[/red]."
 
-msgid "401 由于某些错误, 无法获取ttwid"
-msgstr "Unauthorized request,Unable to get ttwid"
+msgid "0: [bold]全部下载[/bold]"
+msgstr "0: [bold]All downloads[/bold]"
 
-msgid "404 无法找到API端点"
-msgstr "API endpoint not found"
+msgid "API内容请求失败，请更换新cookie后再试"
+msgstr ""
+"API content request failed, please replace the new cookie and try again"
 
-msgid "API服务不可用。类名: {0}"
+msgid "API服务不可用。类名：{0}"
 msgstr "API service is not available. Class name: {0}"
 
-msgid "API错误码：{0}。类名: {1}"
-msgstr "API error code: {0}. Class name: {1}"
-
-msgid "BaseDownloader 请求头headers:{0}"
-msgstr "BaseDownloader 请求头 headers:{0}"
-
 msgid "CLI参数：{0}"
 msgstr "CLI parameters: {0}"
 
+msgid "HTTP状态码错误："
+msgstr "HTTP status code error:"
+
 msgid "HTTP状态错误, 尝试GET请求失败: {0}, 错误详情: {1}"
 msgstr "HTTP status error, Failed GET request attempt: {0}, Error details: {1}"
 
-msgid "HTTP状态错误: {0}, URL: {1}, 尝试次数: {2}"
-msgstr "HTTP status error: {0}, URL: {1}, attempt: {2}"
-
 msgid "HTTP状态错误: {0}, 状态码: {1}"
 msgstr "HTTP status error: {0}, status code: {1}"
 
+msgid "HTTP状态错误：{0}, URL：{1}, 尝试次数：{2}"
+msgstr "HTTP Status Error: {0}, URL: {1}, Attempts: {2}"
+
 msgid "HTTP错误: {0}"
 msgstr "HTTP error: {0}"
 
 msgid "Hello, World!"
 msgstr "Hello, World!"
 
-msgid "SSO检查扫码状态接口地址:"
-msgstr "SSO Check Sweep Status Interface Address:"
+msgid "SSO检查扫码状态接口地址：{0}"
+msgstr "SSO check sweep status interface address: {0}"
 
-msgid "SSO检查登录状态接口地址:"
-msgstr "SSO Check Login Status interface address:"
+msgid "SSO检查登录状态接口地址：{0}"
+msgstr "SSO check login status interface address: {0}"
 
 msgid "SSO登录失败，请重试！"
 msgstr "SSO login failed, please try again！"
 
-msgid "SSO获取二维码接口地址:"
-msgstr "SSO get QR code interface address:"
+msgid "SSO获取二维码接口地址：{0}"
+msgstr "SSO get QR code interface address: {0}"
 
 msgid "TS文件下载失败: {0}"
 msgstr "TS file download failed: {0}"
 
 msgid "TS文件下载超时: {0}"
 msgstr "TS file download timed out: {0}"
 
@@ -126,20 +117,29 @@
 
 msgid "[  {0}  ]:"
 msgstr "[  {0}  ]:"
 
 msgid "[  丢失  ]:"
 msgstr "[  Loss  ]"
 
+msgid "[  丢失  ]：所有链接都无法下载"
+msgstr "[ Missing ]: All links are unavailable for downloading"
+
 msgid "[  失败  ]:"
 msgstr "[  Fails  ]"
 
+msgid "[  失败  ]："
+msgstr "[  Failure  ]"
+
 msgid "[  完成  ]:"
 msgstr "[  Done  ]"
 
+msgid "[  完成  ]："
+msgstr "[  Done  ]"
+
 msgid "[  登录  ]:二维码过期，重新获取！"
 msgstr "[  Login  ]:QR code expired, re-fetch！"
 
 msgid "[  登录  ]:扫描二维码成功！"
 msgstr "[  Login  ]:Successful scanning of QR code！"
 
 msgid "[  登录  ]:扫码环境异常，请前往app验证！"
@@ -155,27 +155,36 @@
 
 msgid "[  登录  ]:访问频繁，请检查参数！"
 msgstr "[  Login  ]:Access is frequent, check the parameters！"
 
 msgid "[  跳过  ]:"
 msgstr "[  Skips  ]"
 
+msgid "[bold yellow]请输入希望下载的合辑序号：[/bold yellow]"
+msgstr ""
+"[bold yellow]Please enter the serial number of the compilation you wish to "
+"download:[/bold yellow]"
+
+msgid "[bold yellow]请输入希望下载的收藏夹序号：[/bold yellow]"
+msgstr ""
+"[bold yellow]Please enter the serial number of the favorite you would like "
+"to download:[/bold yellow]"
+
 msgid "`{0}` 中的 `{1}` 不符合命名模式"
 msgstr "`{1}` in `{0}` does not conform to naming patterns"
 
 msgid "bilibili 或 bili"
 msgstr "bilibili or bili"
 
 msgid ""
-"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取 f2 -d dy --"
-"help，如扫码登录请保留双引号cookie: ，再使用--sso-login命令。"
+"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取。如 `--auto-"
+"cookie edge`"
 msgstr ""
-"cookie cannot be empty. Please provide valid cookie parameters, or "
-"automatically get f2 -d dy --help from your browser, e.g., to scan for login "
-"please keep the double quotes cookie: and then use the --sso-login command。"
+"the cookie cannot be empty. Please provide a valid cookie parameter, or get "
+"it automatically from the browser. For example, `--auto-cookie edge`"
 
 msgid "douyin 或 dy"
 msgstr "douyin or dy"
 
 msgid "f2 请求 Content-Length 时发生未知错误: {0}, 错误详情: {1}"
 msgstr ""
 "f2 Unknown error occurred while requesting Content-Length: {0}, error "
@@ -189,61 +198,59 @@
 
 msgid "m3u8文件或ts文件未找到，可能直播结束"
 msgstr "m3u8 file or ts file not found, possibly the end of the live"
 
 msgid "m3u8文件解析失败: {0}"
 msgstr "failed to parse m3u8 file: {0}"
 
-msgid ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 douyin 新"
-"规则。"
-msgstr ""
-"msToken: Please check and update the msToken in the conf.yaml configuration "
-"file in f2 to match the new douyin rule。"
-
-msgid ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 tiktok 新"
-"规则。"
-msgstr ""
-"msToken: Please check and update the msToken in the conf.yaml configuration "
-"file in f2 to match the new tiktok rules。"
+msgid "msToken API错误：{0}"
+msgstr "msToken API error: {0}"
 
 msgid "neteasy_music 或 nem"
 msgstr "neteasy_music or nem"
 
-msgid "odin_tt: 检查没有通过, 请更新配置文件中的odin_tt"
-msgstr "odin_tt: Check failed, please update the odin_tt in the conf file"
-
 msgid "tiktok 或 tk"
 msgstr "tiktok or tk"
 
 msgid "ttwid: 检查没有通过, 请更新配置文件中的ttwid"
 msgstr "ttwid: Check failed, please update the ttwid in the conf file"
 
+msgid "ttwid无法找到API端点"
+msgstr "ttwid can't find API endpoints"
+
 msgid "twitch 或 tv"
 msgstr "twitch or tv"
 
 msgid "twitter 或 x"
 msgstr "twitter or x"
 
 msgid "weibo 或 wb"
 msgstr "weibo or wb"
 
 msgid "youtube 或 ytb"
 msgstr "youtube or ytb"
 
+msgid "{0} 内容不符合要求"
+msgstr "{0} Content does not meet requirements"
+
+msgid "{0} 在服务器上的总内容长度为：{1} 字节"
+msgstr "{0} Total content length on the server: {1} bytes"
+
+msgid "{0} 已存在，将覆盖"
+msgstr "{0} already exists, will be overwritten"
+
 msgid "{0} 应用配置文件生成成功，保存至 {1}"
 msgstr ""
 "{0} Application configuration file generated successfully, saved to {1}"
 
 msgid "{0} 应用配置未找到"
 msgstr "{0} Application configuration not found"
 
-msgid "{0} 该作品已被屏蔽，无法下载"
-msgstr "{0} This work has been blocked from being downloaded"
+msgid "{0} 无法找到API端点"
+msgstr "{0} Unable to find API endpoint"
 
 msgid "{0} 该作品没有动态封面"
 msgstr "{0} There is no dynamic cover for this work"
 
 msgid "{0} 该作品没有封面"
 msgstr "{0} There is no cover for this work"
 
@@ -255,16 +262,21 @@
 
 msgid "{0} 该图集没有图片链接，无法下载"
 msgstr "{0} The atlas has no image link and cannot be downloaded"
 
 msgid "{0} 页没有找到作品"
 msgstr "{0} Page not found"
 
-msgid "{0}在服务器上的总内容长度为：{1} 字节"
-msgstr "The total content length of {0} on the server is: {1} bytes"
+msgid "{0}: {1} (包含 {2} 个作品，收藏夹ID {3})"
+msgstr "{0}: {1} (contains {2} entries, Favorite ID {3})"
+
+msgid "{0}：{1} (包含 {2} 个作品[以网页实际数量为准]，收藏夹ID {3})"
+msgstr ""
+"{0}:{1} (contains {2} entries [based on actual number of pages], Favorite ID "
+"{3})"
 
 msgid "⏳"
 msgstr "⏳"
 
 msgid "⚠"
 msgstr "⚠"
 
@@ -277,311 +289,393 @@
 msgid ""
 "下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"
 msgstr ""
 "Download works released in the date range, format: 2022-01-01|2023-01-01, "
 "'all' is to download all works"
 
 msgid ""
-"下载模式：主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑(mix), 直播"
-"(live), 推荐作品(feed), 搜索作品(search)"
-msgstr "Download Mode: post, like, collect, mix, live, feed, search"
-
-msgid ""
 "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), "
 "合辑播放列表(mix)"
 msgstr "Download modes: one, post, like, collect, mix"
 
 msgid ""
-"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collect)，"
-"合辑(mix)，直播(live)"
-msgstr "Download Mode: One, Post, Like, Collect, Mix, Live"
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，合辑(mix)，直播(live)"
+msgstr "Download Mode: One, Post, Like, Collection, Favorites, Mix, Live"
+
+msgid ""
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，收藏音乐(music)，合辑(mix)，直播(live)"
+msgstr ""
+"Download mode: single work (one), home page work (post), like works (like), "
+"collection (collection), favorite works (collects), collection of music "
+"(music), compilation (mix), live (live)"
 
 msgid "不存在该模式: {0}"
 msgstr "This mode does not exist: {0}"
 
-msgid "不支持的浏览器选项, 输入f2 dy --help查看更多帮助!"
-msgstr "Unsupported browser options, type f2 dy --help for more help!"
-
 msgid "不能同时初始化和更新配置文件"
 msgstr "Cannot initialize and update configuration files at the same time"
 
 msgid "临时文件已完全下载"
 msgstr "Temporary file has been fully downloaded"
 
 msgid "主播昵称: {0} 开播时间: {1} 直播流清晰度: {2}"
 msgstr "Nickname: {0} Start Time: {1} Streaming Clarity: {2}"
 
 msgid "主配置参数：{0}"
 msgstr "Main configuration parameters: {0}"
 
-msgid "主配置路径： {0}"
+msgid "主配置路径：{0}"
 msgstr "Main configuration path: {0}"
 
-msgid "主页作品接口地址:"
-msgstr "Post interface address:"
+msgid "主页作品接口地址：{0}"
+msgstr "Home page work interface address: {0}"
+
+msgid "主页喜欢作品接口地址：{0}"
+msgstr "HomeLike WorksInterface Address: {0}"
+
+msgid "主页收藏作品接口地址：{0}"
+msgstr "Home Favorite Works Interface Address: {0}"
+
+msgid "从接口每页可获取作品数，不建议超过20"
+msgstr ""
+"The number of works that can be fetched from the interface per page is not "
+"recommended to be more than 20"
 
 msgid "从接口每页可获取作品数，不建议超过20。"
 msgstr ""
 "The number of works that can be fetched from the interface per page is not "
 "recommended to exceed 20。"
 
 msgid ""
 "代理服务器，最多 2 个参数，http与https。空格区分 2 个参数 http://x.x.x.x "
 "https://x.x.x.x"
 msgstr ""
 "Proxy server, up to 2 parameters, http and https. 2 parameters distinguished "
 "by space http://x.x.x.x https://x.x.x.x"
 
+msgid "作品ID: {0} 作品文案: {1} 作者: {2}"
+msgstr "Work ID: {0} Work Text: {1} Author: {2}"
+
+msgid "作品ID：{0} 作品文案：{1} 作者：{2}"
+msgstr "Work ID: {0} Work Text: {1} Author: {2}"
+
+msgid "作品保存位置，支持绝对与相对路径"
+msgstr "Where to save your work, supports absolute and relative paths"
+
 msgid "作品保存位置，支持绝对与相对路径。"
 msgstr "Work save location, support absolute and relative path。"
 
-msgid "作品保存位置，默认为 'Download'"
-msgstr "Where to save your work, default is 'Download'"
-
 msgid "作品发布时间不在指定区间内：{0}"
 msgstr "The work is not published within the specified interval: {0}"
 
 msgid "作品发布时间在指定区间内：作品id {0} 发布时间 {1}"
 msgstr ""
 "The posting time of the work is within the specified interval: work id {0} "
 "posting time {1}"
 
-msgid "作品评论接口地址:"
-msgstr "Post comment interface address:"
+msgid "作品合集ID：{0} 作品合集标题：{1}"
+msgstr "Collection ID: {0} Collection Title: {1}"
 
-msgid "作品详情接口地址:"
-msgstr "Post details interface address:"
+msgid "作品评论接口地址：{0}"
+msgstr "Work comment interface address: {0}"
+
+msgid "作品详情接口地址：{0}"
+msgstr "Work details interface address: {0}"
 
 msgid "使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"
 msgstr ""
 "Use SSO sweep login to get [yellow]cookie[/yellow], save LF master profile"
 
-msgid "使用命令行选项更新配置文件"
-msgstr "Use the command line option to update the configuration file"
+msgid "使用SSO扫码登录获取cookie，保存低频主配置文件"
+msgstr ""
+"Use SSO sweep login to get cookies and save the low-frequency master "
+"configuration file"
 
 msgid "使用命令行选项更新配置文件。需要先使用'-c'选项提供一个配置文件路径"
 msgstr ""
 "Use the command line option to update the configuration file. You need to "
 "provide a configuration file path first with the '-c' option"
 
-msgid "例： f2 dy -h 来获取douyin的命令帮助"
-msgstr "Example: f2 dy -h to get help with douyin commands"
+msgid "例：f2 -d DEBUG dy 日志级别为调试运行"
+msgstr "Example: f2 -d DEBUG dy Log level is debug run"
 
-msgid "全局作品文件命名方式"
-msgstr "Global video file naming convention"
+msgid "例：f2 dy -h/--help 获取douyin的命令帮助"
+msgstr "Example: f2 dy -h/--help Get help for commands in douyin"
 
 msgid "全局作品文件命名方式，前往文档查看更多帮助"
 msgstr "Global file naming convention, go to the documentation for more help"
 
-msgid "关注作品接口地址:"
-msgstr "Follow the works interface address:"
-
-msgid "关注用户直播接口地址:"
-msgstr "Follow user live interface address:"
-
-msgid "内容长度为0，跳过下载"
-msgstr "Content length is 0, skipping download"
+msgid "关注作品接口地址：{0}"
+msgstr "Follow the work interface address: {0}"
 
-msgid "初始化配置文件"
-msgstr "Initializing configuration files"
+msgid "关注用户直播接口地址：{0}"
+msgstr "Follow user live interface address: {0}"
 
 msgid "初始化配置文件。不能同时初始化和更新配置文件"
 msgstr ""
 "Initialize the configuration file. It is not possible to initialize and "
 "update the configuration file at the same time"
 
-msgid "单个视频数据: {0}"
-msgstr "Single video data: {0}"
+msgid "单个作品数据：{0}"
+msgstr "Individual work data: {0}"
 
 msgid "原声"
 msgstr "Music"
 
+msgid "参数"
+msgstr "parameters"
+
 msgid "参数必须是列表类型"
 msgstr "Arguments must be of type list"
 
 msgid "参数必须是字典类型"
 msgstr "Arguments must be of dictionary type"
 
 msgid "参数必须是字符串类型"
 msgstr "Arguments must be of string type"
 
+msgid "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+msgstr ""
+"Parameter validation failed, update {0} in the F2 configuration file to "
+"match {1} new rule"
+
+msgid "另一个程序正在使用此文件或受异步调度影响，该任务需要重新下载"
+msgstr ""
+"Another program is using this file or is affected by asynchronous "
+"scheduling, the task needs to be re-downloaded"
+
 msgid "合辑: {0} 所有作品采集完毕"
 msgstr "Mix: {0} All works have been captured"
 
-msgid "合辑作品接口地址:"
-msgstr "Mix interface address:"
+msgid "合辑作品接口地址：{0}"
+msgstr "Interface address for compilation works: {0}"
 
-msgid "合辑列表接口地址:"
-msgstr "Playlist interface address:"
+msgid "合辑列表接口地址：{0}"
+msgstr "Compilation list interface address: {0}"
 
 msgid "合集: {0} 所有作品采集完毕"
 msgstr "Mix: {0} All works have been collected"
 
-msgid "合集作品接口地址:"
-msgstr "Mix interface address:"
+msgid "合集作品接口地址：{0}"
+msgstr "The interface address for the collection of works: {0}"
 
 msgid "响应状态码: {0}"
 msgstr "Status code: {0}"
 
-msgid "喜欢作品接口地址:"
-msgstr "Like interface address:"
+msgid "喜欢作品接口地址：{0}"
+msgstr "Favorite works interface address: {0}"
 
 msgid "图集"
 msgstr "IMG"
 
 msgid "在 {0} 应用里没有找到帮助文件"
 msgstr "Help file not found in {0} application"
 
+msgid "处理HTTP错误时遇到意外情况：{0}"
+msgstr "Unexpected conditions encountered while handling HTTP errors: {0}"
+
 msgid "子分区: {0} 主播昵称: {1}"
 msgstr "Subpartition: {0} Anchor Nickname: {1}"
 
-msgid "定位上一次作品接口地址:"
-msgstr "Locate the last work interface address:"
+msgid "定位上一次作品接口地址：{0}"
+msgstr "Locate the last work interface address: {0}"
 
 msgid "封面"
 msgstr "Cover"
 
+msgid "尝试删除临时文件失败：{0}"
+msgstr "Attempt to delete temporary file failed: {0}"
+
 msgid "已取消更新配置文件!"
 msgstr "Updating profiles has been canceled!"
 
 msgid "开始执行下载任务，本次共有 {0} 个任务"
 msgstr "Started the download task, there are {0} tasks this time"
 
-msgid "开始爬取合集: {0} 的视频"
-msgstr "Start crawling the videos of the mix: {0}"
+msgid "开始爬取作品：{0}"
+msgstr "Start crawling for entries: {0}"
+
+msgid "开始爬取合集: {0} 的作品"
+msgstr "Start crawling the collection: {0}'s work"
 
 msgid "开始爬取房间号: {0} 的数据"
 msgstr "Start crawling for room number: {0}"
 
-msgid "开始爬取用户: {0} feed的视频"
-msgstr "Start crawling videos from user: {0} feed"
+msgid "开始爬取收藏夹：{0} 的作品"
+msgstr "Start crawling favorites: {0}'s entries"
+
+msgid "开始爬取用户: {0} feed的作品"
+msgstr "Start crawling user: {0} feed entries"
+
+msgid "开始爬取用户: {0} 合集的作品"
+msgstr "Start crawling the User: {0} collection"
+
+msgid "开始爬取用户收藏夹"
+msgstr "Start crawling user favorites"
+
+msgid "开始爬取用户收藏的作品"
+msgstr "Start crawling user favorites"
+
+msgid "开始爬取用户收藏的音乐作品"
+msgstr "Start crawling the user's music collection"
 
-msgid "开始爬取用户: {0} 发布的视频"
-msgstr "Start crawling videos posted by user: {0}"
+msgid "开始爬取用户：{0} 发布的作品"
+msgstr "Start crawling User: {0} Postings"
 
-msgid "开始爬取用户: {0} 合集的视频"
-msgstr "Start crawling user: {0} mix videos"
+msgid "开始爬取用户：{0} 喜欢的作品"
+msgstr "Start Crawling User: {0} Likes"
 
-msgid "开始爬取用户: {0} 喜欢的视频"
-msgstr "Start crawling user: {0} like video"
+msgid "开始爬取用户：{0} 收藏的作品"
+msgstr "Start crawling User: {0} Favorites"
 
-msgid "开始爬取用户: {0} 收藏的视频"
-msgstr "Start crawling user: {0} collect videos"
+msgid "开始爬取用户：{0} 点赞的作品"
+msgstr "Start crawling for entries liked by user:{0}"
 
-msgid "开始爬取用户: {0} 点赞的视频"
-msgstr "Start crawling user: {0} like videos"
+msgid "开始爬取用户：{0} 的作品合集列表"
+msgstr "Start crawling the collection list of user:{0}'s works"
 
-msgid "开始爬取用户: {0} 的视频合集列表"
-msgstr "Start crawling the video play list of user: {0}"
+msgid "开始爬取用户：{0} 的关注用户"
+msgstr "Users: {0} All concerned users captured"
 
-msgid "开始爬取用户收藏的视频"
-msgstr "Start crawling user collect videos"
+msgid "开始爬取用户：{0} 的粉丝"
+msgstr "Start crawling the followers of user:{0}"
 
 msgid "开始爬取直播: {0} 的数据"
 msgstr "Start crawling live: {0}"
 
 msgid "开始爬取第 {0} 页"
 msgstr "Start crawling page {0}"
 
-msgid "开始爬取视频: {0}"
-msgstr "Start crawling video: {0}"
+msgid "异步的任务数"
+msgstr "Number of asynchronous tasks"
 
 msgid "异步的任务数。"
 msgstr "The number of asynchronous tasks。"
 
-msgid "异步的任务数，默认为 10"
-msgstr "The number of asynchronous tasks, default is 10"
+msgid "当前 {0} 直播已结束"
+msgstr "Currently {0} live broadcast is closed"
 
 msgid "当前请求的cursor: {0}"
 msgstr "Currently requested cursor: {0}"
 
+msgid "当前请求的cursor：{0}"
+msgstr "Currently requested cursor: {0}"
+
 msgid "当前请求的max_cursor: {0}"
 msgstr "max_cursor of the current request: {0}"
 
+msgid "当前请求的max_cursor：{0}"
+msgstr "Max_cursor of the current request: {0}"
+
+msgid "当前请求的max_cursor：{0}， max_counts：{1}"
+msgstr "max_cursor of the current request: {0}, max_counts: {1}"
+
+msgid "当前请求的offset：{0}"
+msgstr "Current request offset: {0}"
+
+msgid "当前请求的offset：{0} max_time：{1}"
+msgstr "Offset of current request: {0} max_time: {1}"
+
 msgid "找到了未下载完的文件 {0}, 大小为 {1} 字节"
 msgstr "Found an unfinished file {0}, size is {1} bytes"
 
 msgid "抖音无水印解析"
 msgstr "Douyin de-watermark"
 
 msgid "接口状态码异常 {0}, 请检查重试"
 msgstr "Interface status code exception {0}, please check and retry"
 
+msgid "接口状态码异常 {0}，请检查重试"
+msgstr "Interface status code exception {0}, please check and retry"
+
 msgid "接口状态码异常, 请检查重试"
 msgstr "Interface status code is abnormal, please check and retry"
 
-msgid "收藏作品接口地址:"
-msgstr "Collect interface address:"
+msgid "描述"
+msgstr "descriptions"
 
-msgid "文件区块下载失败: {0}"
+msgid "收藏作品接口地址：{0}"
+msgstr "Favorite Works Interface Address: {0}"
+
+msgid "收藏夹ID：{0} 收藏夹标题：{1}"
+msgstr "Favorite ID: {0} Favorite Title: {1}"
+
+msgid "收藏夹作品接口地址：{0}"
+msgstr "Favorite Works interface address: {0}"
+
+msgid "收藏夹接口地址：{0}"
+msgstr "Favorites interface address: {0}"
+
+msgid "收藏夹：{0} 所有作品采集完毕，共爬取 {1} 个作品"
+msgstr ""
+"Favorites: {0} All entries have been collected, {1} entries were crawled"
+
+msgid "文件区块下载失败：{0}"
 msgstr "File block download failed: {0}"
 
-msgid "文件区块下载超时: {0}"
-msgstr "File block download timed out: {0}"
+msgid "文件区块下载超时：{0}"
+msgstr "File block download timeout: {0}"
 
 msgid "文件名模板字段 {0} 不存在，请检查"
 msgstr "The filename template field {0} does not exist, check the"
 
 msgid "文案"
 msgstr "Desc"
 
 msgid "无效响应类型。响应类型: {0}"
 msgstr "Invalid response type. Response Type: {0}"
 
 msgid "无法从 {0} 浏览器中获取cookie"
 msgstr "Unable to get cookie from {0} browser"
 
-msgid "无法从{0}浏览器中获取cookie"
-msgstr "Unable to get cookies from {0} browser"
-
-msgid "无法找到API端点"
-msgstr "API endpoint not found"
-
 msgid "无法解析作品发布时间：{0}"
 msgstr "Unable to parse work Published: {0}"
 
 msgid "无法读取该TS文件字节长度，将使用默认400kb块大小处理数据"
 msgstr ""
 "Unable to read this TS file byte length, will use default 400kb block size "
 "to process data"
 
 msgid "日期区间参数格式错误，请查阅文档后重试"
 msgstr ""
 "The date range parameter is formatted incorrectly, please consult the "
 "documentation and try again"
 
+msgid "是否保存原声歌词"
+msgstr "Whether to save the original lyrics"
+
+msgid "是否保存视频原声"
+msgstr "Whether to save video soundtrack"
+
 msgid "是否保存视频原声。可选：'yes'、'no'"
 msgstr "Whether to save the original sound of the video. Optional: 'yes', 'no'"
 
-msgid "是否保存视频原声，默认为 'yes'"
-msgstr "Whether to save the original sound of the video, default is 'yes'"
+msgid "是否保存视频封面"
+msgstr "Whether to save the video cover"
 
 msgid "是否保存视频封面。可选：'yes'、'no'"
 msgstr "Whether to save the video cover. Optional: 'yes', 'no'"
 
-msgid "是否保存视频封面，默认为 'yes'"
-msgstr "Whether to save the video cover, default is 'yes'"
+msgid "是否保存视频文案"
+msgstr "Whether to save video desc"
 
 msgid "是否保存视频文案。可选：'yes'、'no'"
 msgstr "Whether to save the video text. Optional: 'yes', 'no'"
 
-msgid "是否保存视频文案，默认为 'yes'"
-msgstr "Whether or not to save the video copy, default is 'yes'"
+msgid "是否保存视频歌词"
+msgstr "Whether to save video lyrics"
+
+msgid "是否将作品保存到单独的文件夹"
+msgstr "Whether to save your video in a separate folder"
 
 msgid "是否将作品保存到单独的文件夹。可选：'yes'、'no'"
 msgstr "Whether to save the work to a separate folder. Optional: 'yes', 'no'"
 
-msgid "是否将作品保存到单独的文件夹，默认为 'yes'"
-msgstr "Whether or not to save the work to a separate folder, default is 'yes'"
-
-msgid "是否自动从浏览器获取cookie，以及从哪个浏览器获取"
-msgstr ""
-"Whether cookies are automatically fetched from browsers, and from which "
-"browsers"
-
 msgid "是否要使用命令行的参数更新配置文件？"
 msgstr ""
 "Should I update the configuration file using parameters from the command "
 "line？"
 
 msgid "显示富文本帮助"
 msgstr "Show Rich Text Help"
@@ -593,290 +687,369 @@
 msgstr "Display language. Default is 'zh_CN'. Optional: 'zh_CN', 'en_US'"
 
 msgid "显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'。不支持配置文件修改。"
 msgstr ""
 "Display language. Default is 'zh_CN'. Optional: 'zh_CN', 'en_US'. "
 "Configuration file modification is not supported。"
 
+msgid "显示语言。默认为 'zh_CN'，可选：'zh_CN'、'en_US'，不支持配置文件修改"
+msgstr ""
+"Display language. Default is 'zh_CN', optional: 'zh_CN', 'en_US', does not "
+"support configuration file modification"
+
 msgid ""
 "更加详细的参数说明请点击[link=https://johnserf-seed.github.io/f2/site-config."
 "html][dark_violet]前往文档[/dark_violet][/]查看"
 msgstr ""
 "For a more detailed description of the parameters, please click "
 "[link=https://johnserf-seed.github.io/f2/site-config.html][dark_violet]Go to "
 "Documentation[/dark_violet][/]View"
 
-msgid "最大作品下载数 默认为 0，表示无限制"
-msgstr ""
-"Maximum number of artwork downloads Default is 0, which means no limitation"
-
 msgid "最大作品下载数。0 表示无限制"
 msgstr "Maximum number of downloads. 0 means unlimited"
 
 msgid "最大数量: {0} 每次请求数量: {1}"
 msgstr "Maximum number: {0} Number per request: {1}"
 
-msgid "朋友作品接口地址:"
-msgstr "Friend's work interface address:"
+msgid "最大数量：{0} 每次请求数量：{1}"
+msgstr "Maximum number: {0} Number per request: {1}"
 
-msgid "未在响应中找到aweme_id"
-msgstr "No aweme_id found in the address of the response"
+msgid "朋友作品接口地址：{0}"
+msgstr "Friend Works interface address: {0}"
 
-msgid "未在响应中找到unique_id"
-msgstr "Unique_id not found in response"
+msgid "未在响应中找到 {0}"
+msgstr "Not found in response {0}"
 
-msgid "未在响应的地址中找到aweme_id, 检查链接是否为作品页"
+msgid "未在响应中找到 {0}，检查链接是否为用户主页。类名: {1}"
 msgstr ""
-"Aweme_id not found in the response address, check if the link is a post page"
+"Did not find {0} in the response, check if the link is to the user's home "
+"page. Class name: {1}"
 
-msgid "未在响应的地址中找到sec_uid, 检查链接是否为用户主页类名: {0}"
+msgid "未在响应的地址中找到aweme_id，检查链接是否为作品页"
 msgstr ""
-"No sec_uid found in the response, check if the link is to the user's "
-"homepage class name: {0}"
+"Not found aweme_id in the address of the response, check if the link is a "
+"works page"
 
-msgid "未在响应的地址中找到sec_user_id, 检查链接是否为用户主页类名: {0}"
+msgid "未在响应的地址中找到sec_user_id，检查链接是否为用户主页类名：{0}"
 msgstr ""
-"Not found sec_user_id in the response, check if the link is to the user's "
-"homepage class name: {0}"
+"Not found sec_user_id in the address of the response, check if the link is "
+"to the user's homepage class name: {0}"
 
-msgid "未在响应的地址中找到webcast_id, 检查链接是否为直播页"
-msgstr "Webcast_id not found in response address, check if link is a live page"
+msgid "未在响应的地址中找到webcast_id，检查链接是否为直播页"
+msgstr ""
+"Webcast_id not found in the address of the response, check if the link is a "
+"live page"
 
-msgid "未找到API端点。类名: {0}"
+msgid "未找到API端点。类名：{0}"
 msgstr "API endpoint not found. Class name: {0}"
 
 msgid "未找到m3u8文件的segments, 尝试获取嵌套的m3u8文件"
 msgstr "No segments found in m3u8 file, trying to get the nested m3u8 file"
 
 msgid "未找到嵌套m3u8文件的segments, 可能直播结束或该主播无法使用m3u8方法解析"
 msgstr ""
 "No segments found in nested m3u8 file, possibly the end of the live or the "
 "anchor cannot use the m3u8 method to parse"
 
-msgid "未授权的请求。类名: {0}"
+msgid "未授权的请求。类名：{0}"
 msgstr "Unauthorized request. Class name: {0}"
 
-msgid "根据作品发布日期区间下载作品，默认为 '0'"
-msgstr ""
-"Download works according to the work release date interval, default is '0'"
-
 msgid ""
 "根据模式提供相应的链接。例如：主页、点赞、收藏作品填入主页链接，单作品填入作"
 "品链接，合辑与直播同上"
 msgstr ""
 "Provide the appropriate link according to the mode. For example: homepage, "
 "likes and favorites fill in the homepage link, single works fill in the "
 "works link, compilations and live streams are the same as above"
 
 msgid "欢迎提交PR适配更多网站"
 msgstr "Welcome to submit PR to adapt more websites"
 
-msgid "每页作品数，默认为 20个作品/页"
-msgstr "The default number of entries per page is 20 entries per page"
+msgid "歌词"
+msgstr "LYRIC"
+
+msgid "歌词数据字段错误：{0}"
+msgstr "Lyrics data field error: {0}"
+
+msgid "歌词数据类型错误：{0}"
+msgstr "Lyrics data type error: {0}"
 
 msgid "没有找到 {0} 应用"
 msgstr "No {0} applications found"
 
 msgid "没有找到符合条件的作品"
 msgstr "No eligible entries found"
 
-msgid "爬取结束，共爬取{0}个视频"
-msgstr "End of crawl, total {0} videos crawled"
+msgid "爬取了 {0} 个关注用户"
+msgstr "Crawled {0} followers"
+
+msgid "爬取了 {0} 个粉丝用户"
+msgstr "Crawled {0} followers"
+
+msgid "爬取结束，共找到 {0} 个收藏夹"
+msgstr "End of crawl, total {0} favorites found"
+
+msgid "爬取结束，共爬取 {0} 个作品"
+msgstr "End of crawl, total {0} entries crawled"
+
+msgid "爬取结束，共爬取 {0} 个合集作品"
+msgstr "End of crawl, total {0} collections crawled"
+
+msgid "爬取结束，共爬取 {0} 个收藏作品"
+msgstr "End of crawl, total {0} favorites crawled"
+
+msgid "爬取结束，共爬取 {0} 个收藏夹"
+msgstr "End of crawl, total {0} favorites crawled"
+
+msgid "爬取结束，共爬取 {0} 个点赞作品"
+msgstr "End of crawl, total {0} liked entries"
+
+msgid "爬取结束，共爬取 {0} 个用户"
+msgstr "End of crawl, total {0} users crawled"
+
+msgid "爬取结束，共爬取 {0} 个音乐作品"
+msgstr "End of crawl, total {0} music entries crawled"
+
+msgid "爬取结束，共爬取 {0} 个首页推荐作品"
+msgstr "End of crawl, total {0} homepage referrals crawled"
+
+msgid "状态"
+msgstr "statuses"
 
 msgid "生成X-Bogus失败: {0})"
 msgstr "Generating X-Bogus failed: {0})"
 
+msgid "生成歌词文件失败：{0}，请检查歌词 `data` 内容"
+msgstr ""
+"Failed to generate lyrics file: {0}, please check lyrics `data` content"
+
 msgid "生成虚假的msToken"
 msgstr "Generate a fake msToken"
 
 msgid "用户: {0} 所有作品采集完毕"
 msgstr "User: {0} All works have been captured"
 
-msgid "用户: {0} 没有视频合集"
-msgstr "Users: {0} No Play list"
+msgid "用户ID：{0} 用户昵称：{1} 用户作品数：{2}"
+msgstr "User ID: {0} User Nickname: {1} Number of User Works: {2}"
+
+msgid "用户ID：{0} 用户昵称：{1} 用户作品数：{2} 额外内容：{3}"
+msgstr "User ID: {0} User Nickname: {1} Number of User Works: {2} Extras: {3}"
+
+msgid "用户信息接口地址：{0}"
+msgstr "User information interface address: {0}"
+
+msgid "用户关注列表接口地址：{0}"
+msgstr "User Follow List interface address: {0}"
+
+msgid "用户收藏的作品采集完毕"
+msgstr "The collection of the user's favorite works is finished"
+
+msgid "用户收藏的音乐作品采集完毕"
+msgstr "The user's collection of music pieces is captured"
+
+msgid "用户没有作品合辑"
+msgstr "Users do not have a collection of works"
 
-msgid "用户信息接口地址:"
-msgstr "User detail interface address:"
+msgid "用户粉丝列表接口地址：{0}"
+msgstr "User fan list interface address: {0}"
 
-msgid "用户收藏的视频采集完毕"
-msgstr "User's collect videos are captured"
+msgid "用户：{0} 所有作品采集完毕"
+msgstr "User: {0} All works are captured"
 
-msgid "由于某些错误, 无法获取msToken"
-msgstr "Unauthorized request,Unable to get msToken"
+msgid "用户：{0} 所有关注用户采集完毕"
+msgstr "Users: {0} All concerned users captured"
 
-msgid "由于某些错误, 无法获取ttwid"
-msgstr "Due to some error, the ttwid could not be retrieved"
+msgid "用户：{0} 所有粉丝采集完毕"
+msgstr "User: {0} All fans captured"
+
+msgid "用户：{0} 没有作品合集"
+msgstr "Users: {0} No collection of works"
 
 msgid ""
 "登录后的[yellow]cookie[/yellow]，如果使用未登录的[yellow]cookie[/yellow]，则"
 "无法持久稳定下载作品"
 msgstr ""
 "Logged in [yellow]cookie[/yellow], if you use a non-logged in "
 "[yellow]cookie[/yellow], you will not be able to download the work in a "
 "persistent and stable manner"
 
-msgid "登录后的cookie"
-msgstr "Cookie after login"
-
 msgid "登录后的cookie，如果使用未登录的cookie，则无法持久稳定下载作品"
 msgstr ""
 "Logged in cookies, if you use a cookie that is not logged in, you will not "
 "be able to download the work in a persistent and stable manner"
 
 msgid "直播"
 msgstr "LIVE"
 
 msgid "直播ID: {0} 直播标题: {1} 直播状态: {2} 观看人数: {3}"
 msgstr "Live ID: {0} Live Title: {1} Live Status: {2} Viewers: {3}"
 
 msgid "直播信息爬取结束"
 msgstr "End of live feed crawling"
 
-msgid "直播已结束"
-msgstr "The live has ended"
+msgid "直播接口地址（room_id）：{0}"
+msgstr "Live streaming interface address (room_id): {0}"
 
-msgid "直播接口地址:"
-msgstr "Live Streaming address:"
+msgid "直播接口地址：{0}"
+msgstr "Live streaming interface address: {0}"
 
-msgid "直播接口地址（room_id）:"
-msgstr "Live streaming interface address (room_id):"
-
-msgid "相关推荐作品接口地址:"
-msgstr "Related address:"
+msgid "相关推荐作品接口地址：{0}"
+msgstr "Related recommended works interface address: {0}"
 
 msgid "第 {0} 次响应内容为空, 状态码: {1}, URL:{2}"
 msgstr "The {0} th response is empty, status code: {1}, URL:{2}"
 
+msgid "第 {0} 页没有找到作品"
+msgstr "Page {0} No work found"
+
+msgid "等待 {0} 秒后继续"
+msgstr "Wait {0} seconds and continue"
+
 msgid "筛选日期区间：{0} 至 {1}"
 msgstr "Filter Date Range: {0} to {1}"
 
+msgid "网络请求并发连接数"
+msgstr "Number of concurrent connections for network requests"
+
 msgid "网络请求并发连接数。"
 msgstr "The number of concurrent connections for network requests。"
 
-msgid "网络请求并发连接数，默认为 5"
-msgstr "Number of concurrent connections for network requests, default is 5"
+msgid "网络请求超时时间"
+msgstr "Network request timeout"
 
 msgid "网络请求超时时间。"
 msgstr "Network request timeout time。"
 
-msgid "网络请求超时时间，默认为 10"
-msgstr "Network request timeout, default is 10"
+msgid "网络请求超时重试数"
+msgstr "Number of network request timeout retries"
 
 msgid "网络请求超时重试数。"
 msgstr "The number of network request timeout retries。"
 
-msgid "网络请求超时重试数，默认为 5"
-msgstr "Network request timeout retries, default is 5"
-
 msgid ""
-"自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、"
-"opera。使用该命令前请确保关闭所选的浏览器"
+"自动从浏览器获取[yellow]cookie[/yellow]，使用该命令前请确保关闭所选的浏览器"
 msgstr ""
-"Automatically get [yellow]cookies[/yellow] from browsers. Options: chrome, "
-"firefox, edge, opera. be sure to close the selected browser before using "
-"this command"
+"Automatically get [yellow]cookies[/yellow] from browsers, make sure to close "
+"the selected browser before using this command"
 
-msgid ""
-"自动从浏览器获取cookie。可选项：chrome、firefox、edge、opera。使用该命令前请"
-"确保关闭所选的浏览器"
+msgid "自动从浏览器获取cookie，使用该命令前请确保关闭所选的浏览器"
 msgstr ""
-"Automatically get cookies from browsers. options: chrome, firefox, edge, "
-"opera. make sure you close the selected browser before using this command"
+"Automatically get cookies from browsers, make sure to close the selected "
+"browser before using this command"
 
-msgid "自动获取Cookie失败: {0}"
-msgstr "handler auto cookie error: {0}"
+msgid "自动获取Cookie失败：{0}"
+msgstr "Failed to get cookie automatically: {0}"
 
 msgid "自定义配置参数：{0}"
 msgstr "Customized configuration parameters: {0}"
 
-msgid "自定义配置路径： {0}"
+msgid "自定义配置路径：{0}"
 msgstr "Custom configuration path: {0}"
 
 msgid "至少提供 secUid 或 uniqueId 中的一个参数"
 msgstr "Provide at least one of secUid or uniqueId as a parameter"
 
-msgid "获取aweme_id失败, {0}"
-msgstr "Failed to get aweme_id, {0}"
+msgid "至少提供 user_id 或 sec_user_id 中的一个参数"
+msgstr "Provide at least one of user_id or sec_user_id"
 
-msgid "获取sec_uid失败, {0}"
-msgstr "Failed to get sec_uid, {0}"
-
-msgid "获取unique_id失败, {0}"
-msgstr "Failed to get unique_id, {0}"
+msgid "获取 {0} 失败，{1}"
+msgstr "Get {0} Failed, {1}"
 
 msgid "获取数据失败。状态码: {0}"
 msgstr "Failed to get data. Status code: {0}"
 
 msgid "获取端点数据失败, 次数达到上限"
 msgstr "Failed to get endpoint data, number of times reached the upper limit"
 
 msgid "要更新配置, 首先需要使用'-c'选项提供一个自定义配置文件路径"
 msgstr ""
 "To update the configuration, you first need to provide a custom "
 "configuration file path using the '-c' option"
 
+msgid "要更新配置，首先需要使用'-c'选项提供一个自定义配置文件路径"
+msgstr ""
+"To update the configuration, you first need to provide a custom "
+"configuration file path using the '-c' option"
+
 msgid "视频"
 msgstr "Video"
 
-msgid "视频ID: {0} 视频文案: {1} 作者: {2}"
+msgid "视频ID：{0} 视频文案：{1} 作者：{2}"
 msgstr "Video ID: {0} Video Copy: {1} Author: {2}"
 
-msgid "视频合集ID: {0} 视频合集标题: {1}"
-msgstr "Video Mix ID: {0} Video Mix Title: {1}"
-
 msgid "解析 {0} 接口 JSON 失败： {1}"
 msgstr "Parsing {0} interface JSON failed: {1}"
 
+msgid "该 {0} 作品已被屏蔽，无法下载"
+msgstr "The {0} work has been blocked from download"
+
 msgid "该链接返回的是room_id，请使用`fetch_user_live_videos_by_room_id`接口"
 msgstr ""
 "This link returns the room_id, use the `fetch_user_live_videos_by_room_id` "
 "interface"
 
-msgid "语言设置，默认为 'zh_CN'"
-msgstr "Language setting, default is 'zh_CN'"
+msgid "请关闭所有已打开的浏览器重试，并且你有适当的权限访问浏览器！"
+msgstr ""
+"Please close all open browsers and retry, and that you have the proper "
+"permissions to access the browser!"
 
-msgid "请关闭所有已打开的浏览器重试, 并且你有适当的权限访问浏览器 !"
+msgid ""
+"请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常"
+"详细信息：{3}"
 msgstr ""
-"Please close all open browsers and try again, and you have the proper "
-"permissions to access the browser !"
+"Request for endpoint failed, please check current network environment. Link: "
+"{0}, Agent: {1}, Exception Class Name: {2}, Exception Details: {3}"
 
 msgid "输入的URL List不合法。类名：{0}"
 msgstr "The input URL List is not legal. Class name: {0}"
 
 msgid "输入的URL不合法。类名：{0}"
 msgstr "The input URL is not legal. Class name: {0}"
 
-msgid "连接到API时发生错误，请检查URL或网络情况。类名: {0}"
-msgstr ""
-"An error occurred while connecting to the API, please check the URL or "
-"network conditions. Class name: {0}"
-
 msgid "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
 msgstr ""
 "Failed to connect to endpoint, check network environment or Agent: {0} "
 "Agent: {1} Class name: {2}"
 
 msgid "连接超时错误: {0}"
 msgstr "Connection timeout error: {0}"
 
+msgid "配置文件不存在"
+msgstr "Configuration file does not exist"
+
 msgid "配置文件已更新!"
 msgstr "Configuration files have been updated!"
 
 msgid "配置文件的路径，[red]最低优先[/red]"
 msgstr "Path to the configuration file, [red]lowest priority[/red]"
 
 msgid "配置文件的路径，最低优先"
 msgstr "Path to configuration file, highest priority"
 
-msgid "除了单个作品外，其他URL都需要用户主页URL"
-msgstr "User homepage URLs are required for all URLs except one video"
+msgid "配置文件路径无写权限"
+msgstr "Configuration file does not exist"
+
+msgid "链接 {0} 内容长度为0，尝试下一个链接是否可用"
+msgstr "link {0} content length 0, try next link if available"
+
+msgid "链接：{0}，状态码 {1}：{2} "
+msgstr "Link: {0}, status code {1}: {2} "
+
+msgid "音乐"
+msgstr "SONG"
+
+msgid "音乐ID：{0} 音乐标题：{1} 作者：{2}"
+msgstr "Music ID: {0} Music Title: {1} Author: {2}"
+
+msgid "音乐收藏接口地址：{0}"
+msgstr "Music Collection interface address: {0}"
 
 msgid "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
 msgstr ""
 "The page is not available, probably due to a regional restriction (proxy). "
 "Class name: {0}"
 
-msgid "首页推荐作品接口地址:"
-msgstr "Home Feed interface address:"
+msgid "首页推荐作品接口地址：{0}"
+msgstr "Home recommended works interface address: {0}"
 
-msgid "首页推荐接口地址:"
-msgstr "Home feed interface address:"
+msgid "首页推荐接口地址：{0}"
+msgstr "Home Recommended Interface Address: {0}"
```

### Comparing `f2-0.0.1.4/f2/languages/zh_CN/LC_MESSAGES/zh_CN.mo` & `f2-0.0.1.5/f2/languages/zh_CN/LC_MESSAGES/zh_CN.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: f2-translate\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"PO-Revision-Date: 2024-02-15 23:12+0800\n"
+"PO-Revision-Date: 2024-04-05 00:25+0800\n"
 "Last-Translator: JohnserfSeed <johnserf-seed@foxmail.com>\n"
 "Language-Team: Chinese Simplified\n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -14,20 +14,14 @@
 "X-Generator: Poedit 3.3.2\n"
 "X-Crowdin-Project: f2-translate\n"
 "X-Crowdin-Project-ID: 631650\n"
 "X-Crowdin-Language: zh-CN\n"
 "X-Crowdin-File: messages.pot\n"
 "X-Crowdin-File-ID: 2\n"
 
-msgid "'{0}' 配置文件路径不存在"
-msgstr "'{0}' 配置文件路径不存在"
-
-msgid "'{0}' 配置文件路径无写权限"
-msgstr "'{0}' 配置文件路径无写权限"
-
 msgid ""
 "- 单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，文案，封面，直播，"
 "原声。"
 msgstr ""
 "- 单个作品，主页作品，点赞作品，收藏作品，合辑作品，图文，文案，封面，直播，"
 "原声。"
 
@@ -59,64 +53,61 @@
 msgid "- 获取微博"
 msgstr "- 获取微博"
 
 msgid "- 获取网易云音乐作品"
 msgstr "- 获取网易云音乐作品"
 
 msgid ""
-"- 记录app的debug到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏感"
-"信息[/red]"
+"- 记录app的调试日志到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏"
+"感信息[/red]"
 msgstr ""
-"- 记录app的debug到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏感"
-"信息[/red]"
-
-msgid "401 由于某些错误, 无法获取ttwid"
-msgstr "401 由于某些错误, 无法获取ttwid"
-
-msgid "404 无法找到API端点"
-msgstr "404 无法找到API端点"
+"- 记录app的调试日志到/logs下，如遇BUG提交Issue时请附带该文件并[red]删除个人敏"
+"感信息[/red]"
 
-msgid "API服务不可用。类名: {0}"
-msgstr "API服务不可用。类名: {0}"
+msgid "0: [bold]全部下载[/bold]"
+msgstr "0: [bold]全部下载[/bold]"
 
-msgid "API错误码：{0}。类名: {1}"
-msgstr "API错误码：{0}。类名: {1}"
+msgid "API内容请求失败，请更换新cookie后再试"
+msgstr "API内容请求失败，请更换新cookie后再试"
 
-msgid "BaseDownloader 请求头headers:{0}"
-msgstr "BaseDownloader 请求头headers:{0}"
+msgid "API服务不可用。类名：{0}"
+msgstr "API服务不可用。类名：{0}"
 
 msgid "CLI参数：{0}"
 msgstr "CLI参数：{0}"
 
+msgid "HTTP状态码错误："
+msgstr "HTTP状态码错误："
+
 msgid "HTTP状态错误, 尝试GET请求失败: {0}, 错误详情: {1}"
 msgstr "HTTP状态错误, 尝试GET请求失败: {0}, 错误详情: {1}"
 
-msgid "HTTP状态错误: {0}, URL: {1}, 尝试次数: {2}"
-msgstr "HTTP状态错误: {0}, URL: {1}, 尝试次数: {2}"
-
 msgid "HTTP状态错误: {0}, 状态码: {1}"
 msgstr "HTTP状态错误: {0}, 状态码: {1}"
 
+msgid "HTTP状态错误：{0}, URL：{1}, 尝试次数：{2}"
+msgstr "HTTP状态错误：{0}, URL：{1}, 尝试次数：{2}"
+
 msgid "HTTP错误: {0}"
 msgstr "HTTP错误: {0}"
 
 msgid "Hello, World!"
 msgstr "你好，世界！"
 
-msgid "SSO检查扫码状态接口地址:"
-msgstr "SSO检查扫码状态接口地址:"
+msgid "SSO检查扫码状态接口地址：{0}"
+msgstr "SSO检查扫码状态接口地址：{0}"
 
-msgid "SSO检查登录状态接口地址:"
-msgstr "SSO检查登录状态接口地址:"
+msgid "SSO检查登录状态接口地址：{0}"
+msgstr "SSO检查登录状态接口地址：{0}"
 
 msgid "SSO登录失败，请重试！"
 msgstr "SSO登录失败，请重试！"
 
-msgid "SSO获取二维码接口地址:"
-msgstr "SSO获取二维码接口地址:"
+msgid "SSO获取二维码接口地址：{0}"
+msgstr "SSO获取二维码接口地址：{0}"
 
 msgid "TS文件下载失败: {0}"
 msgstr "TS文件下载失败: {0}"
 
 msgid "TS文件下载超时: {0}"
 msgstr "TS文件下载超时: {0}"
 
@@ -125,20 +116,29 @@
 
 msgid "[  {0}  ]:"
 msgstr "[  {0}  ]:"
 
 msgid "[  丢失  ]:"
 msgstr "[  丢失  ]:"
 
+msgid "[  丢失  ]：所有链接都无法下载"
+msgstr "[  丢失  ]：所有链接都无法下载"
+
 msgid "[  失败  ]:"
 msgstr "[  失败  ]:"
 
+msgid "[  失败  ]："
+msgstr "[  失败  ]："
+
 msgid "[  完成  ]:"
 msgstr "[  完成  ]:"
 
+msgid "[  完成  ]："
+msgstr "[  完成  ]："
+
 msgid "[  登录  ]:二维码过期，重新获取！"
 msgstr "[  登录  ]:二维码过期，重新获取！"
 
 msgid "[  登录  ]:扫描二维码成功！"
 msgstr "[  登录  ]:扫描二维码成功！"
 
 msgid "[  登录  ]:扫码环境异常，请前往app验证！"
@@ -152,26 +152,32 @@
 
 msgid "[  登录  ]:访问频繁，请检查参数！"
 msgstr "[  登录  ]:访问频繁，请检查参数！"
 
 msgid "[  跳过  ]:"
 msgstr "[  跳过  ]:"
 
+msgid "[bold yellow]请输入希望下载的合辑序号：[/bold yellow]"
+msgstr "[bold yellow]请输入希望下载的合辑序号：[/bold yellow]"
+
+msgid "[bold yellow]请输入希望下载的收藏夹序号：[/bold yellow]"
+msgstr "[bold yellow]请输入希望下载的收藏夹序号：[/bold yellow]"
+
 msgid "`{0}` 中的 `{1}` 不符合命名模式"
 msgstr "`{0}` 中的 `{1}` 不符合命名模式"
 
 msgid "bilibili 或 bili"
 msgstr "bilibili 或 bili"
 
 msgid ""
-"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取 f2 -d dy --"
-"help，如扫码登录请保留双引号cookie: ，再使用--sso-login命令。"
+"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取。如 `--auto-"
+"cookie edge`"
 msgstr ""
-"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取 f2 -d dy --"
-"help，如扫码登录请保留双引号cookie: ，再使用--sso-login命令。"
+"cookie不能为空。请提供有效的 cookie 参数，或自动从浏览器获取。如 `--auto-"
+"cookie edge`"
 
 msgid "douyin 或 dy"
 msgstr "douyin 或 dy"
 
 msgid "f2 请求 Content-Length 时发生未知错误: {0}, 错误详情: {1}"
 msgstr "f2 请求 Content-Length 时发生未知错误: {0}, 错误详情: {1}"
 
@@ -183,60 +189,58 @@
 
 msgid "m3u8文件或ts文件未找到，可能直播结束"
 msgstr "m3u8文件或ts文件未找到，可能直播结束"
 
 msgid "m3u8文件解析失败: {0}"
 msgstr "m3u8文件解析失败: {0}"
 
-msgid ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 douyin 新"
-"规则。"
-msgstr ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 douyin 新"
-"规则。"
-
-msgid ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 tiktok 新"
-"规则。"
-msgstr ""
-"msToken: 请检查并更新 f2 中 conf.yaml 配置文件中的 msToken，以匹配 tiktok 新"
-"规则。"
+msgid "msToken API错误：{0}"
+msgstr "msToken API错误：{0}"
 
 msgid "neteasy_music 或 nem"
 msgstr "neteasy_music 或 nem"
 
-msgid "odin_tt: 检查没有通过, 请更新配置文件中的odin_tt"
-msgstr "odin_tt: 检查没有通过, 请更新配置文件中的odin_tt"
-
 msgid "tiktok 或 tk"
 msgstr "tiktok 或 tk"
 
 msgid "ttwid: 检查没有通过, 请更新配置文件中的ttwid"
 msgstr "ttwid: 检查没有通过, 请更新配置文件中的ttwid"
 
+msgid "ttwid无法找到API端点"
+msgstr "ttwid无法找到API端点"
+
 msgid "twitch 或 tv"
 msgstr "twitch 或 tv"
 
 msgid "twitter 或 x"
 msgstr "twitter 或 x"
 
 msgid "weibo 或 wb"
 msgstr "weibo 或 wb"
 
 msgid "youtube 或 ytb"
 msgstr "youtube 或 ytb"
 
+msgid "{0} 内容不符合要求"
+msgstr "{0} 内容不符合要求"
+
+msgid "{0} 在服务器上的总内容长度为：{1} 字节"
+msgstr "{0} 在服务器上的总内容长度为：{1} 字节"
+
+msgid "{0} 已存在，将覆盖"
+msgstr "{0} 已存在，将覆盖"
+
 msgid "{0} 应用配置文件生成成功，保存至 {1}"
 msgstr "{0} 应用配置文件生成成功，保存至 {1}"
 
 msgid "{0} 应用配置未找到"
 msgstr "{0} 应用配置未找到"
 
-msgid "{0} 该作品已被屏蔽，无法下载"
-msgstr "{0} 该作品已被屏蔽，无法下载"
+msgid "{0} 无法找到API端点"
+msgstr "{0} 无法找到API端点"
 
 msgid "{0} 该作品没有动态封面"
 msgstr "{0} 该作品没有动态封面"
 
 msgid "{0} 该作品没有封面"
 msgstr "{0} 该作品没有封面"
 
@@ -248,16 +252,19 @@
 
 msgid "{0} 该图集没有图片链接，无法下载"
 msgstr "{0} 该图集没有图片链接，无法下载"
 
 msgid "{0} 页没有找到作品"
 msgstr "{0} 页没有找到作品"
 
-msgid "{0}在服务器上的总内容长度为：{1} 字节"
-msgstr "{0}在服务器上的总内容长度为：{1} 字节"
+msgid "{0}: {1} (包含 {2} 个作品，收藏夹ID {3})"
+msgstr "{0}: {1} (包含 {2} 个作品，收藏夹ID {3})"
+
+msgid "{0}：{1} (包含 {2} 个作品[以网页实际数量为准]，收藏夹ID {3})"
+msgstr "{0}：{1} (包含 {2} 个作品[以网页实际数量为准]，收藏夹ID {3})"
 
 msgid "⏳"
 msgstr "⏳"
 
 msgid "⚠"
 msgstr "⚠"
 
@@ -269,302 +276,374 @@
 
 msgid ""
 "下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"
 msgstr ""
 "下载日期区间发布的作品，格式：2022-01-01|2023-01-01，'all' 为下载所有作品"
 
 msgid ""
-"下载模式：主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑(mix), 直播"
-"(live), 推荐作品(feed), 搜索作品(search)"
-msgstr ""
-"下载模式：主页作品(post), 点赞作品(like), 收藏作品(collect), 合辑(mix), 直播"
-"(live), 推荐作品(feed), 搜索作品(search)"
-
-msgid ""
 "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), "
 "合辑播放列表(mix)"
 msgstr ""
 "下载模式：单个作品(one)，主页作品(post), 点赞作品(like), 收藏作品(collect), "
 "合辑播放列表(mix)"
 
 msgid ""
-"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collect)，"
-"合辑(mix)，直播(live)"
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，合辑(mix)，直播(live)"
+msgstr ""
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，合辑(mix)，直播(live)"
+
+msgid ""
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，收藏音乐(music)，合辑(mix)，直播(live)"
 msgstr ""
-"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品(collect)，"
-"合辑(mix)，直播(live)"
+"下载模式：单个作品(one)，主页作品(post)，点赞作品(like)，收藏作品"
+"(collection)，收藏夹作品(collects)，收藏音乐(music)，合辑(mix)，直播(live)"
 
 msgid "不存在该模式: {0}"
 msgstr "不存在该模式: {0}"
 
-msgid "不支持的浏览器选项, 输入f2 dy --help查看更多帮助!"
-msgstr "不支持的浏览器选项, 输入f2 dy --help查看更多帮助!"
-
 msgid "不能同时初始化和更新配置文件"
 msgstr "不能同时初始化和更新配置文件"
 
 msgid "临时文件已完全下载"
 msgstr "临时文件已完全下载"
 
 msgid "主播昵称: {0} 开播时间: {1} 直播流清晰度: {2}"
 msgstr "主播昵称: {0} 开播时间: {1} 直播流清晰度: {2}"
 
 msgid "主配置参数：{0}"
 msgstr "主配置参数：{0}"
 
-msgid "主配置路径： {0}"
-msgstr "主配置路径： {0}"
+msgid "主配置路径：{0}"
+msgstr "主配置路径：{0}"
+
+msgid "主页作品接口地址：{0}"
+msgstr "主页作品接口地址：{0}"
+
+msgid "主页喜欢作品接口地址：{0}"
+msgstr "主页喜欢作品接口地址：{0}"
+
+msgid "主页收藏作品接口地址：{0}"
+msgstr "主页收藏作品接口地址：{0}"
 
-msgid "主页作品接口地址:"
-msgstr "主页作品接口地址:"
+msgid "从接口每页可获取作品数，不建议超过20"
+msgstr "从接口每页可获取作品数，不建议超过20"
 
 msgid "从接口每页可获取作品数，不建议超过20。"
 msgstr "从接口每页可获取作品数，不建议超过20。"
 
 msgid ""
 "代理服务器，最多 2 个参数，http与https。空格区分 2 个参数 http://x.x.x.x "
 "https://x.x.x.x"
 msgstr ""
 "代理服务器，最多 2 个参数，http与https。空格区分 2 个参数 http://x.x.x.x "
 "https://x.x.x.x"
 
+msgid "作品ID: {0} 作品文案: {1} 作者: {2}"
+msgstr "作品ID: {0} 作品文案: {1} 作者: {2}"
+
+msgid "作品ID：{0} 作品文案：{1} 作者：{2}"
+msgstr "作品ID：{0} 作品文案：{1} 作者：{2}"
+
+msgid "作品保存位置，支持绝对与相对路径"
+msgstr "作品保存位置，支持绝对与相对路径"
+
 msgid "作品保存位置，支持绝对与相对路径。"
 msgstr "作品保存位置，支持绝对与相对路径。"
 
-msgid "作品保存位置，默认为 'Download'"
-msgstr "作品保存位置，默认为 'Download'"
-
 msgid "作品发布时间不在指定区间内：{0}"
 msgstr "作品发布时间不在指定区间内：{0}"
 
 msgid "作品发布时间在指定区间内：作品id {0} 发布时间 {1}"
 msgstr "作品发布时间在指定区间内：作品id {0} 发布时间 {1}"
 
-msgid "作品评论接口地址:"
-msgstr "作品评论接口地址:"
+msgid "作品合集ID：{0} 作品合集标题：{1}"
+msgstr "作品合集ID：{0} 作品合集标题：{1}"
+
+msgid "作品评论接口地址：{0}"
+msgstr "作品评论接口地址：{0}"
 
-msgid "作品详情接口地址:"
-msgstr "作品详情接口地址:"
+msgid "作品详情接口地址：{0}"
+msgstr "作品详情接口地址：{0}"
 
 msgid "使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"
 msgstr "使用SSO扫码登录获取[yellow]cookie[/yellow]，保存低频主配置文件"
 
-msgid "使用命令行选项更新配置文件"
-msgstr "使用命令行选项更新配置文件"
+msgid "使用SSO扫码登录获取cookie，保存低频主配置文件"
+msgstr "使用SSO扫码登录获取cookie，保存低频主配置文件"
 
 msgid "使用命令行选项更新配置文件。需要先使用'-c'选项提供一个配置文件路径"
 msgstr "使用命令行选项更新配置文件。需要先使用'-c'选项提供一个配置文件路径"
 
-msgid "例： f2 dy -h 来获取douyin的命令帮助"
-msgstr "例： f2 dy -h 来获取douyin的命令帮助"
+msgid "例：f2 -d DEBUG dy 日志级别为调试运行"
+msgstr "例：f2 -d DEBUG dy 日志级别为调试运行"
 
-msgid "全局作品文件命名方式"
-msgstr "全局作品文件命名方式"
+msgid "例：f2 dy -h/--help 获取douyin的命令帮助"
+msgstr "例：f2 dy -h/--help 获取douyin的命令帮助"
 
 msgid "全局作品文件命名方式，前往文档查看更多帮助"
 msgstr "全局作品文件命名方式，前往文档查看更多帮助"
 
-msgid "关注作品接口地址:"
-msgstr "关注作品接口地址:"
-
-msgid "关注用户直播接口地址:"
-msgstr "关注用户直播接口地址:"
-
-msgid "内容长度为0，跳过下载"
-msgstr "内容长度为0，跳过下载"
+msgid "关注作品接口地址：{0}"
+msgstr "关注作品接口地址：{0}"
 
-msgid "初始化配置文件"
-msgstr "初始化配置文件"
+msgid "关注用户直播接口地址：{0}"
+msgstr "关注用户直播接口地址：{0}"
 
 msgid "初始化配置文件。不能同时初始化和更新配置文件"
 msgstr "初始化配置文件。不能同时初始化和更新配置文件"
 
-msgid "单个视频数据: {0}"
-msgstr "单个视频数据: {0}"
+msgid "单个作品数据：{0}"
+msgstr "单个作品数据：{0}"
 
 msgid "原声"
 msgstr "原声"
 
+msgid "参数"
+msgstr "参数"
+
 msgid "参数必须是列表类型"
 msgstr "参数必须是列表类型"
 
 msgid "参数必须是字典类型"
 msgstr "参数必须是字典类型"
 
 msgid "参数必须是字符串类型"
 msgstr "参数必须是字符串类型"
 
+msgid "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+msgstr "参数验证失败，请更新 F2 配置文件中的 {0}，以匹配 {1} 新规则"
+
+msgid "另一个程序正在使用此文件或受异步调度影响，该任务需要重新下载"
+msgstr "另一个程序正在使用此文件或受异步调度影响，该任务需要重新下载"
+
 msgid "合辑: {0} 所有作品采集完毕"
 msgstr "合辑: {0} 所有作品采集完毕"
 
-msgid "合辑作品接口地址:"
-msgstr "合辑作品接口地址:"
+msgid "合辑作品接口地址：{0}"
+msgstr "合辑作品接口地址：{0}"
 
-msgid "合辑列表接口地址:"
-msgstr "合辑列表接口地址:"
+msgid "合辑列表接口地址：{0}"
+msgstr "合辑列表接口地址：{0}"
 
 msgid "合集: {0} 所有作品采集完毕"
 msgstr "合集: {0} 所有作品采集完毕"
 
-msgid "合集作品接口地址:"
-msgstr "合集作品接口地址:"
+msgid "合集作品接口地址：{0}"
+msgstr "合集作品接口地址：{0}"
 
 msgid "响应状态码: {0}"
 msgstr "响应状态码: {0}"
 
-msgid "喜欢作品接口地址:"
-msgstr "喜欢作品接口地址:"
+msgid "喜欢作品接口地址：{0}"
+msgstr "喜欢作品接口地址：{0}"
 
 msgid "图集"
 msgstr "图集"
 
 msgid "在 {0} 应用里没有找到帮助文件"
 msgstr "在 {0} 应用里没有找到帮助文件"
 
+msgid "处理HTTP错误时遇到意外情况：{0}"
+msgstr "处理HTTP错误时遇到意外情况：{0}"
+
 msgid "子分区: {0} 主播昵称: {1}"
 msgstr "子分区: {0} 主播昵称: {1}"
 
-msgid "定位上一次作品接口地址:"
-msgstr "定位上一次作品接口地址:"
+msgid "定位上一次作品接口地址：{0}"
+msgstr "定位上一次作品接口地址：{0}"
 
 msgid "封面"
 msgstr "封面"
 
+msgid "尝试删除临时文件失败：{0}"
+msgstr "尝试删除临时文件失败：{0}"
+
 msgid "已取消更新配置文件!"
 msgstr "已取消更新配置文件!"
 
 msgid "开始执行下载任务，本次共有 {0} 个任务"
 msgstr "开始执行下载任务，本次共有 {0} 个任务"
 
-msgid "开始爬取合集: {0} 的视频"
-msgstr "开始爬取合集: {0} 的视频"
+msgid "开始爬取作品：{0}"
+msgstr "开始爬取作品：{0}"
+
+msgid "开始爬取合集: {0} 的作品"
+msgstr "开始爬取合集: {0} 的作品"
 
 msgid "开始爬取房间号: {0} 的数据"
 msgstr "开始爬取房间号: {0} 的数据"
 
-msgid "开始爬取用户: {0} feed的视频"
-msgstr "开始爬取用户: {0} feed的视频"
+msgid "开始爬取收藏夹：{0} 的作品"
+msgstr "开始爬取收藏夹：{0} 的作品"
+
+msgid "开始爬取用户: {0} feed的作品"
+msgstr "开始爬取用户: {0} feed的作品"
+
+msgid "开始爬取用户: {0} 合集的作品"
+msgstr "开始爬取用户: {0} 合集的作品"
+
+msgid "开始爬取用户收藏夹"
+msgstr "开始爬取用户收藏夹"
+
+msgid "开始爬取用户收藏的作品"
+msgstr "开始爬取用户收藏的作品"
 
-msgid "开始爬取用户: {0} 发布的视频"
-msgstr "开始爬取用户: {0} 发布的视频"
+msgid "开始爬取用户收藏的音乐作品"
+msgstr "开始爬取用户收藏的音乐作品"
 
-msgid "开始爬取用户: {0} 合集的视频"
-msgstr "开始爬取用户: {0} 合集的视频"
+msgid "开始爬取用户：{0} 发布的作品"
+msgstr "开始爬取用户：{0} 发布的作品"
 
-msgid "开始爬取用户: {0} 喜欢的视频"
-msgstr "开始爬取用户: {0} 喜欢的视频"
+msgid "开始爬取用户：{0} 喜欢的作品"
+msgstr "开始爬取用户：{0} 喜欢的作品"
 
-msgid "开始爬取用户: {0} 收藏的视频"
-msgstr "开始爬取用户: {0} 收藏的视频"
+msgid "开始爬取用户：{0} 收藏的作品"
+msgstr "开始爬取用户：{0} 收藏的作品"
 
-msgid "开始爬取用户: {0} 点赞的视频"
-msgstr "开始爬取用户: {0} 点赞的视频"
+msgid "开始爬取用户：{0} 点赞的作品"
+msgstr "开始爬取用户：{0} 点赞的作品"
 
-msgid "开始爬取用户: {0} 的视频合集列表"
-msgstr "开始爬取用户: {0} 的视频合集列表"
+msgid "开始爬取用户：{0} 的作品合集列表"
+msgstr "开始爬取用户：{0} 的作品合集列表"
 
-msgid "开始爬取用户收藏的视频"
-msgstr "开始爬取用户收藏的视频"
+msgid "开始爬取用户：{0} 的关注用户"
+msgstr "开始爬取用户：{0} 的关注用户"
+
+msgid "开始爬取用户：{0} 的粉丝"
+msgstr "开始爬取用户：{0} 的粉丝"
 
 msgid "开始爬取直播: {0} 的数据"
 msgstr "开始爬取直播: {0} 的数据"
 
 msgid "开始爬取第 {0} 页"
 msgstr "开始爬取第 {0} 页"
 
-msgid "开始爬取视频: {0}"
-msgstr "开始爬取视频: {0}"
+msgid "异步的任务数"
+msgstr "异步的任务数"
 
 msgid "异步的任务数。"
 msgstr "异步的任务数。"
 
-msgid "异步的任务数，默认为 10"
-msgstr "异步的任务数，默认为 10"
+msgid "当前 {0} 直播已结束"
+msgstr "当前 {0} 直播已结束"
 
 msgid "当前请求的cursor: {0}"
 msgstr "当前请求的cursor: {0}"
 
+msgid "当前请求的cursor：{0}"
+msgstr "当前请求的cursor：{0}"
+
 msgid "当前请求的max_cursor: {0}"
 msgstr "当前请求的max_cursor: {0}"
 
+msgid "当前请求的max_cursor：{0}"
+msgstr "当前请求的max_cursor：{0}"
+
+msgid "当前请求的max_cursor：{0}， max_counts：{1}"
+msgstr "当前请求的max_cursor：{0}， max_counts：{1}"
+
+msgid "当前请求的offset：{0}"
+msgstr "当前请求的offset：{0}"
+
+msgid "当前请求的offset：{0} max_time：{1}"
+msgstr "当前请求的offset：{0} max_time：{1}"
+
 msgid "找到了未下载完的文件 {0}, 大小为 {1} 字节"
 msgstr "找到了未下载完的文件 {0}, 大小为 {1} 字节"
 
 msgid "抖音无水印解析"
 msgstr "抖音无水印解析"
 
 msgid "接口状态码异常 {0}, 请检查重试"
 msgstr "接口状态码异常 {0}, 请检查重试"
 
+msgid "接口状态码异常 {0}，请检查重试"
+msgstr "接口状态码异常 {0}，请检查重试"
+
 msgid "接口状态码异常, 请检查重试"
 msgstr "接口状态码异常, 请检查重试"
 
-msgid "收藏作品接口地址:"
-msgstr "收藏作品接口地址:"
+msgid "描述"
+msgstr "描述"
 
-msgid "文件区块下载失败: {0}"
-msgstr "文件区块下载失败: {0}"
+msgid "收藏作品接口地址：{0}"
+msgstr "收藏作品接口地址：{0}"
 
-msgid "文件区块下载超时: {0}"
-msgstr "文件区块下载超时: {0}"
+msgid "收藏夹ID：{0} 收藏夹标题：{1}"
+msgstr "收藏夹ID：{0} 收藏夹标题：{1}"
+
+msgid "收藏夹作品接口地址：{0}"
+msgstr "收藏夹作品接口地址：{0}"
+
+msgid "收藏夹接口地址：{0}"
+msgstr "收藏夹接口地址：{0}"
+
+msgid "收藏夹：{0} 所有作品采集完毕，共爬取 {1} 个作品"
+msgstr "收藏夹：{0} 所有作品采集完毕，共爬取 {1} 个作品"
+
+msgid "文件区块下载失败：{0}"
+msgstr "文件区块下载失败：{0}"
+
+msgid "文件区块下载超时：{0}"
+msgstr "文件区块下载超时：{0}"
 
 msgid "文件名模板字段 {0} 不存在，请检查"
 msgstr "文件名模板字段 {0} 不存在，请检查"
 
 msgid "文案"
 msgstr "文案"
 
 msgid "无效响应类型。响应类型: {0}"
 msgstr "无效响应类型。响应类型: {0}"
 
 msgid "无法从 {0} 浏览器中获取cookie"
 msgstr "无法从 {0} 浏览器中获取cookie"
 
-msgid "无法从{0}浏览器中获取cookie"
-msgstr "无法从{0}浏览器中获取cookie"
-
-msgid "无法找到API端点"
-msgstr "无法找到API端点"
-
 msgid "无法解析作品发布时间：{0}"
 msgstr "无法解析作品发布时间：{0}"
 
 msgid "无法读取该TS文件字节长度，将使用默认400kb块大小处理数据"
 msgstr "无法读取该TS文件字节长度，将使用默认400kb块大小处理数据"
 
 msgid "日期区间参数格式错误，请查阅文档后重试"
 msgstr "日期区间参数格式错误，请查阅文档后重试"
 
+msgid "是否保存原声歌词"
+msgstr "是否保存原声歌词"
+
+msgid "是否保存视频原声"
+msgstr "是否保存视频原声"
+
 msgid "是否保存视频原声。可选：'yes'、'no'"
 msgstr "是否保存视频原声。可选：'yes'、'no'"
 
-msgid "是否保存视频原声，默认为 'yes'"
-msgstr "是否保存视频原声，默认为 'yes'"
+msgid "是否保存视频封面"
+msgstr "是否保存视频封面"
 
 msgid "是否保存视频封面。可选：'yes'、'no'"
 msgstr "是否保存视频封面。可选：'yes'、'no'"
 
-msgid "是否保存视频封面，默认为 'yes'"
-msgstr "是否保存视频封面，默认为 'yes'"
+msgid "是否保存视频文案"
+msgstr "是否保存视频文案"
 
 msgid "是否保存视频文案。可选：'yes'、'no'"
 msgstr "是否保存视频文案。可选：'yes'、'no'"
 
-msgid "是否保存视频文案，默认为 'yes'"
-msgstr "是否保存视频文案，默认为 'yes'"
+msgid "是否保存视频歌词"
+msgstr "是否保存视频歌词"
+
+msgid "是否将作品保存到单独的文件夹"
+msgstr "是否将作品保存到单独的文件夹"
 
 msgid "是否将作品保存到单独的文件夹。可选：'yes'、'no'"
 msgstr "是否将作品保存到单独的文件夹。可选：'yes'、'no'"
 
-msgid "是否将作品保存到单独的文件夹，默认为 'yes'"
-msgstr "是否将作品保存到单独的文件夹，默认为 'yes'"
-
-msgid "是否自动从浏览器获取cookie，以及从哪个浏览器获取"
-msgstr "是否自动从浏览器获取cookie，以及从哪个浏览器获取"
-
 msgid "是否要使用命令行的参数更新配置文件？"
 msgstr "是否要使用命令行的参数更新配置文件？"
 
 msgid "显示富文本帮助"
 msgstr "显示富文本帮助"
 
 msgid "显示经典帮助信息"
@@ -572,263 +651,336 @@
 
 msgid "显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'"
 msgstr "显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'"
 
 msgid "显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'。不支持配置文件修改。"
 msgstr "显示语言。默认为 'zh_CN'。可选：'zh_CN'、'en_US'。不支持配置文件修改。"
 
+msgid "显示语言。默认为 'zh_CN'，可选：'zh_CN'、'en_US'，不支持配置文件修改"
+msgstr "显示语言。默认为 'zh_CN'，可选：'zh_CN'、'en_US'，不支持配置文件修改"
+
 msgid ""
 "更加详细的参数说明请点击[link=https://johnserf-seed.github.io/f2/site-config."
 "html][dark_violet]前往文档[/dark_violet][/]查看"
 msgstr ""
 "更加详细的参数说明请点击[link=https://johnserf-seed.github.io/f2/site-config."
 "html][dark_violet]前往文档[/dark_violet][/]查看"
 
-msgid "最大作品下载数 默认为 0，表示无限制"
-msgstr "最大作品下载数 默认为 0，表示无限制"
-
 msgid "最大作品下载数。0 表示无限制"
 msgstr "最大作品下载数。0 表示无限制"
 
 msgid "最大数量: {0} 每次请求数量: {1}"
 msgstr "最大数量: {0} 每次请求数量: {1}"
 
-msgid "朋友作品接口地址:"
-msgstr "朋友作品接口地址:"
+msgid "最大数量：{0} 每次请求数量：{1}"
+msgstr "最大数量：{0} 每次请求数量：{1}"
 
-msgid "未在响应中找到aweme_id"
-msgstr "未在响应中找到aweme_id"
+msgid "朋友作品接口地址：{0}"
+msgstr "朋友作品接口地址：{0}"
 
-msgid "未在响应中找到unique_id"
-msgstr "未在响应中找到unique_id"
+msgid "未在响应中找到 {0}"
+msgstr "未在响应中找到 {0}"
 
-msgid "未在响应的地址中找到aweme_id, 检查链接是否为作品页"
-msgstr "未在响应的地址中找到aweme_id, 检查链接是否为作品页"
+msgid "未在响应中找到 {0}，检查链接是否为用户主页。类名: {1}"
+msgstr "未在响应中找到 {0}，检查链接是否为用户主页。类名: {1}"
 
-msgid "未在响应的地址中找到sec_uid, 检查链接是否为用户主页类名: {0}"
-msgstr "未在响应的地址中找到sec_uid, 检查链接是否为用户主页类名: {0}"
+msgid "未在响应的地址中找到aweme_id，检查链接是否为作品页"
+msgstr "未在响应的地址中找到aweme_id，检查链接是否为作品页"
 
-msgid "未在响应的地址中找到sec_user_id, 检查链接是否为用户主页类名: {0}"
-msgstr "未在响应的地址中找到sec_user_id, 检查链接是否为用户主页类名: {0}"
+msgid "未在响应的地址中找到sec_user_id，检查链接是否为用户主页类名：{0}"
+msgstr "未在响应的地址中找到sec_user_id，检查链接是否为用户主页类名：{0}"
 
-msgid "未在响应的地址中找到webcast_id, 检查链接是否为直播页"
-msgstr "未在响应的地址中找到webcast_id, 检查链接是否为直播页"
+msgid "未在响应的地址中找到webcast_id，检查链接是否为直播页"
+msgstr "未在响应的地址中找到webcast_id，检查链接是否为直播页"
 
-msgid "未找到API端点。类名: {0}"
-msgstr "未找到API端点。类名: {0}"
+msgid "未找到API端点。类名：{0}"
+msgstr "未找到API端点。类名：{0}"
 
 msgid "未找到m3u8文件的segments, 尝试获取嵌套的m3u8文件"
 msgstr "未找到m3u8文件的segments, 尝试获取嵌套的m3u8文件"
 
 msgid "未找到嵌套m3u8文件的segments, 可能直播结束或该主播无法使用m3u8方法解析"
 msgstr "未找到嵌套m3u8文件的segments, 可能直播结束或该主播无法使用m3u8方法解析"
 
-msgid "未授权的请求。类名: {0}"
-msgstr "未授权的请求。类名: {0}"
-
-msgid "根据作品发布日期区间下载作品，默认为 '0'"
-msgstr "根据作品发布日期区间下载作品，默认为 '0'"
+msgid "未授权的请求。类名：{0}"
+msgstr "未授权的请求。类名：{0}"
 
 msgid ""
 "根据模式提供相应的链接。例如：主页、点赞、收藏作品填入主页链接，单作品填入作"
 "品链接，合辑与直播同上"
 msgstr ""
 "根据模式提供相应的链接。例如：主页、点赞、收藏作品填入主页链接，单作品填入作"
 "品链接，合辑与直播同上"
 
 msgid "欢迎提交PR适配更多网站"
 msgstr "欢迎提交PR适配更多网站"
 
-msgid "每页作品数，默认为 20个作品/页"
-msgstr "每页作品数，默认为 20个作品/页"
+msgid "歌词"
+msgstr "歌词"
+
+msgid "歌词数据字段错误：{0}"
+msgstr "歌词数据字段错误：{0}"
+
+msgid "歌词数据类型错误：{0}"
+msgstr "歌词数据类型错误：{0}"
 
 msgid "没有找到 {0} 应用"
 msgstr "没有找到 {0} 应用"
 
 msgid "没有找到符合条件的作品"
 msgstr "没有找到符合条件的作品"
 
-msgid "爬取结束，共爬取{0}个视频"
-msgstr "爬取结束，共爬取{0}个视频"
+msgid "爬取了 {0} 个关注用户"
+msgstr "爬取了 {0} 个关注用户"
+
+msgid "爬取了 {0} 个粉丝用户"
+msgstr "爬取了 {0} 个粉丝用户"
+
+msgid "爬取结束，共找到 {0} 个收藏夹"
+msgstr "爬取结束，共找到 {0} 个收藏夹"
+
+msgid "爬取结束，共爬取 {0} 个作品"
+msgstr "爬取结束，共爬取 {0} 个作品"
+
+msgid "爬取结束，共爬取 {0} 个合集作品"
+msgstr "爬取结束，共爬取 {0} 个合集作品"
+
+msgid "爬取结束，共爬取 {0} 个收藏作品"
+msgstr "爬取结束，共爬取 {0} 个收藏作品"
+
+msgid "爬取结束，共爬取 {0} 个收藏夹"
+msgstr "爬取结束，共爬取 {0} 个收藏夹"
+
+msgid "爬取结束，共爬取 {0} 个点赞作品"
+msgstr "爬取结束，共爬取 {0} 个点赞作品"
+
+msgid "爬取结束，共爬取 {0} 个用户"
+msgstr "爬取结束，共爬取 {0} 个用户"
+
+msgid "爬取结束，共爬取 {0} 个音乐作品"
+msgstr "爬取结束，共爬取 {0} 个音乐作品"
+
+msgid "爬取结束，共爬取 {0} 个首页推荐作品"
+msgstr "爬取结束，共爬取 {0} 个首页推荐作品"
+
+msgid "状态"
+msgstr "状态"
 
 msgid "生成X-Bogus失败: {0})"
 msgstr "生成X-Bogus失败: {0})"
 
+msgid "生成歌词文件失败：{0}，请检查歌词 `data` 内容"
+msgstr "生成歌词文件失败：{0}，请检查歌词 `data` 内容"
+
 msgid "生成虚假的msToken"
 msgstr "生成虚假的msToken"
 
 msgid "用户: {0} 所有作品采集完毕"
 msgstr "用户: {0} 所有作品采集完毕"
 
-msgid "用户: {0} 没有视频合集"
-msgstr "用户: {0} 没有视频合集"
+msgid "用户ID：{0} 用户昵称：{1} 用户作品数：{2}"
+msgstr "用户ID：{0} 用户昵称：{1} 用户作品数：{2}"
 
-msgid "用户信息接口地址:"
-msgstr "用户信息接口地址:"
+msgid "用户ID：{0} 用户昵称：{1} 用户作品数：{2} 额外内容：{3}"
+msgstr "用户ID：{0} 用户昵称：{1} 用户作品数：{2} 额外内容：{3}"
 
-msgid "用户收藏的视频采集完毕"
-msgstr "用户收藏的视频采集完毕"
+msgid "用户信息接口地址：{0}"
+msgstr "用户信息接口地址：{0}"
 
-msgid "由于某些错误, 无法获取msToken"
-msgstr "由于某些错误, 无法获取msToken"
+msgid "用户关注列表接口地址：{0}"
+msgstr "用户关注列表接口地址：{0}"
 
-msgid "由于某些错误, 无法获取ttwid"
-msgstr "由于某些错误, 无法获取ttwid"
+msgid "用户收藏的作品采集完毕"
+msgstr "用户收藏的作品采集完毕"
+
+msgid "用户收藏的音乐作品采集完毕"
+msgstr "用户收藏的音乐作品采集完毕"
+
+msgid "用户没有作品合辑"
+msgstr "用户没有作品合辑"
+
+msgid "用户粉丝列表接口地址：{0}"
+msgstr "用户粉丝列表接口地址：{0}"
+
+msgid "用户：{0} 所有作品采集完毕"
+msgstr "用户：{0} 所有作品采集完毕"
+
+msgid "用户：{0} 所有关注用户采集完毕"
+msgstr "用户：{0} 所有关注用户采集完毕"
+
+msgid "用户：{0} 所有粉丝采集完毕"
+msgstr "用户：{0} 所有粉丝采集完毕"
+
+msgid "用户：{0} 没有作品合集"
+msgstr "用户：{0} 没有作品合集"
 
 msgid ""
 "登录后的[yellow]cookie[/yellow]，如果使用未登录的[yellow]cookie[/yellow]，则"
 "无法持久稳定下载作品"
 msgstr ""
 "登录后的[yellow]cookie[/yellow]，如果使用未登录的[yellow]cookie[/yellow]，则"
 "无法持久稳定下载作品"
 
-msgid "登录后的cookie"
-msgstr "登录后的cookie"
-
 msgid "登录后的cookie，如果使用未登录的cookie，则无法持久稳定下载作品"
 msgstr "登录后的cookie，如果使用未登录的cookie，则无法持久稳定下载作品"
 
 msgid "直播"
 msgstr "直播"
 
 msgid "直播ID: {0} 直播标题: {1} 直播状态: {2} 观看人数: {3}"
 msgstr "直播ID: {0} 直播标题: {1} 直播状态: {2} 观看人数: {3}"
 
 msgid "直播信息爬取结束"
 msgstr "直播信息爬取结束"
 
-msgid "直播已结束"
-msgstr "直播已结束"
-
-msgid "直播接口地址:"
-msgstr "直播接口地址:"
+msgid "直播接口地址（room_id）：{0}"
+msgstr "直播接口地址（room_id）：{0}"
 
-msgid "直播接口地址（room_id）:"
-msgstr "直播接口地址（room_id）:"
+msgid "直播接口地址：{0}"
+msgstr "直播接口地址：{0}"
 
-msgid "相关推荐作品接口地址:"
-msgstr "相关推荐作品接口地址:"
+msgid "相关推荐作品接口地址：{0}"
+msgstr "相关推荐作品接口地址：{0}"
 
 msgid "第 {0} 次响应内容为空, 状态码: {1}, URL:{2}"
 msgstr "第 {0} 次响应内容为空, 状态码: {1}, URL:{2}"
 
+msgid "第 {0} 页没有找到作品"
+msgstr "第 {0} 页没有找到作品"
+
+msgid "等待 {0} 秒后继续"
+msgstr "等待 {0} 秒后继续"
+
 msgid "筛选日期区间：{0} 至 {1}"
 msgstr "筛选日期区间：{0} 至 {1}"
 
+msgid "网络请求并发连接数"
+msgstr "网络请求并发连接数"
+
 msgid "网络请求并发连接数。"
 msgstr "网络请求并发连接数。"
 
-msgid "网络请求并发连接数，默认为 5"
-msgstr "网络请求并发连接数，默认为 5"
+msgid "网络请求超时时间"
+msgstr "网络请求超时时间"
 
 msgid "网络请求超时时间。"
 msgstr "网络请求超时时间。"
 
-msgid "网络请求超时时间，默认为 10"
-msgstr "网络请求超时时间，默认为 10"
+msgid "网络请求超时重试数"
+msgstr "网络请求超时重试数"
 
 msgid "网络请求超时重试数。"
 msgstr "网络请求超时重试数。"
 
-msgid "网络请求超时重试数，默认为 5"
-msgstr "网络请求超时重试数，默认为 5"
-
 msgid ""
-"自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、"
-"opera。使用该命令前请确保关闭所选的浏览器"
+"自动从浏览器获取[yellow]cookie[/yellow]，使用该命令前请确保关闭所选的浏览器"
 msgstr ""
-"自动从浏览器获取[yellow]cookie[/yellow]。可选项：chrome、firefox、edge、"
-"opera。使用该命令前请确保关闭所选的浏览器"
+"自动从浏览器获取[yellow]cookie[/yellow]，使用该命令前请确保关闭所选的浏览器"
 
-msgid ""
-"自动从浏览器获取cookie。可选项：chrome、firefox、edge、opera。使用该命令前请"
-"确保关闭所选的浏览器"
-msgstr ""
-"自动从浏览器获取cookie。可选项：chrome、firefox、edge、opera。使用该命令前请"
-"确保关闭所选的浏览器"
+msgid "自动从浏览器获取cookie，使用该命令前请确保关闭所选的浏览器"
+msgstr "自动从浏览器获取cookie，使用该命令前请确保关闭所选的浏览器"
 
-msgid "自动获取Cookie失败: {0}"
-msgstr "自动获取Cookie失败: {0}"
+msgid "自动获取Cookie失败：{0}"
+msgstr "自动获取Cookie失败：{0}"
 
 msgid "自定义配置参数：{0}"
 msgstr "自定义配置参数：{0}"
 
-msgid "自定义配置路径： {0}"
-msgstr "自定义配置路径： {0}"
+msgid "自定义配置路径：{0}"
+msgstr "自定义配置路径：{0}"
 
 msgid "至少提供 secUid 或 uniqueId 中的一个参数"
 msgstr "至少提供 secUid 或 uniqueId 中的一个参数"
 
-msgid "获取aweme_id失败, {0}"
-msgstr "获取aweme_id失败, {0}"
-
-msgid "获取sec_uid失败, {0}"
-msgstr "获取sec_uid失败, {0}"
+msgid "至少提供 user_id 或 sec_user_id 中的一个参数"
+msgstr "至少提供 user_id 或 sec_user_id 中的一个参数"
 
-msgid "获取unique_id失败, {0}"
-msgstr "获取unique_id失败, {0}"
+msgid "获取 {0} 失败，{1}"
+msgstr "获取 {0} 失败，{1}"
 
 msgid "获取数据失败。状态码: {0}"
 msgstr "获取数据失败。状态码: {0}"
 
 msgid "获取端点数据失败, 次数达到上限"
 msgstr "获取端点数据失败, 次数达到上限"
 
 msgid "要更新配置, 首先需要使用'-c'选项提供一个自定义配置文件路径"
 msgstr "要更新配置, 首先需要使用'-c'选项提供一个自定义配置文件路径"
 
+msgid "要更新配置，首先需要使用'-c'选项提供一个自定义配置文件路径"
+msgstr "要更新配置，首先需要使用'-c'选项提供一个自定义配置文件路径"
+
 msgid "视频"
 msgstr "视频"
 
-msgid "视频ID: {0} 视频文案: {1} 作者: {2}"
-msgstr "视频ID: {0} 视频文案: {1} 作者: {2}"
-
-msgid "视频合集ID: {0} 视频合集标题: {1}"
-msgstr "视频合集ID: {0} 视频合集标题: {1}"
+msgid "视频ID：{0} 视频文案：{1} 作者：{2}"
+msgstr "视频ID：{0} 视频文案：{1} 作者：{2}"
 
 msgid "解析 {0} 接口 JSON 失败： {1}"
 msgstr "解析 {0} 接口 JSON 失败： {1}"
 
+msgid "该 {0} 作品已被屏蔽，无法下载"
+msgstr "该 {0} 作品已被屏蔽，无法下载"
+
 msgid "该链接返回的是room_id，请使用`fetch_user_live_videos_by_room_id`接口"
 msgstr "该链接返回的是room_id，请使用`fetch_user_live_videos_by_room_id`接口"
 
-msgid "语言设置，默认为 'zh_CN'"
-msgstr "语言设置，默认为 'zh_CN'"
+msgid "请关闭所有已打开的浏览器重试，并且你有适当的权限访问浏览器！"
+msgstr "请关闭所有已打开的浏览器重试，并且你有适当的权限访问浏览器！"
 
-msgid "请关闭所有已打开的浏览器重试, 并且你有适当的权限访问浏览器 !"
-msgstr "请关闭所有已打开的浏览器重试, 并且你有适当的权限访问浏览器 !"
+msgid ""
+"请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常"
+"详细信息：{3}"
+msgstr ""
+"请求端点失败，请检查当前网络环境。 链接：{0}，代理：{1}，异常类名：{2}，异常"
+"详细信息：{3}"
 
 msgid "输入的URL List不合法。类名：{0}"
 msgstr "输入的URL List不合法。类名：{0}"
 
 msgid "输入的URL不合法。类名：{0}"
 msgstr "输入的URL不合法。类名：{0}"
 
-msgid "连接到API时发生错误，请检查URL或网络情况。类名: {0}"
-msgstr "连接到API时发生错误，请检查URL或网络情况。类名: {0}"
-
 msgid "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
 msgstr "连接端点失败，检查网络环境或代理：{0} 代理：{1} 类名：{2}"
 
 msgid "连接超时错误: {0}"
 msgstr "连接超时错误: {0}"
 
+msgid "配置文件不存在"
+msgstr "配置文件不存在"
+
 msgid "配置文件已更新!"
 msgstr "配置文件已更新!"
 
 msgid "配置文件的路径，[red]最低优先[/red]"
 msgstr "配置文件的路径，[red]最低优先[/red]"
 
 msgid "配置文件的路径，最低优先"
 msgstr "配置文件的路径，最低优先"
 
-msgid "除了单个作品外，其他URL都需要用户主页URL"
-msgstr "除了单个作品外，其他URL都需要用户主页URL"
+msgid "配置文件路径无写权限"
+msgstr "配置文件路径无写权限"
+
+msgid "链接 {0} 内容长度为0，尝试下一个链接是否可用"
+msgstr "链接 {0} 内容长度为0，尝试下一个链接是否可用"
+
+msgid "链接：{0}，状态码 {1}：{2} "
+msgstr "链接：{0}，状态码 {1}：{2} "
+
+msgid "音乐"
+msgstr "音乐"
+
+msgid "音乐ID：{0} 音乐标题：{1} 作者：{2}"
+msgstr "音乐ID：{0} 音乐标题：{1} 作者：{2}"
+
+msgid "音乐收藏接口地址：{0}"
+msgstr "音乐收藏接口地址：{0}"
 
 msgid "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
 msgstr "页面不可用，可能是由于区域限制（代理）造成的。类名: {0}"
 
-msgid "首页推荐作品接口地址:"
-msgstr "首页推荐作品接口地址:"
+msgid "首页推荐作品接口地址：{0}"
+msgstr "首页推荐作品接口地址：{0}"
 
-msgid "首页推荐接口地址:"
-msgstr "首页推荐接口地址:"
+msgid "首页推荐接口地址：{0}"
+msgstr "首页推荐接口地址：{0}"
```

### Comparing `f2-0.0.1.4/f2/log/logger.py` & `f2-0.0.1.5/f2/log/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,17 @@
             files_to_delete = all_logs
         else:
             files_to_delete = all_logs[:-keep_last_n]
         for log_file in files_to_delete:
             try:
                 log_file.unlink()
             except PermissionError:
-                self.logger.warning(f"无法删除日志文件 {log_file}, 它正被另一个进程使用")
+                self.logger.warning(
+                    f"无法删除日志文件 {log_file}, 它正被另一个进程使用"
+                )
 
     def shutdown(self):
         for handler in self.logger.handlers:
             handler.close()
             self.logger.removeHandler(handler)
         self.logger.handlers.clear()
         time.sleep(1)  # 确保文件被释放
```

### Comparing `f2-0.0.1.4/f2/utils/_dl.py` & `f2-0.0.1.5/f2/utils/_dl.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,31 @@
         int: Content-Length的值，如果获取失败则返回0 (Value of Content-Length, or 0 if retrieval fails)
     """
     async with httpx.AsyncClient(
         timeout=10.0, transport=httpx.AsyncHTTPTransport(retries=5), proxies=proxies
     ) as client:
         try:
             response = await client.head(url, headers=headers, follow_redirects=True)
+            # 当head请求被禁止时，释放status异常被捕获 (When head requests are forbidden, release status exceptions are caught)
             response.raise_for_status()
+
+            if (
+                response.headers.get("Content-Length") != None
+                and int(response.headers.get("Content-Length")) == 0
+            ):
+                # 如果head请求无法获取Content-Length, 则使用GET请求再次尝试获取
+                response = await client.get(url, headers=headers, follow_redirects=True)
+                response.raise_for_status()
+
         except httpx.ConnectTimeout:
             # 连接超时错误处理 (Handling connection timeout errors)
             logger.error(_("连接超时错误: {0}".format(url)))
-            logger.error("==========================")
+            logger.error("===================================")
             logger.error(f"headers:{headers}, proxies:{proxies}")
-            logger.error("==========================")
+            logger.error("===================================")
             return 0
         # 对HTTP状态错误进行处理 (Handling HTTP status errors)
         except httpx.HTTPStatusError as exc:
             # HEAD或请求不被允许 (HEAD or request not allowed)
             if exc.response.status_code in [405, 403, 401, 302]:
                 try:
                     # 使用GET请求尝试再次获取Content-Length
```

### Comparing `f2-0.0.1.4/f2/utils/_signal.py` & `f2-0.0.1.5/f2/utils/_signal.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/utils/_singleton.py` & `f2-0.0.1.5/f2/utils/_singleton.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/f2/utils/conf_manager.py` & `f2-0.0.1.5/f2/utils/conf_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # path: f2/utils/conf_manager.py
 
 import f2
-import time
 import yaml
 import click
 
 from pathlib import Path
 from f2.exceptions.file_exceptions import (
     FileNotFound,
     FilePermissionError,
@@ -23,22 +22,18 @@
         else:
             self.filepath = Path(get_resource_path(filepath))
         self.config = self.load_config()
 
     def load_config(self) -> dict:
         """从文件中加载配置 (Load the conf from the file)"""
 
-        try:
-            if not self.filepath.exists():
-                raise FileNotFound(_("'{0}' 配置文件路径不存在").format(self.filepath))
-            return yaml.safe_load(self.filepath.read_text(encoding="utf-8")) or {}
-        except FileNotFound as e:
-            e.display_error()
-            time.sleep(2)
-            exit(0)
+        if not self.filepath.exists():
+            raise FileNotFound(_("配置文件不存在"), self.filepath)
+
+        return yaml.safe_load(self.filepath.read_text(encoding="utf-8")) or {}
 
     def get_config(self, app_name: str, default=None) -> dict:
         """
         从配置中获取给定键的值 (Get the value of the given key from the conf)
 
         Args:
             app_name: str: 应用名称 (app name)
@@ -54,17 +49,15 @@
         """将配置保存到文件 (Save the conf to the file)
         Args:
             config: dict: 配置字典 (conf dict)
         """
         try:
             self.filepath.write_text(yaml.dump(config), encoding="utf-8")
         except PermissionError:
-            raise FilePermissionError(
-                _("'{0}' 配置文件路径无写权限").format(self.filepath)
-            )
+            raise FilePermissionError(_("配置文件路径无写权限"), self.filepath)
 
     def backup_config(self):
         """在进行更改前备份配置文件 (Backup the conf file before making changes)"""
         # 如果已经是备份文件，直接返回 (If it is already a backup file, return directly)
         if self.filepath.suffix == ".bak":
             return
```

### Comparing `f2-0.0.1.4/f2/utils/json_filter.py` & `f2-0.0.1.5/f2/utils/json_filter.py`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/.gitignore` & `f2-0.0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/LICENSE` & `f2-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/README.md` & `f2-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `f2-0.0.1.4/pyproject.toml` & `f2-0.0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Customer Service",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 dependencies = [
     "click==8.1.7",
-    "rich==13.6.0",
+    "rich==13.7.1",
     "httpx==0.25.0",
     "aiofiles==22.1.0",
     "aiosqlite==0.19.0",
     "pyyaml==6.0.1",
     "jsonpath-ng==1.6.0",
     "importlib_resources==6.1.0",
     "m3u8==3.6.0",
```

### Comparing `f2-0.0.1.4/PKG-INFO` & `f2-0.0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: f2
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: 🚀Asynchronous based full-platform download tool
 Project-URL: Homepage, https://github.com/Johnserf-Seed/f2
 Project-URL: Documentation, https://johnserf-seed.github.io/f2/
 Project-URL: Chat, https://discord.gg//3PhtPmgHf8
 Project-URL: Source Code, https://github.com/Johnserf-Seed/f2
 Project-URL: Issue Tracker, https://github.com/Johnserf-Seed/f2/issues
 Author-email: Johnserf-Seed <johnserf-seed@foxmail.com>
@@ -28,15 +28,15 @@
 Requires-Dist: jsonpath-ng==1.6.0
 Requires-Dist: m3u8==3.6.0
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: pytest-asyncio==0.21.1
 Requires-Dist: pytest==7.4.2
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: qrcode==7.4.2
-Requires-Dist: rich==13.6.0
+Requires-Dist: rich==13.7.1
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://github.com/Johnserf-Seed/f2/raw/main/docs/public/f2-logo-with-shadow-svg@0.5x.svg" alt="Logo">
 </p>
```

