# Comparing `tmp/joulescope_ui-1.1.0.tar.gz` & `tmp/joulescope_ui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.1.0.tar", last modified: Wed Apr  3 21:18:13 2024, max compression
+gzip compressed data, was "joulescope_ui-1.1.1.tar", last modified: Thu Apr  4 01:10:16 2024, max compression
```

## Comparing `joulescope_ui-1.1.0.tar` & `joulescope_ui-1.1.1.tar`

### file list

```diff
@@ -1,472 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-03 21:18:11.000000 joulescope_ui-1.1.0/joulescope.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.635454 joulescope_ui-1.1.0/joulescope_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-03 21:17:20.000000 joulescope_ui-1.1.0/joulescope_ui/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-03 21:17:20.000000 joulescope_ui-1.1.0/joulescope_ui/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/dev_signal_buffer_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.635454 joulescope_ui-1.1.0/joulescope_ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/device_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js110.py
--rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/devices/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/devices/test/test_device_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/disk_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/entry_points/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/entry_points/zip_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/error_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/expanding_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/filename_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/fonts/DSEG14-Modern/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/fonts/Hack/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/fonts/Hack/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/fonts/Lato/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/fonts/SourceCodePro/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/fonts/SourceSerifPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui/fonts.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/getting_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/help_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/intel_graphics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/jls_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/jls_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/jls_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/jls_v2_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/json_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81002 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   111451 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70795 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   101644 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.639454 joulescope_ui-1.1.0/joulescope_ui/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    97401 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   128233 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70446 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   101226 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72225 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   103098 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.611454 joulescope_ui-1.1.0/joulescope_ui/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    74898 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104820 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)    67661 2024-04-03 21:17:21.000000 joulescope_ui-1.1.0/joulescope_ui/locale/joulescope_ui.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.615454 joulescope_ui-1.1.0/joulescope_ui/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    69349 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    99357 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.615454 joulescope_ui-1.1.0/joulescope_ui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    60506 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    90342 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40944 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/mem_leak_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.643454 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p1/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p1/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.647454 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p2/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/plugins/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/pubsub_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/pubsub_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.647454 joulescope_ui-1.1.0/joulescope_ui/range_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/max_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/plugin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/range_tools/usb_inrush.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.647454 joulescope_ui-1.1.0/joulescope_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.651454 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_128x128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_256x256.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_64x64.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-03 21:18:11.000000 joulescope_ui-1.1.0/joulescope_ui/resources.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/safe_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/shift_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/source_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.651454 joulescope_ui-1.1.0/joulescope_ui/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/font_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.655454 joulescope_ui-1.1.0/joulescope_ui/styles/js1/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_end.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_end_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_more.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/branch_vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/style.html
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/tabs_menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/transparent.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.655454 joulescope_ui-1.1.0/joulescope_ui/styles/system/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/index.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/system/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.655454 joulescope_ui-1.1.0/joulescope_ui/styles/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/test/test_color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/styles/test/test_parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.659454 joulescope_ui-1.1.0/joulescope_ui/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/anno1.anno.jls
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_annotation_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_disk_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_range_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/test/test_versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 21:17:22.000000 joulescope_ui-1.1.0/joulescope_ui/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/ui_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widget_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.659454 joulescope_ui-1.1.0/joulescope_ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.659454 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.663454 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.663454 joulescope_ui-1.1.0/joulescope_ui/widgets/clock/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/clock/clock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.663454 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/log_view_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/profile_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/publish_spy_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.663454 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/current_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_update_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/device_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/device_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/target_power_off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/double_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/draggable_list_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/example/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/example_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/example/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/hamburger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/help/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/help/help_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.667454 joulescope_ui-1.1.0/joulescope_ui/widgets/jls_info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/jls_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/jls_info/jls_info_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/current_offset.png
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/voltage_offset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/memory_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/notes/notes_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/record_status_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/report_issue/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/report_issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/report_issue/report_issue_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24258 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/settings/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/settings/unique_strings_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.671454 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.675454 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.675454 joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/disk_full_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/signal_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.675454 joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/condition_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/active.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/continuous.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/inactive.svg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/searching.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/single.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/trigger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/value/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/value/value_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.679454 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.683454 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/add.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/view_manager_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.683454 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/annotations.md
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/interval_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/line_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/style_defines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/trace.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/text_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_source_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   169445 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/y_range_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/joulescope_ui/zip_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/joulescope_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 21:18:13.000000 joulescope_ui-1.1.0/joulescope_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 21:18:13.687454 joulescope_ui-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-03 21:16:57.000000 joulescope_ui-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-04 01:10:14.000000 joulescope_ui-1.1.1/joulescope.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.334367 joulescope_ui-1.1.1/joulescope_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-04 01:10:04.000000 joulescope_ui-1.1.1/joulescope_ui/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-04 01:10:04.000000 joulescope_ui-1.1.1/joulescope_ui/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/dev_signal_buffer_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.334367 joulescope_ui-1.1.1/joulescope_ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/device_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/devices/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/devices/test/test_device_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/disk_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/entry_points/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/entry_points/zip_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/error_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/expanding_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/filename_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/fonts/DSEG14-Modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/fonts/Hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/fonts/Hack/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/fonts/Lato/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/fonts/SourceSerifPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui/fonts.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/help_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/intel_graphics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/jls_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/jls_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/jls_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/jls_v2_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/json_plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.338367 joulescope_ui-1.1.1/joulescope_ui/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/locale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81002 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   111451 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70795 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   101644 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    97401 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   128233 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70446 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   101226 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72225 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103098 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.342367 joulescope_ui-1.1.1/joulescope_ui/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    74898 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104820 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)    67661 2024-04-04 01:10:05.000000 joulescope_ui-1.1.1/joulescope_ui/locale/joulescope_ui.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    69349 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    99357 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.310367 joulescope_ui-1.1.1/joulescope_ui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    60506 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    90342 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40944 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/mem_leak_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p1/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p1/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.346367 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p2/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/plugins/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/pubsub_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/pubsub_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.350366 joulescope_ui-1.1.1/joulescope_ui/range_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/max_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/plugin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/range_tools/usb_inrush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.350366 joulescope_ui-1.1.1/joulescope_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.354366 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_128x128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_256x256.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_64x64.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-04 01:10:14.000000 joulescope_ui-1.1.1/joulescope_ui/resources.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/safe_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/shift_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/source_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.354366 joulescope_ui-1.1.1/joulescope_ui/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/font_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.362366 joulescope_ui-1.1.1/joulescope_ui/styles/js1/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/branch_vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.362366 joulescope_ui-1.1.1/joulescope_ui/styles/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/system/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.362366 joulescope_ui-1.1.1/joulescope_ui/styles/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/test/test_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/styles/test/test_parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.366366 joulescope_ui-1.1.1/joulescope_ui/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/anno1.anno.jls
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_annotation_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_disk_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_range_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/test/test_versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-04 01:10:06.000000 joulescope_ui-1.1.1/joulescope_ui/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/ui_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widget_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.366366 joulescope_ui-1.1.1/joulescope_ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.366366 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.366366 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.366366 joulescope_ui-1.1.1/joulescope_ui/widgets/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/clock/clock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.370366 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/log_view_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/profile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/publish_spy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.370366 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/current_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_update_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/device_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/device_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/target_power_off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/draggable_list_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/example_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/example/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.374366 joulescope_ui-1.1.1/joulescope_ui/widgets/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/hamburger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/help/help_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/jls_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/jls_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/jls_info/jls_info_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/current_offset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/voltage_offset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/memory_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/notes/notes_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.378366 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.382366 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.382366 joulescope_ui-1.1.1/joulescope_ui/widgets/report_issue/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/report_issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/report_issue/report_issue_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.382366 joulescope_ui-1.1.1/joulescope_ui/widgets/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24258 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/settings/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/settings/unique_strings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.382366 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.386366 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.386366 joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/disk_full_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.386366 joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.386366 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/condition_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/active.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/continuous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/searching.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/single.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/trigger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/value/value_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.390366 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/add.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/view_manager_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.394366 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/annotations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/interval_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/line_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169445 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/y_range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/joulescope_ui/zip_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/joulescope_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-04-04 01:10:16.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 01:10:15.000000 joulescope_ui-1.1.1/joulescope_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 01:10:16.398366 joulescope_ui-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-04 01:09:41.000000 joulescope_ui-1.1.1/setup.py
```

### Comparing `joulescope_ui-1.1.0/CHANGELOG.md` & `joulescope_ui-1.1.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.0
+## 1.1.1
 
 2024 Apr 3
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
 * Added AI translations: ar, de, el, es, fr, ja, ko, zh.
 * Added Intel graphics dialog to display sequence  #245
```

### Comparing `joulescope_ui-1.1.0/CREDITS.html` & `joulescope_ui-1.1.1/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/LICENSE.txt` & `joulescope_ui-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/PKG-INFO` & `joulescope_ui-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.0/README.md` & `joulescope_ui-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope.iss` & `joulescope_ui-1.1.1/joulescope.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Joulescope"
-#define MyAppVersion "1.1.0"
-#define MyAppVersionUnderscores "1_1_0"
+#define MyAppVersion "1.1.1"
+#define MyAppVersionUnderscores "1_1_1"
 #define MyAppPublisher "Jetperch LLC"
 #define MyAppURL "https://www.joulescope.com"
 #define MyAppExeName "joulescope.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application.
 ; Do not use the same AppId value in installers for other applications.
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/CHANGELOG.md` & `joulescope_ui-1.1.1/joulescope_ui/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.0
+## 1.1.1
 
 2024 Apr 3
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
 * Added AI translations: ar, de, el, es, fr, ja, ko, zh.
 * Added Intel graphics dialog to display sequence  #245
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/CREDITS.html` & `joulescope_ui-1.1.1/joulescope_ui/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/__main__.py` & `joulescope_ui-1.1.1/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/about.py` & `joulescope_ui-1.1.1/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/api.py` & `joulescope_ui-1.1.1/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/app.py` & `joulescope_ui-1.1.1/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/capabilities.py` & `joulescope_ui-1.1.1/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.1.1/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/device_update.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220_fuse.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220_fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/js220_updater.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/js220_updater.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/devices/test/test_device_update.py` & `joulescope_ui-1.1.1/joulescope_ui/devices/test/test_device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/disk_monitor.py` & `joulescope_ui-1.1.1/joulescope_ui/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/entry_points/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.1.1/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/entry_points/zip_inspector.py` & `joulescope_ui-1.1.1/joulescope_ui/entry_points/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/error_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/error_window.py` & `joulescope_ui-1.1.1/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/exporter.py` & `joulescope_ui-1.1.1/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/file_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/filename_formatter.py` & `joulescope_ui-1.1.1/joulescope_ui/filename_formatter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.1.1/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.1.1/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.1.1/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.1.1/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.1.1/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/fonts.rcc` & `joulescope_ui-1.1.1/joulescope_ui/fonts.rcc`

 * *Files 3% similar despite different names*

```diff
@@ -193814,70 +193814,70 @@
 002f5150: 0000 0000 0000 0000 0000 0080 0002 0000  ................
 002f5160: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
 002f5170: 0050 0002 0000 000c 0000 001b 0000 0000  .P..............
 002f5180: 0000 0000 0000 0010 0002 0000 0006 0000  ................
 002f5190: 0015 0000 0000 0000 0000 0000 0030 0002  .............0..
 002f51a0: 0000 000e 0000 0007 0000 0000 0000 0000  ................
 002f51b0: 0000 071a 0004 0000 0001 0025 4f27 0000  ...........%O'..
-002f51c0: 018e a5d2 7707 0000 07c4 0004 0000 0001  ....w...........
-002f51d0: 0029 2537 0000 018e a5d2 7703 0000 058c  .)%7......w.....
-002f51e0: 0004 0000 0001 001c 6407 0000 018e a5d2  ........d.......
-002f51f0: 770b 0000 05ba 0004 0000 0001 001d 95a3  w...............
-002f5200: 0000 018e a5d2 7713 0000 0750 0004 0000  ......w....P....
-002f5210: 0001 0026 8517 0000 018e a5d2 7713 0000  ...&........w...
+002f51c0: 018e a6a7 88ba 0000 07c4 0004 0000 0001  ................
+002f51d0: 0029 2537 0000 018e a6a7 88b6 0000 058c  .)%7............
+002f51e0: 0004 0000 0001 001c 6407 0000 018e a6a7  ........d.......
+002f51f0: 88be 0000 05ba 0004 0000 0001 001d 95a3  ................
+002f5200: 0000 018e a6a7 88c6 0000 0750 0004 0000  ...........P....
+002f5210: 0001 0026 8517 0000 018e a6a7 88c6 0000  ...&............
 002f5220: 07fc 0004 0000 0001 002a 5802 0000 018e  .........*X.....
-002f5230: a5d2 7707 0000 082e 0004 0000 0001 002b  ..w............+
-002f5240: c4d1 0000 018e a5d2 770b 0000 062c 0004  ........w....,..
-002f5250: 0000 0001 0020 3160 0000 018e a5d2 770f  ..... 1`......w.
+002f5230: a6a7 88ba 0000 082e 0004 0000 0001 002b  ...............+
+002f5240: c4d1 0000 018e a6a7 88be 0000 062c 0004  .............,..
+002f5250: 0000 0001 0020 3160 0000 018e a6a7 88c2  ..... 1`........
 002f5260: 0000 05f4 0004 0000 0001 001f 01ac 0000  ................
-002f5270: 018e a5d2 770b 0000 078e 0004 0000 0001  ....w...........
-002f5280: 0027 bab6 0000 018e a5d2 770f 0000 0666  .'........w....f
-002f5290: 0004 0000 0001 0021 6449 0000 018e a5d2  .......!dI......
-002f52a0: 7707 0000 06e6 0004 0000 0001 0023 e72d  w............#.-
-002f52b0: 0000 018e a5d2 7703 0000 0862 0004 0000  ......w....b....
-002f52c0: 0001 002d 262d 0000 018e a5d2 770f 0000  ...-&-......w...
+002f5270: 018e a6a7 88c2 0000 078e 0004 0000 0001  ................
+002f5280: 0027 bab6 0000 018e a6a7 88c2 0000 0666  .'.............f
+002f5290: 0004 0000 0001 0021 6449 0000 018e a6a7  .......!dI......
+002f52a0: 88be 0000 06e6 0004 0000 0001 0023 e72d  .............#.-
+002f52b0: 0000 018e a6a7 88b6 0000 0862 0004 0000  ...........b....
+002f52c0: 0001 002d 262d 0000 018e a6a7 88c2 0000  ...-&-..........
 002f52d0: 06a8 0004 0000 0001 0022 8ce5 0000 018e  ........."......
-002f52e0: a5d2 7707 0000 089a 0004 0000 0001 002e  ..w.............
-002f52f0: 90bc 0000 018e a5d2 76f3 0000 08d0 0004  ........v.......
-002f5300: 0000 0001 002e af00 0000 018e a5d2 76f3  ..............v.
+002f52e0: a6a7 88ba 0000 089a 0004 0000 0001 002e  ................
+002f52f0: 90bc 0000 018e a6a7 88aa 0000 08d0 0004  ................
+002f5300: 0000 0001 002e af00 0000 018e a6a7 88aa  ................
 002f5310: 0000 097c 0004 0000 0001 002f 0ab2 0000  ...|......./....
-002f5320: 018e a5d2 76f3 0000 09b0 0004 0000 0001  ....v...........
-002f5330: 002f 293e 0000 018e a5d2 76f3 0000 090c  ./)>......v.....
-002f5340: 0004 0000 0001 002e cd3f 0000 018e a5d2  .........?......
-002f5350: 76f3 0000 094a 0004 0000 0001 002e ec32  v....J.........2
-002f5360: 0000 018e a5d2 76f3 0000 0544 0004 0000  ......v....D....
-002f5370: 0001 001b 3ffe 0000 018e a5d2 771f 0000  ....?.......w...
+002f5320: 018e a6a7 88aa 0000 09b0 0004 0000 0001  ................
+002f5330: 002f 293e 0000 018e a6a7 88aa 0000 090c  ./)>............
+002f5340: 0004 0000 0001 002e cd3f 0000 018e a6a7  .........?......
+002f5350: 88aa 0000 094a 0004 0000 0001 002e ec32  .....J.........2
+002f5360: 0000 018e a6a7 88aa 0000 0544 0004 0000  ...........D....
+002f5370: 0001 001b 3ffe 0000 018e a6a7 88d2 0000  ....?...........
 002f5380: 036a 0004 0000 0001 0010 f545 0000 018e  .j.........E....
-002f5390: a5d2 7717 0000 041a 0004 0000 0001 0014  ..w.............
-002f53a0: f75f 0000 018e a5d2 771b 0000 048c 0004  ._......w.......
-002f53b0: 0000 0001 0017 6f8d 0000 018e a5d2 771b  ......o.......w.
+002f5390: a6a7 88ca 0000 041a 0004 0000 0001 0014  ................
+002f53a0: f75f 0000 018e a6a7 88ce 0000 048c 0004  ._..............
+002f53b0: 0000 0001 0017 6f8d 0000 018e a6a7 88ce  ......o.........
 002f53c0: 0000 04c2 0004 0000 0001 0018 d613 0000  ................
-002f53d0: 018e a5d2 7717 0000 03aa 0004 0000 0001  ....w...........
-002f53e0: 0012 1971 0000 018e a5d2 7717 0000 03de  ...q......w.....
-002f53f0: 0004 0000 0001 0013 8810 0000 018e a5d2  ................
-002f5400: 771f 0000 02dc 0004 0000 0001 000e c39f  w...............
-002f5410: 0000 018e a5d2 771b 0000 0452 0004 0000  ......w....R....
-002f5420: 0001 0016 0ed3 0000 018e a5d2 771f 0000  ............w...
+002f53d0: 018e a6a7 88ca 0000 03aa 0004 0000 0001  ................
+002f53e0: 0012 1971 0000 018e a6a7 88ca 0000 03de  ...q............
+002f53f0: 0004 0000 0001 0013 8810 0000 018e a6a7  ................
+002f5400: 88d2 0000 02dc 0004 0000 0001 000e c39f  ................
+002f5410: 0000 018e a6a7 88ce 0000 0452 0004 0000  ...........R....
+002f5420: 0001 0016 0ed3 0000 018e a6a7 88d2 0000  ................
 002f5430: 0502 0004 0000 0001 001a 2aab 0000 018e  ..........*.....
-002f5440: a5d2 7713 0000 031e 0004 0000 0001 000f  ..w.............
-002f5450: e47b 0000 018e a5d2 7717 0000 02a6 0004  .{......w.......
-002f5460: 0000 0001 000d 65a3 0000 018e a5d2 7713  ......e.......w.
+002f5440: a6a7 88ca 0000 031e 0004 0000 0001 000f  ................
+002f5450: e47b 0000 018e a6a7 88ce 0000 02a6 0004  .{..............
+002f5460: 0000 0001 000d 65a3 0000 018e a6a7 88c6  ......e.........
 002f5470: 0000 01ae 0004 0000 0001 0003 6c6f 0000  ............lo..
-002f5480: 018e a5d2 76ff 0000 008e 0004 0000 0001  ....v...........
-002f5490: 0000 0000 0000 018e a5d2 76ff 0000 018a  ..........v.....
-002f54a0: 0004 0000 0001 0002 e1fa 0000 018e a5d2  ................
-002f54b0: 76ff 0000 010a 0004 0000 0001 0001 72aa  v.............r.
-002f54c0: 0000 018e a5d2 76ff 0000 00e8 0004 0000  ......v.........
-002f54d0: 0001 0000 f2c6 0000 018e a5d2 76ff 0000  ............v...
+002f5480: 018e a6a7 88b2 0000 008e 0004 0000 0001  ................
+002f5490: 0000 0000 0000 018e a6a7 88b2 0000 018a  ................
+002f54a0: 0004 0000 0001 0002 e1fa 0000 018e a6a7  ................
+002f54b0: 88b2 0000 010a 0004 0000 0001 0001 72aa  ..............r.
+002f54c0: 0000 018e a6a7 88b6 0000 00e8 0004 0000  ................
+002f54d0: 0001 0000 f2c6 0000 018e a6a7 88b2 0000  ................
 002f54e0: 015e 0004 0000 0001 0002 7e0b 0000 018e  .^........~.....
-002f54f0: a5d2 76ff 0000 00ba 0004 0000 0001 0000  ..v.............
-002f5500: 8b33 0000 018e a5d2 76ff 0000 01f0 0004  .3......v.......
-002f5510: 0000 0001 0004 74f0 0000 018e a5d2 76ff  ......t.......v.
+002f54f0: a6a7 88b6 0000 00ba 0004 0000 0001 0000  ................
+002f5500: 8b33 0000 018e a6a7 88b2 0000 01f0 0004  .3..............
+002f5510: 0000 0001 0004 74f0 0000 018e a6a7 88b6  ......t.........
 002f5520: 0000 01ce 0004 0000 0001 0003 ee66 0000  .............f..
-002f5530: 018e a5d2 76ff 0000 0130 0004 0000 0001  ....v....0......
-002f5540: 0001 f768 0000 018e a5d2 76ff 0000 0210  ...h......v.....
-002f5550: 0004 0000 0001 0004 f353 0000 018e a5d2  .........S......
-002f5560: 76fb 0000 027a 0004 0000 0001 000b 366d  v....z........6m
-002f5570: 0000 018e a5d2 76fb 0000 0234 0004 0000  ......v....4....
-002f5580: 0001 0007 158f 0000 018e a5d2 76f7 0000  ............v...
+002f5530: 018e a6a7 88b2 0000 0130 0004 0000 0001  .........0......
+002f5540: 0001 f768 0000 018e a6a7 88b2 0000 0210  ...h............
+002f5550: 0004 0000 0001 0004 f353 0000 018e a6a7  .........S......
+002f5560: 88ae 0000 027a 0004 0000 0001 000b 366d  .....z........6m
+002f5570: 0000 018e a6a7 88ae 0000 0234 0004 0000  ...........4....
+002f5580: 0001 0007 158f 0000 018e a6a7 88aa 0000  ................
 002f5590: 0254 0004 0000 0001 0009 2ac5 0000 018e  .T........*.....
-002f55a0: a5d2 76fb                                ..v.
+002f55a0: a6a7 88b2                                ....
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/getting_started.py` & `joulescope_ui-1.1.1/joulescope_ui/getting_started.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/help_ui.py` & `joulescope_ui-1.1.1/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/intel_graphics_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/intel_graphics_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/jls_source.py` & `joulescope_ui-1.1.1/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/jls_v1.py` & `joulescope_ui-1.1.1/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/jls_v2.py` & `joulescope_ui-1.1.1/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/jls_v2_annotations.py` & `joulescope_ui-1.1.1/joulescope_ui/jls_v2_annotations.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/json_plus.py` & `joulescope_ui-1.1.1/joulescope_ui/json_plus.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ar\n"
 "Language-Team: ar <LL@li.org>\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=0 && n%100<=2 ? 4 : 5);\n"
 "MIME-Version: 1.0\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ar <LL@li.org>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: de <LL@li.org>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: el\n"
 "Language-Team: el <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: el <LL@li.org>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: es <LL@li.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: fr <LL@li.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ja <LL@li.org>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/joulescope_ui.pot` & `joulescope_ui-1.1.1/joulescope_ui/locale/joulescope_ui.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Copyright (C) 2024 Jetperch LLC
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT 1.1.0\n"
+"Project-Id-Version: PROJECT 1.1.1\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.14.0\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ko\n"
 "Language-Team: ko <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ko <LL@li.org>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.1/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.1/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-03 16:33-0400\n"
+"POT-Creation-Date: 2024-04-03 18:09-0400\n"
 "PO-Revision-Date: 2024-04-03 14:53-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: zh <LL@li.org>\n"
 "Language: zh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/logging_util.py` & `joulescope_ui-1.1.1/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/main.py` & `joulescope_ui-1.1.1/joulescope_ui/main.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.1.1/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/metadata.py` & `joulescope_ui-1.1.1/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/paths.py` & `joulescope_ui-1.1.1/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/plugins/manager.py` & `joulescope_ui-1.1.1/joulescope_ui/plugins/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,18 +118,19 @@
             if not os.path.isdir(path):
                 os.makedirs(path)
             readme_file = os.path.join(path, 'README.txt')
             if not os.path.isfile(readme_file):
                 with open(readme_file, 'wt') as f:
                     f.write('Default Joulescope UI plugin directory.  Add plugin packages here\n')
             self._paths = [path]
-        for path in reversed(self._paths):
-            sys.path.insert(0, os.path.dirname(os.path.abspath(path)))
+        paths = [os.path.dirname(os.path.abspath(path)) for path in reversed(self._paths)]
+        for path in paths:
+            sys.path.insert(0, path)
         if is_release:
-            os.environ['PYTHONPATH'] = sys.path
+            os.environ['PYTHONPATH'] = os.path.pathsep.join(paths)
         self.pubsub.subscribe(REGISTRY_MANAGER_TOPICS.REGISTRY_ADD, self._on_registry_add)
         self.pubsub.subscribe(REGISTRY_MANAGER_TOPICS.REGISTRY_REMOVE, self._on_registry_remove)
         for item in pkgutil.iter_modules(self._paths):
             if not item.ispkg:
                 continue
             if isinstance(item.module_finder, importlib.machinery.FileFinder):
                 path = item.module_finder.path
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/plugins/selector.py` & `joulescope_ui-1.1.1/joulescope_ui/plugins/selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/plugins/test/plugins/p1/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/plugins/test/plugins/p1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/plugins/test/test_manager.py` & `joulescope_ui-1.1.1/joulescope_ui/plugins/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/process_monitor.py` & `joulescope_ui-1.1.1/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/profile.py` & `joulescope_ui-1.1.1/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/pubsub.py` & `joulescope_ui-1.1.1/joulescope_ui/pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/pubsub_aggregator.py` & `joulescope_ui-1.1.1/joulescope_ui/pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/pubsub_callable.py` & `joulescope_ui-1.1.1/joulescope_ui/pubsub_callable.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/pubsub_proxy.py` & `joulescope_ui-1.1.1/joulescope_ui/pubsub_proxy.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tool.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/cdf.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/frequency.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/histogram.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/max_window.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/plugin_helpers.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/range_tools/usb_inrush.py` & `joulescope_ui-1.1.1/joulescope_ui/range_tools/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/reporter.py` & `joulescope_ui-1.1.1/joulescope_ui/reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/dmg_background@2x.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/dmg_background@2x.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.ico` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_128x128.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_128x128@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_128x128@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_16x16@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_16x16@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_256x256.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_256x256@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_256x256@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_32x32.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_32x32@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_32x32@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_512x512.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_512x512@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_512x512@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_64x64.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icon.iconset/icon_64x64@2.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/icon.iconset/icon_64x64@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.1.1/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/logo-large.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/logo-large.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/logo-small.png` & `joulescope_ui-1.1.1/joulescope_ui/resources/logo-small.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.1.1/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources.py` & `joulescope_ui-1.1.1/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/resources.rcc` & `joulescope_ui-1.1.1/joulescope_ui/resources.rcc`

 * *Files 2% similar despite different names*

```diff
@@ -1416,11 +1416,11 @@
 00005870: 5f00 3600 3400 7800 3600 3400 2e00 6900  _.6.4.x.6.4...i.
 00005880: 6300 6f00 0e03 14ce 8700 6c00 6f00 6700  c.o.......l.o.g.
 00005890: 6f00 2d00 6c00 6100 7200 6700 6500 2e00  o.-.l.a.r.g.e...
 000058a0: 7000 6e00 6700 0e0f ebc7 e700 6c00 6f00  p.n.g.......l.o.
 000058b0: 6700 6f00 2d00 7300 6d00 6100 6c00 6c00  g.o.-.s.m.a.l.l.
 000058c0: 2e00 7000 6e00 6700 0000 0000 0200 0000  ..p.n.g.........
 000058d0: 0300 0000 0100 0000 0000 0000 0000 0000  ................
-000058e0: 2200 0000 0000 0100 0001 9900 0001 8ea5  "...............
-000058f0: d277 2700 0000 0000 0400 0000 0100 0000  .w'.............
-00005900: 0000 0001 8ea5 d277 2700 0000 4400 0000  .......w'...D...
-00005910: 0000 0100 0043 f800 0001 8ea5 d277 27    .....C.......w'
+000058e0: 2200 0000 0000 0100 0001 9900 0001 8ea6  "...............
+000058f0: a788 da00 0000 0000 0400 0000 0100 0000  ................
+00005900: 0000 0001 8ea6 a788 da00 0000 4400 0000  ............D...
+00005910: 0000 0100 0043 f800 0001 8ea6 a788 da    .....C.........
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui/safe_mode.py` & `joulescope_ui-1.1.1/joulescope_ui/safe_mode.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/sanitize.py` & `joulescope_ui-1.1.1/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/shift_key.py` & `joulescope_ui-1.1.1/joulescope_ui/shift_key.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/shortcuts.py` & `joulescope_ui-1.1.1/joulescope_ui/shortcuts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/software_update.py` & `joulescope_ui-1.1.1/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/source_selector.py` & `joulescope_ui-1.1.1/joulescope_ui/source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/README.md` & `joulescope_ui-1.1.1/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.1.1/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.1.1/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.1.1/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.1.1/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.1.1/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/manager.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.1.1/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.1.1/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/anno1.anno.jls` & `joulescope_ui-1.1.1/joulescope_ui/test/anno1.anno.jls`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_annotation_load.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_annotation_load.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_disk_monitor.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub_aggregator.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_reporter.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_source_selector.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_units.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/test/test_versioned_file.py` & `joulescope_ui-1.1.1/joulescope_ui/test/test_versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/time_map.py` & `joulescope_ui-1.1.1/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/tokens.py` & `joulescope_ui-1.1.1/joulescope_ui/tokens.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/tooltip.py` & `joulescope_ui-1.1.1/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/ui_util.py` & `joulescope_ui-1.1.1/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/units.py` & `joulescope_ui-1.1.1/joulescope_ui/units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/urls.py` & `joulescope_ui-1.1.1/joulescope_ui/urls.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/versioned_file.py` & `joulescope_ui-1.1.1/joulescope_ui/versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/view.py` & `joulescope_ui-1.1.1/joulescope_ui/view.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widget_tools.py` & `joulescope_ui-1.1.1/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/clock/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/clock/clock_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/clock/clock_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/developer/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/developer/log_view_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/developer/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/developer/profile_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/developer/profile_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/developer/publish_spy_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/developer/publish_spy_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/developer/pubsub_explorer_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/developer/pubsub_explorer_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/current_limits.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/current_limits.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/device_update_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/device_update_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/fuse.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/device_open.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/device_open.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/fuse_normal.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/double_slider.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/double_slider.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/draggable_list_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/draggable_list_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/jls_info/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/jls_info/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/jls_info/jls_info_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/jls_info/jls_info_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/current_offset.png` & `joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/current_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/js220_cal_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/js220_cal_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/js220_cal/voltage_offset.png` & `joulescope_ui-1.1.1/joulescope_ui/widgets/js220_cal/voltage_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/memory/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/memory/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/notes/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/notes/notes_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/notes/notes_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/record_status_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/record_status_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/index.json` & `joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/record_status/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/record_status/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/report_issue/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/report_issue/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/report_issue/report_issue_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/report_issue/report_issue_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/settings/unique_strings_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/settings/unique_strings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/disk_full_dialog.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/disk_full_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/condition_detector.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/condition_detector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/continuous.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/continuous.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/index.json` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/searching.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/searching.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_const.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_const.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_duration.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/test/test_edge.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/test/test_edge.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/trigger/trigger_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/trigger/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/value/value_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/view_manager/view_manager_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/view_manager/view_manager_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/annotations.md` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/annotations.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/axis_ticks.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/interval_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/interval_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/quantities.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/test_axis_ticks.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/test_axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/test/test_quantities.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/test/test_quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/text_annotation.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/text_annotation.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_source_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_source_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/widgets/waveform/y_range_widget.py` & `joulescope_ui-1.1.1/joulescope_ui/widgets/waveform/y_range_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui/zip_inspector.py` & `joulescope_ui-1.1.1/joulescope_ui/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.1.1/joulescope_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.0/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.1.1/joulescope_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/pyproject.toml` & `joulescope_ui-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.0/setup.py` & `joulescope_ui-1.1.1/setup.py`

 * *Files identical despite different names*

