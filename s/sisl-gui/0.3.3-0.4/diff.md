# Comparing `tmp/sisl-gui-0.3.3.tar.gz` & `tmp/sisl-gui-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sisl-gui-0.3.3.tar", last modified: Fri Oct 27 21:44:33 2023, max compression
+gzip compressed data, was "sisl-gui-0.4.tar", last modified: Thu Apr  4 09:27:58 2024, max compression
```

## Comparing `sisl-gui-0.3.3.tar` & `sisl-gui-0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.887866 sisl-gui-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-10-27 21:44:33.887866 sisl-gui-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-27 21:44:33.887866 sisl-gui-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.867865 sisl-gui-0.3.3/sisl_gui/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.871865 sisl-gui-0.3.3/sisl_gui/build/
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/SIESTAlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/electron.js
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   545651 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/icon.icns
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/pyodide-webworker.js
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)  2059564 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/sisl-0.14.2-cp311-cp311-emscripten_3_1_45_wasm32.whl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.867865 sisl-gui-0.3.3/sisl_gui/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.875866 sisl-gui-0.3.3/sisl_gui/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    26766 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/static/css/main.dee163b6.css
--rw-r--r--   0 runner    (1001) docker     (127)    28543 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/static/css/main.dee163b6.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.879866 sisl-gui-0.3.3/sisl_gui/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)  5100141 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  5960530 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.887866 sisl-gui-0.3.3/sisl_gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.887866 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/emiters.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/flask_socketio/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/server/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-10-27 21:44:18.000000 sisl-gui-0.3.3/sisl_gui/sgui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:44:33.867865 sisl-gui-0.3.3/sisl_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-27 21:44:33.000000 sisl-gui-0.3.3/sisl_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.674256 sisl-gui-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-04 09:27:58.674256 sisl-gui-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-04 09:27:49.000000 sisl-gui-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 09:27:49.000000 sisl-gui-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-04 09:27:58.674256 sisl-gui-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-04 09:27:49.000000 sisl-gui-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.654256 sisl-gui-0.4/sisl_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.658256 sisl-gui-0.4/sisl_gui/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/SIESTAlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/electron.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   545651 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/pyodide-webworker.js
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  2059564 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/sisl-0.14.2-cp311-cp311-emscripten_3_1_45_wasm32.whl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.650256 sisl-gui-0.4/sisl_gui/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.658256 sisl-gui-0.4/sisl_gui/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    26766 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/static/css/main.dee163b6.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28543 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/static/css/main.dee163b6.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.666256 sisl-gui-0.4/sisl_gui/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  5100141 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  5960530 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.674256 sisl-gui-0.4/sisl_gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.674256 sisl-gui-0.4/sisl_gui/server/flask_socketio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/flask_socketio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/flask_socketio/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/flask_socketio/emiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/flask_socketio/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/flask_socketio/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29916 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/server/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-04 09:27:49.000000 sisl-gui-0.4/sisl_gui/sgui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:27:58.654256 sisl-gui-0.4/sisl_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 09:27:58.000000 sisl-gui-0.4/sisl_gui.egg-info/top_level.txt
```

### Comparing `sisl-gui-0.3.3/PKG-INFO` & `sisl-gui-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sisl-gui
-Version: 0.3.3
+Version: 0.4
 Summary: Graphical interface for the sisl visualization module
 Home-page: http://github.com/pfebrer/sisl-gui
 Author: Pol Febrer
 Author-email: pfebrer96@gmail.com
 License: MIT
 Description: This is the graphical interface that you can use to interact with [sisl's](https://github.com/zerothi/sisl) visualization module.
```

### Comparing `sisl-gui-0.3.3/README.md` & `sisl-gui-0.4/README.md`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/setup.cfg` & `sisl-gui-0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sisl-gui
-version = 0.3.3
+version = 0.4
 description = Graphical interface for the sisl visualization module
 url = http://github.com/pfebrer/sisl-gui
 author = Pol Febrer
 author_email = pfebrer96@gmail.com
 license = MIT
 
 [options]
```

### Comparing `sisl-gui-0.3.3/setup.py` & `sisl-gui-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/SIESTAlogo.png` & `sisl-gui-0.4/sisl_gui/build/SIESTAlogo.png`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/apple-touch-icon.png` & `sisl-gui-0.4/sisl_gui/build/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/electron.js` & `sisl-gui-0.4/sisl_gui/build/electron.js`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/favicon-32x32.png` & `sisl-gui-0.4/sisl_gui/build/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/favicon.ico` & `sisl-gui-0.4/sisl_gui/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/icon.icns` & `sisl-gui-0.4/sisl_gui/build/icon.icns`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/index.html` & `sisl-gui-0.4/sisl_gui/build/index.html`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/mstile-150x150.png` & `sisl-gui-0.4/sisl_gui/build/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/pyodide-webworker.js` & `sisl-gui-0.4/sisl_gui/build/pyodide-webworker.js`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/safari-pinned-tab.svg` & `sisl-gui-0.4/sisl_gui/build/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/sisl-0.14.2-cp311-cp311-emscripten_3_1_45_wasm32.whl` & `sisl-gui-0.4/sisl_gui/build/sisl-0.14.2-cp311-cp311-emscripten_3_1_45_wasm32.whl`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/static/css/main.dee163b6.css` & `sisl-gui-0.4/sisl_gui/build/static/css/main.dee163b6.css`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/static/css/main.dee163b6.css.map` & `sisl-gui-0.4/sisl_gui/build/static/css/main.dee163b6.css.map`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js` & `sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js.LICENSE.txt` & `sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/build/static/js/main.32133d32.js.map` & `sisl-gui-0.4/sisl_gui/build/static/js/main.32133d32.js.map`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/launch.py` & `sisl-gui-0.4/sisl_gui/launch.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/server/app.py` & `sisl-gui-0.4/sisl_gui/server/app.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/server/flask_socketio/app.py` & `sisl-gui-0.4/sisl_gui/server/flask_socketio/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,21 @@
 register_environ_variable("SISL_GUI_SERVER_HOST", "localhost",
                           "The host where the GUI will run when self-hosted by the user.",
                           process=str)
 register_environ_variable("SISL_GUI_SERVER_PORT", 4000,
                           "The port where the GUI will run when self-hosted by the user.",
                           process=int)
 
-
 __all__ = ["SocketioApp"]
 
+class SocketioLastUpdateEmiter(SocketioConnection):
+
+    def after_modification(self, obj):
+        return emit("session_last_update", obj.last_update, broadcast=True)
+
 class SocketioApp(App):
 
     connection: SocketioConnection
 
     host: Union[str, None]
     port: Union[int, None]
 
@@ -61,15 +65,15 @@
                             # Maybe instead of threading we can use socketio.start_background_task (see https://github.com/miguelgrinberg/Flask-SocketIO/issues/876)
                             # You can set this to any other async_mode if you don't plan to interact from python (i.e. only through the GUI)
         on = socketio.on
 
         if False:
             listen_to_users(on, emit_session)
 
-        connection = SocketioConnection(socketio)
+        connection = SocketioLastUpdateEmiter(socketio)
 
         self.socketio = socketio
 
         if session is None:
             session = Session()
 
         super().__init__(session=session, connection=connection)
@@ -83,30 +87,29 @@
             if self.session is not None:
                 self.session.logger.exception(err)
 
             emit_error(err)
             emit_session(self.session, broadcast=True)
             raise err
 
-        @on("request_session")
+        @on("request_last_updates")
         @if_user_can("see")
         def send_session(path=None):
-            print("SEND SESSION", self.session)
-            return self.session
+            return self.session.last_update if self.session else {}
 
         @on("apply_method_on_session")
         @if_user_can("edit")
         def apply_method(method_name, kwargs={}, *args):
-            print("APPLYING METHOD ON SESSION", self.session)
 
             session = self.session
 
             if session is None:
                 raise Exception("The app is not associated with any session.")
             
+            session.logger.info(f"Applying method {method_name}")
             session.logger.debug(f"Applying method {method_name} with args {args} and kwargs {kwargs}")
 
             if kwargs is None:
                 # This is because the GUI might send None
                 kwargs = {}
 
             # Remember that if the method is not found an error will be raised
```

### Comparing `sisl-gui-0.3.3/sisl_gui/server/flask_socketio/emiters.py` & `sisl-gui-0.4/sisl_gui/server/flask_socketio/emiters.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/server/flask_socketio/sync.py` & `sisl-gui-0.4/sisl_gui/server/flask_socketio/sync.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/server/flask_socketio/user_management.py` & `sisl-gui-0.4/sisl_gui/server/flask_socketio/user_management.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/server/json.py` & `sisl-gui-0.4/sisl_gui/server/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Implements conversion from python elements to JSON to send the messages."""
 
-from typing import get_type_hints, Type, Dict, Callable
+import typing
+from typing import Type, Dict, Callable, Tuple, Any, Literal, Optional
 
 import pathlib
 
 import simplejson
 from simplejson.encoder import JSONEncoder
 
 from plotly.graph_objects import Figure
@@ -87,27 +88,37 @@
     
     Parameters
     ----------
     annotation : Any
         The annotation of the function argument.
     """
 
+    try:
+        orig = typing.get_origin(annotation)
+        if orig is typing.Literal:
+            input_type = 'select'
+            options = typing.get_args(annotation)
+            return input_type, {"options": options}
+    except:
+        pass
+
+
     if isinstance(annotation, type):
         annotation = annotation.__name__
         
     annotation = str(annotation)
 
     input_type = {
         'str': 'text',
         'int': 'number',
         'float': 'number',
         'bool': 'bool',
     }.get(annotation)
 
-    return input_type
+    return input_type, {}
 
 def as_jsonable(encoder, obj):
     if isinstance(obj, np.ndarray) and not np.issubdtype(obj.dtype, np.number):
         return as_jsonable(encoder, obj.tolist())
     elif isinstance(obj, (list, tuple)):
         return type(obj)([as_jsonable(encoder, v) for v in obj])
     elif isinstance(obj, dict):
@@ -131,77 +142,104 @@
     json_node_cls['id'] = id(node_class)
     json_node_cls['name'] = node_class.__name__
     json_node_cls['doc'] = node_class.__doc__
 
     parameters_help = get_fields_help_from_function(node_class.function)
 
     if hasattr(node_class, "function"):
-        try:
-            type_hints = get_type_hints(node_class.function)
-        except:
-            type_hints = {}
+
+        type_hints = node_class.typehints.copy()
 
         json_node_cls['output_type'] = str(type_hints.pop('return', None))
 
         parameters = inspect.signature(node_class.function).parameters
 
         json_node_cls['parameters'] = {}
         for k, param in parameters.items():
             parameter = {
                 "name": param.name,
                 "kind": param.kind.name,
             }
 
             if k in type_hints:
-                input_type = annotation_to_input_type(type_hints[k])
+                input_type, field_params = annotation_to_input_type(type_hints[k])
                 if input_type is not None:
                     parameter['type'] = input_type
+                    parameter['field_params'] = field_params
             if param.default is not inspect.Parameter.empty and param.default is not Node._blank:
                 parameter['default'] = as_jsonable(encoder, param.default)
 
             json_node_cls['parameters'][k] = parameter
 
+    if hasattr(node_class, "registry"):
+        json_node_cls['registry'] = {
+            str(k): id(node) for k, node in node_class.registry.items()
+        }
+
     return json_node_cls
 
+def get_inputs_mode(node: Node, encoder: Optional[JSONEncoder] = None) -> Tuple[Dict[str, Any], Dict[str, Literal["NODE"]]]:
+    """Given some inputs, finds out which of them are nodes and which are not.
+
+    Parameters
+    ----------
+    node : Node
+        The node for which to get the inputs mode.
+
+    Returns
+    -------
+    inputs
+        The inputs dictionary with the nodes replaced by their IDs.
+    inputs_mode
+        The dictionary indicating which inputs are nodes.
+    """
+    # Go over the inputs and find out which of them contain nodes
+    # We need to mark them so that the GUI knows it. Then, we replace
+    # the nodes by their ID.
+    inputs = {**node.inputs}
+    inputs_mode = {}
+    for k, v in inputs.items():
+        if k  == node._args_inputs_key and len(v) > 0 and isinstance(v[0], Node):
+            # This is the *args input, and it contains nodes
+            inputs_mode[k] = "NODE"
+            inputs[k] = [id(node) for node in v]
+        elif k == node._kwargs_inputs_key and len(v) > 0 and isinstance(list(v.values())[0], Node):
+            # This is the **kwargs input, and it contains nodes
+            inputs_mode[k] = "NODE"
+            inputs[k] = {k: id(node) for k, node in v.items()}
+        elif isinstance(v, Node):
+            # This is a simple input, and it contains a node
+            inputs_mode[k] = "NODE"
+            inputs[k] = id(v)
+        else:
+            inputs[k] = as_jsonable(encoder, v) if encoder is not None else v
+
+    return inputs, inputs_mode
+
 def node_to_json(encoder: JSONEncoder, node: Node):
     """Parses a node into a JSON object that can be sent to the client.
     
     Parameters
     ----------
     node : Node
         The node object to parse.
     """
     json_node = {}
 
     json_node['id'] = id(node)
     json_node['class'] = id(node.__class__)
-    json_node['inputs'] = dict(node.inputs)
-    json_node['logs'] = node.logs
+    
+    json_node["last_log"] = node.last_log
+    if getattr(encoder, "encode_node_logs", True):
+        json_node['logs'] = node.logs
+
     json_node['outdated'] = node._outdated
     json_node['errored'] = node._errored
 
-    # Go over the inputs and find out which of them contain nodes
-    # We need to mark them so that the GUI knows it. Then, we replace
-    # the nodes by their ID.
-    json_node['inputs_mode'] = {}
-    for k, v in json_node['inputs'].items():
-        if k  == node._args_inputs_key and len(v) > 0 and isinstance(v[0], Node):
-            # This is the *args input, and it contains nodes
-            json_node['inputs_mode'][k] = "NODE"
-            json_node['inputs'][k] = [id(node) for node in v]
-        elif k == node._kwargs_inputs_key and len(v) > 0 and isinstance(list(v.values())[0], Node):
-            # This is the **kwargs input, and it contains nodes
-            json_node['inputs_mode'][k] = "NODE"
-            json_node['inputs'][k] = {k: id(node) for k, node in v.items()}
-        elif isinstance(v, Node):
-            # This is a simple input, and it contains a node
-            json_node['inputs_mode'][k] = "NODE"
-            json_node['inputs'][k] = id(v)
-        else:
-            json_node['inputs'][k] = as_jsonable(encoder, v)
+    json_node['inputs'], json_node['inputs_mode'] = get_inputs_mode(node, encoder)
     
     output = node._output
 
     if output is not Node._blank:
         json_node['output_class'] = output.__class__.__name__
 
         json_node['output'] = as_jsonable(encoder, output)
@@ -229,14 +267,18 @@
 class CustomJSONEncoder(JSONEncoder):
     """Custom JSON encoder that can handle more types than the default one.
     
     Specifically, it can handle: node objects, session objects, node classes
     and plotly figures.
     """
 
+    def __init__(self, *args, node_logs: bool = False, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.encode_node_logs = node_logs
+
     def default(self, obj):
 
         if isinstance(obj, Node):
             return node_to_json(self, obj)
         elif isinstance(obj, Figure):
             return obj.to_plotly_json()
         elif hasattr(obj, "to_json"):
```

### Comparing `sisl-gui-0.3.3/sisl_gui/server/sync.py` & `sisl-gui-0.4/sisl_gui/server/sync.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui/sgui.py` & `sisl-gui-0.4/sisl_gui/sgui.py`

 * *Files identical despite different names*

### Comparing `sisl-gui-0.3.3/sisl_gui.egg-info/PKG-INFO` & `sisl-gui-0.4/sisl_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sisl-gui
-Version: 0.3.3
+Version: 0.4
 Summary: Graphical interface for the sisl visualization module
 Home-page: http://github.com/pfebrer/sisl-gui
 Author: Pol Febrer
 Author-email: pfebrer96@gmail.com
 License: MIT
 Description: This is the graphical interface that you can use to interact with [sisl's](https://github.com/zerothi/sisl) visualization module.
```

### Comparing `sisl-gui-0.3.3/sisl_gui.egg-info/SOURCES.txt` & `sisl-gui-0.4/sisl_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

