# Comparing `tmp/tlp_ui-1.6.4.tar.gz` & `tmp/tlp_ui-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlp_ui-1.6.4.tar", max compression
+gzip compressed data, was "tlp_ui-1.6.5.tar", max compression
```

## Comparing `tlp_ui-1.6.4.tar` & `tlp_ui-1.6.5.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0    18046 2016-06-04 05:33:23.000000 tlp_ui-1.6.4/LICENSE.md
--rw-r--r--   0        0        0     1835 2024-01-23 21:55:35.349399 tlp_ui-1.6.4/README.md
--rw-r--r--   0        0        0      867 2024-01-23 22:05:58.223722 tlp_ui-1.6.4/pyproject.toml
--rw-r--r--   0        0        0       51 2024-01-23 22:00:24.997749 tlp_ui-1.6.4/tlpui/__init__.py
--rwxr-xr-x   0        0        0     1373 2024-01-18 20:57:20.319176 tlp_ui-1.6.4/tlpui/__main__.py
--rw-r--r--   0        0        0     1745 2024-01-18 20:57:20.319176 tlp_ui-1.6.4/tlpui/config.py
--rw-r--r--   0        0        0    10924 2024-01-18 20:57:20.319176 tlp_ui-1.6.4/tlpui/configschema/1_3.yaml
--rw-r--r--   0        0        0    11753 2024-01-23 21:55:35.146067 tlp_ui-1.6.4/tlpui/configschema/1_4.yaml
--rw-r--r--   0        0        0    11781 2024-01-23 21:55:35.146067 tlp_ui-1.6.4/tlpui/configschema/1_5.yaml
--rw-r--r--   0        0        0    12038 2024-01-23 21:55:35.146067 tlp_ui-1.6.4/tlpui/configschema/1_6.yaml
--rw-r--r--   0        0        0    11743 2024-01-23 21:55:35.146067 tlp_ui-1.6.4/tlpui/configschema/1_7.yaml
--rw-r--r--   0        0        0    11000 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/configui.py
--rw-r--r--   0        0        0      124 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/constants.py
--rw-r--r--   0        0        0      411 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/css.py
--rw-r--r--   0        0        0    14928 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/defaults/tlp-1_3.conf
--rw-r--r--   0        0        0    18021 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/defaults/tlp-1_4.conf
--rw-r--r--   0        0        0    18076 2024-01-18 20:57:20.322509 tlp_ui-1.6.4/tlpui/defaults/tlp-1_5.conf
--rw-r--r--   0        0        0    19896 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/defaults/tlp-1_6.conf
--rw-r--r--   0        0        0    19301 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/defaults/tlp-1_7.conf
--rw-r--r--   0        0        0      423 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/errorui.py
--rw-r--r--   0        0        0     5949 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/file.py
--rw-r--r--   0        0        0     2037 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/filehelper.py
--rw-r--r--   0        0        0     1063 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/icons/ICON-AUTHORS
--rw-r--r--   0        0        0     5162 2024-01-18 20:57:20.325842 tlp_ui-1.6.4/tlpui/icons/OnAC.svg
--rw-r--r--   0        0        0     6363 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/OnBAT.svg
--rw-r--r--   0        0        0    16723 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/dropin.svg
--rw-r--r--   0        0        0    13119 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/flags/de_DE.png
--rw-r--r--   0        0        0    20436 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/flags/en_EN.png
--rw-r--r--   0        0        0    24372 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/flags/es_ES.png
--rw-r--r--   0        0        0    15290 2024-01-18 20:57:20.329176 tlp_ui-1.6.4/tlpui/icons/flags/fr_FR.png
--rw-r--r--   0        0        0    10944 2024-01-18 20:57:20.332509 tlp_ui-1.6.4/tlpui/icons/flags/id_ID.png
--rw-r--r--   0        0        0    31144 2024-01-18 20:57:20.332509 tlp_ui-1.6.4/tlpui/icons/flags/pt_BR.png
--rw-r--r--   0        0        0    12002 2024-01-18 20:57:20.332509 tlp_ui-1.6.4/tlpui/icons/flags/ru_RU.png
--rw-r--r--   0        0        0    20068 2024-01-18 20:57:20.332509 tlp_ui-1.6.4/tlpui/icons/flags/tr_TR.png
--rw-r--r--   0        0        0    18587 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/flags/zh_CN.png
--rw-r--r--   0        0        0     1882 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/128x128/apps/tlpui.png
--rw-r--r--   0        0        0      511 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/16x16/apps/tlpui.png
--rw-r--r--   0        0        0     3438 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/256x256/apps/tlpui.png
--rw-r--r--   0        0        0      710 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/32x32/apps/tlpui.png
--rw-r--r--   0        0        0     1016 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/48x48/apps/tlpui.png
--rw-r--r--   0        0        0     1144 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/64x64/apps/tlpui.png
--rw-r--r--   0        0        0     1576 2024-01-18 20:57:20.335842 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/96x96/apps/tlpui.png
--rw-r--r--   0        0        0     5166 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/dialog-information-symbolic.svg
--rw-r--r--   0        0        0     5137 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/document-save-symbolic.svg
--rw-r--r--   0        0        0     4283 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/edit-symbolic.svg
--rw-r--r--   0        0        0     4103 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/format-indent-more-symbolic.svg
--rw-r--r--   0        0        0     4037 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/list-add-symbolic.svg
--rw-r--r--   0        0        0     5643 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Audio-symbolic.svg
--rw-r--r--   0        0        0     8885 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Disks-symbolic.svg
--rw-r--r--   0        0        0     5683 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Dock-symbolic.svg
--rw-r--r--   0        0        0     4214 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-General-symbolic.svg
--rw-r--r--   0        0        0     4318 2024-01-18 20:57:20.339176 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Graphics-symbolic.svg
--rw-r--r--   0        0        0     4292 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Network-symbolic.svg
--rw-r--r--   0        0        0     4562 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-PCIe-symbolic.svg
--rw-r--r--   0        0        0     4480 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Processor-symbolic.svg
--rw-r--r--   0        0        0     5140 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-Device-Wizard-symbolic.svg
--rw-r--r--   0        0        0     4625 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-symbolic.svg
--rw-r--r--   0        0        0     4674 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-ThinkPad-Battery-symbolic.svg
--rw-r--r--   0        0        0     7564 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-USB-symbolic.svg
--rw-r--r--   0        0        0     4223 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/view-refresh-symbolic.svg
--rw-r--r--   0        0        0    16902 2024-01-18 20:57:20.342509 tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/apps/tlpui.svg
--rw-r--r--   0        0        0    13685 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/icons/user.svg
--rw-r--r--   0        0        0    18934 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    22006 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1230 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1490 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      585 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      689 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      894 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1040 2024-01-18 20:57:20.345842 tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    18936 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    22008 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1164 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1424 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      582 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      686 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      864 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1010 2024-01-18 20:57:20.349176 tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    18657 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    21657 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1215 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1494 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      624 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      747 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      915 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1080 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    24760 2024-01-18 20:57:20.352509 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    28112 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1251 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1517 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      647 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      755 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      976 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1126 2024-01-18 20:57:20.355842 tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    18533 2024-01-18 20:57:20.359175 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    21530 2024-01-18 20:57:20.359175 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1255 2024-01-18 20:57:20.359175 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1515 2024-01-18 20:57:20.359175 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      615 2024-01-18 20:57:20.359175 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      723 2024-01-18 20:57:20.362509 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      867 2024-01-18 20:57:20.362509 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1013 2024-01-18 20:57:20.362509 tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    18814 2024-01-18 20:57:20.362509 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    21799 2024-01-18 20:57:20.362509 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1273 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1533 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      692 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      800 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      969 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1115 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    28960 2024-01-18 20:57:20.365842 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    32056 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1415 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1675 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      652 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      756 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0     1033 2024-01-18 20:57:20.369175 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1179 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    19415 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    22485 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1272 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1589 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      661 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      822 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      980 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1183 2024-01-18 20:57:20.372508 tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    17500 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    20442 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1202 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1462 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      609 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      713 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      898 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1044 2024-01-18 20:57:20.375842 tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0    17533 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.mo
--rw-r--r--   0        0        0    20475 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.po
--rw-r--r--   0        0        0     1202 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/mainui.mo
--rw-r--r--   0        0        0     1462 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/mainui.po
--rw-r--r--   0        0        0      609 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/statui.mo
--rw-r--r--   0        0        0      713 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/statui.po
--rw-r--r--   0        0        0      898 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.mo
--rw-r--r--   0        0        0     1044 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.po
--rw-r--r--   0        0        0      740 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/language.py
--rw-r--r--   0        0        0    12684 2024-01-23 22:04:39.778186 tlp_ui-1.6.4/tlpui/mainui.py
--rw-r--r--   0        0        0      965 2024-01-18 20:57:20.379175 tlp_ui-1.6.4/tlpui/settings.py
--rw-r--r--   0        0        0     4159 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/settingshelper.py
--rw-r--r--   0        0        0     2522 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/statui.py
--rw-r--r--   0        0        0      529 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/styles.css
--rw-r--r--   0        0        0       38 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/__init__.py
--rw-r--r--   0        0        0     1387 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkcheckbutton.py
--rw-r--r--   0        0        0    11154 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkdisklist.py
--rw-r--r--   0        0        0      324 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkdisklistview.py
--rw-r--r--   0        0        0      658 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkentry.py
--rw-r--r--   0        0        0     1302 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkmultiselection.py
--rw-r--r--   0        0        0     2954 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkpcilist.py
--rw-r--r--   0        0        0      954 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkselection.py
--rw-r--r--   0        0        0      890 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkspinbutton.py
--rw-r--r--   0        0        0      849 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkswitch.py
--rw-r--r--   0        0        0     1412 2024-01-18 20:57:20.382508 tlp_ui-1.6.4/tlpui/ui_config_objects/gtktoggle.py
--rw-r--r--   0        0        0     5093 2024-01-18 20:57:20.385842 tlp_ui-1.6.4/tlpui/ui_config_objects/gtkusblist.py
--rw-r--r--   0        0        0     4709 2024-01-18 20:57:20.385842 tlp_ui-1.6.4/tlpui/uihelper.py
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 tlp_ui-1.6.4/setup.py
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 tlp_ui-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0    18046 2016-06-04 05:33:23.000000 tlp_ui-1.6.5/LICENSE.md
+-rw-r--r--   0        0        0     1835 2024-01-23 21:55:35.349399 tlp_ui-1.6.5/README.md
+-rw-r--r--   0        0        0      867 2024-04-04 18:51:05.162165 tlp_ui-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-04-04 18:50:56.908932 tlp_ui-1.6.5/tlpui/__init__.py
+-rwxr-xr-x   0        0        0     1373 2024-01-18 20:57:20.319176 tlp_ui-1.6.5/tlpui/__main__.py
+-rw-r--r--   0        0        0     1745 2024-01-18 20:57:20.319176 tlp_ui-1.6.5/tlpui/config.py
+-rw-r--r--   0        0        0    10924 2024-01-18 20:57:20.319176 tlp_ui-1.6.5/tlpui/configschema/1_3.yaml
+-rw-r--r--   0        0        0    11753 2024-01-23 21:55:35.146067 tlp_ui-1.6.5/tlpui/configschema/1_4.yaml
+-rw-r--r--   0        0        0    11781 2024-01-23 21:55:35.146067 tlp_ui-1.6.5/tlpui/configschema/1_5.yaml
+-rw-r--r--   0        0        0    12038 2024-01-23 21:55:35.146067 tlp_ui-1.6.5/tlpui/configschema/1_6.yaml
+-rw-r--r--   0        0        0    11743 2024-01-23 21:55:35.146067 tlp_ui-1.6.5/tlpui/configschema/1_7.yaml
+-rw-r--r--   0        0        0    11000 2024-01-18 20:57:20.322509 tlp_ui-1.6.5/tlpui/configui.py
+-rw-r--r--   0        0        0      124 2024-01-18 20:57:20.322509 tlp_ui-1.6.5/tlpui/constants.py
+-rw-r--r--   0        0        0      324 2024-04-04 18:44:46.646795 tlp_ui-1.6.5/tlpui/css.py
+-rw-r--r--   0        0        0    14928 2024-01-18 20:57:20.322509 tlp_ui-1.6.5/tlpui/defaults/tlp-1_3.conf
+-rw-r--r--   0        0        0    18021 2024-01-18 20:57:20.322509 tlp_ui-1.6.5/tlpui/defaults/tlp-1_4.conf
+-rw-r--r--   0        0        0    18076 2024-01-18 20:57:20.322509 tlp_ui-1.6.5/tlpui/defaults/tlp-1_5.conf
+-rw-r--r--   0        0        0    19896 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/defaults/tlp-1_6.conf
+-rw-r--r--   0        0        0    19301 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/defaults/tlp-1_7.conf
+-rw-r--r--   0        0        0      423 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/errorui.py
+-rw-r--r--   0        0        0     5949 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/file.py
+-rw-r--r--   0        0        0     2037 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/filehelper.py
+-rw-r--r--   0        0        0     1063 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/icons/ICON-AUTHORS
+-rw-r--r--   0        0        0     5162 2024-01-18 20:57:20.325842 tlp_ui-1.6.5/tlpui/icons/OnAC.svg
+-rw-r--r--   0        0        0     6363 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/OnBAT.svg
+-rw-r--r--   0        0        0    16723 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/dropin.svg
+-rw-r--r--   0        0        0    13119 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/flags/de_DE.png
+-rw-r--r--   0        0        0    20436 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/flags/en_EN.png
+-rw-r--r--   0        0        0    24372 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/flags/es_ES.png
+-rw-r--r--   0        0        0    15290 2024-01-18 20:57:20.329176 tlp_ui-1.6.5/tlpui/icons/flags/fr_FR.png
+-rw-r--r--   0        0        0    10944 2024-01-18 20:57:20.332509 tlp_ui-1.6.5/tlpui/icons/flags/id_ID.png
+-rw-r--r--   0        0        0    31144 2024-01-18 20:57:20.332509 tlp_ui-1.6.5/tlpui/icons/flags/pt_BR.png
+-rw-r--r--   0        0        0    12002 2024-01-18 20:57:20.332509 tlp_ui-1.6.5/tlpui/icons/flags/ru_RU.png
+-rw-r--r--   0        0        0    20068 2024-01-18 20:57:20.332509 tlp_ui-1.6.5/tlpui/icons/flags/tr_TR.png
+-rw-r--r--   0        0        0    18587 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/flags/zh_CN.png
+-rw-r--r--   0        0        0     1882 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/128x128/apps/tlpui.png
+-rw-r--r--   0        0        0      511 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/16x16/apps/tlpui.png
+-rw-r--r--   0        0        0     3438 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/256x256/apps/tlpui.png
+-rw-r--r--   0        0        0      710 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/32x32/apps/tlpui.png
+-rw-r--r--   0        0        0     1016 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/48x48/apps/tlpui.png
+-rw-r--r--   0        0        0     1144 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/64x64/apps/tlpui.png
+-rw-r--r--   0        0        0     1576 2024-01-18 20:57:20.335842 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/96x96/apps/tlpui.png
+-rw-r--r--   0        0        0     5166 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/dialog-information-symbolic.svg
+-rw-r--r--   0        0        0     5137 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/document-save-symbolic.svg
+-rw-r--r--   0        0        0     4283 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/edit-symbolic.svg
+-rw-r--r--   0        0        0     4103 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/format-indent-more-symbolic.svg
+-rw-r--r--   0        0        0     4037 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/list-add-symbolic.svg
+-rw-r--r--   0        0        0     5643 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Audio-symbolic.svg
+-rw-r--r--   0        0        0     8885 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Disks-symbolic.svg
+-rw-r--r--   0        0        0     5683 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Dock-symbolic.svg
+-rw-r--r--   0        0        0     4214 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-General-symbolic.svg
+-rw-r--r--   0        0        0     4318 2024-01-18 20:57:20.339176 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Graphics-symbolic.svg
+-rw-r--r--   0        0        0     4292 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Network-symbolic.svg
+-rw-r--r--   0        0        0     4562 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-PCIe-symbolic.svg
+-rw-r--r--   0        0        0     4480 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Processor-symbolic.svg
+-rw-r--r--   0        0        0     5140 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-Device-Wizard-symbolic.svg
+-rw-r--r--   0        0        0     4625 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-symbolic.svg
+-rw-r--r--   0        0        0     4674 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-ThinkPad-Battery-symbolic.svg
+-rw-r--r--   0        0        0     7564 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-USB-symbolic.svg
+-rw-r--r--   0        0        0     4223 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/view-refresh-symbolic.svg
+-rw-r--r--   0        0        0    16902 2024-01-18 20:57:20.342509 tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/apps/tlpui.svg
+-rw-r--r--   0        0        0    13685 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/icons/user.svg
+-rw-r--r--   0        0        0    18934 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    22006 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1230 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1490 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      585 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      689 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      894 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1040 2024-01-18 20:57:20.345842 tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    18936 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    22008 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1164 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1424 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      582 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      686 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      864 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1010 2024-01-18 20:57:20.349176 tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    18657 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    21657 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1215 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1494 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      624 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      747 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      915 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1080 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    24760 2024-01-18 20:57:20.352509 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    28112 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1251 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1517 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      647 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      755 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      976 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1126 2024-01-18 20:57:20.355842 tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    18533 2024-01-18 20:57:20.359175 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    21530 2024-01-18 20:57:20.359175 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1255 2024-01-18 20:57:20.359175 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1515 2024-01-18 20:57:20.359175 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      615 2024-01-18 20:57:20.359175 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      723 2024-01-18 20:57:20.362509 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      867 2024-01-18 20:57:20.362509 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1013 2024-01-18 20:57:20.362509 tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    18814 2024-01-18 20:57:20.362509 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    21799 2024-01-18 20:57:20.362509 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1273 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1533 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      692 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      800 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      969 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1115 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    28960 2024-01-18 20:57:20.365842 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    32056 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1415 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1675 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      652 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      756 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0     1033 2024-01-18 20:57:20.369175 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1179 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    19415 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    22485 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1272 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1589 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      661 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      822 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      980 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1183 2024-01-18 20:57:20.372508 tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    17500 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    20442 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1202 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1462 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      609 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      713 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      898 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1044 2024-01-18 20:57:20.375842 tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0    17533 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.mo
+-rw-r--r--   0        0        0    20475 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.po
+-rw-r--r--   0        0        0     1202 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/mainui.mo
+-rw-r--r--   0        0        0     1462 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/mainui.po
+-rw-r--r--   0        0        0      609 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/statui.mo
+-rw-r--r--   0        0        0      713 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/statui.po
+-rw-r--r--   0        0        0      898 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.mo
+-rw-r--r--   0        0        0     1044 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.po
+-rw-r--r--   0        0        0      740 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/language.py
+-rw-r--r--   0        0        0    12684 2024-01-23 22:04:39.778186 tlp_ui-1.6.5/tlpui/mainui.py
+-rw-r--r--   0        0        0      965 2024-01-18 20:57:20.379175 tlp_ui-1.6.5/tlpui/settings.py
+-rw-r--r--   0        0        0     4159 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/settingshelper.py
+-rw-r--r--   0        0        0     2522 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/statui.py
+-rw-r--r--   0        0        0      529 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/styles.css
+-rw-r--r--   0        0        0       38 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/__init__.py
+-rw-r--r--   0        0        0     1387 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkcheckbutton.py
+-rw-r--r--   0        0        0    11154 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkdisklist.py
+-rw-r--r--   0        0        0      324 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkdisklistview.py
+-rw-r--r--   0        0        0      658 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkentry.py
+-rw-r--r--   0        0        0     1302 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkmultiselection.py
+-rw-r--r--   0        0        0     2954 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkpcilist.py
+-rw-r--r--   0        0        0      954 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkselection.py
+-rw-r--r--   0        0        0      890 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkspinbutton.py
+-rw-r--r--   0        0        0      849 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkswitch.py
+-rw-r--r--   0        0        0     1412 2024-01-18 20:57:20.382508 tlp_ui-1.6.5/tlpui/ui_config_objects/gtktoggle.py
+-rw-r--r--   0        0        0     5093 2024-01-18 20:57:20.385842 tlp_ui-1.6.5/tlpui/ui_config_objects/gtkusblist.py
+-rw-r--r--   0        0        0     4709 2024-01-18 20:57:20.385842 tlp_ui-1.6.5/tlpui/uihelper.py
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 tlp_ui-1.6.5/setup.py
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 tlp_ui-1.6.5/PKG-INFO
```

### Comparing `tlp_ui-1.6.4/LICENSE.md` & `tlp_ui-1.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/README.md` & `tlp_ui-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/pyproject.toml` & `tlp_ui-1.6.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tlp-ui"
-version = "1.6.4"
+version = "1.6.5"
 description = "GTK UI for tlp"
 license = "GPL-2.0-or-later"
 authors = ["Daniel Christophis <code@devmind.org>"]
 readme = "README.md"
 homepage = "https://github.com/d4nj1/TLPUI"
 repository = "https://github.com/d4nj1/TLPUI"
 documentation = "https://github.com/d4nj1/TLPUI/docs"
```

### Comparing `tlp_ui-1.6.4/tlpui/__main__.py` & `tlp_ui-1.6.5/tlpui/__main__.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/config.py` & `tlp_ui-1.6.5/tlpui/config.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configschema/1_3.yaml` & `tlp_ui-1.6.5/tlpui/configschema/1_3.yaml`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configschema/1_4.yaml` & `tlp_ui-1.6.5/tlpui/configschema/1_4.yaml`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configschema/1_5.yaml` & `tlp_ui-1.6.5/tlpui/configschema/1_5.yaml`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configschema/1_6.yaml` & `tlp_ui-1.6.5/tlpui/configschema/1_6.yaml`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configschema/1_7.yaml` & `tlp_ui-1.6.5/tlpui/configschema/1_7.yaml`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/configui.py` & `tlp_ui-1.6.5/tlpui/configui.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/defaults/tlp-1_3.conf` & `tlp_ui-1.6.5/tlpui/defaults/tlp-1_3.conf`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/defaults/tlp-1_4.conf` & `tlp_ui-1.6.5/tlpui/defaults/tlp-1_4.conf`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/defaults/tlp-1_5.conf` & `tlp_ui-1.6.5/tlpui/defaults/tlp-1_5.conf`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/defaults/tlp-1_6.conf` & `tlp_ui-1.6.5/tlpui/defaults/tlp-1_6.conf`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/defaults/tlp-1_7.conf` & `tlp_ui-1.6.5/tlpui/defaults/tlp-1_7.conf`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/file.py` & `tlp_ui-1.6.5/tlpui/file.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/filehelper.py` & `tlp_ui-1.6.5/tlpui/filehelper.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/ICON-AUTHORS` & `tlp_ui-1.6.5/tlpui/icons/ICON-AUTHORS`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/OnAC.svg` & `tlp_ui-1.6.5/tlpui/icons/OnAC.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/OnBAT.svg` & `tlp_ui-1.6.5/tlpui/icons/OnBAT.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/dropin.svg` & `tlp_ui-1.6.5/tlpui/icons/dropin.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/de_DE.png` & `tlp_ui-1.6.5/tlpui/icons/flags/de_DE.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/en_EN.png` & `tlp_ui-1.6.5/tlpui/icons/flags/en_EN.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/es_ES.png` & `tlp_ui-1.6.5/tlpui/icons/flags/es_ES.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/fr_FR.png` & `tlp_ui-1.6.5/tlpui/icons/flags/fr_FR.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/id_ID.png` & `tlp_ui-1.6.5/tlpui/icons/flags/id_ID.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/pt_BR.png` & `tlp_ui-1.6.5/tlpui/icons/flags/pt_BR.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/ru_RU.png` & `tlp_ui-1.6.5/tlpui/icons/flags/ru_RU.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/tr_TR.png` & `tlp_ui-1.6.5/tlpui/icons/flags/tr_TR.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/flags/zh_CN.png` & `tlp_ui-1.6.5/tlpui/icons/flags/zh_CN.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/128x128/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/128x128/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/256x256/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/256x256/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/32x32/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/32x32/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/48x48/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/48x48/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/64x64/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/64x64/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/96x96/apps/tlpui.png` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/96x96/apps/tlpui.png`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/dialog-information-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/dialog-information-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/document-save-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/document-save-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/edit-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/edit-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/format-indent-more-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/format-indent-more-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/list-add-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/list-add-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Audio-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Audio-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Disks-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Disks-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Dock-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Dock-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-General-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-General-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Graphics-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Graphics-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Network-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Network-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-PCIe-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-PCIe-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Processor-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Processor-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-Device-Wizard-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-Device-Wizard-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-Radio-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-ThinkPad-Battery-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-ThinkPad-Battery-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-USB-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/tlpui-USB-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/actions/view-refresh-symbolic.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/actions/view-refresh-symbolic.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/themeable/hicolor/scalable/apps/tlpui.svg` & `tlp_ui-1.6.5/tlpui/icons/themeable/hicolor/scalable/apps/tlpui.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/icons/user.svg` & `tlp_ui-1.6.5/tlpui/icons/user.svg`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/de_DE/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/de_DE/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/en_EN/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/en_EN/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/es_ES/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/es_ES/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/fr_FR/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/id_ID/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/id_ID/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/pt_BR/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/ru_RU/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/tr_TR/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/zh_CN/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.po` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/configdescriptions.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/mainui.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/mainui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/mainui.po` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/mainui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/statui.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/statui.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/statui.po` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/statui.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.mo` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.mo`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.po` & `tlp_ui-1.6.5/tlpui/lang/zh_TW/LC_MESSAGES/uihelper.po`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/language.py` & `tlp_ui-1.6.5/tlpui/language.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/mainui.py` & `tlp_ui-1.6.5/tlpui/mainui.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/settings.py` & `tlp_ui-1.6.5/tlpui/settings.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/settingshelper.py` & `tlp_ui-1.6.5/tlpui/settingshelper.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/statui.py` & `tlp_ui-1.6.5/tlpui/statui.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/styles.css` & `tlp_ui-1.6.5/tlpui/styles.css`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkcheckbutton.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkcheckbutton.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkdisklist.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkdisklist.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkentry.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkentry.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkmultiselection.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkmultiselection.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkpcilist.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkpcilist.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkselection.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkselection.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkspinbutton.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkspinbutton.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkswitch.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkswitch.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtktoggle.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtktoggle.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/ui_config_objects/gtkusblist.py` & `tlp_ui-1.6.5/tlpui/ui_config_objects/gtkusblist.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/tlpui/uihelper.py` & `tlp_ui-1.6.5/tlpui/uihelper.py`

 * *Files identical despite different names*

### Comparing `tlp_ui-1.6.4/setup.py` & `tlp_ui-1.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ['pygobject>=3.46.0,<4.0.0', 'pyyaml>=6.0.1,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['tlpui = tlpui.__main__:main']}
 
 setup_kwargs = {
     'name': 'tlp-ui',
-    'version': '1.6.4',
+    'version': '1.6.5',
     'description': 'GTK UI for tlp',
     'long_description': '\n<img src="https://raw.githubusercontent.com/d4nj1/TLPUI/master/tlpui/icons/themeable/hicolor/scalable/apps/tlpui.svg" align="left" alt="TLP UI" width="196px">\n\n## TLP UI\n\nThe Python scripts in this project generate a GTK-UI to change [TLP](https://github.com/linrunner/TLP) configuration files easily.\nIt has the aim to protect users from setting bad configuration and to deliver a basic overview of all the valid configuration values.\n\n<img src="https://raw.githubusercontent.com/d4nj1/TLPUI/master/screenshots/tlpui-01.png" alt="Screenshot" vspace="20px">\n\n### Install and run instructions :ledger:\n\n* [PyPI](https://github.com/d4nj1/TLPUI/blob/master/docs/INSTALL.md#pypi)\n* [Poetry](https://github.com/d4nj1/TLPUI/blob/master/docs/INSTALL.md#poetry)\n* [Python 3](https://github.com/d4nj1/TLPUI/blob/master/docs/INSTALL.md#python-3)\n* [Arch Linux](https://github.com/d4nj1/TLPUI/blob/master/docs/INSTALL.md#arch-linux)\n\n<a href=\'https://flathub.org/apps/details/com.github.d4nj1.tlpui\'><img width=\'240\' alt=\'Download on Flathub\' src=\'https://flathub.org/assets/badges/flathub-badge-en.png\'/></a>\n\n### Current status :sunrise_over_mountains:\n\n* Supports TLP versions 1.3-1.6 - _older TLP versions are supported by [1.6.1](https://github.com/d4nj1/TLPUI/releases/tag/tlpui-1.6.1)_\n* Requires Python 3.8 or greater\n* Configuration can be read and displayed\n* Shows information about configuration changes (defaults/unsaved and drop-in/user config)\n* Changes can be saved with user and sudo permissions (/etc/tlp.conf)\n* tlp-stat can be load in ui (simple and complete)\n\n### To be done :building_construction:\n\n* Weblate translations - [#121](https://github.com/d4nj1/TLPUI/issues/121)\n* Mobile UI - [#111](https://github.com/d4nj1/TLPUI/issues/111)\n* Implement package build pipeline - [#90](https://github.com/d4nj1/TLPUI/issues/90)\n',
     'author': 'Daniel Christophis',
     'author_email': 'code@devmind.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/d4nj1/TLPUI',
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 'icons/themeable/hicolor/96x96/apps/*', 'icons/themeable/hicolor/scalable/
 actions/*', 'icons/themeable/hicolor/scalable/apps/*', 'lang/de_DE/LC_MESSAGES/
 *', 'lang/en_EN/LC_MESSAGES/*', 'lang/es_ES/LC_MESSAGES/*', 'lang/fr_FR/
 LC_MESSAGES/*', 'lang/id_ID/LC_MESSAGES/*', 'lang/pt_BR/LC_MESSAGES/*', 'lang/
 ru_RU/LC_MESSAGES/*', 'lang/tr_TR/LC_MESSAGES/*', 'lang/zh_CN/LC_MESSAGES/*',
 'lang/zh_TW/LC_MESSAGES/*']} install_requires = \ ['pygobject>=3.46.0,<4.0.0',
 'pyyaml>=6.0.1,<7.0.0'] entry_points = \ {'console_scripts': ['tlpui =
-tlpui.__main__:main']} setup_kwargs = { 'name': 'tlp-ui', 'version': '1.6.4',
+tlpui.__main__:main']} setup_kwargs = { 'name': 'tlp-ui', 'version': '1.6.5',
 'description': 'GTK UI for tlp', 'long_description': '\n[TLP UI]\n\n## TLP
 UI\n\nThe Python scripts in this project generate a GTK-UI to change [TLP]
 (https://github.com/linrunner/TLP) configuration files easily.\nIt has the aim
 to protect users from setting bad configuration and to deliver a basic overview
 of all the valid configuration values.\n\n[Screenshot]\n\n### Install and run
 instructions :ledger:\n\n* [PyPI](https://github.com/d4nj1/TLPUI/blob/master/
 docs/INSTALL.md#pypi)\n* [Poetry](https://github.com/d4nj1/TLPUI/blob/master/
```

### Comparing `tlp_ui-1.6.4/PKG-INFO` & `tlp_ui-1.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlp-ui
-Version: 1.6.4
+Version: 1.6.5
 Summary: GTK UI for tlp
 Home-page: https://github.com/d4nj1/TLPUI
 License: GPL-2.0-or-later
 Keywords: battery,power,config
 Author: Daniel Christophis
 Author-email: code@devmind.org
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tlp-ui Version: 1.6.4 Summary: GTK UI for tlp Home-
+Metadata-Version: 2.1 Name: tlp-ui Version: 1.6.5 Summary: GTK UI for tlp Home-
 page: https://github.com/d4nj1/TLPUI License: GPL-2.0-or-later Keywords:
 battery,power,config Author: Daniel Christophis Author-email: code@devmind.org
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v2 or later (GPLv2+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

