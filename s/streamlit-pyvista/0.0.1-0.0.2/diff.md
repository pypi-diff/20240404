# Comparing `tmp/streamlit_pyvista-0.0.1.tar.gz` & `tmp/streamlit_pyvista-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pyvista-0.0.1.tar", max compression
+gzip compressed data, was "streamlit_pyvista-0.0.2.tar", max compression
```

## Comparing `streamlit_pyvista-0.0.1.tar` & `streamlit_pyvista-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      104 2024-03-28 14:44:29.645269 streamlit_pyvista-0.0.1/README.md
--rw-r--r--   0        0        0     1806 2024-03-28 14:44:35.222312 streamlit_pyvista-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2765 2024-03-28 14:44:29.646270 streamlit_pyvista-0.0.1/streamlit_pyvista/MeshViewerComponent.py
--rw-r--r--   0        0        0       89 2024-03-28 14:44:29.646270 streamlit_pyvista-0.0.1/streamlit_pyvista/__init__.py
--rw-r--r--   0        0        0    16608 2024-03-28 14:44:29.646270 streamlit_pyvista-0.0.1/streamlit_pyvista/trame_viewer.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2024-04-04 10:31:45.971112 streamlit_pyvista-0.0.2/README.md
+-rw-r--r--   0        0        0     1806 2024-04-04 10:31:51.643100 streamlit_pyvista-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3671 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/MeshViewerComponent.py
+-rw-r--r--   0        0        0       89 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/__init__.py
+-rw-r--r--   0        0        0    17116 2024-04-04 10:31:45.972112 streamlit_pyvista-0.0.2/streamlit_pyvista/trame_viewer.py
+-rw-r--r--   0        0        0      208 2024-04-04 10:31:45.973112 streamlit_pyvista-0.0.2/streamlit_pyvista/utils.py
+-rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 streamlit_pyvista-0.0.2/PKG-INFO
```

### Comparing `streamlit_pyvista-0.0.1/pyproject.toml` & `streamlit_pyvista-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-pyvista"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Maxime Rochat <rochat.max@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "3.9.3"
```

### Comparing `streamlit_pyvista-0.0.1/streamlit_pyvista/trame_viewer.py` & `streamlit_pyvista-0.0.2/streamlit_pyvista/trame_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import pyvista as pv
-from pyvista import examples
+import argparse
 from pyvista.trame.ui import plotter_ui
 from trame.app import get_server
 from trame.ui.vuetify3 import VAppLayout
 from trame.widgets import vuetify3 as vuetify
 from trame.widgets import html
 from aiohttp import web
 from trame.decorators import TrameApp, change, controller
 
-
 import os
 import numpy as np
 import time, threading
 import asyncio
 from abc import ABC, abstractmethod
 
 from typing import Dict
 
 
-
 @TrameApp()
 class MeshViewer:
 
-    def __init__(self, mesh=None, plotter=None, server=None):
+    def __init__(self, mesh=None, plotter=None, server=None, port=8080):
 
         pv.OFF_SCREEN = True
         self.scalar_bar_exist = None
         if server is None:
-            self.server = get_server()
+            self.server = get_server(port=port)
         else:
             self.server = server
         self.slider_playing = False
         self.path = None
 
         self.mesh = None
         self.clean_mesh = None
@@ -44,14 +42,15 @@
         self.pl = self.setup_pl()
 
         setattr(self, "on_server_bind", self.server.controller.add("on_server_bind")(self.on_server_bind))
 
         # self.replace_mesh(mesh)
         self.my_routes = [
             web.get("/select_mesh", self.change_mesh),
+            web.get("/init_connection", self.init_connection),
         ]
 
         self.setup_state()
 
         self.setup_timer()
 
         self.loop = asyncio.get_event_loop()
@@ -62,16 +61,14 @@
         self.state.options_warp = ["None", "A", "B"]
 
         self.actor = None
         self.width = 800
         self.height = 900
         self.ui = self.build_ui()
 
-
-
     def setup_pl(self) -> pv.Plotter:
         pl = pv.Plotter()
         pl.background_color = self.style["background-color"]
         pl.theme.font.color = self.style["font-color"]
         self.bounds_scalar = None
         self.scalar_bar_exist = False
         self.scalar_bar_mapper = None
@@ -140,15 +137,15 @@
         finally:
             return
 
     @change("warped_field")
     def update_warped_field(self, warped_field, **kwargs):
         if warped_field is None or warped_field == "None":
             return
-        self.update_warp_input(warped_field= warped_field)
+        self.update_warp_input(warped_field=warped_field)
 
     @change("wireframe_on")
     def update_wireframe_on(self, **kwargs):
         self.replace_mesh(self.mesh)
 
     @change("slider_value")
     def slider_value_change(self, slider_value, **kwargs):
@@ -196,44 +193,53 @@
             path = self.path % i
             if not os.path.exists(path):
                 print(f"Error, the file {path} does not exist")
                 return
             self.mesh_array.append(pv.read(path))
 
     async def change_mesh(self, request):
-
         request_body: Dict[str, str] = await request.json()
         self.path = request_body.get("mesh_path", None)
         self.width = request_body.get("width", self.width)
         self.height = request_body.get("height", self.height)
         self.sequence_bounds[1] = request_body.get("nbr_frames", self.sequence_bounds[1])
         print(f"PATH RECEIVED IS {self.path}")
         if self.path is None:
             print("Error : No filepath found in the change mesh request")
             return
 
-        self.handle_new_mesh(self.path, self.sequence_bounds[1])
+        self.clear_viewer()
 
-        self.state.mesh_representation = None
+        self.handle_new_mesh(self.path, self.sequence_bounds[1])
         self.replace_mesh(self.mesh_array[0])
 
         self.state.options = self.mesh_array[0].array_names.copy()
         self.state.options.insert(0, "None")
-        self.state.options_warp = self.mesh_array[0].array_names.copy()
-        self.state.options_warp.insert(0, "None")
+        self.state.options_warp = self.state.options.copy()
 
         self.computes_bounds_scalar()
         self.update_ui()
+        self.pl.reset_camera()
         response_body = {}
         if self.height - self.estimate_controller_height()[1] < 700:
             response_body["request_space"] = 1.65 * self.height
 
-        self.pl.reset_camera()
         return web.json_response(response_body, status=200)
 
+    def clear_scalar_bars(self):
+        if self.pl is None:
+            return
+        bar_to_remove = [key for key in self.pl.scalar_bars.keys()]
+        [self.pl.remove_scalar_bar(title=key) for key in bar_to_remove]
+
+    def clear_viewer(self):
+        self.clear_scalar_bars()
+        self.state.slider_value = 0
+        self.state.mesh_representation = None
+
     def compute_field_interval(self, field=None):
         if field is None:
             field = self.state.mesh_representation
         if field is None or field == "None":
             field = self.state.options[1]
         max_bound = -np.inf
         min_bound = np.inf
@@ -351,39 +357,32 @@
             self.state.play_pause_icon = "mdi-pause"
 
             self.timer.start()
         else:
             self.state.play_pause_icon = "mdi-play"
         self.update_ui()
 
-
     def build_warp_option(self):
         return vuetify.VSelect(
-                v_model=("warped_field"),
-                items=("options_warp", self.state.options_warp),
-                label="Warped Field",
-                hide_details=True,
-                dense=True,
-                outlined=True,
-                classes="pt-1",
-            )
+            v_model=("warped_field"),
+            items=("options_warp", self.state.options_warp),
+            label="Warped Field",
+            hide_details=True,
+            dense=True,
+            outlined=True,
+            classes="pt-1",
+        )
 
     def build_warper(self):
         warper = vuetify.VCol(cols="6")
         with warper:
-            print("array of options ------------------")
-            print(self.state.options_warp)
-            options = ['None', 'U', 'V', 'A', 'E', 'dE']
-            options = self.state.options_warp
-            print(options)
             self.build_warp_option()
 
             # self.option_dropdown(field_linked="warped_field", options=self.state.options)
             if self.state.mesh_representation != "None" and self.state.mesh_representation is not None:
-
                 html.Input(type="number", label="warp",
                            v_model=("warp_input", 0.0),
                            ref=f"warp-input",
                            step="1"
                            )
 
         return warper
@@ -411,22 +410,23 @@
         return 0.2 * self.height, 9 * 30
 
     def build_ui(self):
         control_height = self.estimate_controller_height()[0]
         if not self.state.is_full_screen:
             plotter_height = self.height - control_height
             plotter_height = f"{plotter_height}px"
-            width = f"{self.width}px"
+            width = "100%"
 
 
         else:
             plotter_height = "100%"
             width = "100%"
 
         print(self.height)
+        print("width", width)
 
         with VAppLayout(self.server) as layout:
             with layout.root:
                 with html.Div(
                         style=f"height: {self.height}px ;width:{width}"):  # add the following arg: style="height: 100vh; width:100vw" to have the plotter taking all screen
                     with html.Div(ref="container", style=f"height:{plotter_height};padding: 0;"):
                         with vuetify.VCol(style=f"height:{plotter_height};padding: 0;"):
@@ -440,14 +440,21 @@
                     with vuetify.VCol(style=f"height:{control_height}px;padding: 0;width:100%;"):
                         self.build_mesh_control_layout()
             return layout
 
     def on_server_bind(self, wslink_server):
         wslink_server.app.add_routes(self.my_routes)
 
+    async def init_connection(self, request):
+        response_body = {
+            "select_mesh": "/select_mesh",
+            "host": f"http://127.0.0.1:{self.server.port}"
+        }
+        return web.json_response(response_body, status=200)
+
     def request_full(self):
         self.server.js_call("container", "requestFullscreen")
         # if not self.state.is_full_screen:
         #     self.server.js_call("container", "requestFullscreen")
         # else:
         #     self.server.js_call("", "exitFullscreen()")
         self.state.is_full_screen = not self.state.is_full_screen
@@ -456,24 +463,24 @@
 
 class Component(ABC):
     def __init__(self, state, ctrl):
         self.supported_handler = ["change"]
         self.state = state
         self.ctrl = ctrl
 
-
     # add corresponding decorator to fucntion (change or set)
     @abstractmethod
     def handler(self, new_value, **kwargs):
         pass
 
     @abstractmethod
     def render(self):
         pass
 
 
-
 if __name__ == "__main__":
-    mv = MeshViewer()
+    parser = argparse.ArgumentParser(description='Launch a trame server instance')
+    parser.add_argument('--port', type=int, help='Specify the port of the server')
+    args = parser.parse_args()
+    mv = MeshViewer(port=args.port)
     mv.start_server()
-    # sm = ServerManager()
-    # sm.start_server()
+
```

### Comparing `streamlit_pyvista-0.0.1/PKG-INFO` & `streamlit_pyvista-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-pyvista
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Maxime Rochat
 Author-email: rochat.max@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

