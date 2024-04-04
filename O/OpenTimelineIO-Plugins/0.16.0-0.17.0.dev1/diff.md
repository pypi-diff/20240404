# Comparing `tmp/opentimelineio_plugins-0.16.0.tar.gz` & `tmp/opentimelineio_plugins-0.17.0.dev1.tar.gz`

## Comparing `opentimelineio_plugins-0.16.0.tar` & `opentimelineio_plugins-0.17.0.dev1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/opentimelineio_plugins/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/LICENSE
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/README.md
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/pyproject.toml
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/PKG-INFO
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.16.0/setup.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/LICENSE
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/README.md
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    16313 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 opentimelineio_plugins-0.17.0.dev1/setup.py
```

### Comparing `opentimelineio_plugins-0.16.0/.gitignore` & `opentimelineio_plugins-0.17.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `opentimelineio_plugins-0.16.0/LICENSE` & `opentimelineio_plugins-0.17.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentimelineio_plugins-0.16.0/README.md` & `opentimelineio_plugins-0.17.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `opentimelineio_plugins-0.16.0/pyproject.toml` & `opentimelineio_plugins-0.17.0.dev1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 # Copyright Contributors to the OpenTimelineIO project
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "OpenTimelineIO-Plugins"
-version = "0.16.0"
+version = "0.17.0.dev1"
 description = "OpenTimelineIO with batteries included plug-ins."
 authors = [
   { name="Contributors to the OpenTimelineIO project", email="otio-discussion@lists.aswf.io" },
 ]
 license = { file="LICENSE" }
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "opentimelineio==0.16.0",
+    "opentimelineio==0.17.0.dev1",
+    "otio-aaf-adapter",
+    "otio-burnins-adapter",
+    "otio-xges-adapter",
+    "otio-ale-adapter",
+    "otio-hls-playlist-adapter",
+    "otio-fcpx-xml-adapter",
+    "otio-maya-sequencer-adapter",
+    "otio-cmx3600-adapter",
+    "otio-svg-adapter",
+    "otio-fcp-adapter",
 ]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Multimedia :: Graphics",
     "Topic :: Multimedia :: Video",
     "Topic :: Multimedia :: Video :: Display",
```

### Comparing `opentimelineio_plugins-0.16.0/PKG-INFO` & `opentimelineio_plugins-0.17.0.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: OpenTimelineIO-Plugins
-Version: 0.16.0
+Version: 0.17.0.dev1
 Summary: OpenTimelineIO with batteries included plug-ins.
 Project-URL: Homepage, https://opentimeline.io
 Project-URL: Tracker, https://github.com/OpenTimelineIO/OpenTimelineIO-Plugins/issues
 Author-email: Contributors to the OpenTimelineIO project <otio-discussion@lists.aswf.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
@@ -221,15 +221,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Display
 Classifier: Topic :: Multimedia :: Video :: Non-Linear Editor
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: opentimelineio==0.16.0
+Requires-Dist: opentimelineio==0.17.0.dev1
+Requires-Dist: otio-aaf-adapter
+Requires-Dist: otio-ale-adapter
+Requires-Dist: otio-burnins-adapter
+Requires-Dist: otio-cmx3600-adapter
+Requires-Dist: otio-fcp-adapter
+Requires-Dist: otio-fcpx-xml-adapter
+Requires-Dist: otio-hls-playlist-adapter
+Requires-Dist: otio-maya-sequencer-adapter
+Requires-Dist: otio-svg-adapter
+Requires-Dist: otio-xges-adapter
 Description-Content-Type: text/markdown
 
 # OpenTimelineIO
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenTimelineIO/main/docs/_static/OpenTimelineIO@3xLight.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenTimelineIO/main/docs/_static/OpenTimelineIO@3xDark.png">
```

### Comparing `opentimelineio_plugins-0.16.0/setup.py` & `opentimelineio_plugins-0.17.0.dev1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='opentimelineio-plugins',
-    version='0.16.0',
+    version='0.17.0.dev1',
     description='OpenTimelineIO with batteries included plug-ins.',
     long_description='# OpenTimelineIO\n\n<picture>\n  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenTimelineIO/main/docs/_static/OpenTimelineIO@3xLight.png">\n  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AcademySoftwareFoundation/OpenTimelineIO/main/docs/_static/OpenTimelineIO@3xDark.png">\n  <img alt="OpenTimelineIO Logo" src="./images/OpenTimelineIO@3xDark.png">\n</picture>\n\n[OpenTimelineIO](https://opentimeline.io) is an interchange format and API for\neditorial cut information.\n\nThis package is a convenience includes both OpenTimelineIO and a set of plugins\nmaintained by the OpenTimelineIO community that are commonly used with the\nlibrary.\n\n## Support\n\nThe included plugins are part of the OpenTimelineIO project but may be supported\ndifferently than the OpenTimelineIO core.\n\nThis may include:\n\n- Repos primarily maintained by community members with OpenTimelineIO core team members only providing guidance\n- Repos that aren\'t actively maintained\n\nPlease consult READMEs in individual subproject repos to learn more about their\nmaintainance and support.\n\nLinks\n-----\n\n* Main web site: http://opentimeline.io/\n* Documentation: https://opentimelineio.readthedocs.io/\n* Main Project GitHub: https://github.com/AcademySoftwareFoundation/OpenTimelineIO\n* [Discussion group](https://lists.aswf.io/g/otio-discussion)\n* [Slack channel](https://academysoftwarefdn.slack.com/messages/CMQ9J4BQC)\n  * To join, create an account here first: https://slack.aswf.io/\n* [Presentations](https://github.com/AcademySoftwareFoundation/OpenTimelineIO/wiki/Presentations)\n',
     author_email='Contributors to the OpenTimelineIO project <otio-discussion@lists.aswf.io>',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
@@ -21,13 +21,20 @@
         'Topic :: Multimedia :: Graphics',
         'Topic :: Multimedia :: Video',
         'Topic :: Multimedia :: Video :: Display',
         'Topic :: Multimedia :: Video :: Non-Linear Editor',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     install_requires=[
-        'opentimelineio==0.16.0',
-    ],
-    packages=[
-        'opentimelineio_plugins',
+        'opentimelineio==0.17.0.dev1',
+        'otio-aaf-adapter',
+        'otio-ale-adapter',
+        'otio-burnins-adapter',
+        'otio-cmx3600-adapter',
+        'otio-fcp-adapter',
+        'otio-fcpx-xml-adapter',
+        'otio-hls-playlist-adapter',
+        'otio-maya-sequencer-adapter',
+        'otio-svg-adapter',
+        'otio-xges-adapter',
     ],
 )
```

