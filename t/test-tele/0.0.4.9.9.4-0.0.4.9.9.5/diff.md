# Comparing `tmp/test_tele-0.0.4.9.9.4.tar.gz` & `tmp/test_tele-0.0.4.9.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_tele-0.0.4.9.9.4.tar", max compression
+gzip compressed data, was "test_tele-0.0.4.9.9.5.tar", max compression
```

## Comparing `test_tele-0.0.4.9.9.4.tar` & `test_tele-0.0.4.9.9.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1067 2023-06-26 21:27:24.000000 test_tele-0.0.4.9.9.4/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-04 02:21:38.693662 test_tele-0.0.4.9.9.4/pyproject.toml
--rw-r--r--   0        0        0      204 2024-02-01 01:09:18.935198 test_tele-0.0.4.9.9.4/test_tele/__init__.py
--rw-r--r--   0        0        0     3887 2024-02-01 01:09:18.935198 test_tele-0.0.4.9.9.4/test_tele/betas/extractors manga.py
--rw-r--r--   0        0        0        0 2024-02-17 04:22:31.581491 test_tele-0.0.4.9.9.4/test_tele/bot/__init__.py
--rw-r--r--   0        0        0     4826 2024-04-04 02:03:04.374198 test_tele-0.0.4.9.9.4/test_tele/bot/bot_header.py
--rw-r--r--   0        0        0     1004 2024-02-24 03:24:06.637233 test_tele-0.0.4.9.9.4/test_tele/bot/handlers/__init__.py
--rw-r--r--   0        0        0     3366 2024-02-18 04:44:46.394124 test_tele-0.0.4.9.9.4/test_tele/bot/handlers/callback.py
--rw-r--r--   0        0        0    23279 2024-03-31 14:45:29.985758 test_tele-0.0.4.9.9.4/test_tele/bot/handlers/command.py
--rw-r--r--   0        0        0    15414 2024-04-04 02:28:56.894044 test_tele-0.0.4.9.9.4/test_tele/bot/handlers/incoming_msg.py
--rw-r--r--   0        0        0     1241 2024-02-24 01:23:46.098511 test_tele-0.0.4.9.9.4/test_tele/bot/handlers/inline.py
--rw-r--r--   0        0        0     3187 2024-03-19 01:59:39.240018 test_tele-0.0.4.9.9.4/test_tele/bot/utils.py
--rw-r--r--   0        0        0     2689 2024-03-19 03:45:24.373101 test_tele-0.0.4.9.9.4/test_tele/cli.py
--rw-r--r--   0        0        0     8220 2024-03-19 03:50:48.756493 test_tele-0.0.4.9.9.4/test_tele/config.py
--rw-r--r--   0        0        0     5985 2024-03-17 11:49:43.279629 test_tele-0.0.4.9.9.4/test_tele/config_bot.py
--rw-r--r--   0        0        0      605 2024-02-11 06:00:45.177413 test_tele-0.0.4.9.9.4/test_tele/const.py
--rw-r--r--   0        0        0        0 2024-02-01 01:09:18.945198 test_tele-0.0.4.9.9.4/test_tele/datas/__init__.py
--rw-r--r--   0        0        0     2811 2024-02-07 15:21:01.331824 test_tele-0.0.4.9.9.4/test_tele/datas/database.py
--rw-r--r--   0        0        0     2167 2024-02-09 01:04:46.559675 test_tele-0.0.4.9.9.4/test_tele/datas/db_helper.py
--rw-r--r--   0        0        0        0 2024-02-18 12:14:21.086896 test_tele-0.0.4.9.9.4/test_tele/features/extractors/__init__.py
--rw-r--r--   0        0        0     2686 2024-02-24 03:32:09.053154 test_tele-0.0.4.9.9.4/test_tele/features/extractors/ehentai.py
--rw-r--r--   0        0        0     1839 2024-02-09 06:03:08.405860 test_tele-0.0.4.9.9.4/test_tele/features/extractors/furry.py
--rw-r--r--   0        0        0     5098 2024-02-01 01:09:18.955198 test_tele-0.0.4.9.9.4/test_tele/features/extractors/gelbooru.py
--rw-r--r--   0        0        0     1102 2024-04-02 01:34:18.795422 test_tele-0.0.4.9.9.4/test_tele/features/extractors/instagram.py
--rw-r--r--   0        0        0     9900 2024-02-24 05:43:31.160147 test_tele-0.0.4.9.9.4/test_tele/features/extractors/manga.py
--rw-r--r--   0        0        0     3963 2024-02-17 17:57:38.482468 test_tele-0.0.4.9.9.4/test_tele/features/extractors/pixiv.py
--rw-r--r--   0        0        0     1520 2024-02-17 17:32:50.839753 test_tele-0.0.4.9.9.4/test_tele/features/extractors/realperson.py
--rw-r--r--   0        0        0     3794 2024-02-19 01:44:30.435531 test_tele-0.0.4.9.9.4/test_tele/features/extractors/telegraph.py
--rw-r--r--   0        0        0     5103 2024-04-02 01:11:43.605440 test_tele-0.0.4.9.9.4/test_tele/features/extractors/utils.py
--rw-r--r--   0        0        0        0 2024-02-01 01:09:18.955198 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/__init__.py
--rw-r--r--   0        0        0     3330 2024-02-24 11:06:00.699933 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/furry.py
--rw-r--r--   0        0        0     5151 2024-02-09 14:46:50.905905 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/gelbooru.py
--rw-r--r--   0        0        0     8821 2024-02-24 13:14:29.588513 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/manga.py
--rw-r--r--   0        0        0     3331 2024-02-17 16:58:19.745096 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/pixiv.py
--rw-r--r--   0        0        0     3335 2024-02-17 18:23:15.014470 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/realperson.py
--rw-r--r--   0        0        0     1125 2024-02-09 06:52:51.875319 test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/utils.py
--rw-r--r--   0        0        0     3637 2024-03-19 03:51:18.592395 test_tele-0.0.4.9.9.4/test_tele/live.py
--rw-r--r--   0        0        0      397 2024-03-17 00:32:07.153238 test_tele-0.0.4.9.9.4/test_tele/live_pyrogram.py
--rw-r--r--   0        0        0     3677 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/past.py
--rw-r--r--   0        0        0     2200 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/plugin_models.py
--rw-r--r--   0        0        0     4510 2024-02-17 00:59:24.125861 test_tele-0.0.4.9.9.4/test_tele/plugins/__init__.py
--rw-r--r--   0        0        0      371 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/plugins/caption.py
--rw-r--r--   0        0        0     2516 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/plugins/filter.py
--rw-r--r--   0        0        0      721 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/plugins/fmt.py
--rw-r--r--   0        0        0     1769 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.4/test_tele/plugins/mark.py
--rw-r--r--   0        0        0      495 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.4/test_tele/plugins/ocr.py
--rw-r--r--   0        0        0      706 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.4/test_tele/plugins/replace.py
--rw-r--r--   0        0        0      517 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.4/test_tele/plugins/special.py
--rw-r--r--   0        0        0      954 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.4/test_tele/storage.py
--rw-r--r--   0        0        0        0 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.4/test_tele/user_bot/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-02 14:56:52.652837 test_tele-0.0.4.9.9.4/test_tele/user_bot/telethon.py
--rw-r--r--   0        0        0     9282 2024-03-18 03:37:00.175310 test_tele-0.0.4.9.9.4/test_tele/utils.py
--rw-r--r--   0        0        0     1779 2024-02-07 14:45:19.312552 test_tele-0.0.4.9.9.4/test_tele/web_ui/0_👋_Hello.py
--rw-r--r--   0        0        0     2479 2024-02-01 15:47:13.332016 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/1_🔑_Telegram_Login.py
--rw-r--r--   0        0        0    14836 2024-02-09 02:23:02.796658 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/2_⭐_Bot_Users.py
--rw-r--r--   0        0        0     4287 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/3_🔗_Connection.py
--rw-r--r--   0        0        0     7732 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/4_🔌_Plugins.py
--rw-r--r--   0        0        0     3579 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/5_🏃_Run.py
--rw-r--r--   0        0        0     8271 2024-02-09 02:22:49.180469 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/6_📊_Data_Manager.py
--rw-r--r--   0        0        0        0 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/7_📢_Group_Manager.py
--rw-r--r--   0        0        0     4650 2024-03-17 11:53:14.301529 test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/8_🔬_Advanced.py
--rw-r--r--   0        0        0     1082 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/password.py
--rw-r--r--   0        0        0      455 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.4/test_tele/web_ui/run.py
--rw-r--r--   0        0        0     2902 2024-02-09 02:23:45.115826 test_tele-0.0.4.9.9.4/test_tele/web_ui/utils.py
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 test_tele-0.0.4.9.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-26 21:27:24.000000 test_tele-0.0.4.9.9.5/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-04 02:44:48.508796 test_tele-0.0.4.9.9.5/pyproject.toml
+-rw-r--r--   0        0        0      204 2024-02-01 01:09:18.935198 test_tele-0.0.4.9.9.5/test_tele/__init__.py
+-rw-r--r--   0        0        0     3887 2024-02-01 01:09:18.935198 test_tele-0.0.4.9.9.5/test_tele/betas/extractors manga.py
+-rw-r--r--   0        0        0        0 2024-02-17 04:22:31.581491 test_tele-0.0.4.9.9.5/test_tele/bot/__init__.py
+-rw-r--r--   0        0        0     4770 2024-04-04 02:42:37.658691 test_tele-0.0.4.9.9.5/test_tele/bot/bot_header.py
+-rw-r--r--   0        0        0     1004 2024-02-24 03:24:06.637233 test_tele-0.0.4.9.9.5/test_tele/bot/handlers/__init__.py
+-rw-r--r--   0        0        0     3366 2024-02-18 04:44:46.394124 test_tele-0.0.4.9.9.5/test_tele/bot/handlers/callback.py
+-rw-r--r--   0        0        0    23279 2024-03-31 14:45:29.985758 test_tele-0.0.4.9.9.5/test_tele/bot/handlers/command.py
+-rw-r--r--   0        0        0    15343 2024-04-04 02:44:17.165799 test_tele-0.0.4.9.9.5/test_tele/bot/handlers/incoming_msg.py
+-rw-r--r--   0        0        0     1241 2024-02-24 01:23:46.098511 test_tele-0.0.4.9.9.5/test_tele/bot/handlers/inline.py
+-rw-r--r--   0        0        0     3187 2024-03-19 01:59:39.240018 test_tele-0.0.4.9.9.5/test_tele/bot/utils.py
+-rw-r--r--   0        0        0     2689 2024-03-19 03:45:24.373101 test_tele-0.0.4.9.9.5/test_tele/cli.py
+-rw-r--r--   0        0        0     8220 2024-03-19 03:50:48.756493 test_tele-0.0.4.9.9.5/test_tele/config.py
+-rw-r--r--   0        0        0     5985 2024-03-17 11:49:43.279629 test_tele-0.0.4.9.9.5/test_tele/config_bot.py
+-rw-r--r--   0        0        0      605 2024-02-11 06:00:45.177413 test_tele-0.0.4.9.9.5/test_tele/const.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:09:18.945198 test_tele-0.0.4.9.9.5/test_tele/datas/__init__.py
+-rw-r--r--   0        0        0     2811 2024-02-07 15:21:01.331824 test_tele-0.0.4.9.9.5/test_tele/datas/database.py
+-rw-r--r--   0        0        0     2167 2024-02-09 01:04:46.559675 test_tele-0.0.4.9.9.5/test_tele/datas/db_helper.py
+-rw-r--r--   0        0        0        0 2024-02-18 12:14:21.086896 test_tele-0.0.4.9.9.5/test_tele/features/extractors/__init__.py
+-rw-r--r--   0        0        0     2686 2024-02-24 03:32:09.053154 test_tele-0.0.4.9.9.5/test_tele/features/extractors/ehentai.py
+-rw-r--r--   0        0        0     1839 2024-02-09 06:03:08.405860 test_tele-0.0.4.9.9.5/test_tele/features/extractors/furry.py
+-rw-r--r--   0        0        0     5098 2024-02-01 01:09:18.955198 test_tele-0.0.4.9.9.5/test_tele/features/extractors/gelbooru.py
+-rw-r--r--   0        0        0     1102 2024-04-02 01:34:18.795422 test_tele-0.0.4.9.9.5/test_tele/features/extractors/instagram.py
+-rw-r--r--   0        0        0     9900 2024-02-24 05:43:31.160147 test_tele-0.0.4.9.9.5/test_tele/features/extractors/manga.py
+-rw-r--r--   0        0        0     3963 2024-02-17 17:57:38.482468 test_tele-0.0.4.9.9.5/test_tele/features/extractors/pixiv.py
+-rw-r--r--   0        0        0     1520 2024-02-17 17:32:50.839753 test_tele-0.0.4.9.9.5/test_tele/features/extractors/realperson.py
+-rw-r--r--   0        0        0     3794 2024-02-19 01:44:30.435531 test_tele-0.0.4.9.9.5/test_tele/features/extractors/telegraph.py
+-rw-r--r--   0        0        0     5103 2024-04-02 01:11:43.605440 test_tele-0.0.4.9.9.5/test_tele/features/extractors/utils.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:09:18.955198 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/__init__.py
+-rw-r--r--   0        0        0     3330 2024-02-24 11:06:00.699933 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/furry.py
+-rw-r--r--   0        0        0     5151 2024-02-09 14:46:50.905905 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/gelbooru.py
+-rw-r--r--   0        0        0     8821 2024-02-24 13:14:29.588513 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/manga.py
+-rw-r--r--   0        0        0     3331 2024-02-17 16:58:19.745096 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/pixiv.py
+-rw-r--r--   0        0        0     3335 2024-02-17 18:23:15.014470 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/realperson.py
+-rw-r--r--   0        0        0     1125 2024-02-09 06:52:51.875319 test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/utils.py
+-rw-r--r--   0        0        0     3637 2024-03-19 03:51:18.592395 test_tele-0.0.4.9.9.5/test_tele/live.py
+-rw-r--r--   0        0        0      397 2024-03-17 00:32:07.153238 test_tele-0.0.4.9.9.5/test_tele/live_pyrogram.py
+-rw-r--r--   0        0        0     3677 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/past.py
+-rw-r--r--   0        0        0     2200 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/plugin_models.py
+-rw-r--r--   0        0        0     4510 2024-02-17 00:59:24.125861 test_tele-0.0.4.9.9.5/test_tele/plugins/__init__.py
+-rw-r--r--   0        0        0      371 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/plugins/caption.py
+-rw-r--r--   0        0        0     2516 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/plugins/filter.py
+-rw-r--r--   0        0        0      721 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/plugins/fmt.py
+-rw-r--r--   0        0        0     1769 2024-02-01 01:09:18.965198 test_tele-0.0.4.9.9.5/test_tele/plugins/mark.py
+-rw-r--r--   0        0        0      495 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.5/test_tele/plugins/ocr.py
+-rw-r--r--   0        0        0      706 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.5/test_tele/plugins/replace.py
+-rw-r--r--   0        0        0      517 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.5/test_tele/plugins/special.py
+-rw-r--r--   0        0        0      954 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.5/test_tele/storage.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:09:18.975198 test_tele-0.0.4.9.9.5/test_tele/user_bot/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-02 14:56:52.652837 test_tele-0.0.4.9.9.5/test_tele/user_bot/telethon.py
+-rw-r--r--   0        0        0     9282 2024-03-18 03:37:00.175310 test_tele-0.0.4.9.9.5/test_tele/utils.py
+-rw-r--r--   0        0        0     1779 2024-02-07 14:45:19.312552 test_tele-0.0.4.9.9.5/test_tele/web_ui/0_👋_Hello.py
+-rw-r--r--   0        0        0     2479 2024-02-01 15:47:13.332016 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/1_🔑_Telegram_Login.py
+-rw-r--r--   0        0        0    14836 2024-02-09 02:23:02.796658 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/2_⭐_Bot_Users.py
+-rw-r--r--   0        0        0     4287 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/3_🔗_Connection.py
+-rw-r--r--   0        0        0     7732 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/4_🔌_Plugins.py
+-rw-r--r--   0        0        0     3579 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/5_🏃_Run.py
+-rw-r--r--   0        0        0     8271 2024-02-09 02:22:49.180469 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/6_📊_Data_Manager.py
+-rw-r--r--   0        0        0        0 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/7_📢_Group_Manager.py
+-rw-r--r--   0        0        0     4650 2024-03-17 11:53:14.301529 test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/8_🔬_Advanced.py
+-rw-r--r--   0        0        0     1082 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/password.py
+-rw-r--r--   0        0        0      455 2024-02-01 01:09:18.985198 test_tele-0.0.4.9.9.5/test_tele/web_ui/run.py
+-rw-r--r--   0        0        0     2902 2024-02-09 02:23:45.115826 test_tele-0.0.4.9.9.5/test_tele/web_ui/utils.py
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 test_tele-0.0.4.9.9.5/PKG-INFO
```

### Comparing `test_tele-0.0.4.9.9.4/LICENSE` & `test_tele-0.0.4.9.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/pyproject.toml` & `test_tele-0.0.4.9.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-tele"
-version = "0.0.4.9.9.4"
+version = "0.0.4.9.9.5"
 description = "test tele bot, [beta] support topic, etc."
 authors = ["aahnik <daw@aahnik.dev>"]
 license = "MIT"
 repository = "https://github.com/aahnik/tgcf"
 documentation = "https://github.com/aahnik/tgcf/wiki"
 packages = [
     { include = "test_tele" },
```

### Comparing `test_tele-0.0.4.9.9.4/test_tele/betas/extractors manga.py` & `test_tele-0.0.4.9.9.5/test_tele/betas/extractors manga.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/bot_header.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/bot_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         r'(instagram.com)/'
         r'(p/[^&=%\?\s]{1,}|[^&=%\?\s]{1,}highlights/[^&=%\?\s]{1,18}|[^&=%\?\s]+)')
 
     # Pola regex untuk Newgrounds
     newgrounds_regex = (
         r'(https?://)?(www\.)?'
         r'(newgrounds.com)/'
-        r'(games/[^&=%\?\s]{1,}|movies/[^&=%\?\s]{1,}|art/[^&=%\?\s]{1,}|audio/[^&=%\?\s]{1,})')
+        r'(portal/view/[^&=%\?\s]{1,})')
 
     # Periksa kecocokan dengan pola Twitter
     twitter_match = re.search(twitter_regex, url)
 
     # Periksa kecocokan dengan pola Instagram
     instagram_match = re.search(instagram_regex, url)
```

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/handlers/__init__.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/handlers/callback.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/handlers/callback.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/handlers/command.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/handlers/command.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/handlers/incoming_msg.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/handlers/incoming_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,22 +324,19 @@
     Download the media from the given url.
     currently support youtube only
     """
     if event.message.text.startswith((".", "/")):
         return
 
     url = await accepted_url_validation(event.message.text)
-    # yt_link = await youtube_url_validation(event.message.text)
-
     if not url:
         return
     
     file_name = await determine_url_category(url)
-    cookie = f'config/{file_name}_cookies.txt' if file_name != 'unknown' else ''
-    logging.warning(cookie)
+    cookie = f'config/{file_name}_cookies.txt' if file_name != 'unknown' else 'config/twitter_cookies.txt'
 
     video_title = round(time.time() * 1000)
     msg = await event.reply("Attempting to grab video files..")
 
     try:
         with yt_dlp.YoutubeDL({
             'quiet': True,
```

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/handlers/inline.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/handlers/inline.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/bot/utils.py` & `test_tele-0.0.4.9.9.5/test_tele/bot/utils.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/cli.py` & `test_tele-0.0.4.9.9.5/test_tele/cli.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/config.py` & `test_tele-0.0.4.9.9.5/test_tele/config.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/config_bot.py` & `test_tele-0.0.4.9.9.5/test_tele/config_bot.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/const.py` & `test_tele-0.0.4.9.9.5/test_tele/const.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/datas/database.py` & `test_tele-0.0.4.9.9.5/test_tele/datas/database.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/datas/db_helper.py` & `test_tele-0.0.4.9.9.5/test_tele/datas/db_helper.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/ehentai.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/ehentai.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/furry.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/furry.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/gelbooru.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/gelbooru.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/instagram.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/instagram.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/manga.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/manga.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/pixiv.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/pixiv.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/realperson.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/realperson.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/telegraph.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/telegraph.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/extractors/utils.py` & `test_tele-0.0.4.9.9.5/test_tele/features/extractors/utils.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/furry.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/furry.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/gelbooru.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/gelbooru.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/manga.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/manga.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/pixiv.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/pixiv.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/realperson.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/realperson.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/features/pyrogram/utils.py` & `test_tele-0.0.4.9.9.5/test_tele/features/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/live.py` & `test_tele-0.0.4.9.9.5/test_tele/live.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/past.py` & `test_tele-0.0.4.9.9.5/test_tele/past.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugin_models.py` & `test_tele-0.0.4.9.9.5/test_tele/plugin_models.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/__init__.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/filter.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/fmt.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/fmt.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/mark.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/mark.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/replace.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/replace.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/plugins/special.py` & `test_tele-0.0.4.9.9.5/test_tele/plugins/special.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/storage.py` & `test_tele-0.0.4.9.9.5/test_tele/storage.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/user_bot/telethon.py` & `test_tele-0.0.4.9.9.5/test_tele/user_bot/telethon.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/utils.py` & `test_tele-0.0.4.9.9.5/test_tele/utils.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/0_👋_Hello.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/0_👋_Hello.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/1_🔑_Telegram_Login.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/1_🔑_Telegram_Login.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/2_⭐_Bot_Users.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/2_⭐_Bot_Users.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/3_🔗_Connection.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/3_🔗_Connection.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/4_🔌_Plugins.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/4_🔌_Plugins.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/5_🏃_Run.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/5_🏃_Run.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/6_📊_Data_Manager.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/6_📊_Data_Manager.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/pages/8_🔬_Advanced.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/pages/8_🔬_Advanced.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/password.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/password.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/test_tele/web_ui/utils.py` & `test_tele-0.0.4.9.9.5/test_tele/web_ui/utils.py`

 * *Files identical despite different names*

### Comparing `test_tele-0.0.4.9.9.4/PKG-INFO` & `test_tele-0.0.4.9.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-tele
-Version: 0.0.4.9.9.4
+Version: 0.0.4.9.9.5
 Summary: test tele bot, [beta] support topic, etc.
 Home-page: https://github.com/aahnik/tgcf
 License: MIT
 Author: aahnik
 Author-email: daw@aahnik.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```
