# Comparing `tmp/OpenTimelineIO-0.8.1.tar.gz` & `tmp/OpenTimelineIO-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpenTimelineIO-0.8.1.tar", last modified: Mon Sep 17 18:32:35 2018, max compression
+gzip compressed data, was "dist/OpenTimelineIO-0.9.0.tar", last modified: Tue Nov  6 23:21:51 2018, max compression
```

## Comparing `OpenTimelineIO-0.8.1.tar` & `OpenTimelineIO-0.9.0.tar`

### file list

```diff
@@ -1,82 +1,155 @@
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2094 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/PKG-INFO
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2550 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/SOURCES.txt
--rw-rw-r--   0 steinbach  (5278) gfx        (219)        1 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/dependency_links.txt
--rw-rw-r--   0 steinbach  (5278) gfx        (219)      208 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/entry_points.txt
--rw-rw-r--   0 steinbach  (5278) gfx        (219)        1 2018-09-17 18:31:05.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/not-zip-safe
--rw-rw-r--   0 steinbach  (5278) gfx        (219)       55 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/requires.txt
--rw-rw-r--   0 steinbach  (5278) gfx        (219)       55 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/top_level.txt
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     6035 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     8490 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/adapter.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)      705 2016-12-23 17:20:44.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/builtin_adapters.plugin_manifest.json
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    44567 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/cmx_3600.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    31838 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/fcp_xml.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1603 2017-08-16 16:52:01.000000 OpenTimelineIO-0.8.1/opentimelineio/adapters/otio_json.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/algorithms/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1354 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/algorithms/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     8909 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/algorithms/filter.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2608 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/algorithms/stack_algo.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     7620 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/algorithms/track_algo.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/console/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1296 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineio/console/__init__.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     2105 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineio/console/otiocat.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     3672 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineio/console/otioconvert.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     4589 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineio/console/otiostat.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/core/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1847 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3575 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/composable.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    17142 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/composition.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     6857 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/item.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     5405 2018-08-21 17:27:40.000000 OpenTimelineIO-0.8.1/opentimelineio/core/json_serializer.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2981 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/media_reference.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     7235 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/serializable_object.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4314 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/core/type_registry.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/plugins/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1234 2017-08-16 16:52:01.000000 OpenTimelineIO-0.8.1/opentimelineio/plugins/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     7102 2018-09-17 18:19:04.000000 OpenTimelineIO-0.8.1/opentimelineio/plugins/manifest.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4155 2017-08-16 16:52:01.000000 OpenTimelineIO-0.8.1/opentimelineio/plugins/python_plugin.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1805 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3878 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/clip.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3610 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/effect.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2137 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/external_reference.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     2684 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/gap.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1967 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/generator_reference.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3359 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/marker.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1465 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/missing_reference.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4515 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/serializable_collection.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2726 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/stack.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3915 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/timeline.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     6515 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/track.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4868 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/schema/transition.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1414 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineio/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1992 2018-09-17 18:19:00.000000 OpenTimelineIO-0.8.1/opentimelineio/exceptions.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     5204 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/media_linker.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    25795 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/opentime.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1973 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio/test_utils.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)        0 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/__init__.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    26399 2018-09-17 18:19:03.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/advanced_authoring_format.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     8893 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/ale.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     3456 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/burnins.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1361 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/contrib_adapters.plugin_manifest.json
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     7368 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/extern_maya_sequencer.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     8343 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/extern_rv.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    13959 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/ffmpeg_burnins.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    59485 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/hls_playlist.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4090 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/maya_sequencer.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2560 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/rv.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1199 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineio_contrib/__init__.py
-drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/opentimelineview/
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     1153 2017-08-16 16:52:01.000000 OpenTimelineIO-0.8.1/opentimelineview/__init__.py
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     6888 2018-09-17 18:19:02.000000 OpenTimelineIO-0.8.1/opentimelineview/console.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     5194 2018-09-04 22:28:17.000000 OpenTimelineIO-0.8.1/opentimelineview/details_widget.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)    27513 2018-09-17 18:19:03.000000 OpenTimelineIO-0.8.1/opentimelineview/timeline_widget.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     4090 2018-09-17 18:19:01.000000 OpenTimelineIO-0.8.1/README.md
--rw-rw-r--   0 steinbach  (5278) gfx        (219)       79 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/setup.cfg
--rwxrwxr-x   0 steinbach  (5278) gfx        (219)     6860 2018-09-17 18:32:30.000000 OpenTimelineIO-0.8.1/setup.py
--rw-rw-r--   0 steinbach  (5278) gfx        (219)     2094 2018-09-17 18:32:35.000000 OpenTimelineIO-0.8.1/PKG-INFO
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/.AppleDouble/
+-rw-rw-rw-   0 steinbach  (5278) gfx        (219)      741 2018-10-27 18:19:27.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/.AppleDouble/.Parent
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2072 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/PKG-INFO
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4858 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)        1 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      208 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/entry_points.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)        1 2018-09-17 18:31:05.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/not-zip-safe
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)       64 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/requires.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)       55 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/top_level.txt
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/examples/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/examples/.AppleDouble/
+-rw-rw-rw-   0 steinbach  (5278) gfx        (219)      741 2018-10-27 18:19:27.000000 OpenTimelineIO-0.9.0/examples/.AppleDouble/.Parent
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/otio_counter/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1937 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/otio_counter/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      554 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/otio_counter/adapter.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      282 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/otio_counter/plugin_manifest.json
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1410 2018-10-23 22:36:11.000000 OpenTimelineIO-0.9.0/examples/sample_plugin/setup.py
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     4372 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/examples/conform.py
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     2179 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/examples/flatten_video_tracks.py
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     8712 2018-10-23 22:36:11.000000 OpenTimelineIO-0.9.0/examples/shot_detect.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5035 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/examples/summarize_timing.py
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/opentimelineio/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/opentimelineio/.AppleDouble/
+-rw-rw-rw-   0 steinbach  (5278) gfx        (219)      741 2018-10-27 18:19:27.000000 OpenTimelineIO-0.9.0/opentimelineio/.AppleDouble/.Parent
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6107 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5125 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     9129 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/adapter.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6236 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/adapter.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      828 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/builtin_adapters.plugin_manifest.json
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    44446 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/cmx_3600.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    26208 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/cmx_3600.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    31510 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/fcp_xml.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    22879 2018-11-06 17:19:43.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/fcp_xml.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1603 2017-08-16 16:52:01.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/otio_json.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1037 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/adapters/otio_json.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1354 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      468 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     8872 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/filter.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     7364 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/filter.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2784 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/stack_algo.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1412 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/stack_algo.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     7446 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/track_algo.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4319 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/algorithms/track_algo.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:50.000000 OpenTimelineIO-0.9.0/opentimelineio/console/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1296 2018-09-17 18:19:02.000000 OpenTimelineIO-0.9.0/opentimelineio/console/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      350 2018-10-24 21:09:36.000000 OpenTimelineIO-0.9.0/opentimelineio/console/__init__.pyc
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     2908 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otiocat.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1477 2018-11-02 17:11:02.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otiocat.pyc
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     4076 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otioconvert.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2661 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otioconvert.pyc
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     5118 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otiostat.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6011 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/console/otiostat.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio/core/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1925 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/core/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1166 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3617 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/composable.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3352 2018-11-06 17:42:51.000000 OpenTimelineIO-0.9.0/opentimelineio/core/composable.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    18265 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/composition.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    12919 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/composition.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6921 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/item.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5892 2018-11-06 17:42:51.000000 OpenTimelineIO-0.9.0/opentimelineio/core/item.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5945 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/json_serializer.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5228 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/json_serializer.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3009 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/media_reference.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2316 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/media_reference.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     7456 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/core/serializable_object.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6630 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/serializable_object.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5054 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/core/type_registry.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3914 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/type_registry.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1536 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/core/unknown_schema.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      913 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/core/unknown_schema.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1234 2017-08-16 16:52:01.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      328 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     9008 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/manifest.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6965 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/manifest.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4178 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/python_plugin.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3216 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/plugins/python_plugin.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1845 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1158 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3857 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/clip.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2965 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/clip.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3644 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/effect.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3106 2018-11-06 17:42:51.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/effect.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2137 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/external_reference.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1562 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/external_reference.pyc
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     2684 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/gap.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1255 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/gap.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1967 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/generator_reference.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2081 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/generator_reference.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3466 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/marker.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2774 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/marker.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1466 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/missing_reference.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      851 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/missing_reference.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1463 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/schemadef.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2027 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/schemadef.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4558 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/serializable_collection.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4121 2018-11-06 17:42:51.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/serializable_collection.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2828 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/stack.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2335 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/stack.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3935 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/timeline.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3718 2018-11-06 17:42:51.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/timeline.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     7809 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/track.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     6016 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/track.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4902 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/transition.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3650 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schema/transition.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio/schemadef/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      203 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/schemadef/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      397 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/schemadef/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1458 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      595 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/__init__.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1992 2018-09-17 18:19:00.000000 OpenTimelineIO-0.9.0/opentimelineio/exceptions.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2965 2018-10-24 21:09:35.000000 OpenTimelineIO-0.9.0/opentimelineio/exceptions.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5216 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/hooks.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4743 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/hooks.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5202 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/media_linker.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4350 2018-11-06 17:19:42.000000 OpenTimelineIO-0.9.0/opentimelineio/media_linker.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    25360 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio/opentime.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    21956 2018-11-06 17:46:59.000000 OpenTimelineIO-0.9.0/opentimelineio/opentime.pyc
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1973 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio/test_utils.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1370 2018-10-24 21:09:36.000000 OpenTimelineIO-0.9.0/opentimelineio/test_utils.pyc
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)        0 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/__init__.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    27413 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/advanced_authoring_format.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     8941 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/ale.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     3456 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/burnins.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1573 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/contrib_adapters.plugin_manifest.json
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     7368 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/extern_maya_sequencer.py
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     8343 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/extern_rv.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    27480 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/fcpx_xml.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    13965 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/ffmpeg_burnins.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    59547 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/hls_playlist.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4092 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/maya_sequencer.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2646 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/rv.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1199 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/opentimelineio_contrib/__init__.py
+drwxrwxr-x   0 steinbach  (5278) gfx        (219)        0 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/opentimelineview/
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1153 2017-08-16 16:52:01.000000 OpenTimelineIO-0.9.0/opentimelineview/__init__.py
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     7848 2018-11-06 22:23:46.000000 OpenTimelineIO-0.9.0/opentimelineview/console.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     5196 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineview/details_widget.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     1513 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineview/settings.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    27072 2018-11-06 17:18:52.000000 OpenTimelineIO-0.9.0/opentimelineview/timeline_widget.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)    10154 2018-09-04 22:28:17.000000 OpenTimelineIO-0.9.0/LICENSE.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      460 2018-11-06 17:18:51.000000 OpenTimelineIO-0.9.0/MANIFEST.in
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)      153 2017-08-16 16:52:01.000000 OpenTimelineIO-0.9.0/NOTICE.txt
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     4808 2018-11-06 23:14:17.000000 OpenTimelineIO-0.9.0/README.md
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)       79 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/setup.cfg
+-rwxrwxr-x   0 steinbach  (5278) gfx        (219)     6898 2018-11-06 23:21:32.000000 OpenTimelineIO-0.9.0/setup.py
+-rw-rw-r--   0 steinbach  (5278) gfx        (219)     2072 2018-11-06 23:21:51.000000 OpenTimelineIO-0.9.0/PKG-INFO
```

### Comparing `OpenTimelineIO-0.8.1/OpenTimelineIO.egg-info/PKG-INFO` & `OpenTimelineIO-0.9.0/OpenTimelineIO.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: OpenTimelineIO
-Version: 0.8.1
+Version: 0.9.0
 Summary: Editorial interchange format and API
 Home-page: http://opentimeline.io
 Author: Pixar Animation Studios
 Author-email: opentimelineio@pixar.com
 License: Modified Apache 2.0 License
 Project-URL: Source, https://github.com/PixarAnimationStudios/OpenTimelineIO
-Project-URL: Documentation, https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki
+Project-URL: Documentation, https://opentimelineio.readthedocs.io/
 Project-URL: Issues, https://github.com/PixarAnimationStudios/OpenTimelineIO/issues
 Description: OpenTimelineIO is an interchange format and API for
         editorial cut information. OTIO is not a container format for media, rather it
         contains information about the order and length of cuts and references to
         external media.
         
         OTIO includes both a file format and an API for manipulating that format. It
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
     exceptions,
     plugins,
     media_linker
 )
 
 from .adapter import Adapter  # noqa
 
+# OTIO Json adapter is always available
+from . import otio_json # noqa
+
 
 def suffixes_with_defined_adapters(read=False, write=False):
     """Return a set of all the suffixes that have adapters defined for them."""
 
     if not read and not write:
         read = True
         write = True
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/adapter.py` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,42 +21,44 @@
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
 """Implementation of the OTIO internal `Adapter` system.
 
 For information on writing adapters, please consult:
-    https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki/How-to-Write-an-OpenTimelineIO-Adapter # noqa
+    https://opentimelineio.readthedocs.io/en/latest/tutorials/write-an-adapter.html# # noqa
 """
 
 from .. import (
     core,
     plugins,
     media_linker,
+    hooks,
 )
 
 
 @core.register_type
 class Adapter(plugins.PythonPlugin):
     """Adapters convert between OTIO and other formats.
 
     Note that this class is not subclassed by adapters.  Rather, an adapter is
     a python module that implements at least one of the following functions:
+
         write_to_string(input_otio)
         write_to_file(input_otio, filepath) (optionally inferred)
         read_from_string(input_str)
         read_from_file(filepath) (optionally inferred)
 
     ...as well as a small json file that advertises the features of the adapter
     to OTIO.  This class serves as the wrapper around these modules internal
     to OTIO.  You should not need to extend this class to create new adapters
     for OTIO.
 
     For more information:
-        https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki/How-to-Write-an-OpenTimelineIO-Adapter # noqa
+    https://opentimelineio.readthedocs.io/en/latest/tutorials/write-an-adapter.html# # noqa
     """
     _serializable_label = "Adapter.1"
 
     def __init__(
         self,
         name=None,
         execution_scope=None,
@@ -129,32 +131,41 @@
         else:
             result = self._execute_function(
                 "read_from_file",
                 filepath=filepath,
                 **adapter_argument_map
             )
 
+        # @TODO: pass arguments through?
+        result = hooks.run("post_adapter_read", result)
+
         if media_linker_name and (
             media_linker_name != media_linker.MediaLinkingPolicy.DoNotLinkMedia
         ):
             _with_linked_media_references(
                 result,
                 media_linker_name,
                 media_linker_argument_map
             )
 
+        # @TODO: pass arguments through?
+        result = hooks.run("post_media_linker", result)
+
         return result
 
     def write_to_file(self, input_otio, filepath, **adapter_argument_map):
         """Execute the write_to_file function on this adapter.
 
         If write_to_string exists, but not write_to_file, execute that with
         a trivial file object wrapper.
         """
 
+        # @TODO: pass arguments through?
+        input_otio = hooks.run("pre_adapter_write", input_otio)
+
         if (
             not self.has_feature("write_to_file") and
             self.has_feature("write_to_string")
         ):
             result = self.write_to_string(input_otio, **adapter_argument_map)
             with open(filepath, 'w') as fo:
                 fo.write(result)
@@ -178,28 +189,38 @@
 
         result = self._execute_function(
             "read_from_string",
             input_str=input_str,
             **adapter_argument_map
         )
 
+        # @TODO: pass arguments through?
+        result = hooks.run("post_adapter_read", result)
+
         if media_linker_name and (
             media_linker_name != media_linker.MediaLinkingPolicy.DoNotLinkMedia
         ):
             _with_linked_media_references(
                 result,
                 media_linker_name,
                 media_linker_argument_map
             )
 
+        # @TODO: pass arguments through?
+        # @TODO: Should this run *ONLY* if the media linker ran?
+        result = hooks.run("post_media_linker", result)
+
         return result
 
     def write_to_string(self, input_otio, **adapter_argument_map):
         """Call the write_to_string function on this adapter."""
 
+        # @TODO: pass arguments through?
+        input_otio = hooks.run("pre_adapter_write", input_otio)
+
         return self._execute_function(
             "write_to_string",
             input_otio=input_otio,
             **adapter_argument_map
         )
 
     def __str__(self):
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/builtin_adapters.plugin_manifest.json` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/builtin_adapters.plugin_manifest.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'hooks'": "OrderedDict([('post_adapter_read', []), ('post_media_linker', []), "*

 * *            "('pre_adapter_write', [])])"}*

```diff
@@ -24,9 +24,14 @@
             "execution_scope": "in process",
             "filepath": "cmx_3600.py",
             "name": "cmx_3600",
             "suffixes": [
                 "edl"
             ]
         }
-    ]
+    ],
+    "hooks": {
+        "post_adapter_read": [],
+        "post_media_linker": [],
+        "pre_adapter_write": []
+    }
 }
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/cmx_3600.py` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/cmx_3600.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # language governing permissions and limitations under the Apache License.
 #
 
 """OpenTimelineIO CMX 3600 EDL Adapter"""
 
 # Note: this adapter is not an ideal model for new adapters, but it works.
 # If you want to write your own adapter, please see:
-# https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki/How-to-Write-an-OpenTimelineIO-Adapter
+# https://opentimelineio.readthedocs.io/en/latest/tutorials/write-an-adapter.html#
 
 # TODO: Flesh out Attribute Handler
 # TODO: Add line numbers to errors and warnings
 # TODO: currently tracks with linked audio/video will lose their linkage when
 #       read into OTIO.
 
 import os
@@ -43,26 +43,26 @@
 
 class EDLParseError(otio.exceptions.OTIOError):
     pass
 
 
 # regex for parsing the playback speed of an M2 event
 SPEED_EFFECT_RE = re.compile(
-    "(?P<name>.*?)\s*(?P<speed>[0-9\.]*)\s*(?P<tc>[0-9:]{11})$"
+    r"(?P<name>.*?)\s*(?P<speed>[0-9\.]*)\s*(?P<tc>[0-9:]{11})$"
 )
 
 
 # these are all CMX_3600 transition codes
 # the wipe is written in regex format because it is W### where the ### is
 # a 'wipe code'
 # @TODO: not currently read by the transition code
 transition_regex_map = {
     'C': 'cut',
     'D': 'dissolve',
-    'W\d{3}': 'wipe',
+    r'W\d{3}': 'wipe',
     'KB': 'key_background',
     'K': 'key_foreground',
     'KO': 'key_overlay'
 }
 
 # CMX_3600 supports some shorthand for channel assignments
 # We name the actual tracks V and A1,A2,A3,etc.
@@ -147,15 +147,15 @@
                         # XXX remove 'FF' suffix (writing edl will add it back)
                         if clip.name.endswith(' FF'):
                             clip.name = clip.name[:-3]
                     elif motion is not None:
                         fps = float(
                             SPEED_EFFECT_RE.match(motion).group("speed")
                         )
-                        time_scalar = fps/rate
+                        time_scalar = fps / rate
                         clip.effects.append(
                             otio.schema.LinearTimeWarp(time_scalar=time_scalar)
                         )
 
                 elif self.ignore_timecode_mismatch:
                     # Pretend there was no problem by adjusting the record_out.
                     # Note that we don't actually use record_out after this
@@ -199,15 +199,15 @@
             # to fill that space. This can happen when an EDL has record
             # timecodes that are sparse (e.g. from a single track of a
             # multi-track composition).
             if record_in > track_end and len(track) > 0:
                 gap = otio.schema.Gap()
                 gap.source_range = otio.opentime.TimeRange(
                     start_time=otio.opentime.RationalTime(0, edl_rate),
-                    duration=record_in-track_end
+                    duration=record_in - track_end
                 )
                 track.append(gap)
                 track.source_range.duration += gap.duration()
 
             track.append(clip)
             track.source_range.duration += clip.duration()
 
@@ -293,15 +293,15 @@
                     )
 
                 line_1 = edl_lines.pop(0)
                 line_2 = edl_lines.pop(0)
 
                 comments = []
                 while edl_lines:
-                    if re.match('^\D', edl_lines[0]):
+                    if re.match(r'^\D', edl_lines[0]):
                         comments.append(edl_lines.pop(0))
                     else:
                         break
                 self.add_clip(line_1, comments, rate=rate)
                 self.add_clip(line_2, comments, rate=rate)
 
             elif line[0].isdigit():
@@ -310,15 +310,15 @@
                 comments = []
                 while edl_lines:
                     # any non-numbered lines after an edit decision should be
                     # treated as 'comments'
                     # comments are string tags used by the reader to get extra
                     # information not able to be found in the restricted edl
                     # format
-                    if re.match('^\D', edl_lines[0]):
+                    if re.match(r'^\D', edl_lines[0]):
                         comments.append(edl_lines.pop(0))
                     else:
                         break
 
                 self.add_clip(line, comments, rate=rate)
 
             else:
@@ -392,26 +392,29 @@
             offset = (0, 0, 0)
             power = (1, 1, 1)
             sat = 1.0
 
             if asc_sop:
                 triple = r'([-+]?[\d.]+) ([-+]?[\d.]+) ([-+]?[\d.]+)'
                 m = re.match(
-                    r'\('+triple+'\)\s*\('+triple+'\)\s*\('+triple+'\)',
+                    r'\('
+                    + triple
+                    + r'\)\s*\('
+                    + triple + r'\)\s*\('
+                    + triple + r'\)',
                     asc_sop
                 )
                 if m:
                     floats = [float(g) for g in m.groups()]
                     slope = [floats[0], floats[1], floats[2]]
                     offset = [floats[3], floats[4], floats[5]]
                     power = [floats[6], floats[7], floats[8]]
                 else:
                     raise EDLParseError(
-                        'Invalid ASC_SOP found: {}'.format(asc_sop)
-                        )
+                        'Invalid ASC_SOP found: {}'.format(asc_sop))
 
             if asc_sat:
                 sat = float(asc_sat)
 
             clip.metadata['cdl'] = {
                 'asc_sat': sat,
                 'asc_sop': {
@@ -536,29 +539,29 @@
                         self.edl_rate
                     )
                 )
 
 
 class CommentHandler(object):
     # this is the for that all comment 'id' tags take
-    regex_template = '\*?\s*{id}:?\s*(?P<comment_body>.*)'
+    regex_template = r'\*?\s*{id}:?\s*(?P<comment_body>.*)'
 
     # this should be a map of all known comments that we can read
     # 'FROM CLIP' or 'FROM FILE' is a required comment to link media
     # An exception is raised if both 'FROM CLIP' and 'FROM FILE' are found
     # needs to be ordered so that FROM CLIP NAME gets matched before FROM CLIP
     comment_id_map = collections.OrderedDict([
-            ('FROM CLIP NAME', 'clip_name'),
-            ('FROM CLIP', 'media_reference'),
-            ('FROM FILE', 'media_reference'),
-            ('LOC', 'locator'),
-            ('ASC_SOP', 'asc_sop'),
-            ('ASC_SAT', 'asc_sat'),
-            ('M2', 'motion_effect'),
-            ('\\* FREEZE FRAME', 'freeze_frame'),
+        ('FROM CLIP NAME', 'clip_name'),
+        ('FROM CLIP', 'media_reference'),
+        ('FROM FILE', 'media_reference'),
+        ('LOC', 'locator'),
+        ('ASC_SOP', 'asc_sop'),
+        ('ASC_SAT', 'asc_sat'),
+        ('M2', 'motion_effect'),
+        ('\\* FREEZE FRAME', 'freeze_frame'),
     ])
 
     def __init__(self, comments):
         self.handled = {}
         self.unhandled = []
         for comment in comments:
             self.parse(comment)
@@ -691,29 +694,26 @@
     invalid timecode in the EDL. For example, if a clip's record timecode
     overlaps with the previous cut. Since this is a common mistake in
     many EDLs, you can specify ignore_timecode_mismatch=True, which will
     supress these errors and attempt to guess at the correct record
     timecode based on the source timecode and adjacent cuts.
     For best results, you may wish to do something like this:
 
-    try:
-        timeline = otio.adapters.read_from_string(
-            "mymovie.edl",
-            rate=30
-        )
-    except EDLParseError:
-        report_warning(...)
-        try:
-            timeline = otio.adapters.read_from_string(
-                "mymovie.edl",
-                rate=30,
-                ignore_timecode_mismatch=True
-            )
-        except EDLParseError:
-            report_error(...)
+    Example:
+        >>> try:
+        ...     timeline = otio.adapters.read_from_string("mymovie.edl", rate=30)
+        ... except EDLParseError:
+        ...    print('Log a warning here')
+        ...    try:
+        ...        timeline = otio.adapters.read_from_string(
+        ...            "mymovie.edl",
+        ...            rate=30,
+        ...            ignore_timecode_mismatch=True)
+        ...    except EDLParseError:
+        ...        print('Log an error here')
     """
     parser = EDLParser(
         input_str,
         rate=float(rate),
         ignore_timecode_mismatch=ignore_timecode_mismatch
     )
     result = parser.timeline
@@ -796,34 +796,34 @@
         # |Clip1 45.0|----------------Clip2 200.0-----------------|Clip3 24.0|
 
         # Adjust cut points to match EDL event representation.
         for idx, child in enumerate(track):
             if isinstance(child, otio.schema.Transition):
                 if idx != 0:
                     # Shorten the a-side
-                    track[idx-1].source_range.duration -= child.in_offset
+                    track[idx - 1].source_range.duration -= child.in_offset
 
                 # Lengthen the b-side
-                track[idx+1].source_range.start_time -= child.in_offset
-                track[idx+1].source_range.duration += child.in_offset
+                track[idx + 1].source_range.start_time -= child.in_offset
+                track[idx + 1].source_range.duration += child.in_offset
 
                 # Just clean up the transition for goodness sake
                 in_offset = child.in_offset
                 child.in_offset = otio.opentime.RationalTime(0.0, self._rate)
                 child.out_offset += in_offset
 
         # Group events into either simple clip/a-side or transition and b-side
         # to match EDL edit/event representation and edit numbers.
         events = []
         for idx, child in enumerate(track):
             if isinstance(child, otio.schema.Transition):
                 # Transition will be captured in subsequent iteration.
                 continue
 
-            prv = track[idx-1] if idx > 0 else None
+            prv = track[idx - 1] if idx > 0 else None
 
             if isinstance(prv, otio.schema.Transition):
                 events.append(
                     DissolveEvent(
                         events[-1] if len(events) else None,
                         prv,
                         child,
@@ -867,22 +867,18 @@
 
 def _relevant_timing_effect(clip):
     # check to see if there is more than one timing effect
     effects = _supported_timing_effects(clip)
 
     if effects != clip.effects:
         for thing in clip.effects:
-            if (
-                    thing not in effects
-                    and isinstance(thing, otio.schema.TimeEffect)
-            ):
+            if thing not in effects and isinstance(thing, otio.schema.TimeEffect):
                 raise otio.exceptions.NotSupportedError(
                     "Clip contains timing effects not supported by the EDL"
-                    " adapter.\nClip: {}".format(str(clip))
-                )
+                    " adapter.\nClip: {}".format(str(clip)))
 
     timing_effect = None
     if effects:
         timing_effect = effects[0]
     if len(effects) > 1:
         raise otio.exceptions.NotSupportedError(
             "EDL Adapter only allows one timing effect / clip."
@@ -910,24 +906,17 @@
         if timing_effect:
             if timing_effect.effect_name == "FreezeFrame":
                 line.source_out = line.source_in + otio.opentime.RationalTime(
                     1,
                     line.source_in.rate
                 )
             elif timing_effect.effect_name == "LinearTimeWarp":
+                value = clip.trimmed_range().duration.value / timing_effect.time_scalar
                 line.source_out = (
-                    line.source_in
-                    + otio.opentime.RationalTime(
-                        (
-                            clip.trimmed_range().duration.value
-                            / timing_effect.time_scalar
-                        ),
-                        rate
-                    )
-                )
+                    line.source_in + otio.opentime.RationalTime(value, rate))
 
         range_in_timeline = clip.transformed_time_range(
             clip.trimmed_range(),
             tracks
         )
         line.record_in = range_in_timeline.start_time
         line.record_out = range_in_timeline.end_time_exclusive()
@@ -948,22 +937,21 @@
     def __str__(self):
         return '{type}({name})'.format(
             type=self.clip.schema_name(),
             name=self.clip.name
         )
 
     def to_edl_format(self):
-        '''
+        """
         Example output:
+            002 AX V C        00:00:00:00 00:00:00:05 00:00:00:05 00:00:00:10
+            * FROM CLIP NAME:  test clip2
+            * FROM FILE: S:\\var\\tmp\\test.exr
 
-        002 AX V C        00:00:00:00 00:00:00:05 00:00:00:05 00:00:00:10
-        * FROM CLIP NAME:  test clip2
-        * FROM FILE: S:\var\tmp\test.exr
-        '''
-
+        """
         lines = [self.line.to_edl_format(self.edit_number)]
         lines += self.comments if len(self.comments) else []
 
         return "\n".join(lines)
 
 
 class DissolveEvent(object):
@@ -1041,15 +1029,15 @@
             a_type=a_side.clip.schema_name() if a_side else '',
             a_name=a_side.clip.name if a_side else '',
             b_type=self.b_side_clip.schema_name(),
             b_name=self.b_side_clip.name
         )
 
     def to_edl_format(self):
-        '''
+        """
         Example output:
 
         Cross dissolve...
         002 Clip1 V C     00:00:07:08 00:00:07:08 00:00:01:21 00:00:01:21
         002 Clip2 V D 100 00:00:09:07 00:00:17:15 00:00:01:21 00:00:10:05
         * FROM CLIP NAME:  Clip1
         * FROM CLIP: /var/tmp/clip1.001.exr
@@ -1063,15 +1051,15 @@
         * TO FILE: /var/tmp/clip.001.exr
 
         Fade out...
         002 My_Clip V C     00:00:01:12 00:00:01:12 00:00:00:12 00:00:00:12
         002 BL      V D 012 00:00:00:00 00:00:00:12 00:00:00:12 00:00:01:00
         * FROM CLIP NAME:  My Clip
         * FROM FILE: /var/tmp/clip.001.exr
-        '''
+        """
 
         lines = [
             self.cut_line.to_edl_format(self.edit_number),
             self.dissolve_line.to_edl_format(self.edit_number)
         ]
         lines += self.from_comments if hasattr(self, 'from_comments') else []
         lines += self.to_comments if len(self.to_comments) else []
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/fcp_xml.py` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/fcp_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,18 +161,16 @@
     return dom.toprettyxml(indent='    ')
 
 
 def _is_primary_audio_channel(track):
     # audio may be structured in stereo where each channel occupies a separate
     # track. Some xml logic combines these into a single track upon import.
     # Here we check whether we`re dealing with the first audio channel
-    return (
-        track.attrib.get('currentExplodedTrackIndex', '0') == '0'
-        or track.attrib.get('totalExplodedTrackCount', '1') == '1'
-    )
+    return track.attrib.get('currentExplodedTrackIndex', '0') == '0' or \
+        track.attrib.get('totalExplodedTrackCount', '1') == '1'
 
 
 def _get_transition_cut_point(transition_item, element_map):
     alignment = transition_item.find('./alignment').text
     start = int(transition_item.find('./start').text)
     end = int(transition_item.find('./end').text)
     rate = _parse_rate(transition_item, element_map)
@@ -210,29 +208,26 @@
     url = file_e.find('./pathurl').text
     file_rate = _parse_rate(file_e, element_map)
     timecode_rate = _parse_rate(file_e.find('./timecode'), element_map)
 
     frame_e = file_e.find('./timecode/frame')
     if frame_e is not None:
         start_time = otio.opentime.RationalTime(
-                                            int(frame_e.text),
-                                            timecode_rate
-                                            )
+            int(frame_e.text),
+            timecode_rate)
     else:
         start_time = otio.opentime.from_timecode(
-                                        file_e.find('./timecode/string').text,
-                                        timecode_rate
-                                        )
+            file_e.find('./timecode/string').text,
+            timecode_rate)
 
     duration_e = file_e.find('./duration')
     if duration_e is not None:
         duration = otio.opentime.RationalTime(
-                                        int(duration_e.text),
-                                        file_rate
-                                        )
+            int(duration_e.text),
+            file_rate)
     else:
         duration = otio.opentime.RationalTime(0, file_rate)
 
     available_range = otio.opentime.TimeRange(
         start_time=start_time,
         duration=duration
     )
@@ -251,22 +246,19 @@
     # transition offsets are provided in timeline rate. If they deviate they
     # need to be rescaled to clip item rate
     context_transition_offsets = [
         transition_offsets[0].rescaled_to(rate),
         transition_offsets[1].rescaled_to(rate)
     ]
 
-    in_frame = (
-        int(float(clip_item.find('./in').text))
-        + int(round(context_transition_offsets[0].value))
-    )
-    out_frame = (
-        int(float(clip_item.find('./out').text))
-        - int(round(context_transition_offsets[1].value))
-    )
+    in_value = int(float(clip_item.find('./in').text))
+    in_frame = in_value + int(round(context_transition_offsets[0].value))
+
+    out_value = int(float(clip_item.find('./out').text))
+    out_frame = out_value - int(round(context_transition_offsets[1].value))
 
     source_range = otio.opentime.TimeRange(
         start_time=otio.opentime.RationalTime(in_frame, track_rate),
         duration=otio.opentime.RationalTime(
             out_frame - in_frame,
             track_rate
         )
@@ -297,22 +289,19 @@
     # transition offsets are provided in timeline rate. If they deviate they
     # need to be rescaled to clip item rate
     context_transition_offsets = [
         transition_offsets[0].rescaled_to(item_rate),
         transition_offsets[1].rescaled_to(item_rate)
     ]
 
-    in_frame = (
-        int(float(clip_item.find('./in').text))
-        + int(round(context_transition_offsets[0].value))
-    )
-    out_frame = (
-        int(float(clip_item.find('./out').text))
-        - int(round(context_transition_offsets[1].value))
-    )
+    in_value = int(float(clip_item.find('./in').text))
+    in_frame = in_value + int(round(context_transition_offsets[0].value))
+
+    out_value = int(float(clip_item.find('./out').text))
+    out_frame = out_value - int(round(context_transition_offsets[1].value))
     timecode = media_reference.available_range.start_time
 
     # source_start in xml is taken relative to the start of the media, whereas
     # we want the absolute start time, taking into account the timecode
     start_time = otio.opentime.RationalTime(in_frame, item_rate) + timecode
 
     source_range = otio.opentime.TimeRange(
@@ -373,22 +362,19 @@
     # transition offsets are provided in timeline rate. If they deviate they
     # need to be rescaled to clip item rate
     context_transition_offsets = [
         transition_offsets[0].rescaled_to(source_rate),
         transition_offsets[1].rescaled_to(source_rate)
     ]
 
-    in_frame = (
-        int(track_item.find('./in').text)
-        + int(round(context_transition_offsets[0].value, 0))
-    )
-    out_frame = (
-        int(track_item.find('./out').text)
-        - int(round(context_transition_offsets[1].value))
-    )
+    in_value = int(track_item.find('./in').text)
+    in_frame = in_value + int(round(context_transition_offsets[0].value, 0))
+
+    out_value = int(track_item.find('./out').text)
+    out_frame = out_value - int(round(context_transition_offsets[1].value))
 
     track.source_range = otio.opentime.TimeRange(
         start_time=otio.opentime.RationalTime(in_frame, source_rate),
         duration=otio.opentime.RationalTime(out_frame - in_frame, source_rate)
     )
     return track
 
@@ -646,18 +632,16 @@
     _insert_new_sub_element(
         timecode_e,
         'frame',
         text='{:.0f}'.format(timecode.value)
     )
     display_format = (
         'DF' if (
-            math.ceil(timecode.rate) == 30
-            and math.ceil(timecode.rate) != timecode.rate
-        )
-        else 'NDF'
+            math.ceil(timecode.rate) == 30 and math.ceil(timecode.rate) != timecode.rate
+        ) else 'NDF'
     )
     _insert_new_sub_element(timecode_e, 'displayformat', text=display_format)
 
     # we need to flag the file reference with the content types, otherwise it
     # will not get recognized
     file_media_e = _insert_new_sub_element(file_e, 'media')
     content_types = []
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/adapters/otio_json.py` & `OpenTimelineIO-0.9.0/opentimelineio/adapters/otio_json.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/algorithms/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/algorithms/filter.py` & `OpenTimelineIO-0.9.0/opentimelineio/algorithms/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,19 +88,16 @@
                 else:
                     return thing
 
         filtered_composition(track, fn) => [A,B_1,B_2,B_3,C]
 
     EXAMPLE 4 (prune gaps):
         track :: [Gap, A, Gap]
-        filtered_composition(
-            track,
-            lambda _:_,
-            types_to_prune=(otio.schema.Gap,)
-        ) => [A]
+            filtered_composition(
+                track, lambda _:_, types_to_prune=(otio.schema.Gap,)) => [A]
     """
 
     # deep copy everything
     mutable_object = copy.deepcopy(root)
 
     prune_list = set()
 
@@ -108,18 +105,15 @@
 
     if isinstance(mutable_object, otio.schema.Timeline):
         header_list.append(mutable_object.tracks)
 
     iter_list = header_list + list(mutable_object.each_child())
 
     for child in iter_list:
-        if (
-            _safe_parent(child) is not None
-            and _is_in(child.parent(), prune_list)
-        ):
+        if _safe_parent(child) is not None and _is_in(child.parent(), prune_list):
             prune_list.add(child)
             continue
 
         parent = None
         child_index = None
         if _safe_parent(child) is not None:
             child_index = child.parent().index(child)
@@ -170,56 +164,55 @@
     3. For each item (including root):
         a. if types_to_prune is not None and item is an instance of a type
             in types_to_prune, prune it from the copy, continue.
         b. Otherwise, pass (prev, copy, and next) to reduce_fn. If reduce_fn:
             I.   returns an object: add it to the copy, replacing original
             II.  returns a tuple: insert it into the list, replacing original
             III. returns None: prune it
+
             ** note that reduce_fn is always passed objects from the original
                 deep copy, not what prior calls return.  See below for examples
     4. If an item is pruned, do not traverse its children
     5. Return the new deep copy.
 
     EXAMPLE 1 (filter):
-        track: [A,B,C]
-
-        def fn(prev_item, thing, next_item):
-            if prev_item.name == A:
-                return D # some new clip
-            else:
-                return thing
-        filtered_with_sequence_context(track, fn) => [A,D,C]
+        >>> track = [A,B,C]
+        >>> def fn(prev_item, thing, next_item):
+        ...     if prev_item.name == A:
+        ...         return D # some new clip
+        ...     else:
+        ...         return thing
+        >>> filtered_with_sequence_context(track, fn) => [A,D,C]
 
         order of calls to fn:
             fn(None, A, B) => A
             fn(A, B, C) => D
             fn(B, C, D) => C # !! note that it was passed B instead of D.
 
     EXAMPLE 2 (prune):
-        def fn(prev_item, thing, next_item):
-            if prev_item.name == A:
-                return None # prune the clip
-            else:
-                return thing
-
-        filtered_with_sequence_context(track, fn) => [A,C]
+        >>> track = [A,B,C]
+        >>> def fn(prev_item, thing, next_item):
+        ...    if prev_item.name == A:
+        ...        return None # prune the clip
+        ...   else:
+        ...        return thing
+        >>> filtered_with_sequence_context(track, fn) => [A,C]
 
         order of calls to fn:
             fn(None, A, B) => A
             fn(A, B, C) => None
             fn(B, C, D) => C # !! note that it was passed B instead of D.
 
     EXAMPLE 3 (expand):
-        def fn(prev_item, thing, next_item):
-            if prev_item.name == A:
-                return (D, E) # tuple of new clips
-            else:
-                return thing
-
-        filtered_with_sequence_context(track, fn) => [A, D, E, C]
+        >>> def fn(prev_item, thing, next_item):
+        ...     if prev_item.name == A:
+        ...         return (D, E) # tuple of new clips
+        ...     else:
+        ...         return thing
+        >>> filtered_with_sequence_context(track, fn) => [A, D, E, C]
 
          the order of calls to fn will be:
             fn(None, A, B) => A
             fn(A, B, C) => (D, E)
             fn(B, C, D) => C # !! note that it was passed B instead of D.
     """
 
@@ -234,40 +227,34 @@
         header_list.append(mutable_object.tracks)
 
     iter_list = header_list + list(mutable_object.each_child())
 
     # expand to include prev, next when appropriate
     expanded_iter_list = []
     for child in iter_list:
-        if (
-            _safe_parent(child)
-            and isinstance(child.parent(), otio.schema.Track)
-        ):
+        if _safe_parent(child) and isinstance(child.parent(), otio.schema.Track):
             prev_item, next_item = child.parent().neighbors_of(child)
             expanded_iter_list.append((prev_item, child, next_item))
         else:
             expanded_iter_list.append((None, child, None))
 
     for prev_item, child, next_item in expanded_iter_list:
-        if (
-            _safe_parent(child) is not None
-            and _is_in(child.parent(), prune_list)
-        ):
+        if _safe_parent(child) is not None and _is_in(child.parent(), prune_list):
             prune_list.add(child)
             continue
 
         parent = None
         child_index = None
         if _safe_parent(child) is not None:
             child_index = child.parent().index(child)
             parent = child.parent()
             del child.parent()[child_index]
 
         # first try to prune
-        if (types_to_prune and _isinstance_in(child, types_to_prune)):
+        if types_to_prune and _isinstance_in(child, types_to_prune):
             result = None
         # finally call the user function
         else:
             result = reduce_fn(prev_item, child, next_item)
 
         if child is mutable_object:
             mutable_object = result
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/algorithms/stack_algo.py` & `OpenTimelineIO-0.9.0/opentimelineio/algorithms/stack_algo.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,59 +23,64 @@
 #
 
 __doc__ = """ Algorithms for stack objects. """
 
 import copy
 
 from .. import (
-    schema
+    schema,
 )
 from . import (
     track_algo
 )
 
 
 def flatten_stack(in_stack):
     """Flatten a Stack, or a list of Tracks, into a single Track.
     Note that the 1st Track is the bottom one, and the last is the top.
     """
 
     flat_track = schema.Track()
     flat_track.name = "Flattened"
 
+    # map of track to track.range_of_all_children
+    range_track_map = {}
+
     def _get_next_item(
             in_stack,
             track_index=None,
             trim_range=None
     ):
         if track_index is None:
             # start with the top-most track
-            track_index = len(in_stack)-1
+            track_index = len(in_stack) - 1
         if track_index < 0:
             # if you get to the bottom, you're done
             return
 
         track = in_stack[track_index]
         if trim_range is not None:
             track = track_algo.track_trimmed_to_range(track, trim_range)
+
+        track_map = range_track_map.get(track)
+        if track_map is None:
+            track_map = track.range_of_all_children()
+            range_track_map[track] = track_map
+
         for item in track:
             if (
-                    item.visible() or
-                    track_index == 0 or
-                    isinstance(item, schema.Transition)
+                    item.visible()
+                    or track_index == 0
+                    or isinstance(item, schema.Transition)
             ):
                 yield item
             else:
-                trim = item.range_in_parent()
+                trim = track_map[item]
                 if trim_range is not None:
                     trim.start_time += trim_range.start_time
-                for more in _get_next_item(
-                    in_stack,
-                    track_index-1,
-                    trim
-                ):
+                for more in _get_next_item(in_stack, track_index - 1, trim):
                     yield more
 
     for item in _get_next_item(in_stack):
         flat_track.append(copy.deepcopy(item))
 
     return flat_track
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/algorithms/track_algo.py` & `OpenTimelineIO-0.9.0/opentimelineio/algorithms/track_algo.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,17 +37,19 @@
     outside the trim_range removed and items on the ends trimmed to the
     trim_range. Note that the track is never expanded, only shortened.
     Please note that you could do nearly the same thing non-destructively by
     just setting the Track's source_range but sometimes you want to really cut
     away the stuff outside and that's what this function is meant for."""
     new_track = copy.deepcopy(in_track)
 
+    track_map = new_track.range_of_all_children()
+
     # iterate backwards so we can delete items
     for c, child in reversed(list(enumerate(new_track))):
-        child_range = child.range_in_parent()
+        child_range = track_map[child]
         if not trim_range.overlaps(child_range):
             # completely outside the trim range, so we discard it
             del new_track[c]
         elif trim_range.contains(child_range):
             # completely contained, keep the whole thing
             pass
         else:
@@ -165,16 +167,15 @@
 
     if target_transition.out_offset is None:
         raise RuntimeError(
             "out_offset is None on: {}".format(target_transition)
         )
 
     pre.source_range.start_time = (
-        pre.source_range.end_time_exclusive()
-        - target_transition.in_offset
+        pre.source_range.end_time_exclusive() - target_transition.in_offset
     )
     pre.source_range.duration = trx_duration.rescaled_to(
         pre.source_range.start_time
     )
 
     post = copy.deepcopy(result.next)
     if isinstance(post, schema.Transition):
@@ -188,44 +189,34 @@
 
     post.name = (post.name or "") + "_transition_post"
 
     # ensure that post.source_range is set, because it will get manipulated
     post.source_range = copy.copy(post.trimmed_range())
 
     post.source_range.start_time = (
-        post.source_range.start_time
-        - target_transition.in_offset
+        post.source_range.start_time - target_transition.in_offset
     ).rescaled_to(post.source_range.start_time)
     post.source_range.duration = trx_duration.rescaled_to(
         post.source_range.start_time
     )
 
-    return (pre, target_transition, post)
+    return pre, target_transition, post
 
 
 def _trim_from_transitions(thing, pre=None, post=None):
     """ Trim clips next to transitions. """
 
     result = copy.deepcopy(thing)
 
     # We might not have a source_range yet,
     # We can trim to the computed trimmed_range to
     # ensure we have something.
     result.source_range = result.trimmed_range()
 
     if pre:
-        result.source_range.start_time = (
-            result.source_range.start_time
-            + pre.out_offset
-        )
-        result.source_range.duration = (
-            result.source_range.duration
-            - pre.out_offset
-        )
+        result.source_range.start_time += pre.out_offset
+        result.source_range.duration -= pre.out_offset
 
     if post:
-        result.source_range.duration = (
-            result.source_range.duration
-            - post.in_offset
-        )
+        result.source_range.duration -= post.in_offset
 
     return result
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/console/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/console/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/console/otiocat.py` & `OpenTimelineIO-0.9.0/opentimelineio/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #
 # Copyright 2017 Pixar Animation Studios
 #
 # Licensed under the Apache License, Version 2.0 (the "Apache License")
 # with the following modification; you may not use this file except in
 # compliance with the Apache License and the following modification to it:
 # Section 6. Trademarks. is deleted and replaced with:
@@ -19,51 +18,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the Apache License with the above modification is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
-"""Print the contents of an OTIO file to stdout."""
+"""An editorial interchange format and library.
 
-import argparse
+see: http://opentimeline.io
 
-import opentimelineio as otio
+.. moduleauthor:: Pixar Animation Studios <opentimelineio@pixar.com>
+"""
 
+# flake8: noqa
 
-def _parsed_args():
-    """ parse commandline arguments with argparse """
-
-    parser = argparse.ArgumentParser(
-        description=__doc__,
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter
-    )
-    parser.add_argument(
-        'filepath',
-        type=str,
-        nargs='+',
-        help='files to print the contents of'
-    )
-
-    return parser.parse_args()
-
-
-def _otio_compatible_file_to_json_string(fpath):
-    """Read the file at fpath with the default otio adapter and return the json
-    as a string.
-    """
-
-    adapter = otio.adapters.from_name("otio_json")
-    return adapter.write_to_string(otio.adapters.read_from_file(fpath))
-
-
-def main():
-    """Parse arguments and call _otio_compatible_file_to_json_string."""
-
-    args = _parsed_args()
-
-    for fpath in args.filepath:
-        print(_otio_compatible_file_to_json_string(fpath))
-
-
-if __name__ == '__main__':
-    main()
+# in dependency hierarchy
+from . import (
+    opentime,
+    exceptions,
+    core,
+    schema,
+    schemadef,
+    plugins,
+    media_linker,
+    adapters,
+    hooks,
+    algorithms,
+    test_utils,
+    console,
+)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/console/otioconvert.py` & `OpenTimelineIO-0.9.0/opentimelineio/console/otioconvert.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,17 +77,21 @@
         default=None,
         help="Pick one or more tracks, by 0-based index, separated by commas.",
     )
     parser.add_argument(
         '-m',
         '--media-linker',
         type=str,
-        default=None,
-        help="Specify a media linker.  Default is to use the "
-        "OTIO_DEFAULT_MEDIA_LINKER, if set.",
+        default="Default",
+        help=(
+            "Specify a media linker.  'Default' means use the "
+            "$OTIO_DEFAULT_MEDIA_LINKER if set, 'None' or '' means explicitly "
+            "disable the linker, and anything else is interpreted as the name"
+            " of the media linker to use."
+        )
     )
 
     return parser.parse_args()
 
 
 def main():
     """Parse arguments and convert the files."""
@@ -98,22 +102,26 @@
     if in_adapter is None:
         in_adapter = otio.adapters.from_filepath(args.input).name
 
     out_adapter = args.output_adapter
     if out_adapter is None:
         out_adapter = otio.adapters.from_filepath(args.output).name
 
-    ml = otio.media_linker.MediaLinkingPolicy.ForceDefaultLinker
-    if args.media_linker:
+    # allow user to explicitly set or pass to default or disable the linker.
+    if args.media_linker.lower() == 'default':
+        ml = otio.media_linker.MediaLinkingPolicy.ForceDefaultLinker
+    elif args.media_linker.lower() in ['none', '']:
+        ml = otio.media_linker.MediaLinkingPolicy.DoNotLinkMedia
+    else:
         ml = args.media_linker
 
     result_tl = otio.adapters.read_from_file(
-            args.input,
-            in_adapter,
-            media_linker_name=ml
+        args.input,
+        in_adapter,
+        media_linker_name=ml
     )
 
     if args.tracks:
         result_tracks = []
         for track in args.tracks.split(","):
             result_tracks.append(result_tl.tracks[int(track)])
         result_tl.tracks = result_tracks
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/console/otiostat.py` & `OpenTimelineIO-0.9.0/opentimelineio/console/otiostat.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,25 +72,42 @@
 def _num_tracks(input):
     try:
         return len(input.tracks)
     except AttributeError:
         return 0
 
 
+@stat_check("Tracks are the same length")
+def _equal_length_tracks(tl):
+    if not tl.tracks:
+        return True
+    for i, track in enumerate(tl.tracks):
+        if track.duration() != tl.tracks[0].duration():
+            raise RuntimeError(
+                "track {} is not the same duration as the other tracks."
+                " Track {} duration, vs: {}".format(
+                    i,
+                    track.duration(),
+                    tl.tracks[0].duration()
+                )
+            )
+    return True
+
+
 @stat_check("deepest nesting")
 def _deepest_nesting(input):
     def depth(parent):
         if not isinstance(parent, otio.core.Composition):
             return 1
         d = 0
         for child in parent:
-            d = max(d, depth(child)+1)
+            d = max(d, depth(child) + 1)
         return d
     if isinstance(input, otio.schema.Timeline):
-        return depth(input.tracks)+1
+        return depth(input.tracks) + 1
     else:
         return depth(input)
 
 
 @stat_check("number of clips")
 def _num_clips(input):
     return len(list(input.each_clip()))
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 
 """Internal implementation details of OpenTimelineIO."""
 
 # flake8: noqa
 
 from . import (
-    serializable_object,
+    serializable_object
 )
 from .serializable_object import (
     SerializableObject,
     serializable_field,
     deprecated_field,
 )
 from .composable import (
@@ -57,7 +57,11 @@
     serialize_json_to_file,
     deserialize_json_from_string,
     deserialize_json_from_file,
 )
 from .media_reference import (
     MediaReference,
 )
+from . import unknown_schema
+from .unknown_schema import (
+    UnknownSchema
+)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/composable.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/composable.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 An object that can be composed by tracks.
 """
 
 from . import serializable_object
 from . import type_registry
 
+import copy
+
 
 @type_registry.register_type
 class Composable(serializable_object.SerializableObject):
     """An object that can be composed by tracks.
 
     Base class of:
         Item
@@ -54,15 +56,15 @@
 
     def __init__(self, name=None, metadata=None):
         super(Composable, self).__init__()
         self._parent = None
 
         # initialize the serializable fields
         self.name = name
-        self.metadata = metadata or {}
+        self.metadata = copy.deepcopy(metadata) if metadata else {}
 
     @staticmethod
     def visible():
         """Return the visibility of the Composable. By default True."""
 
         return False
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/composition.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/composition.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,28 +53,37 @@
     _composable_base_class = composable.Composable
 
     def __init__(
         self,
         name=None,
         children=None,
         source_range=None,
+        markers=None,
+        effects=None,
         metadata=None
     ):
         item.Item.__init__(
             self,
             name=name,
             source_range=source_range,
+            markers=markers,
+            effects=effects,
             metadata=metadata
         )
         collections.MutableSequence.__init__(self)
 
+        # Because we know that all children are unique, we store a set
+        # of all the children as well to speed up __contain__ checks.
+        self._child_lookup = set()
+
         self._children = []
         if children:
             # cannot simply set ._children to children since __setitem__ runs
-            # extra logic (assigning ._parent pointers).
+            # extra logic (assigning ._parent pointers) and populates the
+            # internal membership set _child_lookup.
             self.extend(children)
 
     _children = serializable_object.serializable_field(
         "children",
         list,
         "Items contained by this composition."
     )
@@ -109,32 +118,24 @@
                 repr(self.source_range),
                 repr(self.metadata)
             )
         )
 
     transform = serializable_object.deprecated_field()
 
-    def each_child(
-        self,
-        search_range=None,
-        descended_from_type=composable.Composable
-    ):
+    def each_child(self, search_range=None, descended_from_type=composable.Composable):
         for i, child in enumerate(self._children):
             # filter out children who are not in the search range
-            if (
-                search_range
-                and not self.range_of_child_at_index(i).overlaps(search_range)
-            ):
+            if search_range and not self.range_of_child_at_index(i).overlaps(
+                    search_range):
                 continue
 
             # filter out children who are not descended from the specified type
-            if (
-                descended_from_type == composable.Composable
-                or isinstance(child, descended_from_type)
-            ):
+            is_descendant = descended_from_type == composable.Composable
+            if is_descendant or isinstance(child, descended_from_type):
                 yield child
 
             # for children that are compositions, recurse into their children
             if hasattr(child, "each_child"):
                 for valid_child in (
                     c for c in child.each_child(
                         search_range,
@@ -159,15 +160,17 @@
         raise NotImplementedError
 
     def trimmed_range_of_child_at_index(self, index):
         """Return the trimmed range of the child item at index in the time
         range of this composition.
 
         For example, with a track:
+
                        [     ]
+
             [ClipA][ClipB][ClipC]
 
         The range of index 2 (ClipC) will be just like
         range_of_child_at_index() but trimmed based on this Composition's
         source_range.
 
         To be implemented by child.
@@ -199,14 +202,17 @@
     def __deepcopy__(self, md):
         result = super(Composition, self).__deepcopy__(md)
 
         # deepcopy should have already copied the children, so only parent
         # pointers need to be updated.
         [c._set_parent(result) for c in result._children]
 
+        # we also need to reconstruct the membership set of _child_lookup.
+        result._child_lookup.update(result._children)
+
         return result
 
     def _path_to_child(self, child):
         if not isinstance(child, composable.Composable):
             raise TypeError(
                 "An object child of 'Composable' is required,"
                 " not type '{}'".format(
@@ -232,18 +238,19 @@
     def range_of_child(self, child, reference_space=None):
         """The range of the child in relation to another item
         (reference_space), not trimmed based on this
         composition's source_range.
 
         Note that reference_space must be in the same timeline as self.
 
-        For example,
+        For example:
 
-        |     [-----]     | seq
-        [-----------------] Clip A
+            |     [-----]     | seq
+
+            [-----------------] Clip A
 
         If ClipA has duration 17, and seq has source_range: 5, duration 15,
         seq.range_of_child(Clip A) will return (0, 17)
         ignoring the source range of seq.
 
         To get the range of the child with the source_range applied, use the
         trimmed_range_of_child() method.
@@ -262,18 +269,15 @@
             parent_range = parent.range_of_child_at_index(index)
 
             if not result_range:
                 result_range = parent_range
                 current = parent
                 continue
 
-            result_range.start_time = (
-                result_range.start_time
-                + parent_range.start_time
-            )
+            result_range.start_time += parent_range.start_time
             current = parent
 
         if reference_space is not self:
             result_range = self.transformed_time_range(
                 result_range,
                 reference_space
             )
@@ -307,46 +311,45 @@
         """If media beyond the ends of this child are visible due to adjacent
         Transitions (only applicable in a Track) then this will return the
         head and tail offsets as a tuple of RationalTime objects. If no handles
         are present on either side, then None is returned instead of a
         RationalTime.
 
         Example usage:
-        head, tail = track.handles_of_child(clip)
-        if head:
-          ...
-        if tail:
-          ...
+        >>> head, tail = track.handles_of_child(clip)
+        >>> if head:
+        ...     print('Do something')
+        >>> if tail:
+        ...     print('Do something else')
         """
         return (None, None)
 
     def trimmed_range_of_child(self, child, reference_space=None):
-        """ Return range of the child in reference_space coordinates, after the
+        """Get range of the child in reference_space coordinates, after the
         self.source_range is applied.
 
-        For example,
-
+        Example
         |     [-----]     | seq
         [-----------------] Clip A
 
         If ClipA has duration 17, and seq has source_range: 5, duration 10,
         seq.trimmed_range_of_child(Clip A) will return (5, 10)
         Which is trimming the range according to the source_range of seq.
 
         To get the range of the child without the source_range applied, use the
         range_of_child() method.
 
-        Another example:
+        Another example
         |  [-----]   | seq source range starts on frame 4 and goes to frame 8
         [ClipA][ClipB] (each 6 frames long)
 
-        seq.range_of_child(CLipA):
-            0, duration 6
-        seq.trimmed_range_of_child(ClipA):
-            4, duration 2
+        >>> seq.range_of_child(CLipA)
+        0, duration 6
+        >>> seq.trimmed_range_of_child(ClipA):
+        4, duration 2
         """
 
         if not reference_space:
             reference_space = self
 
         if not reference_space == self:
             raise NotImplementedError
@@ -361,18 +364,15 @@
             parent_range = parent.trimmed_range_of_child_at_index(index)
 
             if not result_range:
                 result_range = parent_range
                 current = parent
                 continue
 
-            result_range.start_time = (
-                result_range.start_time
-                + parent_range.start_time
-            )
+            result_range.start_time += parent_range.start_time
             current = parent
 
         if not self.source_range:
             return result_range
 
         new_start_time = max(
             self.source_range.start_time,
@@ -395,18 +395,19 @@
         return opentime.TimeRange(new_start_time, new_duration)
 
     def trim_child_range(self, child_range):
         if not self.source_range:
             return child_range
 
         # cropped out entirely
-        if (
-            self.source_range.start_time >= child_range.end_time_exclusive()
-            or self.source_range.end_time_exclusive() <= child_range.start_time
-        ):
+        past_end_time = self.source_range.start_time >= child_range.end_time_exclusive()
+        before_start_time = \
+            self.source_range.end_time_exclusive() <= child_range.start_time
+
+        if past_end_time or before_start_time:
             return None
 
         if child_range.start_time < self.source_range.start_time:
             child_range = opentime.range_from_start_end_time(
                 self.source_range.start_time,
                 child_range.end_time_exclusive()
             )
@@ -491,17 +492,21 @@
 
         if value in self:
             raise ValueError(
                 "Composable {} already present in this container, instancing"
                 " not allowed in otio compositions.".format(value)
             )
 
-        # unset the old child's parent
+        # unset the old child's parent and delete the membership entry.
         if old is not None:
             old._set_parent(None)
+            self._child_lookup.remove(old)
+
+        # put it into our membership tracking set
+        self._child_lookup.add(value)
 
         # put it into our list of children
         self._children[key] = value
 
         # set the new parent
         if value is not None:
             value._set_parent(self)
@@ -522,28 +527,43 @@
 
         if item in self:
             raise ValueError(
                 "Composable {} already present in this container, instancing"
                 " not allowed in otio compositions.".format(item)
             )
 
+        # set the item's parent and add it to our membership tracking and list
+        # of children
         item._set_parent(self)
+        self._child_lookup.add(item)
         self._children.insert(index, item)
 
+    def __contains__(self, item):
+        """Use our internal membership tracking set to speed up searches."""
+        return item in self._child_lookup
+
     def __len__(self):
         """The len() of a Composition is the # of children in it.
         Note that this also means that a Composition with no children
         is considered False, so take care to test for "if foo is not None"
         versus just "if foo" when the difference matters."""
         return len(self._children)
 
     def __delitem__(self, key):
         # grab the old value
         old = self._children[key]
 
+        # remove it from the membership tracking set
+        if old is not None:
+            if isinstance(key, slice):
+                for val in old:
+                    self._child_lookup.remove(val)
+            else:
+                self._child_lookup.remove(old)
+
         # remove it from our list of children
         del self._children[key]
 
         # unset the old value's parent
         if old is not None:
             if isinstance(key, slice):
                 for val in old:
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/item.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/item.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,22 +57,19 @@
         self,
         name=None,
         source_range=None,
         effects=None,
         markers=None,
         metadata=None,
     ):
-        serializable_object.SerializableObject.__init__(self)
+        super(Item, self).__init__(name=name, metadata=metadata)
 
-        self.name = name
-        self.source_range = source_range
-        self.effects = effects or []
-        self.markers = markers or []
-        self.metadata = metadata or {}
-        self._parent = None
+        self.source_range = copy.deepcopy(source_range)
+        self.effects = copy.deepcopy(effects) if effects else []
+        self.markers = copy.deepcopy(markers) if markers else []
 
     name = serializable_object.serializable_field("name", doc="Item name.")
     source_range = serializable_object.serializable_field(
         "source_range",
         opentime.TimeRange,
         doc="Range of source to trim to.  Can be None or a TimeRange."
     )
@@ -91,23 +88,23 @@
     def available_range(self):
         """Implemented by child classes, available range of media."""
 
         raise NotImplementedError
 
     def trimmed_range(self):
         """The range after applying the source range."""
-
         if self.source_range is not None:
             return copy.copy(self.source_range)
 
         return self.available_range()
 
     def visible_range(self):
         """The range of this item's media visible to its parent.
-        Includes handles revealed by adjacent transitions (if any)."""
+        Includes handles revealed by adjacent transitions (if any).
+        This will always be larger or equal to trimmed_range()."""
         result = self.trimmed_range()
         if self.parent():
             head, tail = self.parent().handles_of_child(self)
             if head:
                 result.start_time -= head
                 result.duration += head
             if tail:
@@ -136,21 +133,22 @@
         """Converts time t in the coordinate system of self to coordinate
         system of to_item.
 
         Note that self and to_item must be part of the same timeline (they must
         have a common ancestor).
 
         Example:
-        0                      20
-        [------*----D----------]
-        [--A--|*----B----|--C--]
-             100 101    110
-        101 in B = 6 in D
 
-        * = t argument
+            0                      20
+            [------t----D----------]
+            [--A-][t----B---][--C--]
+            100    101    110
+            101 in B = 6 in D
+
+        t = t argument
         """
 
         # does not operate in place
         result = copy.copy(t)
 
         if to_item is None:
             return result
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/json_serializer.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/json_serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,29 +30,31 @@
 import json
 
 from . import (
     SerializableObject,
     type_registry,
 )
 
+from .unknown_schema import UnknownSchema
+
 from .. import (
     exceptions,
     opentime,
 )
 
 
 # @TODO: Handle file version drifting
 
 
 class _SerializableObjectEncoder(json.JSONEncoder):
 
     """ Encoder for the SerializableObject OTIO Class and its descendents. """
 
     def default(self, obj):
-        for typename, encfn in _ENCODER_MAP.items():
+        for typename, encfn in _ENCODER_LIST:
             if isinstance(obj, typename):
                 return encfn(obj)
 
         return json.JSONEncoder.default(self, obj)
 
 
 def serialize_json_to_string(root, sort_keys=True, indent=4):
@@ -90,14 +92,28 @@
     result = {
         "OTIO_SCHEMA": input_otio._serializable_label,
     }
     result.update(input_otio.data)
     return result
 
 
+def _encoded_unknown_schema_object(input_otio):
+    orig_label = input_otio.data.get(UnknownSchema._original_label)
+    if not orig_label:
+        raise exceptions.InvalidSerializableLabelError(
+            orig_label
+        )
+    # result is just a dict, not a SerializableObject
+    result = {}
+    result.update(input_otio.data)
+    result["OTIO_SCHEMA"] = orig_label  # override the UnknownSchema label
+    del result[UnknownSchema._original_label]
+    return result
+
+
 def _encoded_time(input_otio):
     return {
         "OTIO_SCHEMA": "RationalTime.1",
         'value': input_otio.value,
         'rate': input_otio.rate
     }
 
@@ -116,21 +132,23 @@
         'offset': _encoded_time(input_otio.offset),
         'scale': input_otio.scale,
         'rate': input_otio.rate
     }
 # @}
 
 
-# Map of functions for encoding OTIO objects to JSON.
-_ENCODER_MAP = {
-    opentime.RationalTime: _encoded_time,
-    opentime.TimeRange: _encoded_time_range,
-    opentime.TimeTransform: _encoded_transform,
-    SerializableObject: _encoded_serializable_object,
-}
+# Ordered list of functions for encoding OTIO objects to JSON.
+# More particular cases should precede more general cases.
+_ENCODER_LIST = [
+    (opentime.RationalTime, _encoded_time),
+    (opentime.TimeRange, _encoded_time_range),
+    (opentime.TimeTransform, _encoded_transform),
+    (UnknownSchema, _encoded_unknown_schema_object),
+    (SerializableObject, _encoded_serializable_object)
+]
 
 # @{ Decoders
 
 
 def _decoded_time(input_otio):
     return opentime.RationalTime(
         input_otio['value'],
@@ -184,20 +202,15 @@
 
     return dct
 
 
 def deserialize_json_from_string(otio_string):
     """ Deserialize a string containing JSON to OTIO objects. """
 
-    json_data = json.loads(otio_string, object_hook=_as_otio)
-
-    if json_data is {}:
-        raise exceptions.CouldNotReadFileError
-
-    return json_data
+    return json.loads(otio_string, object_hook=_as_otio)
 
 
 def deserialize_json_from_file(otio_filepath):
     """ Deserialize the file at otio_filepath containing JSON to OTIO.  """
 
     with open(otio_filepath, 'r') as file_contents:
         result = deserialize_json_from_string(file_contents.read())
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/media_reference.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/media_reference.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     opentime,
 )
 from . import (
     type_registry,
     serializable_object,
 )
 
+import copy
+
 
 @type_registry.register_type
 class MediaReference(serializable_object.SerializableObject):
     """Base Media Reference Class.
 
     Currently handles string printing the child classes, which expose interface
     into its data dictionary.
@@ -48,19 +50,19 @@
 
     def __init__(
         self,
         name=None,
         available_range=None,
         metadata=None
     ):
-        serializable_object.SerializableObject.__init__(self)
+        super(MediaReference, self).__init__()
 
         self.name = name
-        self.available_range = available_range
-        self.metadata = metadata or {}
+        self.available_range = copy.deepcopy(available_range)
+        self.metadata = copy.deepcopy(metadata) or {}
 
     name = serializable_object.serializable_field(
         "name",
         doc="Name of this media reference."
     )
     available_range = serializable_object.serializable_field(
         "available_range",
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/serializable_object.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/serializable_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,30 +43,29 @@
 
     Finally, if you're in the process of upgrading schemas and you want to
     catch code that refers to old attribute names, you can use the
     deprecated_field function. This raises an exception if code attempts to
     read or write to that attribute.  After testing and before pushing, please
     remove references to deprecated_field.
 
-    For example:
-        import opentimelineio as otio
+    For example
 
-        @otio.core.register_type
-        class ExampleChild(otio.core.SerializableObject):
-            _serializable_label = "ExampleChild.7"
+    >>>    import opentimelineio as otio
 
-            child_data = otio.core.serializable_field("child_data", int)
+    >>>    @otio.core.register_type
+    ...    class ExampleChild(otio.core.SerializableObject):
+    ...        _serializable_label = "ExampleChild.7"
+    ...        child_data = otio.core.serializable_field("child_data", int)
 
-            # @TODO: delete once testing shows nothing is referencing this.
-            old_child_data_name = otio.core.deprecated_field()
+    # @TODO: delete once testing shows nothing is referencing this.
+    >>>         old_child_data_name = otio.core.deprecated_field()
 
-
-        @otio.core.upgrade_function_for(ExampleChild, 3)
-        def upgrade_child_to_three(data):
-            return {"child_data" : data["old_child_data_name"]}
+    >>>    @otio.core.upgrade_function_for(ExampleChild, 3)
+    ...    def upgrade_child_to_three(data):
+    ...        return {"child_data" : data["old_child_data_name"]}
     """
 
     # Every child must define a _serializable_label attribute.
     # This attribute is a string in the form of: "SchemaName.VersionNumber"
     # Where VersionNumber is an integer.
     # You can use the classmethods .schema_name() and .schema_version() to
     # query these fields.
@@ -137,14 +136,20 @@
 
     @classmethod
     def schema_version(cls):
         return type_registry.schema_version_from_label(
             cls._serializable_label
         )
 
+    @property
+    def is_unknown_schema(self):
+        # in general, SerializableObject will have a known schema
+        # but UnknownSchema subclass will redefine this property to be True
+        return False
+
     def __copy__(self):
         result = self.__class__()
         result.data = copy.copy(self.data)
 
         return result
 
     def copy(self):
@@ -187,26 +192,23 @@
     """
 
     def getter(self):
         return self.data[name]
 
     def setter(self, val):
         # always allow None values regardless of value of required_type
-        if (
-            required_type is not None
-            and val is not None
-            and not isinstance(val, required_type)
-        ):
-            raise TypeError(
-                "attribute '{}' must be an instance of '{}', not: {}".format(
-                    name,
-                    required_type,
-                    type(val)
+        if required_type is not None and val is not None:
+            if not isinstance(val, required_type):
+                raise TypeError(
+                    "attribute '{}' must be an instance of '{}', not: {}".format(
+                        name,
+                        required_type,
+                        type(val)
+                    )
                 )
-            )
 
         self.data[name] = val
 
     return property(getter, setter, doc=doc)
 
 
 def deprecated_field():
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/core/type_registry.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/type_registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,25 +44,32 @@
 
 def schema_version_from_label(label):
     """Return the schema version from the label name."""
 
     return int(label.split(".")[1])
 
 
+def schema_label_from_name_version(schema_name, schema_version):
+    """Return the serializeable object schema label given the name and version."""
+
+    return "{}.{}".format(schema_name, schema_version)
+
+
 def register_type(classobj, schemaname=None):
     """ Register a class to a Schema Label.
 
     Normally this is used as a decorator.  However, in special cases where a
     type has been renamed, you might need to register the new type to multiple
     schema names.  To do this:
-        @core.register_type
-        class MyNewClass(...):
-            ...
 
-        core.register_type(MyNewClass, "MyOldName")
+    >>>    @core.register_type
+    ...    class MyNewClass(...):
+    ...        pass
+
+    >>>    core.register_type(MyNewClass, "MyOldName")
 
     This will parse the old schema name into the new class type.  You may also
     need to write an upgrade function if the schema itself has changed.
     """
 
     if schemaname is None:
         schemaname = schema_name_from_label(classobj._serializable_label)
@@ -71,18 +78,18 @@
 
     return classobj
 
 
 def upgrade_function_for(cls, version_to_upgrade_to):
     """Decorator for identifying schema class upgrade functions.
 
-    example:
-        @upgrade_function_for(MyClass, 5)
-        def upgrade_to_version_five(data):
-            # ...
+    Example
+    >>>    @upgrade_function_for(MyClass, 5)
+    ...    def upgrade_to_version_five(data):
+    ...        pass
 
     This will get called to upgrade a schema of MyClass to version 5.  My class
     must be a class deriving from otio.core.SerializableObject.
 
     The upgrade function should take a single argument - the dictionary to
     upgrade, and return a dictionary with the fields upgraded.
 
@@ -101,17 +108,22 @@
     return decorator_func
 
 
 def instance_from_schema(schema_name, schema_version, data_dict):
     """Return an instance, of the schema from data in the data_dict."""
 
     if schema_name not in _OTIO_TYPES:
-        raise exceptions.NotSupportedError(
-            "OTIO_SCHEMA: '{}' not in type registry.".format(schema_name)
-        )
+        from .unknown_schema import UnknownSchema
+
+        # create an object of UnknownSchema type to represent the data
+        schema_label = schema_label_from_name_version(schema_name, schema_version)
+        data_dict[UnknownSchema._original_label] = schema_label
+        unknown_label = UnknownSchema._serializable_label
+        schema_name = schema_name_from_label(unknown_label)
+        schema_version = schema_version_from_label(unknown_label)
 
     cls = _OTIO_TYPES[schema_name]
 
     schema_version = int(schema_version)
     if cls.schema_version() < schema_version:
         raise exceptions.UnsupportedSchemaError(
             "Schema '{}' has highest version available '{}', which is lower "
@@ -119,15 +131,18 @@
                 schema_name,
                 cls.schema_version(),
                 schema_version
             )
         )
 
     if cls.schema_version() != schema_version:
-        for version, upgrade_func in (
+        # since the keys are the versions to upgrade to, sorting the keys
+        # before iterating through them should ensure that upgrade functions
+        # are called in order.
+        for version, upgrade_func in sorted(
             _UPGRADE_FUNCTIONS[cls].items()
         ):
             if version < schema_version:
                 continue
 
             data_dict = upgrade_func(data_dict)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/plugins/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/plugins/manifest.py` & `OpenTimelineIO-0.9.0/opentimelineio/plugins/manifest.py`

 * *Files 22% similar despite different names*

```diff
@@ -45,47 +45,97 @@
 
     result = core.deserialize_json_from_file(filepath)
     result.source_files.append(filepath)
     result._update_plugin_source(filepath)
     return result
 
 
+def manifest_from_string(input_string):
+    """Deserialize the json string into a manifest object."""
+
+    result = core.deserialize_json_from_string(input_string)
+
+    # try and get the caller's name
+    name = "unknown"
+    stack = inspect.stack()
+    if len(stack) > 1 and len(stack[1]) > 3:
+        #                     filename     function name
+        name = "{}:{}".format(stack[1][1], stack[1][3])
+
+    # set the value in the manifest
+    src_string = "call to manifest_from_string() in " + name
+    result.source_files.append(src_string)
+    result._update_plugin_source(src_string)
+
+    return result
+
+
 @core.register_type
 class Manifest(core.SerializableObject):
     """Defines an OTIO plugin Manifest.
 
     This is an internal OTIO implementation detail.  A manifest tracks a
     collection of adapters and allows finding specific adapters by suffix
 
     For writing your own adapters, consult:
-        https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki/How-to-Write-an-OpenTimelineIO-Adapter
+        https://opentimelineio.readthedocs.io/en/latest/tutorials/write-an-adapter.html#
     """
     _serializable_label = "PluginManifest.1"
 
     def __init__(self):
-        core.SerializableObject.__init__(self)
+        super(Manifest, self).__init__()
         self.adapters = []
+        self.schemadefs = []
         self.media_linkers = []
         self.source_files = []
 
+        # hook system stuff
+        self.hooks = []
+        self.hook_scripts = []
+
     adapters = core.serializable_field(
         "adapters",
         type([]),
         "Adapters this manifest describes."
     )
+    schemadefs = core.serializable_field(
+        "schemadefs",
+        type([]),
+        "Schemadefs this manifest describes."
+    )
     media_linkers = core.serializable_field(
         "media_linkers",
         type([]),
         "Media Linkers this manifest describes."
     )
+    hooks = core.serializable_field(
+        "hooks",
+        type([]),
+        "Hooks that hooks scripts can be attached to."
+    )
+    hook_scripts = core.serializable_field(
+        "hook_scripts",
+        type([]),
+        "Scripts that can be attached to hooks."
+    )
+
+    def extend(self, another_manifest):
+        """
+        Extend the adapters, schemadefs, and media_linkers lists of this manifest
+        by appending the contents of the corresponding lists of another_manifest.
+        """
+        if another_manifest:
+            self.adapters.extend(another_manifest.adapters)
+            self.schemadefs.extend(another_manifest.schemadefs)
+            self.media_linkers.extend(another_manifest.media_linkers)
 
     def _update_plugin_source(self, path):
         """Track the source .json for a given adapter."""
 
-        for thing in (self.adapters + self.media_linkers):
+        for thing in (self.adapters + self.schemadefs + self.media_linkers):
             thing._json_path = path
 
     def from_filepath(self, suffix):
         """Return the adapter object associated with a given file suffix."""
 
         for adapter in self.adapters:
             if suffix.lower() in adapter.suffixes:
@@ -116,14 +166,20 @@
 
     def adapter_module_from_name(self, name):
         """Return the adapter module associated with a given adapter name."""
 
         adp = self.from_name(name)
         return adp.module()
 
+    def schemadef_module_from_name(self, name):
+        """Return the schemadef module associated with a given schemadef name."""
+
+        adp = self.from_name(name, kind_list="schemadefs")
+        return adp.module()
+
 
 _MANIFEST = None
 
 
 def load_manifest():
     # build the manifest of adapters, starting with builtin adapters
     result = manifest_from_file(
@@ -141,16 +197,15 @@
         contrib_manifest = manifest_from_file(
             os.path.join(
                 os.path.dirname(inspect.getsourcefile(otio_c)),
                 "adapters",
                 "contrib_adapters.plugin_manifest.json"
             )
         )
-        result.adapters.extend(contrib_manifest.adapters)
-        result.media_linkers.extend(contrib_manifest.media_linkers)
+        result.extend(contrib_manifest)
     except ImportError:
         pass
 
     # Discover setuptools-based plugins
     if pkg_resources:
         for plugin in pkg_resources.iter_entry_points(
                 "opentimelineio.plugins"
@@ -170,23 +225,27 @@
                         plugin.module_name,
                         'plugin_manifest.json'
                     )
                     plugin_manifest = core.deserialize_json_from_string(
                         manifest_stream.read().decode('utf-8')
                     )
                     manifest_stream.close()
+                    filepath = pkg_resources.resource_filename(
+                        plugin.module_name,
+                        'plugin_manifest.json'
+                    )
+                    plugin_manifest._update_plugin_source(filepath)
 
             except Exception:
                 logging.exception(
                     "could not load plugin: {}".format(plugin_name)
                 )
                 continue
 
-            result.adapters.extend(plugin_manifest.adapters)
-            result.media_linkers.extend(plugin_manifest.media_linkers)
+            result.extend(plugin_manifest)
     else:
         # XXX: Should we print some kind of warning that pkg_resources isn't
         #        available?
         pass
 
     # read local adapter manifests, if they exist
     _local_manifest_path = os.environ.get("OTIO_PLUGIN_MANIFEST_PATH", None)
@@ -197,17 +256,19 @@
                 # print(
                 #     "Warning: OpenTimelineIO cannot access path '{}' from "
                 #     "$OTIO_PLUGIN_MANIFEST_PATH".format(json_path)
                 # )
                 continue
 
             LOCAL_MANIFEST = manifest_from_file(json_path)
-            result.adapters.extend(LOCAL_MANIFEST.adapters)
-            result.media_linkers.extend(LOCAL_MANIFEST.media_linkers)
+            result.extend(LOCAL_MANIFEST)
 
+    # force the schemadefs to load and add to schemadef module namespace
+    for s in result.schemadefs:
+        s.module()
     return result
 
 
 def ActiveManifest(force_reload=False):
     global _MANIFEST
     if not _MANIFEST or force_reload:
         _MANIFEST = load_manifest()
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/plugins/python_plugin.py` & `OpenTimelineIO-0.9.0/opentimelineio/plugins/python_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def __init__(
         self,
         name=None,
         execution_scope=None,
         filepath=None,
     ):
-        core.SerializableObject.__init__(self)
+        super(PythonPlugin, self).__init__()
         self.name = name
         self.execution_scope = execution_scope
         self.filepath = filepath
         self._json_path = None
         self._module = None
 
     name = core.serializable_field("name", str, "Adapter name.")
@@ -86,38 +86,38 @@
                     )
                 )
 
             filepath = os.path.join(os.path.dirname(self._json_path), filepath)
 
         return filepath
 
-    def _imported_module(self):
-        """Load the module this adapter points at."""
+    def _imported_module(self, namespace):
+        """Load the module this plugin points at."""
 
         pyname = os.path.splitext(os.path.basename(self.module_abs_path()))[0]
         pydir = os.path.dirname(self.module_abs_path())
 
         (file_obj, pathname, description) = imp.find_module(pyname, [pydir])
 
         with file_obj:
             # this will reload the module if it has already been loaded.
             mod = imp.load_module(
-                "opentimelineio.adapters.{}".format(self.name),
+                "opentimelineio.{}.{}".format(namespace, self.name),
                 file_obj,
                 pathname,
                 description
             )
 
             return mod
 
     def module(self):
         """Return the module object for this adapter. """
 
         if not self._module:
-            self._module = self._imported_module()
+            self._module = self._imported_module("adapters")
 
         return self._module
 
     def _execute_function(self, func_name, **kwargs):
         """Execute func_name on this adapter with error checking."""
 
         # collects the error handling into a common place.
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     MissingReference
 )
 from .external_reference import (
     ExternalReference
 )
 from .clip import (
     Clip,
-) 
+)
 from .track import (
     Track,
     TrackKind,
     NeighborGapPolicy,
 )
 from .stack import (
     Stack,
@@ -66,7 +66,10 @@
 )
 from .serializable_collection import (
     SerializableCollection
 )
 from .generator_reference import (
     GeneratorReference
 )
+from .schemadef import (
+    SchemaDef
+)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/clip.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/clip.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,29 +45,30 @@
     _serializable_label = "Clip.1"
 
     def __init__(
         self,
         name=None,
         media_reference=None,
         source_range=None,
+        markers=[],
+        effects=[],
         metadata=None,
     ):
         core.Item.__init__(
             self,
             name=name,
             source_range=source_range,
+            markers=markers,
+            effects=effects,
             metadata=metadata
         )
-        # init everything as None first, so that we will catch uninitialized
-        # values via exceptions
-        self.name = name
 
         if not media_reference:
             media_reference = missing_reference.MissingReference()
-        self._media_reference = media_reference
+        self._media_reference = copy.deepcopy(media_reference)
 
     name = core.serializable_field("name", doc="Name of this clip.")
     transform = core.deprecated_field()
     _media_reference = core.serializable_field(
         "media_reference",
         core.MediaReference,
         "Media reference to the media this clip represents."
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/effect.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,31 @@
 
 """Implementation of Effect OTIO class."""
 
 from .. import (
     core
 )
 
+import copy
+
 
 @core.register_type
 class Effect(core.SerializableObject):
     _serializable_label = "Effect.1"
 
     def __init__(
         self,
         name=None,
         effect_name=None,
         metadata=None
     ):
-        core.SerializableObject.__init__(self)
+        super(Effect, self).__init__()
         self.name = name
         self.effect_name = effect_name
-        self.metadata = metadata or {}
+        self.metadata = copy.deepcopy(metadata) if metadata else {}
 
     name = core.serializable_field(
         "name",
         doc="Name of this effect object. Example: 'BlurByHalfEffect'."
     )
     effect_name = core.serializable_field(
         "effect_name",
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/external_reference.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/external_reference.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/gap.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/gap.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/generator_reference.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/generator_reference.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/marker.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/marker.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         self.metadata = metadata or {}
 
     name = core.serializable_field("name", str, "Name of this marker.")
 
     marked_range = core.serializable_field(
         "marked_range",
         opentime.TimeRange,
-        "Range this marker applies to."
+        "Range this marker applies to, relative to the Item this marker is "
+        "attached to (e.g. the Clip or Track that owns this marker)."
     )
 
     color = core.serializable_field(
         "color",
         required_type=type(MarkerColor.RED),
         doc="Color string for this marker (for example: 'RED'), based on the "
         "otio.schema.marker.MarkerColor enum."
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/missing_reference.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/missing_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # distributed under the Apache License with the above modification is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
 """
-Implementation of the MisingReference media reference schema.
+Implementation of the MissingReference media reference schema.
 """
 
 from .. import (
     core,
 )
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/serializable_collection.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/serializable_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
 """A serializable collection of SerializableObjects."""
 
 import collections
+import copy
 
 from .. import (
     core
 )
 
 from . import (
     clip
@@ -52,19 +53,19 @@
 
     def __init__(
         self,
         name=None,
         children=None,
         metadata=None,
     ):
-        core.SerializableObject.__init__(self)
+        super(SerializableCollection, self).__init__()
 
         self.name = name
         self._children = children or []
-        self.metadata = metadata or {}
+        self.metadata = copy.deepcopy(metadata) if metadata else {}
 
     name = core.serializable_field(
         "name",
         str,
         doc="SerializableCollection name."
     )
     _children = core.serializable_field(
@@ -121,18 +122,16 @@
     def each_child(
         self,
         search_range=None,
         descended_from_type=core.composable.Composable
     ):
         for i, child in enumerate(self._children):
             # filter out children who are not descended from the specified type
-            if (
-                descended_from_type == core.composable.Composable
-                or isinstance(child, descended_from_type)
-            ):
+            is_descendant = descended_from_type == core.composable.Composable
+            if is_descendant or isinstance(child, descended_from_type):
                 yield child
 
             # for children that are compositions, recurse into their children
             if hasattr(child, "each_child"):
                 for valid_child in (
                     c for c in child.each_child(
                         search_range,
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/stack.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,25 @@
     _modname = "schema"
 
     def __init__(
         self,
         name=None,
         children=None,
         source_range=None,
+        markers=None,
+        effects=None,
         metadata=None
     ):
         core.Composition.__init__(
             self,
             name=name,
             children=children,
             source_range=source_range,
+            markers=markers,
+            effects=effects,
             metadata=metadata
         )
 
     def range_of_child_at_index(self, index):
         try:
             child = self[index]
         except IndexError:
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/timeline.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/timeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
 """Implementation of the OTIO built in schema, Timeline object."""
 
+import copy
+
 from .. import (
     core,
     opentime,
 )
 
 from . import stack, track
 
@@ -39,25 +41,25 @@
     def __init__(
         self,
         name=None,
         tracks=None,
         global_start_time=None,
         metadata=None,
     ):
-        core.SerializableObject.__init__(self)
+        super(Timeline, self).__init__()
         self.name = name
         if global_start_time is None:
             global_start_time = opentime.RationalTime(0, 24)
-        self.global_start_time = global_start_time
+        self.global_start_time = copy.deepcopy(global_start_time)
 
         if tracks is None:
             tracks = []
         self.tracks = stack.Stack(name="tracks", children=tracks)
 
-        self.metadata = metadata or {}
+        self.metadata = copy.deepcopy(metadata) if metadata else {}
 
     name = core.serializable_field("name", doc="Name of this timeline.")
     tracks = core.serializable_field(
         "tracks",
         core.Composition,
         doc="Stack of tracks containing items."
     )
@@ -74,19 +76,15 @@
         return (
             "otio.schema.Timeline(name={}, tracks={})".format(
                 repr(self.name),
                 repr(self.tracks)
             )
         )
 
-    def each_child(
-        self,
-        search_range=None,
-        descended_from_type=core.Composable
-     ):
+    def each_child(self, search_range=None, descended_from_type=core.Composable):
         return self.tracks.each_child(search_range, descended_from_type)
 
     def each_clip(self, search_range=None):
         """Return a flat list of each clip, limited to the search_range."""
 
         return self.tracks.each_clip(search_range)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/track.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/track.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,23 +55,27 @@
     _composition_kind = "Track"
     _modname = "schema"
 
     def __init__(
         self,
         name=None,
         children=None,
-        source_range=None,
         kind=TrackKind.Video,
+        source_range=None,
+        markers=None,
+        effects=None,
         metadata=None,
     ):
         core.Composition.__init__(
             self,
             name=name,
             children=children,
             source_range=source_range,
+            markers=markers,
+            effects=effects,
             metadata=metadata
         )
         self.kind = kind
 
     kind = core.serializable_field(
         "kind",
         doc="Composition kind (Stack, Track)"
@@ -101,20 +105,21 @@
     def handles_of_child(self, child):
         """If media beyond the ends of this child are visible due to adjacent
         Transitions (only applicable in a Track) then this will return the
         head and tail offsets as a tuple of RationalTime objects. If no handles
         are present on either side, then None is returned instead of a
         RationalTime.
 
-        Example usage:
-        head, tail = track.handles_of_child(clip)
-        if head:
-          ...
-        if tail:
-          ...
+        Example usage
+
+        >>> head, tail = track.handles_of_child(clip)
+        >>> if head:
+        ...     print('do something')
+        >>> if tail:
+        ...     print('do something else')
         """
         head, tail = None, None
         before, after = self.neighbors_of(child)
         if isinstance(before, transition.Transition):
             head = before.in_offset
         if isinstance(after, transition.Transition):
             tail = after.out_offset
@@ -152,15 +157,15 @@
         with insert_gap == NeighborGapPolicy.never:
         [A, B, C] :: neighbors_of(B) -> (A, C)
         [A, B, C] :: neighbors_of(A) -> (None, B)
         [A, B, C] :: neighbors_of(C) -> (B, None)
         [A] :: neighbors_of(A) -> (None, None)
 
         with insert_gap == NeighborGapPolicy.around_transitions:
-            (assuming A and C are transitions)
+        (assuming A and C are transitions)
         [A, B, C] :: neighbors_of(B) -> (A, C)
         [A, B, C] :: neighbors_of(A) -> (Gap, B)
         [A, B, C] :: neighbors_of(C) -> (B, Gap)
         [A] :: neighbors_of(A) -> (Gap, Gap)
         """
 
         try:
@@ -172,38 +177,66 @@
                     self
                 )
             )
 
         previous, next_item = None, None
 
         # look before index
-        if (
-            index == 0
-            and insert_gap == NeighborGapPolicy.around_transitions
-            and isinstance(item, transition.Transition)
-        ):
-            previous = gap.Gap(
-                source_range=opentime.TimeRange(duration=item.in_offset)
-            )
+        if index == 0:
+            if insert_gap == NeighborGapPolicy.around_transitions:
+                if isinstance(item, transition.Transition):
+                    previous = gap.Gap(
+                        source_range=opentime.TimeRange(duration=item.in_offset))
         elif index > 0:
             previous = self[index - 1]
 
-        if (
-            index == len(self) - 1
-            and insert_gap == NeighborGapPolicy.around_transitions
-            and isinstance(item, transition.Transition)
-        ):
-            next_item = gap.Gap(
-                source_range=opentime.TimeRange(duration=item.out_offset)
-            )
+        if index == len(self) - 1:
+            if insert_gap == NeighborGapPolicy.around_transitions:
+                if isinstance(item, transition.Transition):
+                    next_item = gap.Gap(
+                        source_range=opentime.TimeRange(duration=item.out_offset))
         elif index < len(self) - 1:
             next_item = self[index + 1]
 
         return collections.namedtuple('neighbors', ('previous', 'next'))(
             previous,
             next_item
         )
 
+    def range_of_all_children(self):
+        """Return a dict mapping children to their range in this track."""
+
+        if not self._children:
+            return {}
+
+        result_map = {}
+
+        # Heuristic to guess what the rate should be set to based on the first
+        # thing in the track.
+        first_thing = self._children[0]
+        if isinstance(first_thing, transition.Transition):
+            rate = first_thing.in_offset.rate
+        else:
+            rate = first_thing.trimmed_range().duration.rate
+
+        last_end_time = opentime.RationalTime(0, rate)
+
+        for thing in self._children:
+            if isinstance(thing, transition.Transition):
+                result_map[thing] = opentime.TimeRange(
+                    last_end_time - thing.in_offset,
+                    thing.out_offset + thing.in_offset,
+                )
+            else:
+                last_range = opentime.TimeRange(
+                    last_end_time,
+                    thing.trimmed_range().duration
+                )
+                result_map[thing] = last_range
+                last_end_time = last_range.end_time_exclusive()
+
+        return result_map
+
 
 # the original name for "track" was "sequence" - this will turn "Sequence"
 # found in OTIO files into Track automatically.
 core.register_type(Track, "Sequence")
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/schema/transition.py` & `OpenTimelineIO-0.9.0/opentimelineio/schema/transition.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,22 @@
 
 from .. import (
     opentime,
     core,
     exceptions,
 )
 
+import copy
+
 
 class TransitionTypes:
     """Enum encoding types of transitions.
 
     This is for representing "Dissolves" and "Wipes" defined by the
-    multi-source effect as defined by:
-        SMPTE 258M-2004 7.6.3.2
+    multi-source effect as defined by SMPTE 258M-2004 7.6.3.2
 
     Other effects are handled by the `schema.Effect` class.
     """
 
     # @{ SMPTE transitions.
     SMPTE_Dissolve = "SMPTE_Dissolve"
     # SMPTE_Wipe = "SMPTE_Wipe" -- @TODO
@@ -75,16 +76,16 @@
 
         # init everything as None first, so that we will catch uninitialized
         # values via exceptions
         # if parameters is None:
         #     parameters = {}
         # self.parameters = parameters
         self.transition_type = transition_type
-        self.in_offset = in_offset
-        self.out_offset = out_offset
+        self.in_offset = copy.deepcopy(in_offset)
+        self.out_offset = copy.deepcopy(out_offset)
 
     transition_type = core.serializable_field(
         "transition_type",
         required_type=type(TransitionTypes.SMPTE_Dissolve),
         doc="Kind of transition, as defined by the "
         "schema.transition.TransitionTypes enum."
     )
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio/core/unknown_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,28 +18,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the Apache License with the above modification is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied. See the Apache License for the specific
 # language governing permissions and limitations under the Apache License.
 #
 
-"""An editorial interchange format and library.
+"""
+Implementation of the UnknownSchema schema.
+"""
 
-see: http://opentimeline.io
+from .serializable_object import SerializableObject
+from .type_registry import register_type
 
-.. moduleauthor:: Pixar Animation Studios <opentimelineio@pixar.com>
-"""
 
-# flake8: noqa
+@register_type
+class UnknownSchema(SerializableObject):
+    """Represents an object whose schema is unknown to us."""
+
+    _serializable_label = "UnknownSchema.1"
+    _name = "UnknownSchema"
+    _original_label = "UnknownSchemaOriginalLabel"
 
-# in dependency hierarchy
-from . import (
-    opentime,
-    exceptions,
-    core,
-    schema,
-    plugins,
-    adapters,
-    algorithms,
-    test_utils,
-    console,
-)
+    @property
+    def is_unknown_schema(self):
+        return True
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/exceptions.py` & `OpenTimelineIO-0.9.0/opentimelineio/exceptions.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/media_linker.py` & `OpenTimelineIO-0.9.0/opentimelineio/media_linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     def __init__(
         self,
         name=None,
         execution_scope=None,
         filepath=None,
     ):
-        plugins.PythonPlugin.__init__(self, name, execution_scope, filepath)
+        super(MediaLinker, self).__init__(name, execution_scope, filepath)
 
     def link_media_reference(self, in_clip, media_linker_argument_map=None):
         media_linker_argument_map = media_linker_argument_map or {}
 
         return self._execute_function(
             "link_media_reference",
             in_clip=in_clip,
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/opentime.py` & `OpenTimelineIO-0.9.0/opentimelineio/opentime.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,22 @@
     23.976,
     23.98,
     24,
     25,
     30,
     48,
     50,
-    60
-    )
+    60)
 
 VALID_DROPFRAME_TIMECODE_RATES = (
     29.97,
-    59.94
-    )
+    59.94)
 
 VALID_TIMECODE_RATES = (
-    VALID_NON_DROPFRAME_TIMECODE_RATES + VALID_DROPFRAME_TIMECODE_RATES
-    )
+    VALID_NON_DROPFRAME_TIMECODE_RATES + VALID_DROPFRAME_TIMECODE_RATES)
 
 
 class RationalTime(object):
     """ Represents an instantaneous point in time, value * (1/rate) seconds
     from time 0seconds.
     """
 
@@ -135,14 +132,15 @@
         else:
             scale = other.rate
             value = (self.value_rescaled_to(scale) + other.value)
 
         self.value = value
         self.rate = scale
 
+        # @TODO: make this construct and return a new object
         return self
 
     def __add__(self, other):
         """Returns a RationalTime object that is the sum of self and other.
 
         If self and other have differing time rates, the result will have the
         have the rate of the faster time.
@@ -232,15 +230,15 @@
         return hash((self.value, self.rate))
 
 
 class TimeTransform(object):
     """1D Transform for RationalTime.  Has offset and scale."""
 
     def __init__(self, offset=RationalTime(), scale=1.0, rate=None):
-        self.offset = offset
+        self.offset = copy.copy(offset)
         self.scale = scale
         self.rate = rate
 
     def applied_to(self, other):
         if isinstance(other, TimeRange):
             return range_from_start_end_time(
                 start_time=self.applied_to(other.start_time),
@@ -314,16 +312,16 @@
     lasting duration.value * (1/duration.rate) seconds.
 
     A 0 duration TimeRange is the same as a RationalTime, and contains only the
     start_time of the TimeRange.
     """
 
     def __init__(self, start_time=RationalTime(), duration=RationalTime()):
-        self.start_time = start_time
-        self.duration = duration
+        self.start_time = copy.copy(start_time)
+        self.duration = copy.copy(duration)
 
     def __copy__(self, memodict=None):
         # Construct a new one directly to avoid the overhead of deepcopy
         return TimeRange(
             copy.copy(self.start_time),
             copy.copy(self.duration)
         )
@@ -353,30 +351,29 @@
         If the TimeRange goes from (0, 24) w/ duration (10.5, 24):
         (10, 24)
 
         In other words, the last frame with data (however fractional).
         """
 
         if (
-            self.end_time_exclusive()
-            - self.start_time.rescaled_to(self.duration)
+            self.end_time_exclusive() - self.start_time.rescaled_to(self.duration)
         ).value > 1:
 
             result = (
                 self.end_time_exclusive() - RationalTime(1, self.duration.rate)
             )
 
             # if the duration's value has a fractional component
             if self.duration.value != math.floor(self.duration.value):
                 result = self.end_time_exclusive()
                 result.value = math.floor(result.value)
 
             return result
         else:
-            return self.start_time
+            return copy.deepcopy(self.start_time)
 
     def end_time_exclusive(self):
         """"Time of the first sample outside the time range.
 
         If Start Frame is 10 and duration is 5, then end_time_exclusive is 15,
         even though the last time with data in this range is 14.
 
@@ -385,32 +382,28 @@
         """
 
         return self.duration + self.start_time.rescaled_to(self.duration)
 
     def extended_by(self, other):
         """Construct a new TimeRange that is this one extended by another."""
 
-        result = TimeRange(self.start_time, self.duration)
-        if isinstance(other, TimeRange):
-            result.start_time = min(self.start_time, other.start_time)
-            new_end_time = max(
-                self.end_time_exclusive(),
-                other.end_time_exclusive()
-            )
-            result.duration = duration_from_start_end_time(
-                result.start_time,
-                new_end_time
-            )
-        else:
+        if not isinstance(other, TimeRange):
             raise TypeError(
                 "extended_by requires rtime be a TimeRange, not a '{}'".format(
                     type(other)
                 )
             )
-        return result
+
+        start_time = min(self.start_time, other.start_time)
+        new_end_time = max(
+            self.end_time_exclusive(),
+            other.end_time_exclusive()
+        )
+        duration = duration_from_start_end_time(start_time, new_end_time)
+        return TimeRange(start_time, duration)
 
     # @TODO: remove?
     def clamped(
         self,
         other,
         start_bound=BoundStrategy.Free,
         end_bound=BoundStrategy.Free
@@ -452,17 +445,15 @@
         """Return true if self completely contains other.
 
         (RationalTime or TimeRange)
         """
 
         if isinstance(other, RationalTime):
             return (
-                self.start_time <= other
-                and other < self.end_time_exclusive()
-            )
+                self.start_time <= other and other < self.end_time_exclusive())
         elif isinstance(other, TimeRange):
             return (
                 self.start_time <= other.start_time and
                 self.end_time_exclusive() >= other.end_time_exclusive()
             )
         raise TypeError(
             "contains only accepts on otio.opentime.RationalTime or "
@@ -520,16 +511,15 @@
             )
         )
 
 
 def from_frames(frame, fps):
     """Turn a frame number and fps into a time object.
     :param frame: (:class:`int`) Frame number.
-    :param fps: (:class:`float`) The frame-rate for the (:class:`RationalTime`)
-        instance.
+    :param fps: (:class:`float`) Frame-rate for the (:class:`RationalTime`) instance.
 
     :return: (:class:`RationalTime`) Instance for the frame and fps provided.
     """
 
     return RationalTime(int(frame), fps)
 
 
@@ -547,25 +537,22 @@
     Raises (:class:`TypeError` for wrong type of rate.
     Raises (:class:`VaueError`) for invalid rate value.
 
     :param rate: (:class:`int`) or (:class:`float`) The frame rate in question
     """
     if not isinstance(rate, (int, float)):
         raise TypeError(
-                "rate must be <float> or <int> not {t}".format(t=type(rate))
-                )
+            "rate must be <float> or <int> not {t}".format(t=type(rate)))
 
     if rate not in VALID_TIMECODE_RATES:
         raise ValueError(
             '{rate} is not a valid frame rate, '
             'Please use one of these: {valid}'.format(
-                                                    rate=rate,
-                                                    valid=VALID_TIMECODE_RATES
-                                                    )
-            )
+                rate=rate,
+                valid=VALID_TIMECODE_RATES))
 
 
 def from_timecode(timecode_str, rate):
     """Convert a timecode string into a RationalTime.
 
     :param timecode_str: (:class:`str`) A colon-delimited timecode.
     :param rate: (:class:`float`) The frame-rate to calculate timecode in
@@ -579,23 +566,21 @@
     # Check if rate is drop frame
     rate_is_dropframe = rate in VALID_DROPFRAME_TIMECODE_RATES
 
     # Check if timecode indicates drop frame
     if ';' in timecode_str:
         if not rate_is_dropframe:
             raise ValueError(
-               'Timecode "{}" indicates drop-frame rate '
-               'due to the ";" frame divider. '
-               'Passed rate ({}) is of non-drop-frame rate. '
-               'Valid drop-frame rates are: {}'.format(
-                                        timecode_str,
-                                        rate,
-                                        VALID_DROPFRAME_TIMECODE_RATES
-                                        )
-                )
+                'Timecode "{}" indicates drop-frame rate '
+                'due to the ";" frame divider. '
+                'Passed rate ({}) is of non-drop-frame rate. '
+                'Valid drop-frame rates are: {}'.format(
+                    timecode_str,
+                    rate,
+                    VALID_DROPFRAME_TIMECODE_RATES))
         else:
             timecode_str = timecode_str.replace(';', ':')
 
     hours, minutes, seconds, frames = timecode_str.split(":")
 
     # Timecode is declared in terms of nominal fps
     nominal_fps = int(math.ceil(rate))
@@ -614,16 +599,16 @@
             dropframes = 4
 
     # To use for drop frame compensation
     total_minutes = int(hours) * 60 + int(minutes)
 
     # convert to frames
     value = (
-        ((total_minutes * 60) + int(seconds)) * nominal_fps + int(frames)
-        ) - (dropframes * (total_minutes - (total_minutes // 10)))
+        ((total_minutes * 60) + int(seconds)) * nominal_fps + int(frames)) - \
+        (dropframes * (total_minutes - (total_minutes // 10)))
 
     return RationalTime(value, rate)
 
 
 def to_timecode(time_obj, rate=None):
     """Convert a RationalTime into a timecode string.
 
@@ -667,16 +652,15 @@
     # the number of dropped frames
     frames_per_minute = int(round(rate) * 60) - dropframes
 
     value = time_obj.value
 
     if value < 0:
         raise ValueError(
-            "Negative values are not supported for converting to timecode."
-            )
+            "Negative values are not supported for converting to timecode.")
 
     # If frame_number is greater than 24 hrs, next operation will rollover
     # clock
     value %= frames_per_24_hours
 
     if rate_is_dropframe:
         d = value // frames_per_10_minutes
@@ -693,20 +677,19 @@
     seconds = (value // nominal_fps) % 60
     minutes = ((value // nominal_fps) // 60) % 60
     hours = (((value // nominal_fps) // 60) // 60)
 
     tc = "{HH:02d}:{MM:02d}:{SS:02d}{div}{FF:02d}"
 
     return tc.format(
-                HH=int(hours),
-                MM=int(minutes),
-                SS=int(seconds),
-                div=rate_is_dropframe and ";" or ":",
-                FF=int(frames)
-                )
+        HH=int(hours),
+        MM=int(minutes),
+        SS=int(seconds),
+        div=rate_is_dropframe and ";" or ":",
+        FF=int(frames))
 
 
 def from_time_string(time_str, rate):
     """Convert a time with microseconds string into a RationalTime.
 
     :param time_str: (:class:`str`) A HH:MM:ss.ms time.
     :param rate: (:class:`float`) The frame-rate to calculate timecode in
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio/test_utils.py` & `OpenTimelineIO-0.9.0/opentimelineio/test_utils.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/advanced_authoring_format.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/advanced_authoring_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,31 @@
             result.append(
                 _transcribe(
                     child,
                     parent=item,
                     masterMobs=masterMobs
                 )
             )
+    elif isinstance(item, aaf.component.Selector):
+        # If you mute a clip in media composer, it becomes one of these in the
+        # AAF.
+        result = _transcribe(item.selected, parent=item, masterMobs=masterMobs)
+
+        alternates = [
+            _transcribe(alt, parent=item, masterMobs=masterMobs)
+            for alt in item.alternate_segments()
+        ]
+
+        # muted case -- if there is only one item its muted, otherwise its
+        # a multi cam thing
+        if alternates and len(alternates) == 1:
+            metadata['muted_clip'] = True
+            result.name = str(alternates[0].name) + "_MUTED"
+
+        metadata['alternates'] = alternates
 
     # @TODO: There are a bunch of other AAF object types that we will
     # likely need to add support for. I'm leaving this code here to help
     # future efforts to extract the useful information out of these.
 
     # elif isinstance(item, aaf.storage.File):
     #     self.extendChildItems([item.header])
@@ -580,30 +597,30 @@
                 # Don't touch the Transitions themselves,
                 # only the Clips & Gaps next to them.
                 if not isinstance(child, otio.core.Item):
                     continue
 
                 # Was the item before us a Transition?
                 if c > 0 and isinstance(
-                    thing[c-1],
+                    thing[c - 1],
                     otio.schema.Transition
                 ):
-                    pre_trans = thing[c-1]
+                    pre_trans = thing[c - 1]
 
                     if child.source_range is None:
                         child.source_range = child.trimmed_range()
                     child.source_range.start_time += pre_trans.in_offset
                     child.source_range.duration -= pre_trans.in_offset
 
                 # Is the item after us a Transition?
-                if c < len(thing)-1 and isinstance(
-                    thing[c+1],
+                if c < len(thing) - 1 and isinstance(
+                    thing[c + 1],
                     otio.schema.Transition
                 ):
-                    post_trans = thing[c+1]
+                    post_trans = thing[c + 1]
 
                     if child.source_range is None:
                         child.source_range = child.trimmed_range()
                     child.source_range.duration -= post_trans.out_offset
 
         for child in thing:
             _fix_transitions(child)
@@ -639,37 +656,37 @@
             for c in reversed(range(len(thing))):
                 child = thing[c]
                 if not _contains_something_valuable(child):
                     # TODO: We're discarding metadata... should we retain it?
                     del thing[c]
 
             # Look for Stacks within Stacks
-            c = len(thing)-1
+            c = len(thing) - 1
             while c >= 0:
                 child = thing[c]
                 # Is my child a Stack also?
                 if (
-                    isinstance(child, otio.schema.Stack) and
-                    not _has_effects(child)
+                    isinstance(child, otio.schema.Stack)
+                    and not _has_effects(child)
                 ):
                     # Pull the child's children into the parent
                     num = len(child)
-                    thing[c:c+1] = child[:]
+                    thing[c:c + 1] = child[:]
 
                     # TODO: We may be discarding metadata, should we merge it?
                     # TODO: Do we need to offset the markers in time?
                     thing.markers.extend(child.markers)
                     # Note: we don't merge effects, because we already made
                     # sure the child had no effects in the if statement above.
 
-                    c = c+num
-                c = c-1
+                    c = c + num
+                c = c - 1
 
         # skip redundant containers
-        if len(thing) == 1:
+        if _is_redundant_container(thing):
             # TODO: We may be discarding metadata here, should we merge it?
             result = thing[0].deepcopy()
             # TODO: Do we need to offset the markers in time?
             result.markers.extend(thing.markers)
             # TODO: The order of the effects is probably important...
             # should they be added to the end or the front?
             result.effects.extend(thing.effects)
@@ -687,14 +704,27 @@
 
 def _has_effects(thing):
     if isinstance(thing, otio.core.Item):
         if len(thing.effects) > 0:
             return True
 
 
+def _is_redundant_container(thing):
+    return (
+        isinstance(thing, otio.core.Composition) and
+        (
+            # A container with length of one
+            len(thing) == 1 and
+
+            # ...which contains a container
+            isinstance(thing[0], otio.core.Composition)
+        )
+    )
+
+
 def _contains_something_valuable(thing):
     if isinstance(thing, otio.core.Item):
         if len(thing.effects) > 0 or len(thing.markers) > 0:
             return True
 
     if isinstance(thing, otio.core.Composition):
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/ale.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/ale.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     row = line.split("\t")
 
     if len(row) < len(columns):
         # Fill in blanks for any missing fields in this row
         row.extend([""] * (len(columns) - len(row)))
 
     if len(row) > len(columns):
-        raise ALEParseError("Too many values on row: "+line)
+        raise ALEParseError("Too many values on row: " + line)
 
     try:
 
         # Gather all the columns into a dictionary
         # For expected columns, like Name, Start, etc. we will pop (remove)
         # those from metadata, leaving the rest alone.
         metadata = dict(zip(columns, row))
@@ -80,15 +80,17 @@
                         value
                     ))
             if duration is None:
                 duration = end - start
             if end is None:
                 end = start + duration
             if end != start + duration:
-                raise ALEParseError("Inconsistent Start, End, Duration: "+line)
+                raise ALEParseError(
+                    "Inconsistent Start, End, Duration: " + line
+                )
             clip.source_range = otio.opentime.TimeRange(
                 start,
                 duration
             )
 
         if metadata.get("Source File"):
             source = metadata.pop("Source File")
@@ -128,29 +130,29 @@
             while len(lines):
                 line = nextline(lines)
 
                 if line.strip() == "":
                     break
 
                 if "\t" not in line:
-                    raise ALEParseError("Invalid Heading line: "+line)
+                    raise ALEParseError("Invalid Heading line: " + line)
 
                 segments = line.split("\t")
                 while len(segments) >= 2:
                     key, val = segments.pop(0), segments.pop(0)
                     header[key] = val
                 if len(segments) != 0:
-                    raise ALEParseError("Invalid Heading line: "+line)
+                    raise ALEParseError("Invalid Heading line: " + line)
 
         if "FPS" in header:
             fps = float(header["FPS"])
 
         if line.strip() == "Column":
             if len(lines) == 0:
-                raise ALEParseError("Unexpected end of file after: "+line)
+                raise ALEParseError("Unexpected end of file after: " + line)
 
             line = nextline(lines)
             columns = line.split("\t")
 
         if line.strip() == "Data":
             while len(lines):
                 line = nextline(lines)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/burnins.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/burnins.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/contrib_adapters.plugin_manifest.json` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/contrib_adapters.plugin_manifest.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'adapters'": "{insert: [(0, OrderedDict([('OTIO_SCHEMA', 'Adapter.1'), ('name', 'fcpx_xml'), "*

 * *               "('execution_scope', 'in process'), ('filepath', 'fcpx_xml.py'), ('suffixes', "*

 * *               "['fcpxml'])]))]}"}*

```diff
@@ -1,13 +1,22 @@
 {
     "OTIO_SCHEMA": "PluginManifest.1",
     "adapters": [
         {
             "OTIO_SCHEMA": "Adapter.1",
             "execution_scope": "in process",
+            "filepath": "fcpx_xml.py",
+            "name": "fcpx_xml",
+            "suffixes": [
+                "fcpxml"
+            ]
+        },
+        {
+            "OTIO_SCHEMA": "Adapter.1",
+            "execution_scope": "in process",
             "filepath": "hls_playlist.py",
             "name": "hls_playlist",
             "suffixes": [
                 "m3u8"
             ]
         },
         {
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/extern_maya_sequencer.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/extern_maya_sequencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,16 @@
     else:
         cmds.file(filepath, o=True)
         sys.stdout.write(
             "\nOTIO_JSON_BEGIN\n" +
             otio.adapters.write_to_string(
                 read_sequence(),
                 "otio_json"
-            )
-            + "\nOTIO_JSON_END\n"
+            ) +
+            "\nOTIO_JSON_END\n"
         )
 
     cmds.quit(force=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/extern_rv.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/extern_rv.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/ffmpeg_burnins.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/ffmpeg_burnins.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             'text': options.get('expression') or text,
             'color': options['font_color'],
             'size': options['font_size']
         }
         data.update(options)
         data.update(_drawtext(align, resolution, text, options))
         if 'font' in data and _is_windows():
-            data['font'] = data['font'].replace(os.sep, r'\\'+os.sep)
+            data['font'] = data['font'].replace(os.sep, r'\\' + os.sep)
             data['font'] = data['font'].replace(':', r'\:')
         self.filters['drawtext'].append(draw % data)
 
         if options.get('bg_color') is not None:
             box = BOX % {
                 'border': options['bg_padding'],
                 'color': options['bg_color'],
@@ -414,11 +414,11 @@
     else:
         y_pos = 'h-text_h-%d' % (options['y_offset'])
     return {'x': x_pos, 'y': y_pos}
 
 
 def _frames_to_timecode(frames, framerate):
     return '{0:02d}:{1:02d}:{2:02d}:{3:02d}'.format(
-        int(frames / (3600*framerate)),
-        int(frames / (60*framerate) % 60),
+        int(frames / (3600 * framerate)),
+        int(frames / (60 * framerate) % 60),
         int(frames / framerate % 60),
         int(frames % framerate))
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/hls_playlist.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/hls_playlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,23 +876,23 @@
         "EXT-X-PLAYLIST-TYPE": _handle_track_metadata,
         "EXT-X-INDEPENDENT-SEGMENTS": _handle_track_metadata,
         "EXT-X-BYTERANGE": _handle_BYTERANGE
     }
 
     def _parse_entries(self, playlist_entries, playlist_version):
         """Interpret the entries through the lens of the schema"""
-        current_media_ref = otio.schema.ExternalReference(
-            metadata={
-                FORMAT_METADATA_KEY: {},
-                STREAMING_METADATA_KEY: {}
-            }
-        )
         current_clip = otio.schema.Clip(
-            media_reference=current_media_ref
+            media_reference=otio.schema.ExternalReference(
+                metadata={
+                    FORMAT_METADATA_KEY: {},
+                    STREAMING_METADATA_KEY: {}
+                }
+            )
         )
+        current_media_ref = current_clip.media_reference
         segment_metadata = {}
         current_map_data = {}
         # per section 4.3.3.2 of Pantos HLS, 0 is default start track
         current_track = 0
         for entry in playlist_entries:
             if entry.type == EntryType.URI:
                 # the URI ends the segment definition
@@ -907,23 +907,23 @@
                     STREAMING_METADATA_KEY,
                     {}
                 )[SEQUENCE_NUM_KEY] = current_track
                 self.track.append(current_clip)
                 current_track += 1
 
                 # Set up the next segment definition
-                current_media_ref = otio.schema.ExternalReference(
-                    metadata={
-                        FORMAT_METADATA_KEY: {},
-                        STREAMING_METADATA_KEY: {}
-                    }
-                )
                 current_clip = otio.schema.Clip(
-                    media_reference=current_media_ref
+                    media_reference=otio.schema.ExternalReference(
+                        metadata={
+                            FORMAT_METADATA_KEY: {},
+                            STREAMING_METADATA_KEY: {}
+                        }
+                    )
                 )
+                current_media_ref = current_clip.media_reference
                 continue
             elif entry.type != EntryType.tag:
                 # the rest of the code deals only with tags
                 continue
 
             # Explode the EXT-X-MAP info out
             if entry.tag_name == "EXT-X-MAP":
@@ -1369,16 +1369,16 @@
             track_start = first_segment_streaming_metadata.get(
                 SEQUENCE_NUM_KEY
             )
 
         # If we found a track start or one isn't already set in the
         # metadata, create the tag for it.
         if (
-            track_start is not None
-            or 'EXT-X-MEDIA-SEQUENCE' not in self._playlist_tags
+            track_start is not None or
+            'EXT-X-MEDIA-SEQUENCE' not in self._playlist_tags
         ):
             # Choose a reasonable track start default
             if track_start is None:
                 track_start = 1
             self._playlist_tags['EXT-X-MEDIA-SEQUENCE'] = str(track_start)
 
     def _add_map_entry(self, fragment):
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/maya_sequencer.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/maya_sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     # maya probably puts a bunch of crap on the stdout
     sentinel_str = "OTIO_JSON_BEGIN\n"
     end_sentinel_str = "\nOTIO_JSON_END\n"
     start = out.find(sentinel_str)
     end = out.find(end_sentinel_str)
     result = adapters.read_from_string(
-        out[start+len(sentinel_str):end],
+        out[start + len(sentinel_str):end],
         "otio_json"
     )
 
     if proc.returncode:
         raise RuntimeError(
             "ERROR: extern_maya_sequencer (called through the maya sequencer "
             "file adapter) failed. stderr output: " + err
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/adapters/rv.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/adapters/rv.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # language governing permissions and limitations under the Apache License.
 #
 
 """RvSession Adapter harness"""
 
 import subprocess
 import os
+import copy
 
 from .. import adapters
 
 
 def write_to_file(input_otio, filepath):
     if "OTIO_RV_PYTHON_BIN" not in os.environ:
         raise RuntimeError(
@@ -41,34 +42,36 @@
         raise RuntimeError(
             "'OTIO_RV_PYTHON_LIB' not set, please set this to path to python "
             "directory within the RV installation."
         )
 
     input_data = adapters.write_to_string(input_otio, "otio_json")
 
-    os.environ['PYTHONPATH'] = (
+    base_environment = copy.deepcopy(os.environ)
+
+    base_environment['PYTHONPATH'] = (
         os.pathsep.join(
             [
-                os.environ.setdefault('PYTHONPATH', ''),
+                base_environment.setdefault('PYTHONPATH', ''),
                 os.path.dirname(__file__)
             ]
         )
     )
 
     proc = subprocess.Popen(
         [
-            os.environ["OTIO_RV_PYTHON_BIN"],
+            base_environment["OTIO_RV_PYTHON_BIN"],
             '-m',
             'extern_rv',
             filepath
         ],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
-        env=os.environ
+        env=base_environment
     )
     proc.stdin.write(input_data)
     out, err = proc.communicate()
 
     if out.strip():
         print("stdout: {}".format(out))
     if err.strip():
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineio_contrib/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineio_contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineview/__init__.py` & `OpenTimelineIO-0.9.0/opentimelineview/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenTimelineIO-0.8.1/opentimelineview/console.py` & `OpenTimelineIO-0.9.0/opentimelineview/console.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import sys
 import argparse
 import ast
 from PySide2 import QtWidgets, QtGui
 
 import opentimelineio as otio
 import opentimelineview as otioViewWidget
+from opentimelineview import settings
 
 
 def _parsed_args():
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
@@ -52,28 +53,41 @@
         type=str,
         default=[],
         action='append',
         help='Extra arguments to be passed to adapter in the form of '
         'key=value. Values are strings, numbers or Python literals: True, '
         'False, etc. Can be used multiple times: -a burrito="bar" -a taco=12.'
     )
+    parser.add_argument(
+        '-m',
+        '--media-linker',
+        type=str,
+        default="Default",
+        help=(
+            "Specify a media linker.  'Default' means use the "
+            "$OTIO_DEFAULT_MEDIA_LINKER if set, 'None' or '' means explicitly "
+            "disable the linker, and anything else is interpreted as the name"
+            " of the media linker to use."
+        )
+    )
 
     return parser.parse_args()
 
 
 class TimelineWidgetItem(QtWidgets.QListWidgetItem):
     def __init__(self, timeline, *args, **kwargs):
         super(TimelineWidgetItem, self).__init__(*args, **kwargs)
         self.timeline = timeline
 
 
 class Main(QtWidgets.QMainWindow):
-    def __init__(self, adapter_argument_map, *args, **kwargs):
+    def __init__(self, adapter_argument_map, media_linker, *args, **kwargs):
         super(Main, self).__init__(*args, **kwargs)
         self.adapter_argument_map = adapter_argument_map or {}
+        self.media_linker = media_linker
 
         self._current_file = None
 
         # window options
         self.setWindowTitle('OpenTimelineIO Viewer')
         self.resize(1900, 1200)
 
@@ -121,14 +135,16 @@
         self.tracks_widget.itemSelectionChanged.connect(
             self._change_track
         )
         self.timeline_widget.selection_changed.connect(
             self.details_widget.set_item
         )
 
+        self.setStyleSheet(settings.VIEW_STYLESHEET)
+
     def _file_load(self):
         start_folder = None
         if self._current_file is not None:
             start_folder = os.path.dirname(self._current_file)
 
         extensions = otio.adapters.suffixes_with_defined_adapters(read=True)
 
@@ -149,14 +165,15 @@
     def load(self, path):
         self._current_file = path
         self.setWindowTitle('OpenTimelineIO View: "{}"'.format(path))
         self.details_widget.set_item(None)
         self.tracks_widget.clear()
         file_contents = otio.adapters.read_from_file(
             path,
+            media_linker_name=self.media_linker,
             **self.adapter_argument_map
         )
 
         if isinstance(file_contents, otio.schema.Timeline):
             self.timeline_widget.set_timeline(file_contents)
             self.tracks_widget.setVisible(False)
         elif isinstance(
@@ -183,14 +200,23 @@
         frame.moveCenter(centerPoint)
         self.move(frame.topLeft())
 
 
 def main():
     args = _parsed_args()
 
+    # allow user to explicitly set or pass to default or disable the linker.
+    if args.media_linker.lower() == 'default':
+        ml = otio.media_linker.MediaLinkingPolicy.ForceDefaultLinker
+    elif args.media_linker.lower() in ['none', '']:
+        ml = otio.media_linker.MediaLinkingPolicy.DoNotLinkMedia
+    else:
+        ml = args.media_linker
+
+
     argument_map = {}
     for pair in args.adapter_arg:
         if '=' in pair:
             key, val = pair.split('=', 1)  # only split on the 1st '='
             try:
                 # Sometimes we need to pass a bool, int, list, etc.
                 parsed_value = ast.literal_eval(val)
@@ -203,15 +229,15 @@
                 "error: adapter arguments must be in the form key=value"
                 " got: {}".format(pair)
             )
             sys.exit(1)
 
     application = QtWidgets.QApplication(sys.argv)
 
-    window = Main(argument_map)
+    window = Main(argument_map, ml)
 
     if args.input is not None:
         window.load(args.input)
 
     window.center()
     window.show()
     window.raise_()
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineview/details_widget.py` & `OpenTimelineIO-0.9.0/opentimelineview/details_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         super(Details, self).__init__(*args, **kwargs)
         self.setReadOnly(True)
         self.font = QtGui.QFontDatabase.systemFont(
             QtGui.QFontDatabase.FixedFont)
         self.font.setPointSize(12)
         self.setFont(self.font)
 
-        self.backgroundColor = QtGui.QColor(43, 43, 43)
+        self.backgroundColor = QtGui.QColor(33, 33, 33)
         self.textColor = QtGui.QColor(180, 180, 180)
         self.highlightColor = QtGui.QColor(255, 198, 109)
         self.keywordColor = QtGui.QColor(204, 120, 50)
 
         self.palette = QtGui.QPalette()
         self.palette.setColor(QtGui.QPalette.Base, self.backgroundColor)
         self.palette.setColor(QtGui.QPalette.Text, self.textColor)
@@ -107,20 +107,20 @@
         while index >= 0:
             length = expression.matchedLength()
             firstQuoteIndex = text.index('"', index)
             valueLength = length - (firstQuoteIndex - index) - 2
             self.setFormat(firstQuoteIndex + 1, valueLength, self.value_format)
             index = expression.indexIn(text, index + length)
 
-        expression = QtCore.QRegExp("\\: (null|true|false|[0-9\.]+)")
+        expression = QtCore.QRegExp(r"\\: (null|true|false|[0-9\.]+)")
         index = expression.indexIn(text)
         while index >= 0:
             length = expression.matchedLength()
             self.setFormat(index, length, self.literal_format)
             index = expression.indexIn(text, index + length)
 
-        expression = QtCore.QRegExp("\"OTIO_SCHEMA\"\s*:\s*\".*\"")
+        expression = QtCore.QRegExp(r"\"OTIO_SCHEMA\"\s*:\s*\".*\"")
         index = expression.indexIn(text)
         while index >= 0:
             length = expression.matchedLength()
             self.setFormat(index, length, self.schema_format)
             index = expression.indexIn(text, index + length)
```

### Comparing `OpenTimelineIO-0.8.1/opentimelineview/timeline_widget.py` & `OpenTimelineIO-0.9.0/opentimelineview/timeline_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,27 @@
                 continue
 
             # @TODO: set the marker color if its set from the OTIO object
             marker = Marker(m, None)
             marker.setY(0.5 * MARKER_SIZE)
             marker.setX(
                 (
-                    otio.opentime.to_seconds(m.marked_range.start_time)
-                    - otio.opentime.to_seconds(trimmed_range.start_time)
+                    otio.opentime.to_seconds(m.marked_range.start_time) -
+                    otio.opentime.to_seconds(trimmed_range.start_time)
                 ) * TIME_MULTIPLIER
             )
             marker.setParentItem(self)
 
     def _position_labels(self):
         self.source_in_label.setY(LABEL_MARGIN)
         self.source_out_label.setY(LABEL_MARGIN)
         self.source_name_label.setY(
-            TRACK_HEIGHT
-            - LABEL_MARGIN
-            - self.source_name_label.boundingRect().height()
+            TRACK_HEIGHT -
+            LABEL_MARGIN -
+            self.source_name_label.boundingRect().height()
         )
 
     def _set_labels_rational_time(self):
         trimmed_range = self.item.trimmed_range()
         self.source_in_label.setText(
             '{value}\n@{rate}'.format(
                 value=trimmed_range.start_time.value,
@@ -117,27 +117,29 @@
             '{value}\n@{rate}'.format(
                 value=trimmed_range.end_time_exclusive().value,
                 rate=trimmed_range.end_time_exclusive().rate
             )
         )
 
     def _set_labels_timecode(self):
-        self.source_in_label.setText('{timeline}\n{source}'.format(
+        self.source_in_label.setText(
+            '{timeline}\n{source}'.format(
                 timeline=otio.opentime.to_timecode(
                     self.timeline_range.start_time,
                     self.timeline_range.start_time.rate
                 ),
                 source=otio.opentime.to_timecode(
                     self.item.trimmed_range.start_time,
                     self.item.trimmed_range.start_time.rate
                 )
             )
         )
 
-        self.source_out_label.setText('{timeline}\n{source}'.format(
+        self.source_out_label.setText(
+            '{timeline}\n{source}'.format(
                 timeline=otio.opentime.to_timecode(
                     self.timeline_range.end_time_exclusive(),
                     self.timeline_range.end_time_exclusive().rate
                 ),
                 source=otio.opentime.to_timecode(
                     self.item.trimmed_range.end_time_exclusive(),
                     self.item.trimmed_range.end_time_exclusive().rate
@@ -296,16 +298,16 @@
                 new_item = TransitionItem(item, timeline_range, rect)
             else:
                 print("Warning: could not add item {} to UI.".format(item))
                 continue
 
             new_item.setParentItem(self)
             new_item.setX(
-                otio.opentime.to_seconds(timeline_range.start_time)
-                * TIME_MULTIPLIER
+                otio.opentime.to_seconds(timeline_range.start_time) *
+                TIME_MULTIPLIER
             )
             new_item.counteract_zoom()
 
 
 class Marker(QtWidgets.QGraphicsPolygonItem):
     def __init__(self, marker, *args, **kwargs):
         self.item = marker
@@ -349,16 +351,15 @@
         self.setPen(pen)
 
 
 class CompositionWidget(QtWidgets.QGraphicsScene):
     def __init__(self, composition, *args, **kwargs):
         super(CompositionWidget, self).__init__(*args, **kwargs)
         self.composition = composition
-
-        self.setBackgroundBrush(QtGui.QBrush(QtGui.QColor(64, 78, 87, 255)))
+        self.setBackgroundBrush(QtGui.QBrush(QtGui.QColor(33, 33, 33)))
 
         self._adjust_scene_size()
         self._add_time_slider()
         self._add_tracks()
         self._add_markers()
 
     def _adjust_scene_size(self):
@@ -391,20 +392,20 @@
                 " otio.schema.Stack and otio.schema.Track".format(
                     self.composition,
                     type(self.composition)
                 )
             )
 
         height = (
-            TIME_SLIDER_HEIGHT
-            + (
-                int(has_video_tracks and has_audio_tracks)
-                * MEDIA_TYPE_SEPARATOR_HEIGHT
-            )
-            + len(self.composition) * TRACK_HEIGHT
+            TIME_SLIDER_HEIGHT +
+            (
+                int(has_video_tracks and has_audio_tracks) *
+                MEDIA_TYPE_SEPARATOR_HEIGHT
+            ) +
+            len(self.composition) * TRACK_HEIGHT
         )
 
         self.setSceneRect(
             start_time * TIME_MULTIPLIER,
             0,
             duration * TIME_MULTIPLIER,
             height
@@ -445,16 +446,16 @@
 
             other_tracks = [
                 t for t in self.composition
                 if (
                     t.kind not in (
                         otio.schema.TrackKind.Video,
                         otio.schema.TrackKind.Audio
-                    )
-                    and list(t)
+                    ) and
+                    list(t)
                 )
             ]
         else:
             if self.composition.kind == otio.schema.TrackKind.Video:
                 video_tracks = [self.composition]
             elif self.composition.kind == otio.schema.TrackKind.Audio:
                 audio_tracks = [self.composition]
@@ -468,33 +469,33 @@
                     " '{}'".format(t.name, t.kind)
                 )
 
             video_tracks.extend(other_tracks)
 
         video_tracks_top = TIME_SLIDER_HEIGHT
         audio_tracks_top = (
-            TIME_SLIDER_HEIGHT
-            + len(video_tracks) * TRACK_HEIGHT
-            + int(
+            TIME_SLIDER_HEIGHT +
+            len(video_tracks) * TRACK_HEIGHT +
+            int(
                 bool(video_tracks) and bool(audio_tracks)
             ) * MEDIA_TYPE_SEPARATOR_HEIGHT
         )
 
         for i, track in enumerate(audio_tracks):
             self._add_track(track, audio_tracks_top + i * TRACK_HEIGHT)
 
         for i, track in enumerate(video_tracks):
             self._add_track(track, video_tracks_top + i * TRACK_HEIGHT)
 
     def _add_markers(self):
         for m in self.composition.markers:
             marker = Marker(m, None)
             marker.setX(
-                otio.opentime.to_seconds(m.marked_range.start_time)
-                * TIME_MULTIPLIER
+                otio.opentime.to_seconds(m.marked_range.start_time) *
+                TIME_MULTIPLIER
             )
             marker.setY(TIME_SLIDER_HEIGHT - MARKER_SIZE)
             self.addItem(marker)
 
 
 class CompositionView(QtWidgets.QGraphicsView):
 
@@ -503,15 +504,15 @@
 
     def __init__(self, stack, *args, **kwargs):
         super(CompositionView, self).__init__(*args, **kwargs)
         self.setResizeAnchor(QtWidgets.QGraphicsView.AnchorUnderMouse)
         self.setTransformationAnchor(QtWidgets.QGraphicsView.AnchorUnderMouse)
         self.setScene(CompositionWidget(stack, parent=self))
         self.setAlignment((QtCore.Qt.AlignLeft | QtCore.Qt.AlignTop))
-
+        self.setStyleSheet('border: 0px;')
         self.scene().selectionChanged.connect(self.parse_selection_change)
 
     def parse_selection_change(self):
         selection = self.scene().selectedItems()
         if selection:
             self.selection_changed.emit(selection[-1].item)
 
@@ -593,20 +594,20 @@
         if curSelectedItem.parentItem():
             curTrackYpos = curSelectedItem.parentItem().pos().y()
 
             newXpos = curItemXpos
             newYpos = curTrackYpos - TRACK_HEIGHT
 
             newSelectedItem = self.scene().itemAt(
-                                                  QtCore.QPointF(
-                                                                 newXpos,
-                                                                 newYpos
-                                                                 ),
-                                                  QtGui.QTransform()
-                                                  )
+                QtCore.QPointF(
+                    newXpos,
+                    newYpos
+                ),
+                QtGui.QTransform()
+            )
 
             if not newSelectedItem or isinstance(newSelectedItem, Track):
                 newYpos = newYpos - TRANSITION_HEIGHT
         else:
             newXpos = curItemXpos
             newYpos = curSelectedItem.y()
 
@@ -619,20 +620,20 @@
 
         if curSelectedItem.parentItem():
             curTrackYpos = curSelectedItem.parentItem().pos().y()
             newXpos = curItemXpos
             newYpos = curTrackYpos + TRACK_HEIGHT
 
             newSelectedItem = self.scene().itemAt(
-                                                  QtCore.QPointF(
-                                                                 newXpos,
-                                                                 newYpos
-                                                                 ),
-                                                  QtGui.QTransform()
-                                                  )
+                QtCore.QPointF(
+                    newXpos,
+                    newYpos
+                ),
+                QtGui.QTransform()
+            )
 
             if not newSelectedItem or isinstance(newSelectedItem, Track):
                 newYpos = newYpos + TRANSITION_HEIGHT
 
             if newYpos < TRACK_HEIGHT:
                 newYpos = TRACK_HEIGHT
         else:
@@ -654,32 +655,31 @@
         # maybe a bug in the population of timeline.
         if isinstance(newSelectedItem, QtWidgets.QGraphicsSimpleTextItem):
             newSelectedItem = newSelectedItem.parentItem()
 
         # Validate new item for edge cases
         # If valid, set selected
         if (
-            not isinstance(newSelectedItem, Track)
-            and newSelectedItem
+            not isinstance(newSelectedItem, Track) and newSelectedItem
         ):
             self._deselect_all_items()
             newSelectedItem.setSelected(True)
             self.centerOn(newSelectedItem)
 
     def _get_new_item(self, key_event, curSelectedItem):
         key = key_event.key()
 
         if key in (
-               QtCore.Qt.Key_Left,
-               QtCore.Qt.Key_Right,
-               QtCore.Qt.Key_Up,
-               QtCore.Qt.Key_Down,
-               QtCore.Qt.Key_Return,
-               QtCore.Qt.Key_Enter
-               ):
+                QtCore.Qt.Key_Left,
+                QtCore.Qt.Key_Right,
+                QtCore.Qt.Key_Up,
+                QtCore.Qt.Key_Down,
+                QtCore.Qt.Key_Return,
+                QtCore.Qt.Key_Enter
+        ):
             if key == QtCore.Qt.Key_Left:
                 newSelectedItem = self._get_left_item(curSelectedItem)
             elif key == QtCore.Qt.Key_Right:
                 newSelectedItem = self._get_right_item(curSelectedItem)
             elif key == QtCore.Qt.Key_Up:
                 newSelectedItem = self._get_up_item(curSelectedItem)
             elif key == QtCore.Qt.Key_Down:
```

### Comparing `OpenTimelineIO-0.8.1/setup.py` & `OpenTimelineIO-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             sys.version_info[0],
             sys.version_info[1]
         )
     )
 
 # Metadata that gets stamped into the __init__ files during the build phase.
 PROJECT_METADATA = {
-    "version": "0.8.1",
+    "version": "0.9.0",
     "author": 'Pixar Animation Studios',
     "author_email": 'opentimelineio@pixar.com',
     "license": 'Modified Apache 2.0 License',
 }
 
 METADATA_TEMPLATE = """
 __version__ = "{version}"
@@ -125,15 +125,15 @@
     description='Editorial interchange format and API',
     long_description=LONG_DESCRIPTION,
     url='http://opentimeline.io',
     project_urls={
         'Source':
             'https://github.com/PixarAnimationStudios/OpenTimelineIO',
         'Documentation':
-            'https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki',
+            'https://opentimelineio.readthedocs.io/',
         'Issues':
             'https://github.com/PixarAnimationStudios/OpenTimelineIO/issues',
     },
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Topic :: Multimedia :: Graphics',
@@ -157,14 +157,15 @@
 
     packages=[
         'opentimelineio',
         'opentimelineio.adapters',
         'opentimelineio.algorithms',
         'opentimelineio.core',
         'opentimelineio.schema',
+        'opentimelineio.schemadef',
         'opentimelineio.plugins',
         'opentimelineio.console',
         'opentimelineio_contrib',
         'opentimelineio_contrib.adapters',
         'opentimelineview',
     ],
 
@@ -188,14 +189,15 @@
             'otiostat = opentimelineio.console.otiostat:main',
         ],
     },
     extras_require={
         'dev': [
             'flake8==3.5',
             'coverage==4.5',
+            'tox==3.0',
         ],
         'view': [
             'PySide2==5.11'
         ]
     },
 
     test_suite='setup.test_otio',
```

### Comparing `OpenTimelineIO-0.8.1/PKG-INFO` & `OpenTimelineIO-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: OpenTimelineIO
-Version: 0.8.1
+Version: 0.9.0
 Summary: Editorial interchange format and API
 Home-page: http://opentimeline.io
 Author: Pixar Animation Studios
 Author-email: opentimelineio@pixar.com
 License: Modified Apache 2.0 License
 Project-URL: Source, https://github.com/PixarAnimationStudios/OpenTimelineIO
-Project-URL: Documentation, https://github.com/PixarAnimationStudios/OpenTimelineIO/wiki
+Project-URL: Documentation, https://opentimelineio.readthedocs.io/
 Project-URL: Issues, https://github.com/PixarAnimationStudios/OpenTimelineIO/issues
 Description: OpenTimelineIO is an interchange format and API for
         editorial cut information. OTIO is not a container format for media, rather it
         contains information about the order and length of cuts and references to
         external media.
         
         OTIO includes both a file format and an API for manipulating that format. It
```

