# Comparing `tmp/viaconstructor-0.6.6.tar.gz` & `tmp/viaconstructor-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viaconstructor-0.6.6.tar", last modified: Mon Apr  1 19:41:55 2024, max compression
+gzip compressed data, was "viaconstructor-0.6.7.tar", last modified: Thu Apr  4 15:56:18 2024, max compression
```

## Comparing `viaconstructor-0.6.6.tar` & `viaconstructor-0.6.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/
--rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3885 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.677492 viaconstructor-0.6.6/bin/
--rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/bin/dxfpreview
--rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/bin/gcodepreview
--rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.6/bin/viaconstructor
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.677492 viaconstructor-0.6.6/dxfpreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/dxfpreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/dxfpreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     4131 2022-08-22 19:23:27.000000 viaconstructor-0.6.6/dxfpreview/dxfpreview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.678492 viaconstructor-0.6.6/gcodepreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/gcodepreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/gcodepreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     3630 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/gcodepreview/gcodepreview.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1232 2024-04-01 19:41:02.000000 viaconstructor-0.6.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.680492 viaconstructor-0.6.6/viaconstructor/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/viaconstructor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/viaconstructor/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)    50759 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/calc.py
--rwxr-xr-x   0 root         (0) root         (0)    24883 2023-04-02 20:48:58.000000 viaconstructor-0.6.6/viaconstructor/draw2d.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/dxfcolors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.675492 viaconstructor-0.6.6/viaconstructor/ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/
--rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/HersheyFonts.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/
--rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/cavaliercontours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.683492 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/
--rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
--rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.684491 viaconstructor-0.6.6/viaconstructor/ext/meshcut/
--rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.6/viaconstructor/ext/meshcut/meshcut.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.685492 viaconstructor-0.6.6/viaconstructor/ext/stl/
--rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/__about__.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/base.py
--rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/main.py
--rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/mesh.py
--rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/stl.py
--rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.687492 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/
--rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/bezier.py
--rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/document.py
--rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/misctools.py
--rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/parser.py
--rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/path.py
--rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/paths2svg.py
--rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/polytools.py
--rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/smoothing.py
--rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_io_sax.py
--rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_to_paths.py
--rwxr-xr-x   0 root         (0) root         (0)    53077 2023-04-11 15:48:53.000000 viaconstructor-0.6.6/viaconstructor/gldraw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.691491 viaconstructor-0.6.6/viaconstructor/icons/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.6/viaconstructor/icons/camotics.png
--rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/delete.png
--rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/exit.png
--rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/flip-x.png
--rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/flip-y.png
--rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.6/viaconstructor/icons/fonts.png
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/icons/gears.png
--rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-setup-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-setup.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-tooltable.png
--rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.6/viaconstructor/icons/nesting.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/open.png
--rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.6/viaconstructor/icons/openscad.png
--rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.6/viaconstructor/icons/pause.png
--rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.6/viaconstructor/icons/play.png
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.6/viaconstructor/icons/redraw.png
--rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/repair.png
--rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/rotate.png
--rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-setup-as.png
--rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-setup.png
--rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-tooltable.png
--rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save.png
--rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/scale.png
--rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.6/viaconstructor/icons/select.png
--rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/start.png
--rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.6/viaconstructor/icons/stop.png
--rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/tab-selector.png
--rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/view-2d.png
--rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/view-reset.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.692492 viaconstructor-0.6.6/viaconstructor/input_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/brdread.py
--rwxr-xr-x   0 root         (0) root         (0)    26370 2023-04-14 11:57:42.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/dxfread.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/hpglread.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/imgread.py
--rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/stlread.py
--rwxr-xr-x   0 root         (0) root         (0)    10642 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/svgread.py
--rw-r--r--   0 root         (0) root         (0)     9352 2024-01-09 19:28:37.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/ttfread.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/input_plugins_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.676492 viaconstructor-0.6.6/viaconstructor/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.676492 viaconstructor-0.6.6/viaconstructor/locales/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.693492 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.po
--rwxr-xr-x   0 root         (0) root         (0)    44035 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/machine_cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.693492 viaconstructor-0.6.6/viaconstructor/output_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-04-08 21:07:42.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_grbl.py
--rw-r--r--   0 root         (0) root         (0)    10647 2023-04-08 21:07:27.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_linuxcnc.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-04-08 21:06:43.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/hpgl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/viaconstructor/preview_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10939 2023-04-11 15:48:53.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/gcode.py
--rw-r--r--   0 root         (0) root         (0)     9321 2023-04-02 20:48:58.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/hpgl.py
--rwxr-xr-x   0 root         (0) root         (0)    22521 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/setupdefaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/viaconstructor/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9012 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/tools/font.py
--rw-r--r--   0 root         (0) root         (0)     8791 2024-04-01 19:39:59.000000 viaconstructor-0.6.6/viaconstructor/tools/gear.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.6/viaconstructor/vc_types.py
--rwxr-xr-x   0 root         (0) root         (0)   126674 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/viaconstructor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3885 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3690 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/
+-rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.333472 viaconstructor-0.6.7/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/bin/dxfpreview
+-rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/bin/gcodepreview
+-rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.7/bin/viaconstructor
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.333472 viaconstructor-0.6.7/dxfpreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/dxfpreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/dxfpreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4087 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/dxfpreview/dxfpreview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.334472 viaconstructor-0.6.7/gcodepreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/gcodepreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/gcodepreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3564 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/gcodepreview/gcodepreview.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1232 2024-04-04 15:55:51.000000 viaconstructor-0.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.336472 viaconstructor-0.6.7/viaconstructor/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/viaconstructor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/viaconstructor/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)    50043 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/calc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24211 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/draw2d.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.7/viaconstructor/dxfcolors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.331472 viaconstructor-0.6.7/viaconstructor/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.337472 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/
+-rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/HersheyFonts.py
+-rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.337472 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/
+-rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/cavaliercontours.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.338472 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/
+-rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
+-rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.340472 viaconstructor-0.6.7/viaconstructor/ext/meshcut/
+-rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.7/viaconstructor/ext/meshcut/meshcut.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.341472 viaconstructor-0.6.7/viaconstructor/ext/stl/
+-rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/__about__.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/base.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/main.py
+-rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/stl.py
+-rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.343472 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/bezier.py
+-rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/document.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/misctools.py
+-rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/parser.py
+-rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/path.py
+-rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/paths2svg.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/polytools.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/smoothing.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_to_paths.py
+-rwxr-xr-x   0 root         (0) root         (0)    51945 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/gldraw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.347472 viaconstructor-0.6.7/viaconstructor/icons/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.7/viaconstructor/icons/camotics.png
+-rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/delete.png
+-rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/exit.png
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/flip-x.png
+-rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/flip-y.png
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.7/viaconstructor/icons/fonts.png
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/icons/gears.png
+-rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-setup-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-setup.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.7/viaconstructor/icons/nesting.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/open.png
+-rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.7/viaconstructor/icons/openscad.png
+-rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.7/viaconstructor/icons/pause.png
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.7/viaconstructor/icons/play.png
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.7/viaconstructor/icons/redraw.png
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/repair.png
+-rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/rotate.png
+-rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-setup-as.png
+-rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-setup.png
+-rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save.png
+-rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/scale.png
+-rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.7/viaconstructor/icons/select.png
+-rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/start.png
+-rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.7/viaconstructor/icons/stop.png
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/tab-selector.png
+-rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/view-2d.png
+-rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/view-reset.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.348472 viaconstructor-0.6.7/viaconstructor/input_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/brdread.py
+-rwxr-xr-x   0 root         (0) root         (0)    25832 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/dxfread.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/hpglread.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/imgread.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/stlread.py
+-rwxr-xr-x   0 root         (0) root         (0)    10584 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/svgread.py
+-rw-r--r--   0 root         (0) root         (0)     9336 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/ttfread.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.331472 viaconstructor-0.6.7/viaconstructor/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.332472 viaconstructor-0.6.7/viaconstructor/locales/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.348472 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.po
+-rwxr-xr-x   0 root         (0) root         (0)    39246 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/machine_cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.349472 viaconstructor-0.6.7/viaconstructor/output_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10849 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_grbl.py
+-rw-r--r--   0 root         (0) root         (0)    11015 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_linuxcnc.py
+-rw-r--r--   0 root         (0) root         (0)     7376 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/hpgl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.349472 viaconstructor-0.6.7/viaconstructor/preview_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10745 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/gcode.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/hpgl.py
+-rwxr-xr-x   0 root         (0) root         (0)    22882 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/setupdefaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/viaconstructor/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8970 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/tools/font.py
+-rw-r--r--   0 root         (0) root         (0)     8709 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/tools/gear.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.7/viaconstructor/vc_types.py
+-rwxr-xr-x   0 root         (0) root         (0)   122156 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/viaconstructor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.336472 viaconstructor-0.6.7/viaconstructor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-04 15:56:18.000000 viaconstructor-0.6.7/viaconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/top_level.txt
```

### Comparing `viaconstructor-0.6.6/LICENSE` & `viaconstructor-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/PKG-INFO` & `viaconstructor-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.6
+Version: 0.6.7
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.6/README.md` & `viaconstructor-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/dxfpreview/dxfpreview.py` & `viaconstructor-0.6.7/dxfpreview/dxfpreview.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from os import environ
 
 from PIL import Image, ImageDraw, ImageFont
 
 reader_plugins: dict = {}
 for reader in ("dxfread", "hpglread", "stlread", "svgread", "ttfread"):
     try:
-        drawing_reader = importlib.import_module(
-            f".{reader}", "viaconstructor.input_plugins"
-        )
+        drawing_reader = importlib.import_module(f".{reader}", "viaconstructor.input_plugins")
         reader_plugins[reader] = drawing_reader.DrawReader
     except Exception as reader_error:  # pylint: disable=W0703
         print(f"ERRO while loading input plugin {reader}: {reader_error}")
 
 
 def main() -> int:
     """main function."""
@@ -108,17 +106,15 @@
         environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
         import pygame  # pylint: disable=C0415
         from pygame.locals import QUIT  # pylint: disable=C0415,E0611
 
         pygame.init()  # pylint: disable=E1101
         pygame.display.set_caption(f"dxfpreview ({filename})")
         screen = pygame.display.set_mode((screen_width, screen_height))
-        screen.blit(
-            pygame.image.fromstring(out.tobytes(), out.size, out.mode).convert(), (0, 0)
-        )
+        screen.blit(pygame.image.fromstring(out.tobytes(), out.size, out.mode).convert(), (0, 0))
         pygame.display.flip()
         while True:
             for events in pygame.event.get():
                 if events.type == QUIT:
                     return 0
 
     return 0
```

### Comparing `viaconstructor-0.6.6/gcodepreview/gcodepreview.py` & `viaconstructor-0.6.7/gcodepreview/gcodepreview.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,17 @@
     # init output
     out = Image.new("RGB", (screen_width, screen_height), screen_color)
     fnt = ImageFont.truetype("FreeMono.ttf", 24)
     draw = ImageDraw.Draw(out)
 
     # draw grid
     for pos_x in range(0, int(size[0]), 10):
-        draw_line(
-            {"X": pos_x, "Y": 0.0}, {"X": pos_x, "Y": size[1]}, color=(27, 27, 27)
-        )
+        draw_line({"X": pos_x, "Y": 0.0}, {"X": pos_x, "Y": size[1]}, color=(27, 27, 27))
     for pos_y in range(0, int(size[1]), 10):
-        draw_line(
-            {"X": 0.0, "Y": pos_y}, {"X": size[0], "Y": pos_y}, color=(27, 27, 27)
-        )
+        draw_line({"X": 0.0, "Y": pos_y}, {"X": size[0], "Y": pos_y}, color=(27, 27, 27))
 
     # draw path
     gcode_parser.draw(draw_line)
 
     # draw info
     if screen_width >= 320 or screen_height >= 240:
         info = f"W={round(size[0], 2)}\nH={round(size[1], 2)}\nminZ={minmax[2]}"
@@ -96,17 +92,15 @@
         environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
         import pygame  # pylint: disable=C0415
         from pygame.locals import QUIT  # pylint: disable=C0415,E0611
 
         pygame.init()  # pylint: disable=E1101
         pygame.display.set_caption(f"gcodepreview ({filename})")
         screen = pygame.display.set_mode((screen_width, screen_height))
-        screen.blit(
-            pygame.image.fromstring(out.tobytes(), out.size, out.mode).convert(), (0, 0)
-        )
+        screen.blit(pygame.image.fromstring(out.tobytes(), out.size, out.mode).convert(), (0, 0))
         pygame.display.flip()
         while True:
             for events in pygame.event.get():
                 if events.type == QUIT:
                     return 0
 
     return 0
```

### Comparing `viaconstructor-0.6.6/setup.py` & `viaconstructor-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from setuptools import setup
 
 
 setup(
     name='viaconstructor',
-    version='0.6.6',
+    version='0.6.7',
     author='Oliver Dippel',
     author_email='o.dippel@gmx.de',
     packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'viaconstructor.tools', 'gcodepreview', 'dxfpreview'],
     package_data={'viaconstructor.ext.cavaliercontours': ['lib/libCavalierContours.x86_64-linux.so'], 'viaconstructor/ext/nest2D': ['nest2D.cpython-39-x86_64-linux-gnu.so']},
     scripts=['bin/viaconstructor','bin/gcodepreview','bin/dxfpreview'],
     url='https://github.com/multigcs/viaconstructor',
     license='LICENSE',
```

### Comparing `viaconstructor-0.6.6/viaconstructor/calc.py` & `viaconstructor-0.6.7/viaconstructor/calc.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,17 +197,15 @@
 def calc_distance3d(p_1, p_2):
     """gets the distance between two points in 3D."""
     return math.hypot(p_1[0] - p_2[0], p_1[1] - p_2[1], p_1[2] - p_2[2])
 
 
 def is_between(p_1, p_2, p_3):
     """checks if a point is between 2 other points."""
-    return round(math.hypot(p_1[0] - p_3[0], p_1[1] - p_3[1]), 2) + round(
-        math.hypot(p_1[0] - p_2[0], p_1[1] - p_2[1]), 2
-    ) == round(math.hypot(p_2[0] - p_3[0], p_2[1] - p_3[1]), 2)
+    return round(math.hypot(p_1[0] - p_3[0], p_1[1] - p_3[1]), 2) + round(math.hypot(p_1[0] - p_2[0], p_1[1] - p_2[1]), 2) == round(math.hypot(p_2[0] - p_3[0], p_2[1] - p_3[1]), 2)
 
 
 def line_center_2d(p_1, p_2):
     """gets the center point between 2 points in 2D."""
     center_x = (p_1[0] + p_2[0]) / 2
     center_y = (p_1[1] + p_2[1]) / 2
     return (center_x, center_y)
@@ -240,20 +238,16 @@
         dtheta -= TWO_PI
     while dtheta < -math.pi:
         dtheta += TWO_PI
     return dtheta
 
 
 def quadratic_bezier(curv_pos, points):
-    curve_x = (1 - curv_pos) * (
-        (1 - curv_pos) * points[0][0] + curv_pos * points[1][0]
-    ) + curv_pos * ((1 - curv_pos) * points[1][0] + curv_pos * points[2][0])
-    curve_y = (1 - curv_pos) * (
-        (1 - curv_pos) * points[0][1] + curv_pos * points[1][1]
-    ) + curv_pos * ((1 - curv_pos) * points[1][1] + curv_pos * points[2][1])
+    curve_x = (1 - curv_pos) * ((1 - curv_pos) * points[0][0] + curv_pos * points[1][0]) + curv_pos * ((1 - curv_pos) * points[1][0] + curv_pos * points[2][0])
+    curve_y = (1 - curv_pos) * ((1 - curv_pos) * points[0][1] + curv_pos * points[1][1]) + curv_pos * ((1 - curv_pos) * points[1][1] + curv_pos * points[2][1])
     return curve_x, curve_y
 
 
 def point_of_line(p_1, p_2, line_pos):
     return [
         p_1[0] + (p_2[0] - p_1[0]) * line_pos,
         p_1[1] + (p_2[1] - p_1[1]) * line_pos,
@@ -503,19 +497,15 @@
             max_x = obj.segments[0].start[0]
             max_y = obj.segments[0].start[1]
             for segment in obj.segments:
                 min_x = min(min_x, segment.start[0], segment.end[0])
                 min_y = min(min_y, segment.start[1], segment.end[1])
                 max_x = max(max_x, segment.start[0], segment.end[0])
                 max_y = max(max_y, segment.start[1], segment.end[1])
-            uid = hashlib.md5(
-                f"{int(min_x * 100)}_{int(min_y * 100)}_{int(max_x * 100)}_{int(max_y * 100)}".encode(
-                    "utf-8"
-                )
-            ).hexdigest()
+            uid = hashlib.md5(f"{int(min_x * 100)}_{int(min_y * 100)}_{int(max_x * 100)}_{int(max_y * 100)}".encode("utf-8")).hexdigest()
             obj_uid = f"{obj_idx}:{uid}"
 
             objects[obj_uid] = obj
             obj_idx += 1
             last = None
 
         if not found:
@@ -539,17 +529,15 @@
     """checks if a point is inside an polygon in vertex format."""
     angle = 0.0
     start_x = vertex_data[0][-1]
     start_y = vertex_data[1][-1]
     point_0 = point[0]
     point_1 = point[1]
     for end_x, end_y in zip(vertex_data[0], vertex_data[1]):
-        angle += angle_2d(
-            (start_x - point_0, start_y - point_1), (end_x - point_0, end_y - point_1)
-        )
+        angle += angle_2d((start_x - point_0, start_y - point_1), (end_x - point_0, end_y - point_1))
         start_x = end_x
         start_y = end_y
     return bool(abs(angle) >= math.pi)
 
 
 def bulge_points(start, end, bulge, parts=10):
     points = []
@@ -577,17 +565,15 @@
     points = []
 
     if no_bulge:
         if interpolate > 0:
             last_x = vertex_data[0][-1]
             last_y = vertex_data[1][-1]
             last_b = vertex_data[2][-1]
-            for pos_x, pos_y, bulge in zip(
-                vertex_data[0], vertex_data[1], vertex_data[2]
-            ):
+            for pos_x, pos_y, bulge in zip(vertex_data[0], vertex_data[1], vertex_data[2]):
                 if last_b > 0.0:
                     points += bulge_points(
                         (last_x * scale, last_y * scale),
                         (pos_x * scale, pos_y * scale),
                         last_b,
                         interpolate,
                     )
@@ -687,17 +673,15 @@
             ):
                 inter = lines_intersect(check[0], check[1], segment.start, segment.end)
                 if inter:
                     length = calc_distance(segment.start, segment.end)
                     if length > 0.0:
                         if bulge != 0.0:
 
-                            inter = get_half_bulge_point(
-                                (last_x, last_y), (pos_x, pos_y), bulge
-                            )
+                            inter = get_half_bulge_point((last_x, last_y), (pos_x, pos_y), bulge)
 
                         return (obj_idx, segment_idx, inter)
     return ()
 
 
 def found_next_segment_point(mpos, objects):
     nearest = ()
@@ -764,34 +748,30 @@
             last_x = vertex_data[0][-1]
             last_y = vertex_data[1][-1]
             last_bulge = vertex_data[2][-1]
         else:
             last_x = None
             last_y = None
             last_bulge = None
-        for pos_x, pos_y, next_bulge in zip(
-            vertex_data[0], vertex_data[1], vertex_data[2]
-        ):
+        for pos_x, pos_y, next_bulge in zip(vertex_data[0], vertex_data[1], vertex_data[2]):
             if last_x is not None:
                 line_start = (last_x, last_y)
                 line_end = (pos_x, pos_y)
                 for check in (
                     ((mpos[0] - 5, mpos[1] - 5), (mpos[0] + 5, mpos[1] + 5)),
                     ((mpos[0] + 5, mpos[1] - 5), (mpos[0] - 5, mpos[1] + 5)),
                     ((mpos[0] - 5, mpos[1]), (mpos[0] + 5, mpos[1])),
                 ):
                     inter = lines_intersect(check[0], check[1], line_start, line_end)
                     if inter:
                         length = calc_distance(line_start, line_end)
                         if length > offset.setup["tabs"]["width"]:
                             angle = angle_of_line((last_x, last_y), (pos_x, pos_y))
                             if last_bulge != 0.0:
-                                inter = get_half_bulge_point(
-                                    (last_x, last_y), (pos_x, pos_y), last_bulge
-                                )
+                                inter = get_half_bulge_point((last_x, last_y), (pos_x, pos_y), last_bulge)
 
                             start_x = inter[0] + 3 * math.sin(angle)
                             start_y = inter[1] - 3 * math.cos(angle)
                             end_x = inter[0] - 3 * math.sin(angle)
                             end_y = inter[1] + 3 * math.cos(angle)
                             return (start_x, start_y), (end_x, end_y)
 
@@ -852,34 +832,28 @@
 
         points_check = [points]
         if obj.inner_objects and obj.setup["pockets"]["islands"]:
             for idx in obj.inner_objects:
                 polyline_offset = polyline_offsets.get(f"{idx}.0")
                 if polyline_offset is not None:
                     vertex_data = vertex_data_cache(polyline_offset)
-                    points_check.append(
-                        vertex2points(
-                            vertex_data, no_bulge=True, interpolate=interpolate
-                        )
-                    )
+                    points_check.append(vertex2points(vertex_data, no_bulge=True, interpolate=interpolate))
 
         # get bounding box
         bounding = points_to_boundingbox(points)
         y_pos = bounding[1] + abs_tool_radius
         bounding_ydiff = bounding[3] - bounding[1]
         steps_y = int(bounding_ydiff / abs_tool_radius) - 1
         abs_tool_radius = bounding_ydiff / steps_y
         while y_pos <= bounding[3] - abs_tool_radius:
             intersects = set()
             for points in points_check:
                 last = points[-1]
                 for point in points:
-                    intersect = lines_intersect(
-                        (bounding[0] - 1, y_pos), (bounding[2] + 1, y_pos), last, point
-                    )
+                    intersect = lines_intersect((bounding[0] - 1, y_pos), (bounding[2] + 1, y_pos), last, point)
                     if intersect is not None:
                         intersects.add(intersect[0])
                     last = point
             if len(intersects) > 1:
                 sortet_list = sorted(intersects, key=float)
                 point_inter = iter(sortet_list)
                 for point_x1, point_x2 in zip(point_inter, point_inter):
@@ -887,17 +861,15 @@
                         (
                             (point_x1 + abs_tool_radius * 0.6, y_pos),
                             (point_x2 - abs_tool_radius * 0.6, y_pos),
                         )
                     )
             y_pos += abs_tool_radius
 
-        output_lines = lines_to_path(
-            lines, max_vdist=abs_tool_radius * 2, max_dist=abs_tool_radius * 2
-        )
+        output_lines = lines_to_path(lines, max_vdist=abs_tool_radius * 2, max_dist=abs_tool_radius * 2)
         if output_lines:
             last = output_lines[0]
             polyline = []
             polyline.append(last[0])
             polyline.append(last[1])
             for line in output_lines[1:]:
                 if last[1] != line[0]:
@@ -930,31 +902,27 @@
                 is_pocket=2,
                 parent_id=parent_id,
             )
             pocket_idx += 1
     elif HAVE_PYCLIPPER and obj.inner_objects and obj.setup["pockets"]["islands"]:
         subjs = []
         vertex_data = vertex_data_cache(polyline)
-        points = vertex2points(
-            vertex_data, no_bulge=True, scale=1000.0, interpolate=interpolate
-        )
+        points = vertex2points(vertex_data, no_bulge=True, scale=1000.0, interpolate=interpolate)
         pco = pyclipper.PyclipperOffset()  # pylint: disable=E1101
         pco.AddPath(
             points,
             pyclipper.JT_ROUND,  # pylint: disable=E1101
             pyclipper.ET_CLOSEDPOLYGON,  # pylint: disable=E1101
         )
         level = len(obj.outer_objects)
         for idx in obj.inner_objects:
             polyline_offset = polyline_offsets.get(f"{idx}.0")
             if polyline_offset and polyline_offset.level == level + 1:
                 vertex_data = vertex_data_cache(polyline_offset)
-                points = vertex2points(
-                    vertex_data, no_bulge=True, scale=1000.0, interpolate=interpolate
-                )
+                points = vertex2points(vertex_data, no_bulge=True, scale=1000.0, interpolate=interpolate)
                 pco.AddPath(
                     points,
                     pyclipper.JT_ROUND,  # pylint: disable=E1101
                     pyclipper.ET_CLOSEDPOLYGON,  # pylint: disable=E1101
                 )
         subjs = pco.Execute(-abs_tool_radius * 1000)
 
@@ -1064,17 +1032,15 @@
                         offset_idx,
                         vertex_data_org,
                         parent_id,
                     )
     return offset_idx
 
 
-def object2polyline_offsets(
-    diameter, obj, obj_idx, max_outer, polyline_offsets, small_circles=False
-):
+def object2polyline_offsets(diameter, obj, obj_idx, max_outer, polyline_offsets, small_circles=False):
     """calculates the offset line(s) of one object"""
 
     new_polyline_offsets = {}
 
     def overcut() -> None:
         quarter_pi = math.pi / 4
         radius_3 = abs(tool_radius * 3)
@@ -1186,17 +1152,15 @@
 
     vertex_data = object2vertex(obj)
     polyline = cavc.Polyline(vertex_data, is_closed=obj.closed)
     polyline.cache = vertex_data
 
     offset_idx = 0
     if polyline.is_closed() and tool_offset != "none":
-        polyline_offset_list = polyline.parallel_offset(
-            delta=tool_radius, check_self_intersect=True
-        )
+        polyline_offset_list = polyline.parallel_offset(delta=tool_radius, check_self_intersect=True)
         if polyline_offset_list:
             for polyline_offset in polyline_offset_list:
                 vertex_data = polyline_offset.vertex_data()
                 polyline_offset.cache = vertex_data
                 polyline_offset.level = len(obj.outer_objects)
                 polyline_offset.start = obj.start
                 polyline_offset.tool_offset = tool_offset
@@ -1309,17 +1273,15 @@
 
             if obj_copy["setup"]["mill"]["reverse"]:
                 do_reverse = 1 - do_reverse
 
             if do_reverse:
                 reverse_object(obj_copy)
 
-            object2polyline_offsets(
-                diameter, obj_copy, obj_idx, max_outer, polyline_offsets, small_circles
-            )
+            object2polyline_offsets(diameter, obj_copy, obj_idx, max_outer, polyline_offsets, small_circles)
 
     print("")
     return polyline_offsets
 
 
 # analyze size
 def objects2minmax(objects):
@@ -1342,40 +1304,26 @@
             max_x = max(max_x, segment.start[0])
             max_x = max(max_x, segment.end[0])
             max_y = max(max_y, segment.start[1])
             max_y = max(max_y, segment.end[1])
     return (min_x, min_y, max_x, max_y)
 
 
-def rotate_point(
-    origin_x: float, origin_y: float, point_x: float, point_y: float, angle: float
-) -> tuple:
-    new_x = (
-        origin_x
-        + math.cos(angle) * (point_x - origin_x)
-        - math.sin(angle) * (point_y - origin_y)
-    )
-    new_y = (
-        origin_y
-        + math.sin(angle) * (point_x - origin_x)
-        + math.cos(angle) * (point_y - origin_y)
-    )
+def rotate_point(origin_x: float, origin_y: float, point_x: float, point_y: float, angle: float) -> tuple:
+    new_x = origin_x + math.cos(angle) * (point_x - origin_x) - math.sin(angle) * (point_y - origin_y)
+    new_y = origin_y + math.sin(angle) * (point_x - origin_x) + math.cos(angle) * (point_y - origin_y)
     return (new_x, new_y)
 
 
-def rotate_object(
-    obj: VcObject, origin_x: float, origin_y: float, angle: float
-) -> None:
+def rotate_object(obj: VcObject, origin_x: float, origin_y: float, angle: float) -> None:
     """rotates an object"""
     for segment in obj.segments:
         for ptype in ("start", "end", "center"):
             if ptype in segment:
-                segment[ptype] = rotate_point(
-                    origin_x, origin_y, segment[ptype][0], segment[ptype][1], angle
-                )
+                segment[ptype] = rotate_point(origin_x, origin_y, segment[ptype][0], segment[ptype][1], angle)
 
 
 def move_object(obj: VcObject, xoff: float, yoff: float) -> None:
     """moves an object"""
     for segment in obj.segments:
         for ptype in ("start", "end", "center"):
             if ptype in segment:
```

### Comparing `viaconstructor-0.6.6/viaconstructor/draw2d.py` & `viaconstructor-0.6.7/viaconstructor/draw2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,15 @@
                 self.update()
             elif self.mbutton == 2:
                 if self.selector_mode == "tab":
                     sel_idx = -1
                     sel_dist = -1
                     for tab_idx, tab in enumerate(self.project["tabs"]["data"]):
                         tab_pos = line_center_2d(tab[0], tab[1])
-                        dist = calc_distance(
-                            (self.mouse_pos_x, self.mouse_pos_y), tab_pos
-                        )
+                        dist = calc_distance((self.mouse_pos_x, self.mouse_pos_y), tab_pos)
                         if sel_dist < 0 or dist < sel_dist:
                             sel_dist = dist
                             sel_idx = tab_idx
 
                     if 0.0 < sel_dist < 10.0:
                         del self.project["tabs"]["data"][sel_idx]
                         self.update_drawing()
@@ -187,81 +185,44 @@
         self.mpos = None
         draw_all(self.project)
 
     def mouse_pos_to_real_pos(self, mouse_pos) -> tuple:
         min_max = self.project["minMax"]
         mouse_pos_x = mouse_pos.x()
         mouse_pos_y = self.screen_h - mouse_pos.y()
-        real_pos_x = (
-            (
-                (mouse_pos_x / self.screen_w - 0.5 + self.trans_x)
-                / painter["scale"]
-                / painter["scale_xyz"]
-            )
-            + (self.size_x / 2)
-            + min_max[0]
-        )
-        real_pos_y = (
-            (
-                (mouse_pos_y / self.screen_h - 0.5 + self.trans_y)
-                / painter["scale"]
-                / painter["scale_xyz"]
-                * self.aspect
-            )
-            + (self.size_y / 2)
-            + min_max[1]
-        )
+        real_pos_x = ((mouse_pos_x / self.screen_w - 0.5 + self.trans_x) / painter["scale"] / painter["scale_xyz"]) + (self.size_x / 2) + min_max[0]
+        real_pos_y = ((mouse_pos_y / self.screen_h - 0.5 + self.trans_y) / painter["scale"] / painter["scale_xyz"] * self.aspect) + (self.size_y / 2) + min_max[1]
         return (real_pos_x, real_pos_y)
 
     def mouseMoveEvent(self, event) -> None:  # pylint: disable=C0103
         """mouse moved."""
         if self.mbutton == 1:
             moffset = self.mpos - event.pos()
             self.trans_x = self.trans_x_last + moffset.x() / self.screen_w
             self.trans_y = self.trans_y_last - moffset.y() / self.screen_h * self.aspect
             draw_all(self.project)
         elif self.selector_mode == "tab":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_tab_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["offsets"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_tab_point((self.mouse_pos_x, self.mouse_pos_y), self.project["offsets"])
             draw_all(self.project)
         elif self.selector_mode == "start":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_point_on_segment(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_point_on_segment((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
             draw_all(self.project)
         elif self.selector_mode == "delete":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
             draw_all(self.project)
         elif self.selector_mode == "oselect":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
             draw_all(self.project)
         elif self.selector_mode == "repair":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_open_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_open_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
             if self.selection:
                 selection_end = found_next_open_segment_point(
                     (self.mouse_pos_x, self.mouse_pos_y),
                     self.project["objects"],
                     max_dist=10.0,
                     exclude=(self.selection[2], self.selection[3]),
                 )
@@ -407,43 +368,37 @@
         painter["ctx"].setPen(QPen(QtCore.Qt.green, 1, QtCore.Qt.SolidLine))  # type: ignore  # pylint: disable=I1101
     else:
         painter["ctx"].setPen(QPen(QtCore.Qt.red, 1, QtCore.Qt.SolidLine))  # type: ignore  # pylint: disable=I1101
 
     draw_line_2d(p_from, p_to)
 
 
-def draw_object_edges(
-    project: dict, selected: int = -1  # pylint: disable=W0613
-) -> None:
+def draw_object_edges(project: dict, selected: int = -1) -> None:  # pylint: disable=W0613
     """draws the edges of an object"""
     unit = project["setup"]["machine"]["unit"]
     depth = project["setup"]["mill"]["depth"]
     tabs_height = project["setup"]["tabs"]["height"]
     unitscale = 1.0
     if unit == "inch":
         unitscale = 25.4
         depth *= unitscale
         tabs_height *= unitscale
 
     depths = []
     for obj in project["objects"].values():
-        if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-            "layer", ""
-        ).startswith("_TABS"):
+        if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
             continue
         odepth = obj["setup"]["mill"]["depth"]
         if odepth not in depths:
             depths.append(odepth)
     depths.sort()
 
     painter["ctx"].setPen(QPen(QtCore.Qt.white, 2, QtCore.Qt.SolidLine))  # type: ignore  # pylint: disable=I1101
     for _obj_idx, obj in project["objects"].items():
-        if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-            "layer", ""
-        ).startswith("_TABS"):
+        if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
             continue
 
         for segment in obj.segments:
             draw_line_2d(segment.start, segment.end)
 
     # tabs
     painter["ctx"].setPen(QPen(QtCore.Qt.blue, 4, QtCore.Qt.SolidLine))  # type: ignore  # pylint: disable=I1101
@@ -566,19 +521,15 @@
     painter["ctx"].setPen(QPen(QtCore.Qt.green, 1, QtCore.Qt.SolidLine))  # type: ignore  # pylint: disable=I1101
 
     if project["glwidget"]:
         if not draw_machinecode_path(project):
             print("error while drawing machine commands")
 
     selected = -1
-    if (
-        project["glwidget"]
-        and project["glwidget"].selection_set
-        and project["glwidget"].selector_mode in {"delete", "oselect"}
-    ):
+    if project["glwidget"] and project["glwidget"].selection_set and project["glwidget"].selector_mode in {"delete", "oselect"}:
         selected = project["glwidget"].selection_set[2]
 
     draw_object_edges(project, selected=selected)
 
     if project["glwidget"].selection:
         if project["glwidget"].selector_mode == "start":
             draw_line_2d(
```

### Comparing `viaconstructor-0.6.6/viaconstructor/dxfcolors.py` & `viaconstructor-0.6.7/viaconstructor/dxfcolors.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/HersheyFonts.py` & `viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/HersheyFonts.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/cavaliercontours.py` & `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/cavaliercontours.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so` & `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so` & `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/meshcut/meshcut.py` & `viaconstructor-0.6.7/viaconstructor/ext/meshcut/meshcut.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/stl/base.py` & `viaconstructor-0.6.7/viaconstructor/ext/stl/base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/stl/main.py` & `viaconstructor-0.6.7/viaconstructor/ext/stl/main.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/stl/stl.py` & `viaconstructor-0.6.7/viaconstructor/ext/stl/stl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/stl/utils.py` & `viaconstructor-0.6.7/viaconstructor/ext/stl/utils.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/__init__.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/bezier.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/document.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/misctools.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/parser.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/path.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/paths2svg.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/polytools.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/smoothing.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_io_sax.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_to_paths.py` & `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/gldraw.py` & `viaconstructor-0.6.7/viaconstructor/gldraw.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,17 +130,15 @@
         else:
             self.aspect = self.frameGeometry().height() / self.frameGeometry().width()
 
         height = 0.2
         width = height * self.aspect
 
         if self.ortho:
-            GL.glOrtho(
-                -height * 2.5, height * 2.5, -width * 2.5, width * 2.5, -1000, 1000
-            )
+            GL.glOrtho(-height * 2.5, height * 2.5, -width * 2.5, width * 2.5, -1000, 1000)
         else:
             GL.glFrustum(-height, height, -width, width, 0.5, 100.0)
 
         GL.glMatrixMode(GL.GL_MODELVIEW)
         GL.glLoadIdentity()
         GL.glClearColor(0.0, 0.0, 0.0, 1.0)
         GL.glClear(GL.GL_COLOR_BUFFER_BIT | GL.GL_DEPTH_BUFFER_BIT)
@@ -415,18 +413,15 @@
                     if dist >= 1.0:
                         pdist = 1.0 / dist
                         next_pos = point_of_line3d(last_pos, next_pos, pdist)
                     else:
                         pdist = 1.0
                     self.project["simulation_last"] = next_pos
                     if pdist >= 1.0:
-                        if (
-                            self.project["simulation_pos"]
-                            < len(self.project["simulation_data"]) - 1
-                        ):
+                        if self.project["simulation_pos"] < len(self.project["simulation_data"]) - 1:
                             self.project["simulation_pos"] += 1
                         else:
                             self.project["simulation_pos"] = 0
                             self.project["simulation"] = False
 
                 self.draw_tool(self.project["simulation_last"], spindle, diameter)
 
@@ -593,17 +588,15 @@
                 self.update()
             elif self.mbutton == 2:
                 if self.selector_mode == "tab":
                     sel_idx = -1
                     sel_dist = -1
                     for tab_idx, tab in enumerate(self.project["tabs"]["data"]):
                         tab_pos = line_center_2d(tab[0], tab[1])
-                        dist = calc_distance(
-                            (self.mouse_pos_x, self.mouse_pos_y), tab_pos
-                        )
+                        dist = calc_distance((self.mouse_pos_x, self.mouse_pos_y), tab_pos)
                         if sel_dist < 0 or dist < sel_dist:
                             sel_dist = dist
                             sel_idx = tab_idx
 
                     if 0.0 < sel_dist < 10.0:
                         del self.project["tabs"]["data"][sel_idx]
                         self.update_drawing()
@@ -632,76 +625,39 @@
         self.mbutton = None
         self.mpos = None
 
     def mouse_pos_to_real_pos(self, mouse_pos) -> tuple:
         min_max = self.project["minMax"]
         mouse_pos_x = mouse_pos.x()
         mouse_pos_y = self.screen_h - mouse_pos.y()
-        real_pos_x = (
-            (
-                (mouse_pos_x / self.screen_w - 0.5 + self.trans_x)
-                / self.scale
-                / self.scale_xyz
-            )
-            + (self.size_x / 2)
-            + min_max[0]
-        )
-        real_pos_y = (
-            (
-                (mouse_pos_y / self.screen_h - 0.5 + self.trans_y)
-                / self.scale
-                / self.scale_xyz
-                * self.aspect
-            )
-            + (self.size_y / 2)
-            + min_max[1]
-        )
+        real_pos_x = ((mouse_pos_x / self.screen_w - 0.5 + self.trans_x) / self.scale / self.scale_xyz) + (self.size_x / 2) + min_max[0]
+        real_pos_y = ((mouse_pos_y / self.screen_h - 0.5 + self.trans_y) / self.scale / self.scale_xyz * self.aspect) + (self.size_y / 2) + min_max[1]
         return (real_pos_x, real_pos_y)
 
     def mouseMoveEvent(self, event) -> None:  # pylint: disable=C0103
         """mouse moved."""
         if self.mbutton == 1:
             moffset = self.mpos - event.pos()
             self.trans_x = self.trans_x_last + moffset.x() / self.screen_w
             self.trans_y = self.trans_y_last - moffset.y() / self.screen_h * self.aspect
         elif self.selector_mode == "tab":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_tab_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["offsets"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_tab_point((self.mouse_pos_x, self.mouse_pos_y), self.project["offsets"])
         elif self.selector_mode == "start":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_point_on_segment(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_point_on_segment((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
         elif self.selector_mode == "delete":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
         elif self.selector_mode == "oselect":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
         elif self.selector_mode == "repair":
-            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(
-                event.pos()
-            )
-            self.selection = found_next_open_segment_point(
-                (self.mouse_pos_x, self.mouse_pos_y), self.project["objects"]
-            )
+            (self.mouse_pos_x, self.mouse_pos_y) = self.mouse_pos_to_real_pos(event.pos())
+            self.selection = found_next_open_segment_point((self.mouse_pos_x, self.mouse_pos_y), self.project["objects"])
             if self.selection:
                 selection_end = found_next_open_segment_point(
                     (self.mouse_pos_x, self.mouse_pos_y),
                     self.project["objects"],
                     max_dist=10.0,
                     exclude=(self.selection[2], self.selection[3]),
                 )
@@ -976,24 +932,20 @@
             False,
             True,
         )
         GL.glEnd()
         # Size-X
         GL.glColor3f(1.0, 0.0, 0.0)
         GL.glBegin(GL.GL_LINES)
-        draw_text(
-            f"{round(size_x, 2)}", center_x, start_y - 5 - 6, mill_depth, 0.5, True
-        )
+        draw_text(f"{round(size_x, 2)}", center_x, start_y - 5 - 6, mill_depth, 0.5, True)
         GL.glEnd()
         # Size-Y
         GL.glColor3f(0.0, 0.0, 1.0)
         GL.glBegin(GL.GL_LINES)
-        draw_text(
-            f"{round(size_y, 2)}", end_x + 5, center_y, mill_depth, 0.5, False, True
-        )
+        draw_text(f"{round(size_y, 2)}", end_x + 5, center_y, mill_depth, 0.5, False, True)
         GL.glEnd()
 
 
 def draw_object_ids(project: dict, selected: int = -1) -> None:
     """draws the object id's as text"""
     GL.glNormal3f(0, 0, 1)
     for obj_idx, obj in project["objects"].items():
@@ -1003,17 +955,15 @@
             GL.glColor3f(1.0, 1.0, 1.01)
         else:
             GL.glLineWidth(2)
             GL.glColor3f(0.63, 0.36, 0.11)
 
         GL.glBegin(GL.GL_LINES)
 
-        if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-            "layer", ""
-        ).startswith("_TABS"):
+        if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
             continue
         p_x = obj["segments"][0]["start"][0]
         p_y = obj["segments"][0]["start"][1]
         for (x_1, y_1), (x_2, y_2) in font.lines_for_text(f"#{obj_idx.split(':')[0]}"):
             GL.glVertex3f(p_x + x_1, p_y + y_1, 5.0)
             GL.glVertex3f(p_x + x_2, p_y + y_2, 5.0)
         GL.glEnd()
@@ -1029,28 +979,24 @@
     if unit == "inch":
         unitscale = 25.4
         depth *= unitscale
         tabs_height *= unitscale
 
     depths = []
     for obj in project["objects"].values():
-        if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-            "layer", ""
-        ).startswith("_TABS"):
+        if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
             continue
         odepth = obj["setup"]["mill"]["depth"]
         if odepth not in depths:
             depths.append(odepth)
     depths.sort()
     for depth in depths:
         GL.glNormal3f(0, 0, 1)
         for obj_idx, obj in project["objects"].items():
-            if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-                "layer", ""
-            ).startswith("_TABS"):
+            if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
                 continue
 
             color = (1.0, 1.0, 1.0)
             if project["setup"]["view"]["colors_show"] and obj.color in dxfcolors:
                 color = dxfcolors[obj.color][0:3]
 
             odepth = obj["setup"]["mill"]["depth"]
@@ -1075,17 +1021,15 @@
 
             # top
             GL.glBegin(GL.GL_LINES)
             for segment in obj.segments:
                 if segment.bulge != 0.0 and interpolate:
                     last_x = segment.start[0]
                     last_y = segment.start[1]
-                    for point in bulge_points(
-                        segment.start, segment.end, segment.bulge
-                    ):
+                    for point in bulge_points(segment.start, segment.end, segment.bulge):
                         GL.glVertex3f(last_x, last_y, 0.0)
                         GL.glVertex3f(point[0], point[1], 0.0)
                         last_x = point[0]
                         last_y = point[1]
                     GL.glVertex3f(last_x, last_y, 0.0)
                     GL.glVertex3f(segment.end[0], segment.end[1], 0.0)
                 else:
@@ -1096,17 +1040,15 @@
             # bottom
             if odepth == depth:
                 GL.glBegin(GL.GL_LINES)
                 for segment in obj.segments:
                     if segment.bulge != 0.0 and interpolate:
                         last_x = segment.start[0]
                         last_y = segment.start[1]
-                        for point in bulge_points(
-                            segment.start, segment.end, segment.bulge
-                        ):
+                        for point in bulge_points(segment.start, segment.end, segment.bulge):
                             GL.glVertex3f(last_x, last_y, depth)
                             GL.glVertex3f(point[0], point[1], depth)
                             last_x = point[0]
                             last_y = point[1]
                         GL.glVertex3f(last_x, last_y, depth)
                         GL.glVertex3f(segment.end[0], segment.end[1], depth)
                     else:
@@ -1178,48 +1120,42 @@
     unitscale = 1.0
     if unit == "inch":
         unitscale = 25.4
         depth *= unitscale
 
     depths = []
     for obj in project["objects"].values():
-        if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-            "layer", ""
-        ).startswith("_TABS"):
+        if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
             continue
         odepth = obj["setup"]["mill"]["depth"]
         if odepth not in depths:
             depths.append(odepth)
     depths.append(0.0)
     depths.sort()
 
     for depth in depths:
 
         GL.glColor4f(color[0], color[1], color[2], alpha)
         # object faces (side)
         GL.glBegin(GL.GL_TRIANGLES)
         for obj in project["objects"].values():
-            if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-                "layer", ""
-            ).startswith("_TABS"):
+            if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
                 continue
 
             odepth = obj["setup"]["mill"]["depth"]
             if odepth > depth:
                 continue
 
             depth *= unitscale
 
             for segment in obj.segments:
                 last_x = segment.start[0]
                 last_y = segment.start[1]
                 if segment.bulge != 0.0 and interpolate:
-                    for point in bulge_points(
-                        segment.start, segment.end, segment.bulge
-                    ):
+                    for point in bulge_points(segment.start, segment.end, segment.bulge):
                         add_triangle(
                             (last_x, last_y, 0.0),
                             (last_x, last_y, depth),
                             (point[0], point[1], 0.0),
                             (obj.tool_offset == "inside"),
                         )
                         add_triangle(
@@ -1247,39 +1183,33 @@
         # object faces (top)
         GL.glNormal3f(0, 0, 1)
         tess = gluNewTess()
         gluTessProperty(tess, GLU_TESS_WINDING_RULE, GLU_TESS_WINDING_ODD)
         gluTessCallback(tess, GLU_TESS_BEGIN, GL.glBegin)
         gluTessCallback(tess, GLU_TESS_VERTEX, GL.glVertex)
         gluTessCallback(tess, GLU_TESS_END, GL.glEnd)
-        gluTessCallback(
-            tess, GLU_TESS_COMBINE, lambda _points, _vertices, _weights: _points
-        )
+        gluTessCallback(tess, GLU_TESS_COMBINE, lambda _points, _vertices, _weights: _points)
         gluTessBeginPolygon(tess, 0)
         for obj in project["objects"].values():
-            if obj.get("layer", "").startswith("BREAKS:") or obj.get(
-                "layer", ""
-            ).startswith("_TABS"):
+            if obj.get("layer", "").startswith("BREAKS:") or obj.get("layer", "").startswith("_TABS"):
                 continue
 
             odepth = obj["setup"]["mill"]["depth"]
             if odepth > depth:
                 continue
 
             depth *= unitscale
 
             if obj.closed:
                 gluTessBeginContour(tess)
                 for segment in obj.segments:
                     p_xy = (segment.start[0], segment.start[1], depth)
                     gluTessVertex(tess, p_xy, p_xy)
                     if segment.bulge != 0.0 and interpolate:
-                        for point in bulge_points(
-                            segment.start, segment.end, segment.bulge
-                        ):
+                        for point in bulge_points(segment.start, segment.end, segment.bulge):
                             p_xy = (point[0], point[1], depth)
                             gluTessVertex(tess, p_xy, p_xy)
                     p_xy = (segment.end[0], segment.end[1], depth)
                     gluTessVertex(tess, p_xy, p_xy)
                 gluTessEndContour(tess)
         gluTessEndPolygon(tess)
         gluDeleteTess(tess)
@@ -1318,17 +1248,15 @@
                     gluTessVertex(tess, p_xy, p_xy)
                 gluTessEndContour(tess)
         gluTessEndPolygon(tess)
         gluDeleteTess(tess)
         """
 
 
-def draw_line(
-    p_1: dict, p_2: dict, options: str, project: dict, tool_number: int = 0
-) -> None:
+def draw_line(p_1: dict, p_2: dict, options: str, project: dict, tool_number: int = 0) -> None:
     """callback function for Parser to draw the lines"""
     if project["setup"]["machine"]["g54"]:
         p_from = (p_1["X"], p_1["Y"], p_1["Z"])
         p_to = (p_2["X"], p_2["Y"], p_2["Z"])
     else:
         unit = project["setup"]["machine"]["unit"]
         unitscale = 1.0
```

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/camotics.png` & `viaconstructor-0.6.7/viaconstructor/icons/camotics.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/delete.png` & `viaconstructor-0.6.7/viaconstructor/icons/delete.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/exit.png` & `viaconstructor-0.6.7/viaconstructor/icons/exit.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/flip-x.png` & `viaconstructor-0.6.7/viaconstructor/icons/flip-x.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/flip-y.png` & `viaconstructor-0.6.7/viaconstructor/icons/flip-y.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/fonts.png` & `viaconstructor-0.6.7/viaconstructor/icons/fonts.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/gears.png` & `viaconstructor-0.6.7/viaconstructor/icons/gears.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/load-setup-gcode.png` & `viaconstructor-0.6.7/viaconstructor/icons/load-setup-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/load-setup.png` & `viaconstructor-0.6.7/viaconstructor/icons/load-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/load-tooltable.png` & `viaconstructor-0.6.7/viaconstructor/icons/load-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/nesting.png` & `viaconstructor-0.6.7/viaconstructor/icons/nesting.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/open.png` & `viaconstructor-0.6.7/viaconstructor/icons/open.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/openscad.png` & `viaconstructor-0.6.7/viaconstructor/icons/openscad.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/pause.png` & `viaconstructor-0.6.7/viaconstructor/icons/pause.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/play.png` & `viaconstructor-0.6.7/viaconstructor/icons/play.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/redraw.png` & `viaconstructor-0.6.7/viaconstructor/icons/redraw.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/repair.png` & `viaconstructor-0.6.7/viaconstructor/icons/repair.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/rotate.png` & `viaconstructor-0.6.7/viaconstructor/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/save-gcode.png` & `viaconstructor-0.6.7/viaconstructor/icons/save-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/save-setup-as.png` & `viaconstructor-0.6.7/viaconstructor/icons/save-setup-as.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/save-setup.png` & `viaconstructor-0.6.7/viaconstructor/icons/save-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/save-tooltable.png` & `viaconstructor-0.6.7/viaconstructor/icons/save-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/save.png` & `viaconstructor-0.6.7/viaconstructor/icons/save.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/scale.png` & `viaconstructor-0.6.7/viaconstructor/icons/scale.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/start.png` & `viaconstructor-0.6.7/viaconstructor/icons/start.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/stop.png` & `viaconstructor-0.6.7/viaconstructor/icons/stop.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/tab-selector.png` & `viaconstructor-0.6.7/viaconstructor/icons/tab-selector.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/view-2d.png` & `viaconstructor-0.6.7/viaconstructor/icons/view-2d.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/icons/view-reset.png` & `viaconstructor-0.6.7/viaconstructor/icons/view-reset.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/brdread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/brdread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/dxfread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/dxfread.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,17 +127,15 @@
         dxfread_scale.setValue(1.0)
         dialog.layout.addWidget(dxfread_scale)
 
         dxfread_select_layers = {}
         if filename.lower().endswith(".dxf"):
             doc = ezdxf.readfile(filename)
             for layer in doc.layers:
-                dxfread_select_layers[layer.dxf.name] = QCheckBox(
-                    f"select layer: {layer.dxf.name}"
-                )
+                dxfread_select_layers[layer.dxf.name] = QCheckBox(f"select layer: {layer.dxf.name}")
                 dxfread_select_layers[layer.dxf.name].setChecked(True)
                 dialog.layout.addWidget(dxfread_select_layers[layer.dxf.name])
 
         dialog.layout.addWidget(dialog.buttonBox)
         dialog.setLayout(dialog.layout)
 
         if dialog.exec():
@@ -146,46 +144,36 @@
             if not args.dxfread_color_layers:
                 selection = []
                 for layer, stat in dxfread_select_layers.items():
                     if stat.isChecked():
                         selection.append(layer)
                 args.dxfread_select_layers = selection
 
-    def __init__(
-        self, filename: str, args: argparse.Namespace = None
-    ):  # pylint: disable=W0613
+    def __init__(self, filename: str, args: argparse.Namespace = None):  # pylint: disable=W0613
         """converting dxf into single segments."""
         self.filename = filename
-        if self.filename.lower().endswith(".svg") and os.path.isfile(
-            "/usr/share/inkscape/extensions/dxf_outlines.py"
-        ):
+        if self.filename.lower().endswith(".svg") and os.path.isfile("/usr/share/inkscape/extensions/dxf_outlines.py"):
             print("INFO: converting svg to dxf with inkscape")
             print("    you can disable this with: --dxfread-no-svg")
             _fd, tmp_path = tempfile.mkstemp()
-            os.system(
-                f"cd /usr/share/inkscape/extensions/ ; python3 dxf_outlines.py --output='{tmp_path}' '{os.path.realpath(self.filename)}'"
-            )
+            os.system(f"cd /usr/share/inkscape/extensions/ ; python3 dxf_outlines.py --output='{tmp_path}' '{os.path.realpath(self.filename)}'")
             self.doc = ezdxf.readfile(tmp_path)
             os.remove(tmp_path)
         elif self.filename.lower().endswith(BITMAP_FORMATS) and potrace:
             print("INFO: converting bitmap to dxf with potrace")
             print("    you can disable this with: --dxfread-no-bmp")
             _fd, tmp_path = tempfile.mkstemp()
 
             if not self.filename.lower().endswith(".bmp"):
                 _fd2, tmp_path2 = tempfile.mkstemp()
-                os.system(
-                    f"{convert} '{os.path.realpath(self.filename)}' '{tmp_path2}.bmp'"
-                )
+                os.system(f"{convert} '{os.path.realpath(self.filename)}' '{tmp_path2}.bmp'")
                 os.system(f"{potrace} -b dxf -o '{tmp_path}' '{tmp_path2}.bmp'")
                 os.remove(f"{tmp_path2}.bmp")
             else:
-                os.system(
-                    f"{potrace} -b dxf -o '{tmp_path}' '{os.path.realpath(self.filename)}'"
-                )
+                os.system(f"{potrace} -b dxf -o '{tmp_path}' '{os.path.realpath(self.filename)}'")
             self.doc = ezdxf.readfile(tmp_path)
             os.remove(tmp_path)
         else:
             self.doc = ezdxf.readfile(self.filename)
 
         if args is None or args.dxfread_scale == 0.0:
             self.scale = 1.0
@@ -286,17 +274,15 @@
             pos = (element.dxf.insert[0], element.dxf.insert[1])
             font_face = fonts.FontFace(family="Times New Roman")
             paths = text2path.make_paths_from_str(element.dxf.text, font_face)
             scale = element.dxf.height
             text_offset = (offset[0] + pos[0], offset[1] + pos[1])
             text_offset = (offset[0] + pos[0], offset[1] + pos[1])
             for path in paths:
-                self._add_path(
-                    path, text_offset, pscale=scale, layer=layer, color=color
-                )
+                self._add_path(path, text_offset, pscale=scale, layer=layer, color=color)
 
         elif dxftype == "LINE":
             dist = calc_distance(
                 (element.dxf.start.x, element.dxf.start.y),
                 (element.dxf.end.x, element.dxf.end.y),
             )
             if dist > self.MIN_DIST:
@@ -334,19 +320,15 @@
             else:
                 start_angle = element.dxf.start_angle
                 adiff = element.dxf.end_angle - element.dxf.start_angle
             if adiff < 0.0:
                 adiff += 360.0
 
             # fixing 132_2000.dxf
-            if (
-                element.dxf.extrusion
-                and len(element.dxf.extrusion) == 3
-                and element.dxf.extrusion[2] == -1.0
-            ):
+            if element.dxf.extrusion and len(element.dxf.extrusion) == 3 and element.dxf.extrusion[2] == -1.0:
                 element.dxf.center = (-element.dxf.center[0], element.dxf.center[1])
 
             # split arcs in maximum 20mm long segments and minimum 45°
             num_parts = (element.dxf.radius * 2 * math.pi) / 20.0
             if num_parts > 0:
                 gstep = 360.0 / num_parts
             else:
@@ -378,18 +360,16 @@
                                     ),
                                     "end": (
                                         (end.x + offset[0]) * self.scale,
                                         (end.y + offset[1]) * self.scale,
                                     ),
                                     "bulge": bulge,
                                     "center": (
-                                        (element.dxf.center[0] + offset[0])
-                                        * self.scale,
-                                        (element.dxf.center[1] + offset[1])
-                                        * self.scale,
+                                        (element.dxf.center[0] + offset[0]) * self.scale,
+                                        (element.dxf.center[1] + offset[1]) * self.scale,
                                     ),
                                 }
                             )
                         )
                     angle += astep
 
             else:
@@ -541,17 +521,15 @@
                 self.backup_ok = True
             except Exception as error:  # pylint: disable=W0703,W0621
                 print(f"ERROR: can not make backup of file: {self.filename}: {error}")
                 return
 
         delete_layers = []
         for layer in self.doc.layers:
-            if layer.dxf.name.startswith("BREAKS:") or layer.dxf.name.startswith(
-                "_TABS"
-            ):
+            if layer.dxf.name.startswith("BREAKS:") or layer.dxf.name.startswith("_TABS"):
                 delete_layers.append(layer.dxf.name)
 
         for layer_name in delete_layers:
             for element in self.model_space:
                 if element.dxf.layer == layer_name:
                     element.destroy()
             self.doc.layers.remove(layer_name)
@@ -559,17 +537,15 @@
         tabs_layer = self.doc.layers.add("_TABS")
         tabs_layer.color = 1
         for tab in tabs:
             self.model_space.add_line(tab[0], tab[1], dxfattribs={"layer": "_TABS"})
         try:
             self.doc.saveas(self.filename)
         except Exception as save_error:  # pylint: disable=W0703
-            print(
-                f"ERROR while saving tabs to dxf file ({self.filename}): {save_error}"
-            )
+            print(f"ERROR while saving tabs to dxf file ({self.filename}): {save_error}")
 
     def save_starts(self, objects: dict) -> None:
 
         if not self.backup_ok:
             try:
                 shutil.copy2(self.filename, f"/{self.filename}.{int(time.time())}")
                 self.backup_ok = True
@@ -594,17 +570,15 @@
             start = obj.get("start")
             if start:
                 self.model_space.add_line(start, start, dxfattribs={"layer": "_STARTS"})
 
         try:
             self.doc.saveas(self.filename)
         except Exception as save_error:  # pylint: disable=W0703
-            print(
-                f"ERROR while saving tabs to dxf file ({self.filename}): {save_error}"
-            )
+            print(f"ERROR while saving tabs to dxf file ({self.filename}): {save_error}")
 
     def save_setup(self, setup: str) -> None:
 
         if not self.backup_ok:
             try:
                 shutil.copy2(self.filename, f"{self.filename}.{int(time.time())}")
                 self.backup_ok = True
@@ -621,32 +595,25 @@
             for element in self.model_space:
                 if element.dxf.layer == layer_name:
                     element.destroy()
             self.doc.layers.remove(layer_name)
 
         tabs_layer = self.doc.layers.add("_CAMCFG")
         tabs_layer.color = 1
-        self.model_space.add_mtext(
-            setup, dxfattribs={"style": "DejaVu Sans", "layer": "_CAMCFG"}
-        )
+        self.model_space.add_mtext(setup, dxfattribs={"style": "DejaVu Sans", "layer": "_CAMCFG"})
         try:
             self.doc.saveas(self.filename)
             self.cam_setup = setup
         except Exception as save_error:  # pylint: disable=W0703
-            print(
-                f"ERROR while saving setup to dxf file ({self.filename}): {save_error}"
-            )
+            print(f"ERROR while saving setup to dxf file ({self.filename}): {save_error}")
 
     @staticmethod
     def suffix(args: argparse.Namespace = None) -> list[str]:
         suffixes = ["dxf"]
-        if not hasattr(args, "dxfread_no_bmp") or (
-            not args.dxfread_no_svg
-            and os.path.isfile("/usr/share/inkscape/extensions/dxf_outlines.py")
-        ):
+        if not hasattr(args, "dxfread_no_bmp") or (not args.dxfread_no_svg and os.path.isfile("/usr/share/inkscape/extensions/dxf_outlines.py")):
             suffixes.append("svg")
         if not hasattr(args, "dxfread_no_bmp") or (not args.dxfread_no_bmp and potrace):
             if convert:
                 suffixes += BITMAP_FORMATS
             else:
                 suffixes.append("bmp")
         return suffixes
```

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/hpglread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/hpglread.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import math
 
 from ..calc import angle_of_line, calc_distance  # pylint: disable=E0402
 from ..input_plugins_base import DrawReaderBase
 
 
 class DrawReader(DrawReaderBase):
-    def __init__(
-        self, filename: str, args: argparse.Namespace = None
-    ):  # pylint: disable=W0613
+    def __init__(self, filename: str, args: argparse.Namespace = None):  # pylint: disable=W0613
         """converting hpgl into single segments."""
         self.filename = filename
         self.segments: list[dict] = []
 
         self.state: dict = {
             "move_mode": "",
             "offsets": "OFF",
@@ -75,41 +73,29 @@
                 if line[0:2] == "AR":
                     center_x += last_x
                     center_y += last_y
                 angle = float(params[2])
                 # if len(params) == 4:
                 #    resolution = params[3]
                 radius = calc_distance((last_x, last_y), (center_x, center_y))
-                start_angle = (
-                    angle_of_line((last_x, last_y), (center_x, center_y))
-                    * 180
-                    / math.pi
-                )
+                start_angle = angle_of_line((last_x, last_y), (center_x, center_y)) * 180 / math.pi
                 if angle < 0:
                     for angle_set in range(0, int(abs(angle)) + 1):
-                        new_x = center_x + radius * math.sin(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
-                        new_y = center_y + radius * math.cos(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
+                        new_x = center_x + radius * math.sin((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
+                        new_y = center_y + radius * math.cos((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
                         self._add_line(
                             (last_x, last_y),
                             (new_x, new_y),
                         )
                         last_x = new_x
                         last_y = new_y
                 else:
                     for angle_set in range(int(abs(angle)), -1, -1):
-                        new_x = center_x - radius * math.sin(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
-                        new_y = center_y - radius * math.cos(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
+                        new_x = center_x - radius * math.sin((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
+                        new_y = center_y - radius * math.cos((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
                         self._add_line(
                             (last_x, last_y),
                             (new_x, new_y),
                         )
                         last_x = new_x
                         last_y = new_y
                 line = ""
```

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/imgread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/imgread.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         )
         parser.add_argument(
             "--imgread-lines",
             help="imgread: do not merge lines",
             action="store_true",
         )
 
-    def __init__(
-        self, filename: str, args: argparse.Namespace = None  # pylint: disable=W0613
-    ):
+    def __init__(self, filename: str, args: argparse.Namespace = None):  # pylint: disable=W0613
         """slicing and converting stl into single segments."""
         self.filename = filename
         self.segments = []
 
         image_data = Image.open(filename).convert("L")
 
         print(f"Image-Size: {image_data.width}x{image_data.height}")
```

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/stlread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/stlread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/svgread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/svgread.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,15 @@
 
         dialog.layout.addWidget(dialog.buttonBox)
         dialog.setLayout(dialog.layout)
 
         if dialog.exec():
             args.svgread_as_lines = svgread_as_lines.isChecked()
 
-    def __init__(
-        self, filename: str, args: argparse.Namespace = None
-    ):  # pylint: disable=W0613
+    def __init__(self, filename: str, args: argparse.Namespace = None):  # pylint: disable=W0613
         """converting svg into single segments."""
         self.filename = filename
         self.segments: list[dict] = []
 
         (
             paths,
             attributes,  # pylint: disable=W0612
@@ -177,17 +175,15 @@
                     self.min_max[2] = max(self.min_max[2], segment[point][0])
                     self.min_max[3] = max(self.min_max[3], segment[point][1])
 
         self.size = []
         self.size.append(self.min_max[2] - self.min_max[0])
         self.size.append(self.min_max[3] - self.min_max[1])
 
-    def add_arc(
-        self, center, radius, start_angle=0.0, end_angle=360.0, layer="0"
-    ) -> None:
+    def add_arc(self, center, radius, start_angle=0.0, end_angle=360.0, layer="0") -> None:
         adiff = end_angle - start_angle
         if adiff < 0.0:
             adiff += 360.0
         # split arcs in maximum 20mm long segments and minimum 45°
         num_parts = (radius * 2 * math.pi) / 20.0
         if num_parts > 0:
             gstep = 360.0 / num_parts
@@ -275,14 +271,12 @@
         svgdata.append("<!-- viaconstructor:setup")
         svgdata.append(setup)
         svgdata.append("-->")
         try:
             open(self.filename, "w").write("\n".join(svgdata).strip())
             self.cam_setup = setup
         except Exception as save_error:  # pylint: disable=W0703
-            print(
-                f"ERROR while saving setup to svg file ({self.filename}): {save_error}"
-            )
+            print(f"ERROR while saving setup to svg file ({self.filename}): {save_error}")
 
     @staticmethod
     def suffix(args: argparse.Namespace = None) -> list[str]:  # pylint: disable=W0613
         return ["svg"]
```

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins/ttfread.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins/ttfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,15 @@
                 continue
             if char == "\n":
                 ctx["pos"][0] = 0  # type: ignore
                 ctx["pos"][1] -= 1000 * scale  # type: ignore
                 continue
             face.load_char(
                 char,
-                freetype.FT_LOAD_DEFAULT  # pylint: disable=E1101
-                | freetype.FT_LOAD_NO_BITMAP,  # pylint: disable=E1101
+                freetype.FT_LOAD_DEFAULT | freetype.FT_LOAD_NO_BITMAP,  # pylint: disable=E1101  # pylint: disable=E1101
             )
             face.glyph.outline.decompose(
                 ctx,
                 move_to=self.move_to,
                 line_to=self.line_to,
                 conic_to=self.conic_to,
                 cubic_to=self.cubic_to,
```

### Comparing `viaconstructor-0.6.6/viaconstructor/input_plugins_base.py` & `viaconstructor-0.6.7/viaconstructor/input_plugins_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         return self.size
 
     def draw(self, draw_function, user_data=()) -> None:
         for segment in self.segments:
             draw_function(segment.start, segment.end, *user_data)
 
     def _add_line(self, start, end, layer="0", scale=1.0, bulge=0.0) -> list[float]:
-        dist = calc_distance(
-            (start[0] * scale, start[1] * scale), (end[0] * scale, end[1] * scale)
-        )
+        dist = calc_distance((start[0] * scale, start[1] * scale), (end[0] * scale, end[1] * scale))
         if dist > 0.001:
             self.segments.append(
                 VcSegment(
                     {
                         "type": "LINE",
                         "object": None,
                         "layer": layer,
```

### Comparing `viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.mo` & `viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.po` & `viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/machine_cmd.py` & `viaconstructor-0.6.7/viaconstructor/machine_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 
     def absolute(self, active=True) -> None:
         pass
 
     def tool_offsets(self, offset="none") -> None:
         pass
 
-    def machine_offsets(
-        self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True
-    ) -> None:
+    def machine_offsets(self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True) -> None:
         pass
 
     def program_start(self) -> None:
         pass
 
     def program_end(self) -> None:
         pass
@@ -77,22 +75,18 @@
 
     def spindle_ccw(self, speed: int, pause: int = 1) -> None:
         pass
 
     def linear(self, x_pos=None, y_pos=None, z_pos=None) -> None:
         pass
 
-    def arc_cw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_cw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         pass
 
-    def arc_ccw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_ccw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         pass
 
     def get(self, numbers=False) -> str:  # pylint: disable=W0613
         return ""
 
 
 def machine_cmd_begin(project: dict, post: PostProcessor) -> None:
@@ -105,22 +99,16 @@
         fast_move_z *= unitscale
 
     if project["setup"]["machine"]["comments"]:
         post.comment("--------------------------------------------------")
         post.comment("Generator: viaConstructor")
         post.comment(f"Filename: {project['filename_draw']}")
         post.comment(f"Tool-Mode: {project['setup']['machine']['mode']}")
-        if (
-            project["setup"]["workpiece"]["offset_x"] != 0.0
-            or project["setup"]["workpiece"]["offset_y"] != 0.0
-            or project["setup"]["workpiece"]["offset_z"] != 0.0
-        ):
-            post.comment(
-                f"Offsets: {project['setup']['workpiece']['offset_x']}, {project['setup']['workpiece']['offset_y']}, {project['setup']['workpiece']['offset_z']}"
-            )
+        if project["setup"]["workpiece"]["offset_x"] != 0.0 or project["setup"]["workpiece"]["offset_y"] != 0.0 or project["setup"]["workpiece"]["offset_z"] != 0.0:
+            post.comment(f"Offsets: {project['setup']['workpiece']['offset_x']}, {project['setup']['workpiece']['offset_y']}, {project['setup']['workpiece']['offset_z']}")
         post.comment("--------------------------------------------------")
     post.separation()
 
     post.program_start()
 
     post.unit(project["setup"]["machine"]["unit"])
     post.tool_offsets("none")
@@ -212,81 +200,60 @@
             tab_width = min(tab_width, arc_lenght)
             if tab_width > 0.0 and circumference > 0.0:
                 tab_angle = (math.pi * 2) / (circumference / tab_width)
             else:
                 tab_angle = 0.1
 
             for tab in tabs.get("data", ()):
-                inters = lines_intersect(
-                    (last[0], last[1]), (point[0], point[1]), tab[0], tab[1]
-                )
+                inters = lines_intersect((last[0], last[1]), (point[0], point[1]), tab[0], tab[1])
                 if inters:
-                    half_angle = (
-                        start_angle + (end_angle - start_angle) / 2 - (tab_angle / 2)
-                    )
-                    (
-                        start,  # pylint: disable=W0612
-                        end,
-                        bulge,
-                    ) = ezdxf.math.arc_to_bulge(
+                    half_angle = start_angle + (end_angle - start_angle) / 2 - (tab_angle / 2)
+                    (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                         center,
                         start_angle,
                         half_angle,
                         radius,
                     )
                     post.arc_ccw(
                         x_pos=end[0],
                         y_pos=end[1],
                         z_pos=set_depth,
                         i_pos=(center[0] - last[0]),
                         j_pos=(center[1] - last[1]),
                     )
                     last = end
 
-                    if (
-                        project["setup"]["machine"]["mode"] != "mill"
-                        or "Z" not in project["axis"]
-                    ):
+                    if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                         post.spindle_off()
 
                     if tabs_type == "rectangle":
                         post.linear(
                             x_pos=end[0],
                             y_pos=end[1],
                             z_pos=tabs_depth,
                         )
                     else:
                         half_angle = start_angle + (end_angle - start_angle) / 2
-                        (
-                            start,
-                            end,
-                            bulge,
-                        ) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
+                        (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                             center,
                             start_angle,
                             half_angle,
                             radius,
                         )
                         post.arc_ccw(
                             x_pos=end[0],
                             y_pos=end[1],
                             z_pos=tabs_depth,
                             i_pos=(center[0] - last[0]),
                             j_pos=(center[1] - last[1]),
                         )
                         last = end
 
-                    half_angle = (
-                        start_angle + (end_angle - start_angle) / 2 + (tab_angle / 2)
-                    )
-                    (
-                        start,
-                        end,
-                        bulge,
-                    ) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
+                    half_angle = start_angle + (end_angle - start_angle) / 2 + (tab_angle / 2)
+                    (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                         center,
                         start_angle,
                         half_angle,
                         radius,
                     )
                     if tabs_type == "rectangle":
                         post.arc_ccw(
@@ -306,18 +273,15 @@
                             x_pos=end[0],
                             y_pos=end[1],
                             z_pos=set_depth,
                             i_pos=(center[0] - last[0]),
                             j_pos=(center[1] - last[1]),
                         )
                     last = end
-                    if (
-                        project["setup"]["machine"]["mode"] != "mill"
-                        or "Z" not in project["axis"]
-                    ):
+                    if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                         post.spindle_cw(
                             tool["speed"],
                             tool["pause"],
                         )
                     break
 
         post.arc_ccw(
@@ -341,81 +305,60 @@
             tab_width = min(tab_width, arc_lenght)
             if tab_width > 0.0 and circumference > 0.0:
                 tab_angle = (math.pi * 2) / (circumference / tab_width)
             else:
                 tab_angle = 0.1
 
             for tab in tabs.get("data", ()):
-                inters = lines_intersect(
-                    (last[0], last[1]), (point[0], point[1]), tab[0], tab[1]
-                )
+                inters = lines_intersect((last[0], last[1]), (point[0], point[1]), tab[0], tab[1])
                 if inters:
-                    half_angle = (
-                        start_angle + (end_angle - start_angle) / 2 + (tab_angle / 2)
-                    )
-                    (
-                        start,
-                        end,
-                        bulge,
-                    ) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
+                    half_angle = start_angle + (end_angle - start_angle) / 2 + (tab_angle / 2)
+                    (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                         center,
                         start_angle,
                         half_angle,
                         radius,
                     )
                     post.arc_cw(
                         x_pos=end[0],
                         y_pos=end[1],
                         z_pos=set_depth,
                         i_pos=(center[0] - last[0]),
                         j_pos=(center[1] - last[1]),
                     )
                     last = end
 
-                    if (
-                        project["setup"]["machine"]["mode"] != "mill"
-                        or "Z" not in project["axis"]
-                    ):
+                    if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                         post.spindle_off()
 
                     if tabs_type == "rectangle":
                         post.linear(
                             x_pos=end[0],
                             y_pos=end[1],
                             z_pos=tabs_depth,
                         )
                     else:
                         half_angle = start_angle + (end_angle - start_angle) / 2
-                        (
-                            start,
-                            end,
-                            bulge,
-                        ) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
+                        (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                             center,
                             start_angle,
                             half_angle,
                             radius,
                         )
                         post.arc_cw(
                             x_pos=end[0],
                             y_pos=end[1],
                             z_pos=tabs_depth,
                             i_pos=(center[0] - last[0]),
                             j_pos=(center[1] - last[1]),
                         )
                         last = end
 
-                    half_angle = (
-                        start_angle + (end_angle - start_angle) / 2 - (tab_angle / 2)
-                    )
-                    (
-                        start,
-                        end,
-                        bulge,
-                    ) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
+                    half_angle = start_angle + (end_angle - start_angle) / 2 - (tab_angle / 2)
+                    (start, end, bulge,) = ezdxf.math.arc_to_bulge(  # pylint: disable=W0612
                         center,
                         start_angle,
                         half_angle,
                         radius,
                     )
                     if tabs_type == "rectangle":
                         post.arc_cw(
@@ -436,18 +379,15 @@
                             y_pos=end[1],
                             z_pos=set_depth,
                             i_pos=(center[0] - last[0]),
                             j_pos=(center[1] - last[1]),
                         )
 
                     last = end
-                    if (
-                        project["setup"]["machine"]["mode"] != "mill"
-                        or "Z" not in project["axis"]
-                    ):
+                    if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                         post.spindle_cw(
                             tool["speed"],
                             tool["pause"],
                         )
                     break
 
         post.arc_cw(
@@ -456,35 +396,30 @@
             z_pos=set_depth,
             i_pos=(center[0] - last[0]),
             j_pos=(center[1] - last[1]),
         )
     else:
         tab_list = {}
         for tab in tabs.get("data", ()):
-            inters = lines_intersect(
-                (last[0], last[1]), (point[0], point[1]), tab[0], tab[1]
-            )
+            inters = lines_intersect((last[0], last[1]), (point[0], point[1]), tab[0], tab[1])
             if inters:
                 dist = calc_distance((last[0], last[1]), inters)
                 tab_list[dist] = inters
 
         if tab_list:
             for tab_dist in sorted(tab_list.keys()):
                 angle = angle_of_line((last[0], last[1]), tab_list[tab_dist]) + HALF_PI
 
                 tab_start_x = last[0] + (tab_dist - (tab_width / 2)) * math.sin(angle)
                 tab_start_y = last[1] - (tab_dist - (tab_width / 2)) * math.cos(angle)
                 tab_end_x = last[0] + (tab_dist + (tab_width / 2)) * math.sin(angle)
                 tab_end_y = last[1] - (tab_dist + (tab_width / 2)) * math.cos(angle)
 
                 post.linear(x_pos=tab_start_x, y_pos=tab_start_y, z_pos=set_depth)
-                if (
-                    project["setup"]["machine"]["mode"] != "mill"
-                    or "Z" not in project["axis"]
-                ):
+                if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                     post.spindle_off()
 
                 if tabs_type == "rectangle":
                     post.linear(x_pos=tab_start_x, y_pos=tab_start_y, z_pos=tabs_depth)
                 else:
                     post.linear(
                         x_pos=tab_list[tab_dist][0],
@@ -493,18 +428,15 @@
                     )
 
                 if tabs_type == "rectangle":
                     post.linear(x_pos=tab_end_x, y_pos=tab_end_y, z_pos=tabs_depth)
 
                 post.linear(x_pos=tab_end_x, y_pos=tab_end_y, z_pos=set_depth)
 
-                if (
-                    project["setup"]["machine"]["mode"] != "mill"
-                    or "Z" not in project["axis"]
-                ):
+                if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                     post.spindle_cw(
                         tool["speed"],
                         tool["pause"],
                     )
 
         post.linear(x_pos=point[0], y_pos=point[1], z_pos=set_depth)
 
@@ -523,54 +455,41 @@
     nearest_idx: int = 0
     nearest_point = 0
     for offset_num, offset in polylines.items():
         if master_idx and master_idx not in offset.outer_objects and master_idx != offset.obj_idx:
             continue
 
         # no order
-        if (
-            objectorder == "unordered" and offset_num not in milling
-        ):  # pylint: disable=R0916
+        if objectorder == "unordered" and offset_num not in milling:  # pylint: disable=R0916
             vertex_data = vertex_data_cache(offset)
             dist = calc_distance(last_pos, (vertex_data[0][0], vertex_data[1][0]))
             nearest_dist = dist
             nearest_idx = offset_num
             nearest_point = 0
             found = True
             break
 
         # find nearest
-        if offset_num not in milling and (  # pylint: disable=R0916
-            (
-                (level == -1 or offset.level == level)
-                and offset.setup["tool"]["number"] == tool
-                and offset.setup["mill"]["active"]
-            )
-        ):
+        if offset_num not in milling and (((level == -1 or offset.level == level) and offset.setup["tool"]["number"] == tool and offset.setup["mill"]["active"])):  # pylint: disable=R0916
 
             if offset.setup["pockets"]["insideout"]:
                 sub_found = False
                 for pocket_offset_num, pocket_offset in polylines.items():
-                    if (
-                        pocket_offset.is_pocket != 0
-                        and pocket_offset_num not in milling
-                    ):
+                    if pocket_offset.is_pocket != 0 and pocket_offset_num not in milling:
                         if pocket_offset_num.startswith(f"{offset_num}."):
                             sub_found = True
                             break
                 # skip this offset while found a sub offset
                 if sub_found:
                     continue
 
             vertex_data = vertex_data_cache(offset)
             if offset.is_closed():
                 if offset.start:
-                    point_num = found_next_offset_point(
-                        (offset.start[0], offset.start[1]), offset
-                    )
+                    point_num = found_next_offset_point((offset.start[0], offset.start[1]), offset)
                     if point_num:
                         point_num = point_num[2]
                         pos_x = vertex_data[0][point_num]
                         pos_y = vertex_data[1][point_num]
                         dist = calc_distance(last_pos, (pos_x, pos_y))
                         if nearest_dist is None or dist < nearest_dist:
                             nearest_dist = dist
@@ -586,26 +505,22 @@
                             nearest_idx = offset_num
                             nearest_point = point_num
                             found = True
                         point_num += 1
             else:
                 # on open objects, test first and last point
                 if len(vertex_data) > 0 and len(vertex_data[0]) > 0:
-                    dist = calc_distance(
-                        last_pos, (vertex_data[0][0], vertex_data[1][0])
-                    )
+                    dist = calc_distance(last_pos, (vertex_data[0][0], vertex_data[1][0]))
                     if nearest_dist is None or dist < nearest_dist:
                         nearest_dist = dist
                         nearest_idx = offset_num
                         nearest_point = 0
                         found = True
                     if not offset.fixed_direction:
-                        dist = calc_distance(
-                            last_pos, (vertex_data[0][-1], vertex_data[1][-1])
-                        )
+                        dist = calc_distance(last_pos, (vertex_data[0][-1], vertex_data[1][-1]))
                         if nearest_dist is None or dist < nearest_dist:
                             nearest_dist = dist
                             nearest_idx = offset_num
                             nearest_point = len(vertex_data[0]) - 1
                             found = True
 
     return (found, nearest_idx, nearest_point, nearest_dist)
@@ -647,24 +562,19 @@
                 master_ids.append(obj_idx)
     else:
         master_ids = [""]
 
     for master_idx in master_ids:
         levels = range(project["maxOuter"], -1, -1)
         # ignore levels
-        #levels = [-1]
+        # levels = [-1]
         for level in levels:
             for tool in tools:
                 while True:
-                    (
-                        found,
-                        nearest_idx,
-                        nearest_point,
-                        nearest_dist,
-                    ) = get_nearest_free_object(
+                    (found, nearest_idx, nearest_point, nearest_dist,) = get_nearest_free_object(
                         polylines,
                         level,
                         tool,
                         last_pos,
                         milling,
                         objectorder,
                         master_idx,
@@ -736,40 +646,27 @@
                                 diameter = entry["diameter"]
                         if diameter is None:
                             print("ERROR: TOOL not found")
                             break
 
                         if project["setup"]["machine"]["comments"]:
                             post.separation()
-                            post.comment(
-                                "--------------------------------------------------"
-                            )
+                            post.comment("--------------------------------------------------")
                             post.comment(f"Level: {level}")
                             post.comment(f"Order: {order}")
                             post.comment(f"Object: {nearest_idx}")
-                            post.comment(
-                                f"Distance: {round(obj_distance * unitscale, 4)}{unit}"
-                            )
+                            post.comment(f"Distance: {round(obj_distance * unitscale, 4)}{unit}")
                             post.comment(f"Closed: {is_closed}")
                             post.comment(f"isPocket: {polyline.is_pocket != 0}")
-                            if (
-                                project["setup"]["machine"]["mode"] != "laser"
-                                and "Z" in project["axis"]
-                            ):
-                                post.comment(
-                                    f"Depth: {polyline.setup['mill']['depth']}{unit} / {polyline.setup['mill']['step']}{unit}"
-                                )
+                            if project["setup"]["machine"]["mode"] != "laser" and "Z" in project["axis"]:
+                                post.comment(f"Depth: {polyline.setup['mill']['depth']}{unit} / {polyline.setup['mill']['step']}{unit}")
                             post.comment(f"Tool-Diameter: {diameter}{unit}")
                             if polyline.tool_offset:
-                                post.comment(
-                                    f"Tool-Offset: {diameter / 2.0}{unit} {polyline.tool_offset}"
-                                )
-                            post.comment(
-                                "--------------------------------------------------"
-                            )
+                                post.comment(f"Tool-Offset: {diameter / 2.0}{unit} {polyline.tool_offset}")
+                            post.comment("--------------------------------------------------")
 
                         # toolchange
                         if project["setup"]["machine"]["mode"] == "mill":
                             post.move(z_pos=fast_move_z)
                             if project["setup"]["machine"]["supports_toolchange"]:
                                 post.tool(polyline.setup["tool"]["number"])
                             post.spindle_cw(
@@ -783,31 +680,25 @@
                         depth = min(depth, min_depth)
 
                         if coolant_mist:
                             post.coolant_mist()
                         if coolant_flood:
                             post.coolant_flood()
 
-                        if (
-                            project["setup"]["machine"]["mode"] == "mill"
-                            and "Z" in project["axis"]
-                        ):
+                        if project["setup"]["machine"]["mode"] == "mill" and "Z" in project["axis"]:
                             if not (was_pocket and nearest_dist < diameter):
                                 post.move(z_pos=fast_move_z)
                             elif helix_mode:
                                 post.move(z_pos=0.0)
                             else:
                                 post.move(z_pos=depth)
 
                         was_pocket = polyline.is_pocket > 0
 
-                        if (
-                            project["setup"]["machine"]["mode"] != "mill"
-                            or "Z" not in project["axis"]
-                        ):
+                        if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                             depth = 0.0
                             post.move(z_pos=depth)
 
                         lead_in_active = polyline.setup["leads"]["in"]
                         lead_out_active = polyline.setup["leads"]["out"]
                         if not is_closed:
                             # only on closed contours
@@ -821,132 +712,76 @@
                             # lead-out only on single pathes
                             lead_out_active = "off"
 
                         if lead_in_active != "off":
                             lead_in_lenght = polyline.setup["leads"]["in_lenght"]
                             line_angle = angle_of_line(points[0], points[1])
                             if lead_in_active == "straight":
-                                lead_in_x = points[0][0] - lead_in_lenght * math.sin(
-                                    line_angle
-                                )
-                                lead_in_y = points[0][1] + lead_in_lenght * math.cos(
-                                    line_angle
-                                )
+                                lead_in_x = points[0][0] - lead_in_lenght * math.sin(line_angle)
+                                lead_in_y = points[0][1] + lead_in_lenght * math.cos(line_angle)
                             else:
                                 lead_radius = lead_in_lenght * 2 / math.pi
                                 if polyline.setup["mill"]["reverse"]:
-                                    lead_in_center_x = points[0][
-                                        0
-                                    ] + lead_radius * math.sin(line_angle)
-                                    lead_in_center_y = points[0][
-                                        1
-                                    ] - lead_radius * math.cos(line_angle)
-                                    lead_in_x = lead_in_center_x + lead_radius * math.sin(
-                                        line_angle - HALF_PI
-                                    )
-                                    lead_in_y = lead_in_center_y - lead_radius * math.cos(
-                                        line_angle - HALF_PI
-                                    )
+                                    lead_in_center_x = points[0][0] + lead_radius * math.sin(line_angle)
+                                    lead_in_center_y = points[0][1] - lead_radius * math.cos(line_angle)
+                                    lead_in_x = lead_in_center_x + lead_radius * math.sin(line_angle - HALF_PI)
+                                    lead_in_y = lead_in_center_y - lead_radius * math.cos(line_angle - HALF_PI)
                                 else:
-                                    line_angle = (
-                                        angle_of_line(points[0], points[1]) + math.pi
-                                    )
-                                    lead_in_center_x = points[0][
-                                        0
-                                    ] + lead_radius * math.sin(line_angle)
-                                    lead_in_center_y = points[0][
-                                        1
-                                    ] - lead_radius * math.cos(line_angle)
-                                    lead_in_x = lead_in_center_x + lead_radius * math.sin(
-                                        line_angle + HALF_PI
-                                    )
-                                    lead_in_y = lead_in_center_y - lead_radius * math.cos(
-                                        line_angle + HALF_PI
-                                    )
+                                    line_angle = angle_of_line(points[0], points[1]) + math.pi
+                                    lead_in_center_x = points[0][0] + lead_radius * math.sin(line_angle)
+                                    lead_in_center_y = points[0][1] - lead_radius * math.cos(line_angle)
+                                    lead_in_x = lead_in_center_x + lead_radius * math.sin(line_angle + HALF_PI)
+                                    lead_in_y = lead_in_center_y - lead_radius * math.cos(line_angle + HALF_PI)
                             post.move(x_pos=lead_in_x, y_pos=lead_in_y)
                         else:
                             post.move(x_pos=points[0][0], y_pos=points[0][1])
 
                         if lead_out_active != "off":
                             lead_out_lenght = polyline.setup["leads"]["out_lenght"]
                             line_angle = angle_of_line(points[0], points[1])
                             if lead_out_active == "straight":
-                                lead_out_x = points[0][0] - lead_out_lenght * math.sin(
-                                    line_angle
-                                )
-                                lead_out_y = points[0][1] + lead_out_lenght * math.cos(
-                                    line_angle
-                                )
+                                lead_out_x = points[0][0] - lead_out_lenght * math.sin(line_angle)
+                                lead_out_y = points[0][1] + lead_out_lenght * math.cos(line_angle)
                             else:
                                 lead_radius = lead_out_lenght * 2 / math.pi
                                 if polyline.setup["mill"]["reverse"]:
-                                    lead_out_center_x = points[0][
-                                        0
-                                    ] + lead_radius * math.sin(line_angle)
-                                    lead_out_center_y = points[0][
-                                        1
-                                    ] - lead_radius * math.cos(line_angle)
-                                    lead_out_x = lead_out_center_x + lead_radius * math.sin(
-                                        line_angle + HALF_PI
-                                    )
-                                    lead_out_y = lead_out_center_y - lead_radius * math.cos(
-                                        line_angle + HALF_PI
-                                    )
+                                    lead_out_center_x = points[0][0] + lead_radius * math.sin(line_angle)
+                                    lead_out_center_y = points[0][1] - lead_radius * math.cos(line_angle)
+                                    lead_out_x = lead_out_center_x + lead_radius * math.sin(line_angle + HALF_PI)
+                                    lead_out_y = lead_out_center_y - lead_radius * math.cos(line_angle + HALF_PI)
                                 else:
-                                    line_angle = (
-                                        angle_of_line(points[0], points[1]) + math.pi
-                                    )
-                                    lead_out_center_x = points[0][
-                                        0
-                                    ] + lead_radius * math.sin(line_angle)
-                                    lead_out_center_y = points[0][
-                                        1
-                                    ] - lead_radius * math.cos(line_angle)
-                                    lead_out_x = lead_out_center_x + lead_radius * math.sin(
-                                        line_angle - HALF_PI
-                                    )
-                                    lead_out_y = lead_out_center_y - lead_radius * math.cos(
-                                        line_angle - HALF_PI
-                                    )
+                                    line_angle = angle_of_line(points[0], points[1]) + math.pi
+                                    lead_out_center_x = points[0][0] + lead_radius * math.sin(line_angle)
+                                    lead_out_center_y = points[0][1] - lead_radius * math.cos(line_angle)
+                                    lead_out_x = lead_out_center_x + lead_radius * math.sin(line_angle - HALF_PI)
+                                    lead_out_y = lead_out_center_y - lead_radius * math.cos(line_angle - HALF_PI)
 
                         last_depth = 0.0
                         passes = 1
                         while True:
                             depth = max(depth, max_depth)
 
-                            if (
-                                project["setup"]["machine"]["mode"] != "laser"
-                                and "Z" in project["axis"]
-                            ):
+                            if project["setup"]["machine"]["mode"] != "laser" and "Z" in project["axis"]:
                                 if project["setup"]["machine"]["comments"]:
                                     post.comment(f"- Depth: {depth}{unit} -")
 
                             if not is_closed:
-                                if (
-                                    project["setup"]["machine"]["mode"] == "mill"
-                                    and "Z" in project["axis"]
-                                ):
+                                if project["setup"]["machine"]["mode"] == "mill" and "Z" in project["axis"]:
                                     post.move(z_pos=fast_move_z)
                                 post.move(x_pos=points[0][0], y_pos=points[0][1])
 
-                            if (
-                                project["setup"]["machine"]["mode"] != "laser"
-                                and "Z" in project["axis"]
-                            ):
+                            if project["setup"]["machine"]["mode"] != "laser" and "Z" in project["axis"]:
                                 post.feedrate(polyline.setup["tool"]["rate_v"])
                                 if helix_mode:
                                     post.linear(z_pos=last_depth)
                                 else:
                                     post.linear(z_pos=depth)
                                 post.feedrate(polyline.setup["tool"]["rate_h"])
 
-                            if (
-                                project["setup"]["machine"]["mode"] != "mill"
-                                or "Z" not in project["axis"]
-                            ):
+                            if project["setup"]["machine"]["mode"] != "mill" or "Z" not in project["axis"]:
                                 post.spindle_cw(
                                     polyline.setup["tool"]["speed"],
                                     polyline.setup["tool"]["pause"],
                                 )
 
                             if lead_in_active != "off":
 
@@ -974,17 +809,15 @@
 
                             trav_distance = 0
                             last = points[0]
                             for point in points:
                                 if helix_mode:
                                     trav_distance += calc_distance(point, last)
                                     depth_diff = depth - last_depth
-                                    set_depth = last_depth + (
-                                        trav_distance / obj_distance * depth_diff
-                                    )
+                                    set_depth = last_depth + (trav_distance / obj_distance * depth_diff)
                                 else:
                                     set_depth = depth
                                 segment2machine_cmd(
                                     project,
                                     post,
                                     last,
                                     point,
@@ -997,17 +830,15 @@
 
                             if is_closed:
                                 point = points[0]
 
                                 if helix_mode:
                                     trav_distance += calc_distance(point, last)
                                     depth_diff = depth - last_depth
-                                    set_depth = last_depth + (
-                                        trav_distance / obj_distance * depth_diff
-                                    )
+                                    set_depth = last_depth + (trav_distance / obj_distance * depth_diff)
                                 else:
                                     set_depth = depth
                                 segment2machine_cmd(
                                     project,
                                     post,
                                     last,
                                     point,
@@ -1025,18 +856,15 @@
                             if depth <= max_depth - zoffset:
                                 if helix_mode:
                                     helix_mode = False
                                     continue
                                 break
                             depth += step
 
-                            if (
-                                project["setup"]["machine"]["mode"] == "laser"
-                                and polyline.setup["mill"]["passes"] == passes
-                            ) or "Z" not in project["axis"]:
+                            if (project["setup"]["machine"]["mode"] == "laser" and polyline.setup["mill"]["passes"] == passes) or "Z" not in project["axis"]:
                                 break
 
                             passes += 1
 
                         if lead_out_active != "off":
                             if lead_out_active == "straight":
                                 post.linear(
```

### Comparing `viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_grbl.py` & `viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_grbl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import math
+
 from ..machine_cmd import PostProcessor  # pylint: disable=E0402
 
 
 class PostProcessorGcodeGrbl(PostProcessor):
     def __init__(self, project):
         self.project = project
         self.comments = self.project["setup"]["machine"]["comments"]
+        self.arcs = self.project["setup"]["machine"]["arcs"]
         self.gcode: list[str] = []
         self.x_pos: float = None
         self.y_pos: float = None
         self.z_pos: float = None
         self.rate: int = 0
         self.speed: int = -1
         self.offsets: tuple[float, float, float] = (0.0, 0.0, 0.0)
@@ -70,23 +73,19 @@
             if offset == "none":
                 self.gcode.append("G40")
             elif offset == "left":
                 self.gcode.append("G41")
             else:
                 self.gcode.append("G42")
 
-    def machine_offsets(
-        self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True
-    ) -> None:
+    def machine_offsets(self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True) -> None:
         self.offsets_reset = False
         if not soft and offsets != (0.0, 0.0, 0.0):
             self.offsets_reset = True
-            self.gcode.append(
-                f"G10 L2 P1 X{offsets[0]:.12f} Y{offsets[1]:.12f} Z{offsets[2]:.12f} (workpiece offsets for G54)"
-            )
+            self.gcode.append(f"G10 L2 P1 X{offsets[0]:.12f} Y{offsets[1]:.12f} Z{offsets[2]:.12f} (workpiece offsets for G54)")
             self.gcode.append("G54")
         if soft:
             self.offsets = (
                 offsets[0] / self.scale,
                 offsets[1] / self.scale,
                 offsets[2] / self.scale,
             )
@@ -122,23 +121,19 @@
             self.gcode.append(f"G00 Z{fast_move_z}")
 
             # tool off
             if self.speed > 0:
                 self.spindle_off()
 
             if self.project["setup"]["machine"]["toolchange_pre"]:
-                for part in self.project["setup"]["machine"]["toolchange_pre"].split(
-                    "\n"
-                ):
+                for part in self.project["setup"]["machine"]["toolchange_pre"].split("\n"):
                     self.gcode.append(part)
             self.gcode.append(f"M06 T{number}")
             if self.project["setup"]["machine"]["toolchange_post"]:
-                for part in self.project["setup"]["machine"]["toolchange_post"].split(
-                    "\n"
-                ):
+                for part in self.project["setup"]["machine"]["toolchange_post"].split("\n"):
                     self.gcode.append(part)
 
             # tool to safe z
             if self.z_pos != fast_move_z:
                 self.gcode.append(f"G00 Z{fast_move_z}")
 
             # tool to last xy
@@ -154,17 +149,15 @@
     def spindle_off(self) -> None:
         if self.comments:
             self.gcode.append("M05 (Spindle off)")
         else:
             self.gcode.append("M05")
         self.tool_running = 0
         if self.project["setup"]["machine"]["spindle_off_post"]:
-            for part in self.project["setup"]["machine"]["spindle_off_post"].split(
-                "\n"
-            ):
+            for part in self.project["setup"]["machine"]["spindle_off_post"].split("\n"):
                 self.gcode.append(part)
 
     def coolant_mist(self) -> None:
         self.gcode.append("M07 (mist on)")
 
     def coolant_flood(self) -> None:
         self.gcode.append("M08 (flood on)")
@@ -223,55 +216,61 @@
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{(z_pos + self.offsets[2]) * self.scale:.12f}")
             self.z_pos = z_pos
         if line:
             self.gcode.append("G01 " + " ".join(line))
 
-    def arc_cw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_cw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         line = []
         if x_pos is not None and self.x_pos != x_pos:
             line.append(f"X{(x_pos + self.offsets[0]) * self.scale:.12f}")
             self.x_pos = x_pos
         if y_pos is not None and self.y_pos != y_pos:
             line.append(f"Y{(y_pos + self.offsets[1]) * self.scale:.12f}")
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{(z_pos + self.offsets[2]) * self.scale:.12f}")
             self.z_pos = z_pos
-        if i_pos is not None:
-            line.append(f"I{i_pos:.12f}")
-        if j_pos is not None:
-            line.append(f"J{j_pos:.12f}")
-        if r_pos is not None:
-            line.append(f"R{r_pos:.12f}")
+        if self.arcs == "r":
+            if i_pos is not None and j_pos is not None:
+                r_pos = math.dist((0, 0), (i_pos, j_pos))
+                line.append(f"R{r_pos:.12f}")
+        else:
+            if i_pos is not None:
+                line.append(f"I{i_pos:.12f}")
+            if j_pos is not None:
+                line.append(f"J{j_pos:.12f}")
+            if r_pos is not None:
+                line.append(f"R{r_pos:.12f}")
         if line:
             self.gcode.append("G02 " + " ".join(line))
 
-    def arc_ccw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_ccw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         line = []
         if x_pos is not None and self.x_pos != x_pos:
             line.append(f"X{(x_pos + self.offsets[0]) * self.scale:.12f}")
             self.x_pos = x_pos
         if y_pos is not None and self.y_pos != y_pos:
             line.append(f"Y{(y_pos + self.offsets[1]) * self.scale:.12f}")
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{(z_pos + self.offsets[2]) * self.scale:.12f}")
             self.z_pos = z_pos
-        if i_pos is not None:
-            line.append(f"I{i_pos:.12f}")
-        if j_pos is not None:
-            line.append(f"J{j_pos:.12f}")
-        if r_pos is not None:
-            line.append(f"R{r_pos:.12f}")
+        if self.arcs == "r":
+            if i_pos is not None and j_pos is not None:
+                r_pos = math.dist((0, 0), (i_pos, j_pos))
+                line.append(f"R{r_pos:.12f}")
+        else:
+            if i_pos is not None:
+                line.append(f"I{i_pos:.12f}")
+            if j_pos is not None:
+                line.append(f"J{j_pos:.12f}")
+            if r_pos is not None:
+                line.append(f"R{r_pos:.12f}")
         if line:
             self.gcode.append("G03 " + " ".join(line))
 
     def get(self, numbers=False) -> str:
         output = []
         if numbers:
             line_number = 1
```

### Comparing `viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_linuxcnc.py` & `viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_linuxcnc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import math
+
 from ..machine_cmd import PostProcessor  # pylint: disable=E0402
 
 
 class PostProcessorGcodeLinuxCNC(PostProcessor):
     def __init__(self, project):
         self.project = project
         self.comments = self.project["setup"]["machine"]["comments"]
+        self.arcs = self.project["setup"]["machine"]["arcs"]
         self.gcode: list[str] = []
         self.x_pos: float = None
         self.y_pos: float = None
         self.z_pos: float = None
         self.rate: int = 0
         self.speed: int = -1
         self.offsets: tuple[float, float, float] = (0.0, 0.0, 0.0)
@@ -69,23 +72,19 @@
             if offset == "none":
                 self.gcode.append("G40")
             elif offset == "left":
                 self.gcode.append("G41")
             else:
                 self.gcode.append("G42")
 
-    def machine_offsets(
-        self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True
-    ) -> None:
+    def machine_offsets(self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True) -> None:
         self.offsets_reset = False
         if not soft and offsets != (0.0, 0.0, 0.0):
             self.offsets_reset = True
-            self.gcode.append(
-                f"G10 L2 P1 X{offsets[0]:.6f} Y{offsets[1]:.6f} Z{offsets[2]:.6f} (workpiece offsets for G54)"
-            )
+            self.gcode.append(f"G10 L2 P1 X{offsets[0]:.6f} Y{offsets[1]:.6f} Z{offsets[2]:.6f} (workpiece offsets for G54)")
             self.gcode.append("G54")
         if soft:
             self.offsets = (
                 offsets[0] / self.scale,
                 offsets[1] / self.scale,
                 offsets[2] / self.scale,
             )
@@ -121,23 +120,19 @@
             self.gcode.append(f"G00 Z{fast_move_z}")
 
             # tool off
             if self.speed > 0:
                 self.spindle_off()
 
             if self.project["setup"]["machine"]["toolchange_pre"]:
-                for part in self.project["setup"]["machine"]["toolchange_pre"].split(
-                    "\n"
-                ):
+                for part in self.project["setup"]["machine"]["toolchange_pre"].split("\n"):
                     self.gcode.append(part)
             self.gcode.append(f"M06 T{number}")
             if self.project["setup"]["machine"]["toolchange_post"]:
-                for part in self.project["setup"]["machine"]["toolchange_post"].split(
-                    "\n"
-                ):
+                for part in self.project["setup"]["machine"]["toolchange_post"].split("\n"):
                     self.gcode.append(part)
 
             # tool to safe z
             if self.z_pos != fast_move_z:
                 self.gcode.append(f"G00 Z{fast_move_z}")
 
             # tool to last xy
@@ -153,17 +148,15 @@
     def spindle_off(self) -> None:
         if self.comments:
             self.gcode.append("M05 (Spindle off)")
         else:
             self.gcode.append("M05")
         self.tool_running = 0
         if self.project["setup"]["machine"]["spindle_off_post"]:
-            for part in self.project["setup"]["machine"]["spindle_off_post"].split(
-                "\n"
-            ):
+            for part in self.project["setup"]["machine"]["spindle_off_post"].split("\n"):
                 self.gcode.append(part)
 
     def coolant_mist(self) -> None:
         self.gcode.append("M07 (mist on)")
 
     def coolant_flood(self) -> None:
         self.gcode.append("M08 (flood on)")
@@ -222,55 +215,61 @@
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{round((z_pos + self.offsets[2]) * self.scale, 6):.6f}")
             self.z_pos = z_pos
         if line:
             self.gcode.append("G01 " + " ".join(line))
 
-    def arc_cw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_cw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         line = []
         if x_pos is not None and self.x_pos != x_pos:
             line.append(f"X{round((x_pos + self.offsets[0]) * self.scale, 6):.6f}")
             self.x_pos = x_pos
         if y_pos is not None and self.y_pos != y_pos:
             line.append(f"Y{round((y_pos + self.offsets[1]) * self.scale, 6):.6f}")
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{round((z_pos + self.offsets[2]) * self.scale, 6):.6f}")
             self.z_pos = z_pos
-        if i_pos is not None:
-            line.append(f"I{round(i_pos, 6):.6f}")
-        if j_pos is not None:
-            line.append(f"J{round(j_pos, 6):.6f}")
-        if r_pos is not None:
-            line.append(f"R{round(r_pos, 6):.6f}")
+        if self.arcs == "r":
+            if i_pos is not None and j_pos is not None:
+                r_pos = math.dist((0, 0), (i_pos, j_pos))
+                line.append(f"R{round(r_pos, 6):.6f}")
+        else:
+            if i_pos is not None:
+                line.append(f"I{round(i_pos, 6):.6f}")
+            if j_pos is not None:
+                line.append(f"J{round(j_pos, 6):.6f}")
+            if r_pos is not None:
+                line.append(f"R{round(r_pos, 6):.6f}")
         if line:
             self.gcode.append("G02 " + " ".join(line))
 
-    def arc_ccw(
-        self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None
-    ) -> None:
+    def arc_ccw(self, x_pos=None, y_pos=None, z_pos=None, i_pos=None, j_pos=None, r_pos=None) -> None:
         line = []
         if x_pos is not None and self.x_pos != x_pos:
             line.append(f"X{round((x_pos + self.offsets[0]) * self.scale, 6):.6f}")
             self.x_pos = x_pos
         if y_pos is not None and self.y_pos != y_pos:
             line.append(f"Y{round((y_pos + self.offsets[1]) * self.scale, 6):.6f}")
             self.y_pos = y_pos
         if z_pos is not None and self.z_pos != z_pos:
             line.append(f"Z{round((z_pos + self.offsets[2]) * self.scale, 6):.6f}")
             self.z_pos = z_pos
-        if i_pos is not None:
-            line.append(f"I{round(i_pos, 6):.6f}")
-        if j_pos is not None:
-            line.append(f"J{round(j_pos, 6):.6f}")
-        if r_pos is not None:
-            line.append(f"R{round(r_pos, 6):.6f}")
+        if self.arcs == "r":
+            if i_pos is not None and j_pos is not None:
+                r_pos = math.dist((0, 0), (i_pos, j_pos))
+                line.append(f"R{round(r_pos, 6):.6f}")
+        else:
+            if i_pos is not None:
+                line.append(f"I{round(i_pos, 6):.6f}")
+            if j_pos is not None:
+                line.append(f"J{round(j_pos, 6):.6f}")
+            if r_pos is not None:
+                line.append(f"R{round(r_pos, 6):.6f}")
         if line:
             self.gcode.append("G03 " + " ".join(line))
 
     def get(self, numbers=False) -> str:
         output = []
         if numbers:
             line_number = 1
```

### Comparing `viaconstructor-0.6.6/viaconstructor/output_plugins/hpgl.py` & `viaconstructor-0.6.7/viaconstructor/output_plugins/hpgl.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
         else:
             self.hpgl.append("PR")
 
     def program_start(self) -> None:
         self.toolrun = False
         self.hpgl.append("PU")
 
-    def machine_offsets(
-        self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True
-    ) -> None:
+    def machine_offsets(self, offsets: tuple[float, float, float] = (0.0, 0.0, 0.0), soft: bool = True) -> None:
         self.offsets = offsets
 
     def program_end(self) -> None:
         self.toolrun = False
         self.hpgl.append("PU")
 
     def comment(self, text) -> None:
@@ -146,17 +144,15 @@
         if y_pos is not None:
             self.y_pos = int((y_pos + self.offsets[1]) * self.scale)
         if z_pos is not None:
             self.z_pos = int((z_pos + self.offsets[2]) * self.scale)
         if x_pos is not None and y_pos is not None:
             center_x = self.last_x + i_pos * self.scale
             center_y = self.last_y + j_pos * self.scale
-            self.arc_move(
-                self.last_x, self.last_y, self.x_pos, self.y_pos, center_x, center_y, 2
-            )
+            self.arc_move(self.last_x, self.last_y, self.x_pos, self.y_pos, center_x, center_y, 2)
             self.last_x = self.x_pos
             self.last_y = self.y_pos
 
     def arc_ccw(
         self,
         x_pos=None,
         y_pos=None,
@@ -170,17 +166,15 @@
         if y_pos is not None:
             self.y_pos = int((y_pos + self.offsets[0]) * self.scale)
         if z_pos is not None:
             self.z_pos = int((z_pos + self.offsets[0]) * self.scale)
         if x_pos is not None and y_pos is not None:
             center_x = self.last_x + i_pos * self.scale
             center_y = self.last_y + j_pos * self.scale
-            self.arc_move(
-                self.last_x, self.last_y, self.x_pos, self.y_pos, center_x, center_y, 3
-            )
+            self.arc_move(self.last_x, self.last_y, self.x_pos, self.y_pos, center_x, center_y, 3)
             self.last_x = self.x_pos
             self.last_y = self.y_pos
 
     def get(self, numbers=False) -> str:  # pylint: disable=W0613
         output = ""
         last_word = ""
         for cmd in self.hpgl:
```

### Comparing `viaconstructor-0.6.6/viaconstructor/preview_plugins/gcode.py` & `viaconstructor-0.6.7/viaconstructor/preview_plugins/gcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,15 @@
                     self.linear_move(cords, True)
                 elif self.state["move_mode"] == 1:
                     self.linear_move(cords, False)
                 elif self.state["move_mode"] in {2, 3}:
                     if "R" in cords:
                         self.arc_move_r(self.state["move_mode"], cords, cords["R"])
                     elif "I" in ldata and "J" in ldata:
-                        self.arc_move_ij(
-                            self.state["move_mode"], cords, ldata["I"], ldata["J"]
-                        )
+                        self.arc_move_ij(self.state["move_mode"], cords, ldata["I"], ldata["J"])
 
         minp = {}
         maxp = {}
         for axis in ("X", "Y", "Z"):
             minp[axis] = self.path[0][0][axis]
             maxp[axis] = self.path[0][0][axis]
         for segment in self.path:
@@ -158,34 +156,26 @@
             movements.append((line[0]["X"], line[0]["Y"], line[0]["Z"]))
         minmax = self.get_minmax()
         size = self.get_size()
         stock_x = size[0] + tool_diameter * 4
         stock_y = size[1] + tool_diameter * 4
         stock_z = size[2] - minmax[5]
         tool_length = stock_z + 10
-        scad_data = [
-            f"module tool() {{cylinder(h={tool_length},d={tool_diameter},center=false,$fn={8});}}"
-        ]
-        scad_data.append(
-            f"module stock() {{translate(v=[{minmax[0] - tool_diameter * 2},{minmax[1] - tool_diameter * 2},{-stock_z}]) cube(size=[{stock_x},{stock_y},{stock_z}],center=false);}}"
-        )
+        scad_data = [f"module tool() {{cylinder(h={tool_length},d={tool_diameter},center=false,$fn={8});}}"]
+        scad_data.append(f"module stock() {{translate(v=[{minmax[0] - tool_diameter * 2},{minmax[1] - tool_diameter * 2},{-stock_z}]) cube(size=[{stock_x},{stock_y},{stock_z}],center=false);}}")
         scad_data.append("difference() {")
         scad_data.append("  stock();")
         scad_data.append("  union() {")
         for (s_x, s_y, s_z), (e_x, e_y, e_z) in zip(movements, movements[1:]):
-            scad_data.append(
-                f"    hull() {{translate(v=[{s_x},{s_y},{s_z}]) tool(); translate(v=[{e_x},{e_y},{e_z-0.01}]) tool();}}"
-            )
+            scad_data.append(f"    hull() {{translate(v=[{s_x},{s_y},{s_z}]) tool(); translate(v=[{e_x},{e_y},{e_z-0.01}]) tool();}}")
         scad_data.append("  }")
         scad_data.append("}")
         return "\n".join(scad_data)
 
-    def linear_move(
-        self, cords: dict, fast: bool = False  # pylint: disable=W0613
-    ) -> None:
+    def linear_move(self, cords: dict, fast: bool = False) -> None:  # pylint: disable=W0613
         for axis in self.state["position"]:
             if axis in cords:
                 cords[axis] /= self.state["scale"]
             else:
                 cords[axis] = self.state["position"][axis]
 
         self.path.append([self.state["position"], cords, self.state["spindle"]["dir"]])
@@ -202,17 +192,15 @@
         diff_y = cords["Y"] - last_pos["Y"]
         arc_r = cords["R"]
         if diff_x == 0.0 and diff_y == 0.0:
             return
         h_x2_div_d = 4.0 * arc_r * arc_r - diff_x * diff_x - diff_y * diff_y
         if h_x2_div_d < 0:
             print("### ARC ERROR ###")
-            self.path.append(
-                [self.state["position"], cords, self.state["spindle"]["dir"]]
-            )
+            self.path.append([self.state["position"], cords, self.state["spindle"]["dir"]])
             self.state["position"] = cords
             return
         h_x2_div_d = -math.sqrt(h_x2_div_d) / math.hypot(diff_x, diff_y)
         if angle_dir == 3:
             h_x2_div_d = -h_x2_div_d
         if arc_r < 0:
             h_x2_div_d = -h_x2_div_d
@@ -229,17 +217,15 @@
                 cords[axis] = self.state["position"][axis]
 
         last_pos = self.state["position"]
         center_x = last_pos["X"] + i
         center_y = last_pos["Y"] + j
         if radius is None:
             radius = calc_distance((center_x, center_y), (last_pos["X"], last_pos["Y"]))
-        start_angle = angle_of_line(
-            (center_x, center_y), (last_pos["X"], last_pos["Y"])
-        )
+        start_angle = angle_of_line((center_x, center_y), (last_pos["X"], last_pos["Y"]))
         end_angle = angle_of_line((center_x, center_y), (cords["X"], cords["Y"]))
 
         if angle_dir == 2:
             if start_angle < end_angle:
                 end_angle = end_angle - math.pi * 2
         elif angle_dir == 3:
             if start_angle > end_angle:
```

### Comparing `viaconstructor-0.6.6/viaconstructor/preview_plugins/hpgl.py` & `viaconstructor-0.6.7/viaconstructor/preview_plugins/hpgl.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,38 +50,26 @@
                 if line[0:2] == "AR":
                     center_x += last_x
                     center_y += last_y
                 angle = float(params[2])
                 # if len(params) == 4:
                 #    resolution = params[3]
                 radius = calc_distance((last_x, last_y), (center_x, center_y))
-                start_angle = (
-                    angle_of_line((last_x, last_y), (center_x, center_y))
-                    * 180
-                    / math.pi
-                )
+                start_angle = angle_of_line((last_x, last_y), (center_x, center_y)) * 180 / math.pi
                 if angle < 0:
                     for angle_set in range(0, int(abs(angle)) + 1):
-                        new_x = center_x + radius * math.sin(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
-                        new_y = center_y + radius * math.cos(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
+                        new_x = center_x + radius * math.sin((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
+                        new_y = center_y + radius * math.cos((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
                         self.linear_move({"X": new_x, "Y": new_y}, False)
                         last_x = new_x
                         last_y = new_y
                 else:
                     for angle_set in range(int(abs(angle)), -1, -1):
-                        new_x = center_x - radius * math.sin(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
-                        new_y = center_y - radius * math.cos(
-                            (start_angle + angle_set) * math.pi / 180 + math.pi / 2
-                        )
+                        new_x = center_x - radius * math.sin((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
+                        new_y = center_y - radius * math.cos((start_angle + angle_set) * math.pi / 180 + math.pi / 2)
                         self.linear_move({"X": new_x, "Y": new_y}, False)
                         last_x = new_x
                         last_y = new_y
 
                 line = ""
             elif line.startswith("PA"):
                 absolute = True
@@ -147,17 +135,15 @@
         if rounding:
             for segment in self.path:
                 for axis in ("X", "Y", "Z"):
                     segment[0][axis] = round(segment[0][axis], 6)
                     segment[1][axis] = round(segment[1][axis], 6)
         return self.path
 
-    def linear_move(
-        self, cords: dict, fast: bool = False  # pylint: disable=W0613
-    ) -> None:
+    def linear_move(self, cords: dict, fast: bool = False) -> None:  # pylint: disable=W0613
         for axis in self.state["position"]:
             if axis not in cords:
                 cords[axis] = self.state["position"][axis]
         self.path.append([self.state["position"], cords, self.state["spindle"]["dir"]])
         self.state["position"] = cords
 
     def arc_move_r(self, angle_dir, cords, radius) -> None:  # pylint: disable=W0613
@@ -169,17 +155,15 @@
         diff_y = cords["Y"] - last_pos["Y"]
         arc_r = cords["R"]
         if diff_x == 0.0 and diff_y == 0.0:
             return
         h_x2_div_d = 4.0 * arc_r * arc_r - diff_x * diff_x - diff_y * diff_y
         if h_x2_div_d < 0:
             print("### ARC ERROR ###")
-            self.path.append(
-                [self.state["position"], cords, self.state["spindle"]["dir"]]
-            )
+            self.path.append([self.state["position"], cords, self.state["spindle"]["dir"]])
             self.state["position"] = cords
             return
         h_x2_div_d = -math.sqrt(h_x2_div_d) / math.hypot(diff_x, diff_y)
         if angle_dir == 3:
             h_x2_div_d = -h_x2_div_d
         if arc_r < 0:
             h_x2_div_d = -h_x2_div_d
@@ -194,17 +178,15 @@
                 cords[axis] = self.state["position"][axis]
 
         last_pos = self.state["position"]
         center_x = last_pos["X"] + i
         center_y = last_pos["Y"] + j
         if radius is None:
             radius = calc_distance((center_x, center_y), (last_pos["X"], last_pos["Y"]))
-        start_angle = angle_of_line(
-            (center_x, center_y), (last_pos["X"], last_pos["Y"])
-        )
+        start_angle = angle_of_line((center_x, center_y), (last_pos["X"], last_pos["Y"]))
         end_angle = angle_of_line((center_x, center_y), (cords["X"], cords["Y"]))
 
         if angle_dir == 2:
             if start_angle < end_angle:
                 end_angle = end_angle - math.pi * 2
         elif angle_dir == 3:
             if start_angle > end_angle:
```

### Comparing `viaconstructor-0.6.6/viaconstructor/setupdefaults.py` & `viaconstructor-0.6.7/viaconstructor/setupdefaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,24 @@
                 "options": (
                     ("mm", _("mm")),
                     ("inch", _("inch")),
                 ),
                 "title": _("Unit"),
                 "tooltip": _("Unit of the machine"),
             },
+            "arcs": {
+                "default": "ij",
+                "type": "select",
+                "options": (
+                    ("ij", _("offset")),
+                    ("r", _("radius")),
+                ),
+                "title": _("Arcs-Mode (G2/G3)"),
+                "tooltip": _("Arcs-Mode - G2/G3 with IJ or R (experimental)"),
+            },
             "g54": {
                 "default": False,
                 "type": "bool",
                 "title": _("machine supports g54"),
                 "tooltip": _("machine supports g54"),
             },
             "supports_toolchange": {
```

### Comparing `viaconstructor-0.6.6/viaconstructor/tools/font.py` & `viaconstructor-0.6.7/viaconstructor/tools/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,16 +152,15 @@
                     continue
                 if char == "\n":
                     ctx["pos"][0] = 0  # type: ignore
                     ctx["pos"][1] -= 1000 * scale  # type: ignore
                     continue
                 face.load_char(
                     char,
-                    freetype.FT_LOAD_DEFAULT  # pylint: disable=E1101
-                    | freetype.FT_LOAD_NO_BITMAP,  # pylint: disable=E1101
+                    freetype.FT_LOAD_DEFAULT | freetype.FT_LOAD_NO_BITMAP,  # pylint: disable=E1101  # pylint: disable=E1101
                 )
                 face.glyph.outline.decompose(
                     ctx,
                     move_to=self.move_to,
                     line_to=self.line_to,
                     conic_to=self.conic_to,
                     cubic_to=self.cubic_to,
@@ -171,17 +170,15 @@
 
         except Exception as error:  # pylint: disable=W0703
             print(f"ERROR: while loading font file: {fontfile}: {error}")
 
         self.painter.end()
 
     def draw_line_preview(self, point, ctx):
-        self.painter.drawLine(
-            QLineF(ctx["last"][0], 90 - ctx["last"][1], point[0], 90 - point[1])
-        )
+        self.painter.drawLine(QLineF(ctx["last"][0], 90 - ctx["last"][1], point[0], 90 - point[1]))
 
     def move_to(self, point_a, ctx):
         point = (
             point_a.x * ctx["scale"][0] + ctx["pos"][0],
             point_a.y * ctx["scale"][1] + ctx["pos"][1],
         )
         ctx["max"] = max(ctx["max"], point[0])
```

### Comparing `viaconstructor-0.6.6/viaconstructor/tools/gear.py` & `viaconstructor-0.6.7/viaconstructor/tools/gear.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,17 @@
     outer_circle = Point(0.0, 0.0).buffer(outer_radius)
     # print(outer_circle)
 
     poly_list = []
     prev_X = None
     ll = 2 * tooth_width / pitch_radius
     for theta in numpy.linspace(0, ll, frame_count):
-        X = rotation(
-            profile + numpy.array((-theta * pitch_radius, pitch_radius)), theta
-        )
+        X = rotation(profile + numpy.array((-theta * pitch_radius, pitch_radius)), theta)
         if prev_X is not None:
-            poly_list.append(
-                MultiPoint([x for x in X] + [x for x in prev_X]).convex_hull
-            )
+            poly_list.append(MultiPoint([x for x in X] + [x for x in prev_X]).convex_hull)
         prev_X = X
 
     def circle_sector(angle, r):
         box_a = rotate(box(0.0, -2 * r, 2 * r, 2 * r), -angle / 2, Point(0.0, 0.0))
         box_b = rotate(box(-2 * r, -2 * r, 0, 2 * r), angle / 2, Point(0.0, 0.0))
         return Point(0.0, 0.0).buffer(r).difference(box_a.union(box_b))
 
@@ -170,17 +166,15 @@
                 teeth_count=teeth,
                 tooth_width=width,
                 pressure_angle=deg2rad(angle),
                 backlash=backlash,
                 frame_count=16,
             )
 
-            temp_file = tempfile.NamedTemporaryFile(
-                prefix=f"gear_{teeth}_{width}_{angle}_{backlash}_", suffix=".dxf"
-            )
+            temp_file = tempfile.NamedTemporaryFile(prefix=f"gear_{teeth}_{width}_{angle}_{backlash}_", suffix=".dxf")
             temp_file.close()
             output_file = temp_file.name
             print(f"saving gear to tempfile: {output_file}")
 
             doc = ezdxf.new("R2010")
             msp = doc.modelspace()
             doc.units = ezdxf.units.MM
```

### Comparing `viaconstructor-0.6.6/viaconstructor/vc_types.py` & `viaconstructor-0.6.7/viaconstructor/vc_types.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.6/viaconstructor/viaconstructor.py` & `viaconstructor-0.6.7/viaconstructor/viaconstructor.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,15 @@
     HAVE_NEST = True
 except Exception:  # pylint: disable=W0703
     HAVE_NEST = False
 
 reader_plugins: dict = {}
 for reader in ("dxfread", "hpglread", "stlread", "svgread", "ttfread", "imgread"):
     try:
-        drawing_reader = importlib.import_module(
-            f".{reader}", "viaconstructor.input_plugins"
-        )
+        drawing_reader = importlib.import_module(f".{reader}", "viaconstructor.input_plugins")
         reader_plugins[reader] = drawing_reader.DrawReader
     except Exception as reader_error:  # pylint: disable=W0703
         sys.stderr.write(f"ERRO while loading input plugin {reader}: {reader_error}\n")
 
 
 DEBUG = False
 TIMESTAMP = 0
@@ -136,30 +134,26 @@
 
 
 _ = no_translation
 lang = os.environ.get("LANGUAGE")
 if lang:
     localedir = os.path.join(Path(__file__).resolve().parent, "locales")
     try:
-        lang_translations = gettext.translation(
-            "base", localedir=localedir, languages=[lang]
-        )
+        lang_translations = gettext.translation("base", localedir=localedir, languages=[lang])
 
         lang_translations.install()
         _ = lang_translations.gettext
     except FileNotFoundError:
         sys.stderr.write(f"WARNING: localedir not found {localedir}\n")
 
 
 class ViaConstructor:  # pylint: disable=R0904
     """viaconstructor main class."""
 
-    LAYER_REGEX = re.compile(
-        r"([a-zA-Z]{1,4}):\s*([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))"
-    )
+    LAYER_REGEX = re.compile(r"([a-zA-Z]{1,4}):\s*([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))")
 
     project: dict = {
         "engine": "3D",
         "setup_defaults": setup_defaults(_),
         "filename_draw": "",
         "filename_machine_cmd": "",
         "suffix": "ngc",
@@ -221,17 +215,15 @@
                         )
                     else:
                         (
                             center,
                             start_angle,  # pylint: disable=W0612
                             end_angle,  # pylint: disable=W0612
                             radius,  # pylint: disable=W0612
-                        ) = ezdxf.math.bulge_to_arc(
-                            segment.start, segment.end, segment.bulge
-                        )
+                        ) = ezdxf.math.bulge_to_arc(segment.start, segment.end, segment.bulge)
                         msp.add_arc(
                             center=center,
                             radius=radius,
                             start_angle=start_angle * 180 / math.pi,
                             end_angle=end_angle * 180 / math.pi,
                             dxfattribs={"layer": segment.layer, "color": segment.color},
                         )
@@ -253,18 +245,15 @@
 
         debug("run_calculation: centercalc")
 
         psetup: dict = self.project["setup"]
         min_max = objects2minmax(self.project["objects"])
         self.project["minMax"] = min_max
         if psetup["workpiece"]["zero"] == "original":
-            if (
-                min_max[0] != self.project["origin"][0]
-                or min_max[1] != self.project["origin"][1]
-            ):
+            if min_max[0] != self.project["origin"][0] or min_max[1] != self.project["origin"][1]:
                 move_objects(self.project["objects"], -min_max[0], -min_max[1])
                 move_objects(
                     self.project["objects"],
                     self.project["origin"][0],
                     self.project["origin"][1],
                 )
         elif psetup["workpiece"]["zero"] == "bottomLeft":
@@ -292,17 +281,15 @@
             psetup,
             self.project["objects"],
             self.project["maxOuter"],
         )
 
         # create machine commands
         debug("run_calculation: machine_commands")
-        output_plugin: Union[
-            PostProcessorHpgl, PostProcessorGcodeLinuxCNC, PostProcessorGcodeGrbl
-        ]
+        output_plugin: Union[PostProcessorHpgl, PostProcessorGcodeLinuxCNC, PostProcessorGcodeGrbl]
         if self.project["setup"]["machine"]["plugin"] == "gcode_linuxcnc":
             output_plugin = PostProcessorGcodeLinuxCNC(
                 self.project,
             )
             self.project["suffix"] = output_plugin.suffix()
             self.project["axis"] = output_plugin.axis()
         elif self.project["setup"]["machine"]["plugin"] == "gcode_grbl":
@@ -314,17 +301,15 @@
         elif self.project["setup"]["machine"]["plugin"] == "hpgl":
             output_plugin = PostProcessorHpgl(
                 self.project,
             )
             self.project["suffix"] = output_plugin.suffix()
             self.project["axis"] = output_plugin.axis()
         else:
-            eprint(
-                f"ERROR: Unknown machine output plugin: {self.project['setup']['machine']['plugin']}"
-            )
+            eprint(f"ERROR: Unknown machine output plugin: {self.project['setup']['machine']['plugin']}")
             sys.exit(1)
         self.project["machine_cmd"] = polylines2machine_cmd(self.project, output_plugin)
         debug("run_calculation: update textwidget")
         if self.project["textwidget"]:
             self.project["textwidget"].clear()
             self.project["textwidget"].insertPlainText(self.project["machine_cmd"])
             self.project["textwidget"].verticalScrollBar().setValue(0)
@@ -428,22 +413,16 @@
                             )
 
         self.project["minMax"] = objects2minmax(self.project["objects"])
         self.update_tabs_data()
         self.update_drawing()
 
     def _toolbar_scale(self) -> None:
-        scale, dialog_ok = QInputDialog.getText(
-            self.project["window"], _("Workpiece-Scale"), _("Scale-Factor:"), text="1.0"
-        )
-        if (
-            dialog_ok
-            and str(scale).replace(".", "").isnumeric()
-            and float(scale) != 1.0
-        ):
+        scale, dialog_ok = QInputDialog.getText(self.project["window"], _("Workpiece-Scale"), _("Scale-Factor:"), text="1.0")
+        if dialog_ok and str(scale).replace(".", "").isnumeric() and float(scale) != 1.0:
             scale_objects(self.project["objects"], float(scale))
             self.project["minMax"] = objects2minmax(self.project["objects"])
             self.update_tabs_data()
             self.update_drawing()
 
     def _toolbar_view_2d(self) -> None:
         """center view."""
@@ -540,41 +519,33 @@
         else:
             eprint(f"STATUS: {message}")
 
     def _toolbar_save_machine_cmd(self) -> None:
         """save machine_cmd."""
         self.status_bar_message(f"{self.info} - save machine_cmd..")
         file_dialog = QFileDialog(self.main)
-        file_dialog.setNameFilters(
-            [f"{self.project['suffix']} (*.{self.project['suffix']})"]
-        )
-        self.project[
-            "filename_machine_cmd"
-        ] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
+        file_dialog.setNameFilters([f"{self.project['suffix']} (*.{self.project['suffix']})"])
+        self.project["filename_machine_cmd"] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
         name = file_dialog.getSaveFileName(
             self.main,
             "Save File",
             self.project["filename_machine_cmd"],
             f"{self.project['suffix']} (*.{self.project['suffix']})",
         )
         if name[0] and self.machine_cmd_save(name[0]):
-            self.status_bar_message(
-                f"{self.info} - save machine-code..done ({name[0]})"
-            )
+            self.status_bar_message(f"{self.info} - save machine-code..done ({name[0]})")
         else:
             self.status_bar_message(f"{self.info} - save machine-code..cancel")
 
     def _toolbar_save_dxf(self) -> None:
         """save doawing as dxf."""
         self.status_bar_message(f"{self.info} - save drawing as dxf..")
         file_dialog = QFileDialog(self.main)
         file_dialog.setNameFilters(["dxf (*.dxf)"])
-        self.project[
-            "filename_machine_cmd"
-        ] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.dxf"
+        self.project["filename_machine_cmd"] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.dxf"
         name = file_dialog.getSaveFileName(
             self.main,
             "Save File",
             self.project["filename_machine_cmd"],
             "dxf (*.dxf)",
         )
         if name[0] and self.save_objects_as_dxf(name[0]):
@@ -583,20 +554,16 @@
             self.status_bar_message(f"{self.info} - save dxf..cancel")
 
     def _toolbar_save_project(self) -> None:
         """save project."""
         self.status_bar_message(f"{self.info} - save project..")
         file_dialog = QFileDialog(self.main)
         file_dialog.setNameFilters(["vcp (*.vcp)"])
-        filename_default = (
-            f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.vcp"
-        )
-        self.project[
-            "filename_machine_cmd"
-        ] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.vcp"
+        filename_default = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.vcp"
+        self.project["filename_machine_cmd"] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.vcp"
         name = file_dialog.getSaveFileName(
             self.main,
             "Save File",
             filename_default,
             "vcp (*.vcp)",
         )
         if name[0]:
@@ -686,17 +653,15 @@
             self.status_bar_message(f"{self.info} - save setup..error")
 
     def _toolbar_load_setup_from(self) -> None:
         """load setup from."""
         self.status_bar_message(f"{self.info} - load setup from..")
         file_dialog = QFileDialog(self.main)
         file_dialog.setNameFilters(["setup (*.json)"])
-        name = file_dialog.getOpenFileName(
-            self.main, "Load Setup", self.args.setup, "setup (*.json)"
-        )
+        name = file_dialog.getOpenFileName(self.main, "Load Setup", self.args.setup, "setup (*.json)")
         if name[0] and self.setup_load(name[0]):
             self.project["status"] = "CHANGE"
             self.update_global_setup()
             self.update_object_setup()
             self.global_changed(0)
             self.update_drawing()
             self.project["status"] = "READY"
@@ -705,17 +670,15 @@
             self.status_bar_message(f"{self.info} - load setup from..cancel")
 
     def _toolbar_save_setup_as(self) -> None:
         """save setup as."""
         self.status_bar_message(f"{self.info} - save setup as..")
         file_dialog = QFileDialog(self.main)
         file_dialog.setNameFilters(["setup (*.json)"])
-        name = file_dialog.getSaveFileName(
-            self.main, "Save Setup", self.args.setup, "setup (*.json)"
-        )
+        name = file_dialog.getSaveFileName(self.main, "Save Setup", self.args.setup, "setup (*.json)")
         if name[0] and self.setup_save(name[0]):
             self.status_bar_message(f"{self.info} - save setup as..done ({name[0]})")
         else:
             self.status_bar_message(f"{self.info} - ave setup as..cancel")
 
     def _toolbar_load_setup_from_drawing(self) -> None:
         if self.project["draw_reader"].can_load_setup:  # type: ignore
@@ -725,23 +688,19 @@
                 self.update_object_setup()
                 self.global_changed(0)
                 self.prepare_segments()
                 self.update_drawing()
                 self.project["status"] = "READY"
                 self.status_bar_message(f"{self.info} - load setup from drawing..done")
             else:
-                self.status_bar_message(
-                    f"{self.info} - load setup from drawing..failed"
-                )
+                self.status_bar_message(f"{self.info} - load setup from drawing..failed")
 
     def _toolbar_save_setup_to_drawing(self) -> None:
         if self.project["draw_reader"].can_save_setup:  # type: ignore
-            self.project["draw_reader"].save_setup(  # type: ignore
-                json.dumps(self.project["setup"], indent=4, sort_keys=True)
-            )
+            self.project["draw_reader"].save_setup(json.dumps(self.project["setup"], indent=4, sort_keys=True))  # type: ignore
             self.status_bar_message(f"{self.info} - save setup to drawing..done")
 
     def toggle_layer(self, item):
         layer = self.project["layerwidget"].item(item.row(), 0).text()
         self.project["layers"][layer] = not self.project["layers"][layer]
         self.update_layers()
 
@@ -754,17 +713,15 @@
 
     def update_layers(self) -> None:
         if "layerwidget" in self.project:
             self.project["layerwidget"].setRowCount(len(self.project["layers"]))
             row_idx = 0
             for layer, enabled in self.project["layers"].items():
                 self.project["layerwidget"].setItem(row_idx, 0, QTableWidgetItem(layer))
-                self.project["layerwidget"].setItem(
-                    row_idx, 1, QTableWidgetItem("enabled" if enabled else "disabled")
-                )
+                self.project["layerwidget"].setItem(row_idx, 1, QTableWidgetItem("enabled" if enabled else "disabled"))
                 row_idx += 1
 
     def update_drawing(self, draw_only=False) -> None:
         """update drawings."""
         if not self.project["draw_reader"]:
             return
 
@@ -877,40 +834,32 @@
         if diameter is None:
             print("ERROR: nest: TOOL not found")
             return
 
         unit = self.project["setup"]["machine"]["unit"]
         if unit == "inch":
             diameter *= 25.4
-        tool_vc = self.project["setup"]["workpiece"]["materialtable"][material_idx][
-            "vc"
-        ]
+        tool_vc = self.project["setup"]["workpiece"]["materialtable"][material_idx]["vc"]
         tool_speed = tool_vc * 1000 / (diameter * math.pi)
         tool_speed = int(min(tool_speed, machine_toolspeed))
         if diameter <= 4.0:
             fz_key = "fz4"
         elif diameter <= 8.0:
             fz_key = "fz8"
         else:
             fz_key = "fz12"
-        material_fz = self.project["setup"]["workpiece"]["materialtable"][material_idx][
-            fz_key
-        ]
+        material_fz = self.project["setup"]["workpiece"]["materialtable"][material_idx][fz_key]
         feedrate = tool_speed * blades * material_fz
         feedrate = int(min(feedrate, machine_feedrate))
 
         info_test = []
         info_test.append("Some Milling and Tool Values will be changed:")
         info_test.append("")
-        info_test.append(
-            f" Feedrate: {feedrate} {'(!MACHINE-LIMIT)' if feedrate == machine_feedrate else ''}"
-        )
-        info_test.append(
-            f" Tool-Speed: {tool_speed} {'(!MACHINE-LIMIT)' if tool_speed == machine_toolspeed else ''}"
-        )
+        info_test.append(f" Feedrate: {feedrate} {'(!MACHINE-LIMIT)' if feedrate == machine_feedrate else ''}")
+        info_test.append(f" Tool-Speed: {tool_speed} {'(!MACHINE-LIMIT)' if tool_speed == machine_toolspeed else ''}")
         info_test.append("")
         ret = QMessageBox.question(
             self.main,  # type: ignore
             "Warning",
             "\n".join(info_test),
             QMessageBox.Ok | QMessageBox.Cancel,  # type: ignore
         )
@@ -929,17 +878,15 @@
         self.update_object_setup()
         self.update_drawing()
         self.project["status"] = "READY"
 
     def tools_select(self, tool_idx) -> None:
         self.project["status"] = "CHANGE"
         old_tool_number = self.project["setup"]["tool"]["number"]
-        new_tool_number = int(
-            self.project["setup"]["tool"]["tooltable"][tool_idx]["number"]
-        )
+        new_tool_number = int(self.project["setup"]["tool"]["tooltable"][tool_idx]["number"])
         self.project["setup"]["tool"]["number"] = new_tool_number
         for obj in self.project["objects"].values():
             if obj.setup["tool"]["number"] == old_tool_number:
                 obj.setup["tool"]["number"] = new_tool_number
         self.update_global_setup()
         self.update_object_setup()
         self.global_changed(0)
@@ -1060,40 +1007,24 @@
                     for row_idx in range(entry["widget_obj"].rowCount()):
                         col_idx = 0
                         for key, col_type in entry["columns"].items():
                             if entry["widget_obj"].item(row_idx, col_idx + 1) is None:
                                 print("TABLE_ERROR")
                                 continue
                             if col_type["type"] == "str":
-                                value = (
-                                    entry["widget_obj"]
-                                    .item(row_idx, col_idx + 1)
-                                    .text()
-                                )
+                                value = entry["widget_obj"].item(row_idx, col_idx + 1).text()
                                 setup_data[sname][ename][row_idx][key] = str(value)
                             elif col_type["type"] == "mstr":
-                                value = (
-                                    entry["widget_obj"]
-                                    .item(row_idx, col_idx + 1)
-                                    .toPlainText()
-                                )
+                                value = entry["widget_obj"].item(row_idx, col_idx + 1).toPlainText()
                                 setup_data[sname][ename][row_idx][key] = str(value)
                             elif col_type["type"] == "int":
-                                value = (
-                                    entry["widget_obj"]
-                                    .item(row_idx, col_idx + 1)
-                                    .text()
-                                )
+                                value = entry["widget_obj"].item(row_idx, col_idx + 1).text()
                                 setup_data[sname][ename][row_idx][key] = int(value)
                             elif col_type["type"] == "float":
-                                value = (
-                                    entry["widget_obj"]
-                                    .item(row_idx, col_idx + 1)
-                                    .text()
-                                )
+                                value = entry["widget_obj"].item(row_idx, col_idx + 1).text()
                                 setup_data[sname][ename][row_idx][key] = float(value)
                             col_idx += 1
                 elif entry["type"] == "color":
                     pass
                 else:
                     eprint(f"Unknown setup-type: {entry['type']}")
                 if setup_data[sname][ename] != self.project["setup"][sname][ename]:
@@ -1140,43 +1071,25 @@
                     for row_idx in range(entry["widget"].rowCount()):
                         col_idx = 0
                         for key, col_type in entry["columns"].items():
                             if entry["widget"].item(row_idx, col_idx + 1) is None:
                                 print("TABLE_ERROR")
                                 continue
                             if col_type["type"] == "str":
-                                value = (
-                                    entry["widget"].item(row_idx, col_idx + 1).text()
-                                )
-                                self.project["setup"][sname][ename][row_idx][key] = str(
-                                    value
-                                )
+                                value = entry["widget"].item(row_idx, col_idx + 1).text()
+                                self.project["setup"][sname][ename][row_idx][key] = str(value)
                             elif col_type["type"] == "mstr":
-                                value = (
-                                    entry["widget"]
-                                    .item(row_idx, col_idx + 1)
-                                    .toPlainText()
-                                )
-                                self.project["setup"][sname][ename][row_idx][key] = str(
-                                    value
-                                )
+                                value = entry["widget"].item(row_idx, col_idx + 1).toPlainText()
+                                self.project["setup"][sname][ename][row_idx][key] = str(value)
                             elif col_type["type"] == "int":
-                                value = (
-                                    entry["widget"].item(row_idx, col_idx + 1).text()
-                                )
-                                self.project["setup"][sname][ename][row_idx][key] = int(
-                                    value
-                                )
+                                value = entry["widget"].item(row_idx, col_idx + 1).text()
+                                self.project["setup"][sname][ename][row_idx][key] = int(value)
                             elif col_type["type"] == "float":
-                                value = (
-                                    entry["widget"].item(row_idx, col_idx + 1).text()
-                                )
-                                self.project["setup"][sname][ename][row_idx][
-                                    key
-                                ] = float(value)
+                                value = entry["widget"].item(row_idx, col_idx + 1).text()
+                                self.project["setup"][sname][ename][row_idx][key] = float(value)
                             col_idx += 1
                 elif entry["type"] == "color":
                     pass
                 else:
                     eprint(f"Unknown setup-type: {entry['type']}")
 
         if self.project["setup"]["mill"]["step"] >= 0.0:
@@ -1187,47 +1100,38 @@
 
         self.project["segments"] = deepcopy(self.project["segments_org"])
         self.project["segments"] = clean_segments(self.project["segments"])
         for obj in self.project["objects"].values():
             for sect in ("mill", "tool", "pockets", "tabs", "leads"):
                 for key, global_value in self.project["setup"][sect].items():
                     # change object value only if the value changed and the value diffs again the last value in global
-                    if (
-                        global_value != old_setup[sect][key]
-                        and obj["setup"][sect][key] == old_setup[sect][key]
-                    ):
+                    if global_value != old_setup[sect][key] and obj["setup"][sect][key] == old_setup[sect][key]:
                         obj["setup"][sect][key] = self.project["setup"][sect][key]
 
         self.project["maxOuter"] = find_tool_offsets(self.project["objects"])
         self.update_object_setup()
 
         if not self.project["setup"]["view"]["autocalc"]:
             return
         self.update_drawing()
 
     def _toolbar_load_machine_cmd_setup(self) -> None:
-        self.project[
-            "filename_machine_cmd"
-        ] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
+        self.project["filename_machine_cmd"] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
         if os.path.isfile(self.project["filename_machine_cmd"]):
-            self.status_bar_message(
-                f"{self.info} - loading setup from machinecode: {self.project['filename_machine_cmd']}"
-            )
+            self.status_bar_message(f"{self.info} - loading setup from machinecode: {self.project['filename_machine_cmd']}")
             with open(self.project["filename_machine_cmd"], "r") as fd_machine_cmd:
                 gdata = fd_machine_cmd.read()
                 for g_line in gdata.split("\n"):
                     if g_line.startswith("(setup={"):
                         setup_json = g_line.strip("()").split("=", 1)[1]
                         ndata = json.loads(setup_json)
                         for sname in self.project["setup"]:
                             self.project["setup"][sname].update(ndata.get(sname, {}))
                         self.update_drawing()
-                        self.status_bar_message(
-                            f"{self.info} - loading setup from machinecode..done"
-                        )
+                        self.status_bar_message(f"{self.info} - loading setup from machinecode..done")
                         return
         self.status_bar_message(f"{self.info} - loading setup from machinecode..failed")
 
     def _toolbar_load_tooltable(self) -> None:
         """load tooltable."""
         self.status_bar_message(f"{self.info} - load tooltable..")
         file_dialog = QFileDialog(self.main)
@@ -1238,17 +1142,15 @@
             "",
             "tooltables (*.json *.tbl);;linuxcnc (*.tbl);;camotics (*.json)",
         )
         if name[0]:
             try:
                 tooldata = open(name[0], "r").read()
             except Exception as save_error:  # pylint: disable=W0703
-                self.status_bar_message(
-                    f"{self.info} - load tooltable ..failed ({save_error})"
-                )
+                self.status_bar_message(f"{self.info} - load tooltable ..failed ({save_error})")
 
             ret = QMessageBox.question(
                 self.main,  # type: ignore
                 "Ask",
                 "Replacing the tooltable ?",
                 QMessageBox.Yes | QMessageBox.No,  # type: ignore
             )
@@ -1339,29 +1241,23 @@
 
             elif name[0].endswith(".tbl"):
                 tooltable_tbl = []
                 for tool in self.project["setup"]["tool"]["tooltable"]:
                     number = str(tool["number"])
                     if number == "99":
                         continue
-                    tooltable_tbl.append(
-                        f"T{number} P{number} Z{0.0} D{tool['diameter']} ;{tool['name']} / blades:{tool['blades']}"
-                    )
+                    tooltable_tbl.append(f"T{number} P{number} Z{0.0} D{tool['diameter']} ;{tool['name']} / blades:{tool['blades']}")
                 tooltable_tbl.append("")
                 tooldata = "\n".join(tooltable_tbl)
 
             try:
                 open(name[0], "w").write(tooldata)
-                self.status_bar_message(
-                    f"{self.info} - save tooltable as..done ({name[0]})"
-                )
+                self.status_bar_message(f"{self.info} - save tooltable as..done ({name[0]})")
             except Exception as save_error:  # pylint: disable=W0703
-                self.status_bar_message(
-                    f"{self.info} - save tooltable as..failed ({save_error})"
-                )
+                self.status_bar_message(f"{self.info} - save tooltable as..failed ({save_error})")
         else:
             self.status_bar_message(f"{self.info} - save tooltable as..cancel")
 
     def _toolbar_exit(self) -> None:
         """exit button."""
         if os.environ.get("LINUXCNCVERSION"):
             print(self.project["machine_cmd"])
@@ -1835,46 +1731,34 @@
                     entry["widget"].setText(self.project["setup"][sname][ename])
                 elif entry["type"] == "mstr":
                     entry["widget"].setPlainText(self.project["setup"][sname][ename])
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
 
-                    if (
-                        entry.get("column_defaults") is not None
-                        and str(self.project["setup"][sname][ename][-1][first_element])
-                        != ""
-                    ):
+                    if entry.get("column_defaults") is not None and str(self.project["setup"][sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         self.project["setup"][sname][ename].append(new_row)
 
                     table = entry["widget"]
                     table.setRowCount(len(self.project["setup"][sname][ename]))
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
                     for col_idx, title in enumerate(entry["columns"]):
-                        table.setHorizontalHeaderItem(
-                            col_idx + idxf_offset, QTableWidgetItem(title)
-                        )
+                        table.setHorizontalHeaderItem(col_idx + idxf_offset, QTableWidgetItem(title))
                     for row_idx, row in enumerate(self.project["setup"][sname][ename]):
                         if entry["selectable"]:
                             button = QPushButton()
-                            button.setIcon(
-                                QIcon(
-                                    os.path.join(
-                                        self.module_root, "icons", "select.png"
-                                    )
-                                )
-                            )
+                            button.setIcon(QIcon(os.path.join(self.module_root, "icons", "select.png")))
                             button.setToolTip(_("select this row"))
                             button.clicked.connect(partial(self.table_select, sname, ename, row_idx))  # type: ignore
                             table.setCellWidget(row_idx, 0, button)
                             table.resizeColumnToContents(0)
                         for col_idx, key in enumerate(entry["columns"]):
                             table.setItem(
                                 row_idx,
@@ -1972,19 +1856,15 @@
                     mlineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
                     mlineedit.textChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(mlineedit)
                     entry["widget"] = mlineedit
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
-                    if (
-                        entry.get("column_defaults") is not None
-                        and str(self.project["setup"][sname][ename][-1][first_element])
-                        != ""
-                    ):
+                    if entry.get("column_defaults") is not None and str(self.project["setup"][sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         self.project["setup"][sname][ename].append(new_row)
 
                     table = QTableWidget()
                     label.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
@@ -1992,27 +1872,19 @@
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
                     for col_idx, title in enumerate(entry["columns"]):
-                        table.setHorizontalHeaderItem(
-                            col_idx + idxf_offset, QTableWidgetItem(title)
-                        )
+                        table.setHorizontalHeaderItem(col_idx + idxf_offset, QTableWidgetItem(title))
                     for row_idx, row in enumerate(self.project["setup"][sname][ename]):
                         if entry["selectable"]:
                             button = QPushButton()
-                            button.setIcon(
-                                QIcon(
-                                    os.path.join(
-                                        self.module_root, "icons", "select.png"
-                                    )
-                                )
-                            )
+                            button.setIcon(QIcon(os.path.join(self.module_root, "icons", "select.png")))
                             button.setToolTip(_("select this row"))
                             button.clicked.connect(partial(self.table_select, sname, ename, row_idx))  # type: ignore
                             table.setCellWidget(row_idx, 0, button)
                             table.resizeColumnToContents(0)
                         for col_idx, key in enumerate(entry["columns"]):
                             item = QTableWidgetItem(str(row[key]))
                             table.setItem(
@@ -2102,45 +1974,34 @@
                     entry["widget_obj"].setText(setup_data[sname][ename])
                 elif entry["type"] == "mstr":
                     entry["widget_obj"].setPlainText(setup_data[sname][ename])
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
 
-                    if (
-                        entry.get("column_defaults") is not None
-                        and str(setup_data[sname][ename][-1][first_element]) != ""
-                    ):
+                    if entry.get("column_defaults") is not None and str(setup_data[sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         setup_data[sname][ename].append(new_row)
 
                     table = entry["widget_obj"]
                     table.setRowCount(len(setup_data[sname][ename]))
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
                     for col_idx, title in enumerate(entry["columns"]):
-                        table.setHorizontalHeaderItem(
-                            col_idx + idxf_offset, QTableWidgetItem(title)
-                        )
+                        table.setHorizontalHeaderItem(col_idx + idxf_offset, QTableWidgetItem(title))
                     for row_idx, row in enumerate(setup_data[sname][ename]):
                         if entry["selectable"]:
                             button = QPushButton()
-                            button.setIcon(
-                                QIcon(
-                                    os.path.join(
-                                        self.module_root, "icons", "select.png"
-                                    )
-                                )
-                            )
+                            button.setIcon(QIcon(os.path.join(self.module_root, "icons", "select.png")))
                             button.setToolTip(_("select this row"))
                             button.clicked.connect(partial(self.table_select, sname, ename, row_idx))  # type: ignore
                             table.setCellWidget(row_idx, 0, button)
                             table.resizeColumnToContents(0)
                         for col_idx, key in enumerate(entry["columns"]):
                             table.setItem(
                                 row_idx,
@@ -2250,19 +2111,15 @@
                     mlineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
                     mlineedit.textChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(mlineedit)
                     entry["widget_obj"] = mlineedit
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
-                    if (
-                        entry.get("column_defaults") is not None
-                        and str(self.project["setup"][sname][ename][-1][first_element])
-                        != ""
-                    ):
+                    if entry.get("column_defaults") is not None and str(self.project["setup"][sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         self.project["setup"][sname][ename].append(new_row)
 
                     table = QTableWidget()
                     table.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
@@ -2270,27 +2127,19 @@
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
                     for col_idx, title in enumerate(entry["columns"]):
-                        table.setHorizontalHeaderItem(
-                            col_idx + idxf_offset, QTableWidgetItem(title)
-                        )
+                        table.setHorizontalHeaderItem(col_idx + idxf_offset, QTableWidgetItem(title))
                     for row_idx, row in enumerate(self.project["setup"][sname][ename]):
                         if entry["selectable"]:
                             button = QPushButton()
-                            button.setIcon(
-                                QIcon(
-                                    os.path.join(
-                                        self.module_root, "icons", "select.png"
-                                    )
-                                )
-                            )
+                            button.setIcon(QIcon(os.path.join(self.module_root, "icons", "select.png")))
                             button.setToolTip(_("select this row"))
                             button.clicked.connect(partial(self.table_select, sname, ename, row_idx))  # type: ignore
                             table.setCellWidget(row_idx, 0, button)
                             table.resizeColumnToContents(0)
                         for col_idx, key in enumerate(entry["columns"]):
                             item = QTableWidgetItem(str(row[key]))
                             table.setItem(
@@ -2402,17 +2251,15 @@
             object_active_obj = None
             for obj_idx, obj in self.project["objects"].items():
                 if obj_idx.startswith(f"{object_active}:"):
                     object_active_obj = obj
 
             center = points_to_center(object2points(object_active_obj))
 
-            rotate_object(
-                object_active_obj, center[0], center[1], angle * math.pi / 180.0
-            )
+            rotate_object(object_active_obj, center[0], center[1], angle * math.pi / 180.0)
             if with_childs:
                 for inner in object_active_obj["inner_objects"]:
                     rotate_object(
                         self.project["objects"][inner],
                         center[0],
                         center[1],
                         angle * math.pi / 180.0,
@@ -2465,17 +2312,15 @@
 
             center = points_to_center(object2points(object_active_obj))
             move_object(object_active_obj, -center[0], -center[1])
             scale_object(object_active_obj, scale)
             move_object(object_active_obj, center[0], center[1])
             if with_childs:
                 for inner in object_active_obj["inner_objects"]:
-                    center = points_to_center(
-                        object2points(self.project["objects"][inner])
-                    )
+                    center = points_to_center(object2points(self.project["objects"][inner]))
                     move_object(self.project["objects"][inner], -center[0], -center[1])
                     scale_object(self.project["objects"][inner], scale)
                     move_object(self.project["objects"][inner], center[0], center[1])
 
             self.update_tabs_data()
             self.update_drawing()
 
@@ -2512,17 +2357,15 @@
             main_idx = obj_idx.split(":")[0]
             main_uid = obj_idx.split(":")[1]
             idx_list = [oid.split(":")[0] for oid in self.project["objects"]]
             sub_idx = 1
             while f"{main_idx},{sub_idx}" in idx_list:
                 sub_idx += 1
             new_obj_idx = f"{main_idx},{sub_idx}:{main_uid}"
-            self.project["objects"][new_obj_idx] = deepcopy(
-                self.project["objects"][obj_idx]
-            )
+            self.project["objects"][new_obj_idx] = deepcopy(self.project["objects"][obj_idx])
 
             move_object(
                 self.project["objects"][new_obj_idx],
                 offset_x,
                 offset_y,
             )
             return new_obj_idx
@@ -2534,39 +2377,25 @@
             object_active_obj = None
             object_active_obj_idx = ""
             for obj_idx, obj in self.project["objects"].items():
                 if obj_idx.startswith(f"{object_active}:"):
                     object_active_obj = obj
                     object_active_obj_idx = obj_idx
 
-            bounding_box = points_to_boundingbox(
-                object2points(self.project["objects"][object_active_obj_idx])
-            )
+            bounding_box = points_to_boundingbox(object2points(self.project["objects"][object_active_obj_idx]))
             offset_x = 0
             offset_y = 0
             if offset_direction == "left":
-                offset_x = (
-                    0 - (bounding_box[2] - bounding_box[0]) - bounding_box[0] - 10
-                )
+                offset_x = 0 - (bounding_box[2] - bounding_box[0]) - bounding_box[0] - 10
             elif offset_direction == "right":
-                offset_x = (
-                    (self.project["minMax"][2] - self.project["minMax"][0])
-                    - bounding_box[0]
-                    + 10
-                )
+                offset_x = (self.project["minMax"][2] - self.project["minMax"][0]) - bounding_box[0] + 10
             elif offset_direction == "top":
-                offset_y = (
-                    (self.project["minMax"][3] - self.project["minMax"][1])
-                    - bounding_box[1]
-                    + 10
-                )
+                offset_y = (self.project["minMax"][3] - self.project["minMax"][1]) - bounding_box[1] + 10
             elif offset_direction == "bottom":
-                offset_y = (
-                    0 - (bounding_box[3] - bounding_box[1]) - bounding_box[1] - 10
-                )
+                offset_y = 0 - (bounding_box[3] - bounding_box[1]) - bounding_box[1] - 10
 
             new_obj_idx = clone_object(object_active_obj_idx, offset_x, offset_y)
             if new_obj_idx is not None and with_childs:
                 for inner in object_active_obj["inner_objects"]:
                     clone_object(inner, offset_x, offset_y)
 
             self.combobjwidget.clear()
@@ -2732,31 +2561,25 @@
             dialog.setLayout(dialog.layout)  # type: ignore
 
             if dialog.exec():
                 plugin_name = combobox.currentText()
                 reader_plugin = reader_plugins[plugin_name]
 
         reader_plugin = reader_plugins[plugin_name]
-        if (
-            not no_setup
-            and self.main is not None
-            and hasattr(reader_plugin, "preload_setup")
-        ):
+        if not no_setup and self.main is not None and hasattr(reader_plugin, "preload_setup"):
             reader_plugin.preload_setup(filename, self.args)
         self.project["draw_reader"] = reader_plugin(filename, self.args)
         if reader_plugin.can_save_tabs:
             self.save_tabs = "ask"
 
         if self.project["draw_reader"]:
             debug("load_drawing: get segments")
             self.project["segments_org"] = self.project["draw_reader"].get_segments()
             self.project["filename_draw"] = filename
-            self.project[
-                "filename_machine_cmd"
-            ] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
+            self.project["filename_machine_cmd"] = f"{'.'.join(self.project['filename_draw'].split('.')[:-1])}.{self.project['suffix']}"
             debug("load_drawing: prepare_segments")
             self.prepare_segments()
             debug("load_drawing: done")
 
             # disable some options on big drawings for a better view
             if len(self.project["objects"]) >= 50:
                 self.project["setup"]["view"]["autocalc"] = False
@@ -2790,17 +2613,15 @@
                 print("ERROR: nest: TOOL not found")
                 return
 
             scad_data = parser.openscad(diameter)
             open(f"{TEMP_PREFIX}viaconstructor-preview.scad", "w").write(scad_data)
 
             def openscad_show():
-                process = subprocess.Popen(
-                    [openscad, f"{TEMP_PREFIX}viaconstructor-preview.scad"]
-                )
+                process = subprocess.Popen([openscad, f"{TEMP_PREFIX}viaconstructor-preview.scad"])
                 while True:
                     time.sleep(0.5)
                     return_code = process.poll()
                     if return_code is not None:
                         break
                 self.project["preview_open"].setEnabled(True)
                 os.remove(f"{TEMP_PREFIX}viaconstructor-preview.scad")
@@ -2839,25 +2660,19 @@
                 "resolution": 0.294723,
                 "tools": tools,
                 "files": [
                     f"{TEMP_PREFIX}viaconstructor-preview.ngc",
                 ],
             }
 
-            open(f"{TEMP_PREFIX}viaconstructor-preview.ngc", "w").write(
-                self.project["machine_cmd"]
-            )
-            open(f"{TEMP_PREFIX}viaconstructor-preview.camotics", "w").write(
-                json.dumps(camotics_data, indent=4, sort_keys=True)
-            )
+            open(f"{TEMP_PREFIX}viaconstructor-preview.ngc", "w").write(self.project["machine_cmd"])
+            open(f"{TEMP_PREFIX}viaconstructor-preview.camotics", "w").write(json.dumps(camotics_data, indent=4, sort_keys=True))
 
             def camotics_show():
-                process = subprocess.Popen(
-                    [camotics, f"{TEMP_PREFIX}viaconstructor-preview.camotics"]
-                )
+                process = subprocess.Popen([camotics, f"{TEMP_PREFIX}viaconstructor-preview.camotics"])
                 while True:
                     time.sleep(0.5)
                     return_code = process.poll()
                     if return_code is not None:
                         break
                 os.remove(f"{TEMP_PREFIX}viaconstructor-preview.camotics")
                 os.remove(f"{TEMP_PREFIX}viaconstructor-preview.ngc")
@@ -2876,39 +2691,33 @@
                 print("ERROR: nest: TOOL not found")
                 return
 
             scad_data = parser.openscad(diameter)
             open(f"{TEMP_PREFIX}viaconstructor-preview.scad", "w").write(scad_data)
 
             def openscad_convert():
-                os.system(
-                    f"{openscad} -o {TEMP_PREFIX}viaconstructor-preview.png {TEMP_PREFIX}viaconstructor-preview.scad"
-                )
+                os.system(f"{openscad} -o {TEMP_PREFIX}viaconstructor-preview.png {TEMP_PREFIX}viaconstructor-preview.scad")
                 image = QImage(f"{TEMP_PREFIX}viaconstructor-preview.png")
                 self.project["imgwidget"].setPixmap(QPixmap.fromImage(image))
                 self.project["preview_generate"].setEnabled(True)
                 self.project["preview_generate"].setText(_("generate Preview"))
                 os.remove(f"{TEMP_PREFIX}viaconstructor-preview.scad")
 
             self.project["preview_generate"].setEnabled(False)
-            self.project["preview_generate"].setText(
-                _("generating preview image with openscad.... please wait")
-            )
+            self.project["preview_generate"].setText(_("generating preview image with openscad.... please wait"))
             threading.Thread(target=openscad_convert).start()
 
     def __init__(self) -> None:
         """viaconstructor main init."""
         debug("main: startup")
         setproctitle.setproctitle("viaconstructor")  # pylint: disable=I1101
 
         # arguments
         parser = argparse.ArgumentParser()
-        parser.add_argument(
-            "filename", help="input file", type=str, nargs="?", default=None
-        )
+        parser.add_argument("filename", help="input file", type=str, nargs="?", default=None)
         parser.add_argument(
             "--engine",
             help="display engine",
             type=str,
             default="3D",
         )
         parser.add_argument(
@@ -3001,17 +2810,15 @@
         if self.project["engine"] == "2D":
             self.project["glwidget"] = CanvasWidget(self.project, self.update_drawing)
         else:
             self.project["glwidget"] = GLWidget(self.project, self.update_drawing)
 
         self.project["imgwidget"] = QLabel()
         self.project["imgwidget"].setBackgroundRole(QPalette.Base)  # type: ignore
-        self.project["imgwidget"].setSizePolicy(
-            QSizePolicy.Ignored, QSizePolicy.Ignored  # type: ignore
-        )
+        self.project["imgwidget"].setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Ignored)  # type: ignore
         self.project["imgwidget"].setScaledContents(True)
 
         self.main = QMainWindow()
         self.main.setWindowTitle("viaConstructor")
         self.main.setCentralWidget(self.project["window"])
 
         self.this_dir, self.this_filename = os.path.split(__file__)
@@ -3038,33 +2845,25 @@
         if openscad or camotics:
             preview = QWidget()
             preview.setContentsMargins(0, 0, 0, 0)
             preview_vbox = QVBoxLayout(preview)
             preview_vbox.setContentsMargins(0, 0, 0, 0)
             if openscad:
                 self.project["preview_generate"] = QPushButton(_("generate Preview"))
-                self.project["preview_generate"].setToolTip(
-                    _("this may take some time")
-                )
+                self.project["preview_generate"].setToolTip(_("this may take some time"))
                 self.project["preview_generate"].pressed.connect(self.generate_preview)
                 preview_vbox.addWidget(self.project["preview_generate"])
                 self.project["preview_open"] = QPushButton(_("view in openscad"))
                 self.project["preview_open"].setToolTip(_("open's preview in openscad"))
-                self.project["preview_open"].pressed.connect(
-                    self.open_preview_in_openscad
-                )
+                self.project["preview_open"].pressed.connect(self.open_preview_in_openscad)
                 preview_vbox.addWidget(self.project["preview_open"])
             if camotics:
                 self.project["preview_open2"] = QPushButton(_("view in camotics"))
-                self.project["preview_open2"].setToolTip(
-                    _("open's preview in camotics")
-                )
-                self.project["preview_open2"].pressed.connect(
-                    self.open_preview_in_camotics
-                )
+                self.project["preview_open2"].setToolTip(_("open's preview in camotics"))
+                self.project["preview_open2"].pressed.connect(self.open_preview_in_camotics)
                 preview_vbox.addWidget(self.project["preview_open2"])
 
             preview_vbox.addWidget(self.project["imgwidget"])
             tabwidget.addTab(preview, _("&Preview"))
 
         right_gridlayout = QGridLayout()
         right_gridlayout.addWidget(tabwidget)
```

### Comparing `viaconstructor-0.6.6/viaconstructor.egg-info/PKG-INFO` & `viaconstructor-0.6.7/viaconstructor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.6
+Version: 0.6.7
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.6/viaconstructor.egg-info/SOURCES.txt` & `viaconstructor-0.6.7/viaconstructor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

