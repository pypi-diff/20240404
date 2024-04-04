# Comparing `tmp/PyQtUIkit-2.0.9.tar.gz` & `tmp/PyQtUIkit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.0.9.tar", last modified: Wed Apr  3 12:18:32 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.1.0.tar", last modified: Thu Apr  4 19:10:24 2024, max compression
```

## Comparing `PyQtUIkit-2.0.9.tar` & `PyQtUIkit-2.1.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.880630 PyQtUIkit-2.0.9/
--rw-rw-rw-   0        0        0     1090 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-03 12:18:32.880630 PyQtUIkit-2.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.849391 PyQtUIkit-2.0.9/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3835 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.849391 PyQtUIkit-2.0.9/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.849391 PyQtUIkit-2.0.9/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.864999 PyQtUIkit-2.0.9/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.880630 PyQtUIkit-2.0.9/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559097 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1346 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.880630 PyQtUIkit-2.0.9/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1488 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     4174 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2785 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9981 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4180 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1468 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     7356 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    12024 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16473 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4507 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:18:32.849391 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 12:18:32.000000 PyQtUIkit-2.0.9/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 12:18:32.880630 PyQtUIkit-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-03 12:17:12.000000 PyQtUIkit-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.421768 PyQtUIkit-2.1.0/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3835 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.437391 PyQtUIkit-2.1.0/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.437391 PyQtUIkit-2.1.0/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.453012 PyQtUIkit-2.1.0/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.453012 PyQtUIkit-2.1.0/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559097 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1346 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1505 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7833 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2785 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    10004 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4293 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1468 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1173 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7507 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    13356 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17249 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4620 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:10:24.421768 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 19:10:24.000000 PyQtUIkit-2.1.0/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:10:24.468640 PyQtUIkit-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-04 19:09:51.000000 PyQtUIkit-2.1.0/setup.py
```

### Comparing `PyQtUIkit-2.0.9/LICENSE` & `PyQtUIkit-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PKG-INFO` & `PyQtUIkit-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.9
+Version: 2.1.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/_icons.py` & `PyQtUIkit-2.1.0/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.1.0/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.1.0/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/core/font.py` & `PyQtUIkit-2.1.0/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.1.0/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.1.0/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.1.0/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.1.0/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.1.0/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.1.0/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.1.0/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.1.0/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
 from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
 from PyQtUIkit.widgets.flow_layout import KitFlowLayout
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
-from PyQtUIkit.widgets.button import KitButton, KitIconButton
+from PyQtUIkit.widgets.button import KitButton, KitIconButton, KitLayoutButton
 from PyQtUIkit.widgets.line_edit import KitLineEdit
 from PyQtUIkit.widgets.list_widget import KitListWidget, KitListWidgetItem
 from PyQtUIkit.widgets.main_window import KitMainWindow
 from PyQtUIkit.widgets.spin_box import KitSpinBox
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.combo_box import KitComboBox, KitComboBoxItem
 from PyQtUIkit.widgets.checkbox import KitCheckBox
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/hbox_layout.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,123 @@
-from PyQt6.QtCore import Qt
-from PyQt6.QtWidgets import QPushButton, QVBoxLayout
+from PyQt6.QtCore import QMargins
+from PyQt6.QtWidgets import QWidget, QHBoxLayout
 
-from PyQtUIkit.core import IconProperty, EnumProperty, IntProperty, PaletteProperty, KitFont, FontProperty, \
-    SignalProperty, MethodsProperty
-from PyQtUIkit.themes import ThemeManager
-from PyQtUIkit.widgets import KitIconWidget
-from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
-
-
-class KitButton(QPushButton, _KitGroupItem):
-    main_palette = PaletteProperty('main_palette', 'Main')
-    icon = IconProperty('icon')
-    font = FontProperty('font')
-    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
-    on_click = SignalProperty('on_click', 'clicked')
+from PyQtUIkit.core.properties import IntProperty, MethodsProperty
+from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
-    def __init__(self, text='', icon=None):
+
+class KitHBoxLayout(QWidget, _KitWidget):
+    border = IntProperty('border', 0)
+    radius = IntProperty('radius', 4)
+
+    def __init__(self):
         super().__init__()
-        self.__widgets = []
-        self.setCursor(Qt.CursorShape.PointingHandCursor)
+        self._widgets = []
+        self.main_palette = 'Transparent'
 
-        self.setText(text)
-        self._icon = icon
+        strange_layout = QHBoxLayout()
+        strange_layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(strange_layout)
+
+        strange_widget = QWidget()
+        strange_layout.addWidget(strange_widget)
+
+        self.__layout = QHBoxLayout()
+        self.__layout.setContentsMargins(0, 0, 0, 0)
+        self.__layout.setSpacing(0)
+        strange_widget.setLayout(self.__layout)
 
+        self._add_child_func = self.addWidget
         self._build_from_kui()
 
-    def _apply_theme(self):
-        if not self._tm or not self._tm.active:
-            return
-        self.setFont(self.font.get(self.font_size))
-        self.setStyleSheet(f"""
-QPushButton {{
-    color: {self.main_palette.text};
-    background-color: {self.main_palette.main};
-    border: {self.border}px solid {self.border_palette.main};
-    {self._border_radius_css()}
-    padding: 3px 8px 3px 8px;
-}}
-QPushButton::hover {{
-    background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self.border_palette.selected};
-}}
-QPushButton::disabled {{
-    color: {self.main_palette.main};
-    border-color: {self.border_palette.main};
-}}
-QPushButton::checked {{
-    background-color: {self.main_palette.selected};
-    border: {self.border}px solid {self.border_palette.selected};
-}}
-QPushButton::menu-indicator {{
-    image: none;
-    subcontrol-origin: padding;
-    padding-right: 5px;
-    subcontrol-position: right;
-}}""")
-        if self.icon is not None:
-            self.setIcon(self.icon.icon(self.main_palette.text))
-
-    text = MethodsProperty(QPushButton.text, QPushButton.setText)
-
-
-class KitIconButton(QPushButton, _KitGroupItem):
-    main_palette = PaletteProperty('main_palette', 'Main')
-    icon = IconProperty('icon')
-    on_click = SignalProperty('on_click', 'clicked')
+    def addWidget(self, widget: QWidget, stretch: int = None, alignment=None):
+        if alignment is not None:
+            self.__layout.addWidget(widget, stretch, alignment)
+        elif stretch is not None:
+            self.__layout.addWidget(widget, stretch)
+        else:
+            self.__layout.addWidget(widget)
+        self._widgets.append(widget)
+        if hasattr(widget, '_set_tm'):
+            widget._set_tm(self._tm)
+
+    def insertWidget(self, index: int, widget: QWidget, stretch: int = None, alignment=None):
+        if alignment is not None:
+            self.__layout.insertWidget(index, widget, stretch, alignment)
+        elif stretch is not None:
+            self.__layout.insertWidget(index, widget, stretch)
+        else:
+            self.__layout.insertWidget(index, widget)
+        self._widgets.insert(index, widget)
+        if hasattr(widget, '_set_tm'):
+            widget._set_tm(self._tm)
+
+    def deleteWidget(self, w: int | QWidget):
+        if isinstance(w, int):
+            w = self.__layout.takeAt(w).widget()
+        w.setParent(None)
+        return w
+
+    def clear(self):
+        for _ in range(self.__layout.count()):
+            self.__layout.takeAt(0).widget().setParent(None)
+        self._widgets.clear()
+
+    def setAlignment(self, a):
+        self.__layout.setAlignment(a)
+
+    def getAlignment(self):
+        return self.__layout.alignment()
+
+    def setSpacing(self, spacing):
+        self.__layout.setSpacing(spacing)
+
+    def getSpacing(self):
+        return self.__layout.spacing()
+
+    def setContentsMargins(self, left: int, top: int, right: int, bottom: int) -> None:
+        self.__layout.setContentsMargins(left, top, right, bottom)
+
+    def getContentsMargins(self):
+        return self.__layout.contentsMargins()
+
+    def _set_margins(self, margins):
+        if isinstance(margins, int):
+            self.setContentsMargins(margins, margins, margins, margins)
+        elif len(margins) == 1:
+            self.__layout.setContentsMargins(margins[0], margins[0], margins[0], margins[0])
+        elif len(margins) == 2:
+            self.__layout.setContentsMargins(margins[0], margins[1], margins[0], margins[1])
+        elif len(margins) == 4:
+            self.__layout.setContentsMargins(*margins)
+        else:
+            raise ValueError
 
-    def __init__(self, icon=''):
-        super().__init__()
-        self.__widgets = []
-        self._icon = icon
-        self._main_palette = 'Main'
-        self.setCursor(Qt.CursorShape.PointingHandCursor)
-
-        self.__layout = QVBoxLayout()
-        self.setLayout(self.__layout)
-
-        self._icon_label = KitIconWidget()
-        self._icon_label._use_text_only = False
-        self.__layout.addWidget(self._icon_label)
+    def contentsMargins(self) -> QMargins:
+        return self.__layout.contentsMargins()
 
-    def _set_tm(self, tm: ThemeManager):
-        super()._set_tm(tm)
-        self._icon_label._set_tm(tm)
+    def count(self):
+        return self.__layout.count()
 
-    def _set_size(self, x, y=None):
-        if isinstance(x, int) and isinstance(y, int):
-            self.setFixedSize(x, y)
-        elif y is None:
-            self.setFixedSize(x, x)
-        else:
-            self.setFixedSize(x)
+    def _set_tm(self, tm):
+        super()._set_tm(tm)
+        for el in self._widgets:
+            if hasattr(el, '_set_tm'):
+                el._set_tm(tm)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
-        self._icon_label.icon = self.icon
-        self._icon_label._main_palette = self._main_palette
-        self.__layout.setContentsMargins(*[min(self.width(), self.height()) // 5] * 4)
+        for el in self._widgets:
+            if hasattr(el, '_apply_theme'):
+                el._apply_theme()
         self.setStyleSheet(f"""
-QPushButton {{
-    background-color: {self.main_palette.main};
-    border: {self.border}px solid {self.border_palette.main};
-    {self._border_radius_css()}
-    padding: 3px 8px 3px 8px;
-}}
-QPushButton::hover {{
-    background-color: {self.main_palette.hover};
-    border: {self.border}px solid {self.border_palette.selected};
-}}
-QPushButton::disabled {{
-    color: {self.main_palette.main};
-    border-color: {self.border_palette.main};
-}}
-QPushButton::checked {{
-    background-color: {self.main_palette.selected};
-    border: {self.border}px solid {self.border_palette.selected};
-}}
-QPushButton::menu-indicator {{
-    image: none;
-    subcontrol-position: right;
-}}""")
-
-    size = MethodsProperty(QPushButton.size, _set_size)
+        QWidget {{
+            background-color: {self.main_palette.main};
+            border: {self.border}px solid {self.border_palette.main};
+            border-radius: {self.radius}px;
+        }}
+        """)
+
+    padding = MethodsProperty(getContentsMargins, _set_margins)
+    spacing = MethodsProperty(getSpacing, setSpacing)
+    alignment = MethodsProperty(getAlignment, setAlignment)
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/combo_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     icon = IconProperty('icon')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, name='', value=None, icon=''):
         super().__init__()
         self._name = name
-        self._value = value or name
+        self._value = value if value is not None else name
         self._icon = icon
         self.setCheckable(True)
         self.clicked.connect(self._on_clicked)
         self.setText(self._name)
         self.setFixedHeight(24)
         self.setCursor(Qt.CursorShape.PointingHandCursor)
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/vbox_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from PyQt6.QtCore import QMargins
-from PyQt6.QtWidgets import QWidget, QHBoxLayout
+from PyQt6.QtWidgets import QWidget, QVBoxLayout
 
 from PyQtUIkit.core.properties import IntProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
-class KitHBoxLayout(QWidget, _KitWidget):
+class KitVBoxLayout(QWidget, _KitWidget):
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
 
     def __init__(self):
         super().__init__()
         self._widgets = []
-        self.main_palette = 'Transparent'
+        self._main_palette = 'Transparent'
 
-        strange_layout = QHBoxLayout()
+        strange_layout = QVBoxLayout()
         strange_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(strange_layout)
 
         strange_widget = QWidget()
         strange_layout.addWidget(strange_widget)
 
-        self.__layout = QHBoxLayout()
+        self.__layout = QVBoxLayout()
         self.__layout.setContentsMargins(0, 0, 0, 0)
         self.__layout.setSpacing(0)
         strange_widget.setLayout(self.__layout)
 
         self._add_child_func = self.addWidget
         self._build_from_kui()
 
@@ -77,15 +77,17 @@
     def setContentsMargins(self, left: int, top: int, right: int, bottom: int) -> None:
         self.__layout.setContentsMargins(left, top, right, bottom)
 
     def getContentsMargins(self):
         return self.__layout.contentsMargins()
 
     def _set_margins(self, margins):
-        if len(margins) == 1:
+        if isinstance(margins, int):
+            self.setContentsMargins(margins, margins, margins, margins)
+        elif len(margins) == 1:
             self.__layout.setContentsMargins(margins[0], margins[0], margins[0], margins[0])
         elif len(margins) == 2:
             self.__layout.setContentsMargins(margins[0], margins[1], margins[0], margins[1])
         elif len(margins) == 4:
             self.__layout.setContentsMargins(*margins)
         else:
             raise ValueError
@@ -115,7 +117,11 @@
             border-radius: {self.radius}px;
         }}
         """)
 
     padding = MethodsProperty(getContentsMargins, _set_margins)
     spacing = MethodsProperty(getSpacing, setSpacing)
     alignment = MethodsProperty(getAlignment, setAlignment)
+    max_width = MethodsProperty(QWidget.maximumWidth, QWidget.setMaximumWidth)
+    min_width = MethodsProperty(QWidget.minimumWidth, QWidget.setMinimumWidth)
+    max_height = MethodsProperty(QWidget.maximumHeight, QWidget.setMaximumHeight)
+    min_height = MethodsProperty(QWidget.minimumHeight, QWidget.setMinimumHeight)
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/spin_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty, MethodsProperty, SignalProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem, KitGroup as _KitGroup
 
 
 class KitSpinBox(QWidget, _KitGroupItem):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
+
     valueChanged = pyqtSignal(object)
     valueEdited = pyqtSignal(object)
+    editingFinished = pyqtSignal()
+
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, func=int):
         super().__init__()
         self._min = 0
         self._max = 100
@@ -80,26 +83,29 @@
         self._last_pos = self._line_edit.cursorPosition()
 
     def _on_editing_finished(self):
         text = self._line_edit.text()
         if not text:
             self._line_edit.setText('0')
             self._on_text_edited()
+        self.editingFinished.emit()
 
     def _decrease(self):
-        self.setValue(round(self.value() - self._step, 2))
-        self.valueChanged.emit(self.value())
-        self._line_edit.selectAll()
-        self._line_edit.setFocus()
+        self.setValue(round(self.value - self._step, 2))
+        self.valueChanged.emit(self.value)
+        # self._line_edit.selectAll()
+        # self._line_edit.setFocus()
+        self.editingFinished.emit()
 
     def _increase(self):
-        self.setValue(round(self.value() + self._step, 2))
-        self.valueChanged.emit(self.value())
-        self._line_edit.selectAll()
-        self._line_edit.setFocus()
+        self.setValue(round(self.value + self._step, 2))
+        self.valueChanged.emit(self.value)
+        # self._line_edit.selectAll()
+        # self._line_edit.setFocus()
+        self.editingFinished.emit()
 
     def setRange(self, minimum, maximum):
         self._min = minimum
         self._max = maximum
         self._on_text_edited(False)
 
     def setMinimum(self, minimum):
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tab_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 class KitTab(QPushButton, _KitWidget):
     radius_top = IntProperty('radius_top', 5)
     radius_bottom = IntProperty('radius_bottom', 0)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     selected = pyqtSignal(object)
+    closeRequested = pyqtSignal()
     _mousePress = pyqtSignal(object)
     _mouseRelease = pyqtSignal()
     icon = IconProperty('icon')
 
     def __init__(self, name, value=None, icon=''):
         super().__init__()
         self._name = name
@@ -50,16 +51,18 @@
 
         self.__label = KitLabel(name)
         self.__label.setContentsMargins(4, 0, 4, 0)
         layout.addWidget(self.__label)
 
         self.__button_close = KitIconButton(icon='solid-xmark')
         self.__button_close.border = 0
-        self.__button_close.size = 18
+        self.__button_close.size = 16
+        self.__button_close.radius = 8
         self.__button_close.hide()
+        self.__button_close.on_click = self.closeRequested.emit
         layout.addWidget(self.__button_close)
 
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
     def _set_checked(self, flag):
         self.__checked = flag
         self._apply_theme()
@@ -127,42 +130,45 @@
         self.__label._apply_theme()
         self.__icon_widget.setHidden(not self.icon)
         self.__icon_widget.icon = self.icon
         self.__button_close._apply_theme()
 
 
 class KitTabBar(KitHBoxLayout, _KitWidget):
-    main_palette = PaletteProperty('main_palette', 'Bg')
     tabs_palette = PaletteProperty('tabs_palette', 'Main')
     height = IntProperty('height', 26)
-    border = IntProperty('border', 0)
-    radius = IntProperty('radius', 4)
+    radius_top = IntProperty('radius_top', 6)
+    radius_bottom = IntProperty('radius_bottom', 0)
 
-    currentChanged = pyqtSignal(int)
+    currentChanged = pyqtSignal(object)
+    tabCloseRequested = pyqtSignal(int)
+    tabMoved = pyqtSignal(int, int)
 
     def __init__(self):
         super().__init__()
         self.__tabs: list[KitTab] = []
         self.__current = None
         self.__tabs_closable = False
         self.__tabs_movable = False
         self.setContentsMargins(0, 0, 0, 0)
+        self.radius = 0
         self.setSpacing(0)
         self._main_palette = 'Bg'
 
         self.__button_left = KitButton(icon='solid-chevron-left')
         self.__button_left.border = 0
         self.__button_left.setFixedWidth(20)
         self.__button_left.clicked.connect(self._scroll_left)
         self.addWidget(self.__button_left)
 
         self.__scroll_area = KitScrollArea()
         self.addWidget(self.__scroll_area)
         self.__layout = _TabLayout(self.__tabs)
         self.__scroll_area.setWidget(self.__layout)
+        self.__layout.tabMoved.connect(self.tabMoved.emit)
         self.__scroll_area.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
         self.__button_right = KitButton(icon='solid-chevron-right')
         self.__button_right.border = 0
         self.__button_right.setFixedWidth(20)
         self.__button_right.clicked.connect(self._scroll_right)
         self.addWidget(self.__button_right)
@@ -172,44 +178,64 @@
 
     def insertTab(self, index, tab: str | KitTab):
         if isinstance(tab, str):
             tab = KitTab(tab)
         tab._set_closable(self.__tabs_closable)
         tab._set_tm(self._tm)
         tab.selected.connect(lambda: self.setCurrentTab(tab))
+        tab.closeRequested.connect(lambda: self._close_requested(tab))
         tab._mousePress.connect(self.__layout.on_mouse_press)
         tab._mouseRelease.connect(self.__layout.on_mouse_release)
         self.__tabs.insert(index, tab)
         self.__layout.update_tabs()
         if self.__current is None:
             self.__current = tab
             tab._set_checked(True)
 
     def _scroll_left(self):
-        self.__scroll_area.scroll(-10)
+        self.__scroll_area.scroll(-50)
 
     def _scroll_right(self):
-        self.__scroll_area.scroll(10)
+        self.__scroll_area.scroll(50)
+
+    def _close_requested(self, tab):
+        self.tabCloseRequested.emit(self.__tabs.index(tab))
 
     def setTabsClosable(self, flag):
         self.__tabs_closable = flag
         for el in self.__tabs:
             el._set_closable(flag)
 
     def setTabsMovable(self, flag):
         self.__tabs_movable = flag
         self.__layout.set_tabs_movable(flag)
 
     def setCurrentTab(self, tab: int | KitTab):
         if isinstance(tab, int):
-            tab = self.__tabs[tab]
-        self.__current._set_checked(False)
+            try:
+                tab = self.__tabs[tab]
+            except IndexError:
+                tab = None
+        if self.__current:
+            self.__current._set_checked(False)
         self.__current = tab
-        self.__current._set_checked(True)
-        self.currentChanged.emit(self.__tabs.index(tab))
+        if self.__current:
+            self.__current._set_checked(True)
+        self.currentChanged.emit(None if tab is None else self.__tabs.index(tab))
+
+    def tabsCount(self):
+        return len(self.__tabs)
+
+    def removeTab(self, index):
+        tab = self.__tabs.pop(index)
+        self.__layout.update_tabs()
+        if self.__current == tab:
+            self.setCurrentTab(min(index, self.tabsCount() - 1))
+        self.__button_left.setHidden(self.__layout.width() <= self.width())
+        self.__button_right.setHidden(self.__layout.width() <= self.width())
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
         for el in self.__tabs:
             el._set_tm(tm)
 
     def resizeEvent(self, a0) -> None:
@@ -223,20 +249,24 @@
         self.__scroll_area.main_palette = self.main_palette
         self.__scroll_area.setFixedHeight(self.height)
         self.__button_left.main_palette = self.main_palette
         self.__button_right.main_palette = self.main_palette
         super()._apply_theme()
         for el in self.__tabs:
             el.main_palette = self.tabs_palette
+            el.radius_top = self.radius_top
+            el.radius_bottom = self.radius_bottom
             el.setFixedHeight(self.height)
             el._apply_theme()
         self.__layout.update_tabs()
 
 
 class _TabLayout(QWidget):
+    tabMoved = pyqtSignal(int, int)
+
     def __init__(self, widgets: list[KitTab]):
         super().__init__()
         self.__widgets = widgets
         self.__tabs_movable = False
         self.__widgets_positions = [0 for _ in widgets]
         self.__last_pos = QPoint(0, 0)
         self.__tab_move: KitTab | None = None
@@ -293,20 +323,22 @@
     def set_tabs_movable(self, flag):
         self.__tabs_movable = flag
 
     def __move_right(self, index):
         self.__widgets[index], self.__widgets[index + 1] = self.__widgets[index + 1], self.__widgets[index]
         self.__widgets_positions[index + 1] = self.__widgets_positions[index] + self.__tab_move.width()
         self.__move_tab(index + 1)
+        self.tabMoved.emit(self.__tab_move_index, self.__tab_move_index - 1)
         self.__tab_move_index -= 1
 
     def __move_left(self, index):
         self.__widgets[index], self.__widgets[index - 1] = self.__widgets[index - 1], self.__widgets[index]
         self.__widgets_positions[index] = self.__widgets_positions[index - 1] + self.__widgets[index - 1].width()
         self.__move_tab(index - 1)
+        self.tabMoved.emit(self.__tab_move_index, self.__tab_move_index + 1)
         self.__tab_move_index += 1
 
     def __move_tab(self, index):
         tab = self.__widgets[index]
         if index in self.__animations:
             self.__animations[index].stop()
         anim = QPropertyAnimation(tab, b'pos')
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.1.0/PyQtUIkit/widgets/tree_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.setContentsMargins(0, 0, 0, 0)
         self.setSpacing(0)
 
         self.__button = QPushButton()
         self.__button.mousePressEvent = self._on_clicked
         self.__button.mouseMoveEvent = self._on_move
         self.__button.mouseReleaseEvent = self._on_released
+        self.__button.mouseDoubleClickEvent = self._on_double_clicked
         self.addWidget(self.__button)
 
         self.__top_layout = QHBoxLayout()
         self.__top_layout.setContentsMargins(0, 0, 0, 0)
         self.__top_layout.setSpacing(3)
         self.__button.setLayout(self.__top_layout)
 
@@ -151,15 +152,19 @@
 
     def firstExpand(self):
         pass
 
     def _on_clicked(self, a0):
         QPushButton.mousePressEvent(self.__button, a0)
         self.__last_pos = a0.pos()
-        self.__root._item_click(self)
+        self.__root._item_click(self, right=a0.button() == Qt.MouseButton.RightButton)
+
+    def _on_double_clicked(self, a0):
+        QPushButton.mouseDoubleClickEvent(self.__button, a0)
+        self.__root._item_double_click(self)
 
     def _select(self, multi=False):
         self.__selected = True
         self._apply_selected_theme()
         if multi:
             for el in self.__children:
                 el._select(True)
@@ -309,21 +314,25 @@
     item_height = IntProperty('item_height', 24)
     movable = BoolProperty('movable', False)
     selection_type = EnumProperty('selection_type', SelectionType, SelectionType.SINGLE)
     items_palette = PaletteProperty('items_palette', 'Main')
 
     currentItemChanged = pyqtSignal(object)
     moveRequested = pyqtSignal(object, object)
+    doubleClicked = pyqtSignal(object)
+    contextMenuRequested = pyqtSignal(QPoint, KitTreeWidgetItem)
 
     def __init__(self):
         super().__init__()
         self.__children = []
         self._main_palette = 'Main'
         self._items_palette = 'Main'
         self._border = 1
+        self.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
+        self.customContextMenuRequested.connect(self._on_context_menu)
 
         self.__shift = False
         self.__control = False
         self.__current = None
         self.__selected = []
         self.__selected_level = 0
 
@@ -351,15 +360,15 @@
         self.__current = item
 
     def _request_move(self, item, pos):
         dest, _ = self.__tree._find_by_pos(pos - self.__widget.mapToGlobal(QPoint(0, 0)))
         if dest:
             self.moveRequested.emit(item, dest)
 
-    def _item_click(self, item: KitTreeWidgetItem):
+    def _item_click(self, item: KitTreeWidgetItem, right=False):
         if self.selection_type == KitTreeWidget.SelectionType.MULTI:
             if self.__control:
                 if not item.selected():
                     self._add_to_selected(item)
                 else:
                     self._remove_from_selected(item)
             elif self.__shift:
@@ -375,14 +384,21 @@
             self.__selected.clear()
             self.__selected.append(item)
             item._select()
             if isinstance(self.__current, KitTreeWidgetItem):
                 self.__current._deselect()
         self._set_current(item)
 
+    def _item_double_click(self, item: KitTreeWidgetItem):
+        self.doubleClicked.emit(item)
+
+    def _on_context_menu(self, pos):
+        item, _ = self.__tree._find_by_pos(pos)
+        self.contextMenuRequested.emit(pos, item)
+
     def _add_to_selected(self, item: KitTreeWidgetItem):
         if not self.__selected:
             self.__selected.append(item)
             self.__selected_level = item.level()
             item._select(multi=False)
         else:
             while self.__selected_level > item.level():
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.1.0/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.9
+Version: 2.1.0
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.9/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.1.0/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 PyQtUIkit/widgets/list_widget.py
 PyQtUIkit/widgets/main_window.py
 PyQtUIkit/widgets/menu.py
 PyQtUIkit/widgets/navigation.py
 PyQtUIkit/widgets/progress_bar.py
 PyQtUIkit/widgets/radio.py
 PyQtUIkit/widgets/scroll_area.py
+PyQtUIkit/widgets/separator.py
 PyQtUIkit/widgets/spin_box.py
 PyQtUIkit/widgets/spinner.py
 PyQtUIkit/widgets/tab_bar.py
 PyQtUIkit/widgets/tabs.py
 PyQtUIkit/widgets/text_edit.py
 PyQtUIkit/widgets/toggle.py
 PyQtUIkit/widgets/tree_widget.py
```

### Comparing `PyQtUIkit-2.0.9/setup.py` & `PyQtUIkit-2.1.0/setup.py`

 * *Files identical despite different names*

