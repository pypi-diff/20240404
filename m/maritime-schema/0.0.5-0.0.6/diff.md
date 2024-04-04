# Comparing `tmp/maritime-schema-0.0.5.tar.gz` & `tmp/maritime-schema-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maritime-schema-0.0.5.tar", last modified: Fri Mar 22 13:16:42 2024, max compression
+gzip compressed data, was "maritime-schema-0.0.6.tar", last modified: Thu Apr  4 13:40:39 2024, max compression
```

## Comparing `maritime-schema-0.0.5.tar` & `maritime-schema-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.829392 maritime-schema-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-22 13:16:42.829392 maritime-schema-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 13:16:42.829392 maritime-schema-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.821392 maritime-schema-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.825392 maritime-schema-0.0.5/src/maritime_schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.825392 maritime-schema-0.0.5/src/maritime_schema/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/cli/publish_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.825392 maritime-schema-0.0.5/src/maritime_schema/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25365 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/types/caga.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/types/caga_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.825392 maritime-schema-0.0.5/src/maritime_schema/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/utils/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/src/maritime_schema/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.829392 maritime-schema-0.0.5/src/maritime_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-22 13:16:42.000000 maritime-schema-0.0.5/src/maritime_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:42.825392 maritime-schema-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-22 13:16:34.000000 maritime-schema-0.0.5/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15960 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.367265 maritime-schema-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.367265 maritime-schema-0.0.6/src/maritime_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/src/maritime_schema/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/cli/publish_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/src/maritime_schema/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26460 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/types/caga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/types/caga_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/src/maritime_schema/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/utils/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/src/maritime_schema/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/src/maritime_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15960 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 13:40:39.000000 maritime-schema-0.0.6/src/maritime_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:40:39.371265 maritime-schema-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 13:40:23.000000 maritime-schema-0.0.6/tests/test_api.py
```

### Comparing `maritime-schema-0.0.5/LICENSE` & `maritime-schema-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maritime-schema-0.0.5/pyproject.toml` & `maritime-schema-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6d61 7269 7469 6d65 2d73 6368 656d   "maritime-schem
 00000080: 6122 0d0a 7665 7273 696f 6e20 3d20 2230  a"..version = "0
-00000090: 2e30 2e35 220d 0a64 6573 6372 6970 7469  .0.5"..descripti
+00000090: 2e30 2e36 220d 0a64 6573 6372 6970 7469  .0.6"..descripti
 000000a0: 6f6e 203d 2022 5079 7468 6f6e 2064 6174  on = "Python dat
 000000b0: 6120 636c 6173 7365 7320 616e 6420 4a53  a classes and JS
 000000c0: 4f4e 2073 6368 656d 6174 6120 666f 7220  ON schemata for 
 000000d0: 6d61 7269 7469 6d65 2074 7261 6666 6963  maritime traffic
 000000e0: 2073 6365 6e61 7269 6f73 2e22 0d0a 7265   scenarios."..re
 000000f0: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
 00000100: 6422 0d0a 7265 7175 6972 6573 2d70 7974  d"..requires-pyt
```

### Comparing `maritime-schema-0.0.5/src/maritime_schema/cli/publish_schema.py` & `maritime-schema-0.0.6/src/maritime_schema/cli/publish_schema.py`

 * *Files identical despite different names*

### Comparing `maritime-schema-0.0.5/src/maritime_schema/types/caga.py` & `maritime-schema-0.0.6/src/maritime_schema/types/caga.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,249 +133,304 @@
     current_direction: float = Field(None, description="The current direction in degrees", examples=[90.0])
     wave_spectrum: WaveSpectra = Field(None, description="The wave spectrum", examples=[WaveSpectra.JONSWAP])
     significant_wave_height: float = Field(None, description="The significant wave height in meters", examples=[3.0])
     wave_period: float = Field(None, description="The wave period in seconds", examples=[12.0])
     wave_direction: float = Field(None, description="The wave direction in degrees", examples=[270.0])
     visibility: float = Field(None, description="The visibility in nautical miles", examples=[5.0])
     conditions: WeatherCondition = Field(
-        None, description="The overall weather conditions", examples=[WeatherCondition.Clear]
+        None,
+        description="The overall weather conditions",
+        examples=[WeatherCondition.Clear],
     )
 
 
 class Position(BaseModelConfig):
-    latitude: Optional[float] = Field(None, ge=-90, le=90, description="WGS-84 latitude", examples=[51.2131])
-    longitude: Optional[float] = Field(None, ge=-180, le=180, description="WGS-84 longitude", examples=[11.2131])
+    latitude: float = Field(None, ge=-90, le=90, description="WGS-84 latitude", examples=[51.2131])
+    longitude: float = Field(None, ge=-180, le=180, description="WGS-84 longitude", examples=[11.2131])
     model_config = ConfigDict(extra="allow")
 
 
 class ShipStatic(BaseModelConfig):
     """Static ship data that will not change during the scenario."""
 
     id: UUID = Field(..., description="Unique Identifier", examples=[uuid4()])
-    length: Optional[float] = Field(None, gt=0, description="Length of the ship in meters", examples=[230.0])
-    width: Optional[float] = Field(None, gt=0, description="Width of the ship in meters", examples=[30.0])
+    length: float = Field(None, gt=0, description="Length of the ship in meters", examples=[230.0])
+    width: float = Field(None, gt=0, description="Width of the ship in meters", examples=[30.0])
     height: Optional[float] = Field(None, gt=0, description="Height of the ship in meters", examples=[15.0])
+    speed_max: Optional[float] = Field(None, gt=0, description="Maximum speed of the ship in knots", examples=[15.0])
     mmsi: Optional[int] = Field(
-        None, ge=100000000, le=999999999, description="Maritime Mobile Service Identity (MMSI)", examples=[123456789]
+        None,
+        ge=100000000,
+        le=999999999,
+        description="Maritime Mobile Service Identity (MMSI)",
+        examples=[123456789],
     )
     imo: Optional[int] = Field(None, ge=1000000, le=9999999, description="IMO Number", examples=[1234567])
-    name: Optional[str] = Field(None, description="Ship title", examples=["RMS Titanic"])
+    name: Optional[str] = Field(None, description="Ship name", examples=["RMS Titanic"])
     ship_type: Optional[GeneralShipType] = Field(None, description="General ship type, based on AIS")
     model_config = ConfigDict(extra="allow")
 
 
 class Initial(BaseModelConfig):
-    position: Optional[Position] = Field(
+    position: Position = Field(
         None,
-        title="Longitude and Latitude Values",
-        description="A geographical coordinate",
+        description="Initial longitude and latitude of the ship.",
         examples=[create_position_example()],
     )
-    sog: Optional[float] = Field(
+    sog: float = Field(
         None,
         ge=0,
-        title="Initial ship speed over ground",
         description="Initial ship speed over ground in knots",
         examples=[10.0],
     )
-    cog: Optional[float] = Field(
+    cog: float = Field(
         None,
         ge=0,
         le=360,
-        title="Initial ship course over ground",
         description="Initial ship course over ground in degrees",
         examples=[45.0],
     )
-    heading: Optional[float] = Field(
-        None, ge=0, le=360, title="Initial ship heading", description="Initial ship heading in degrees", examples=[45.2]
+    heading: float = Field(
+        None,
+        ge=0,
+        le=360,
+        description="Initial ship heading in degrees",
+        examples=[45.2],
     )
     nav_status: Optional[AISNavStatus] = Field(None, description="AIS Navigational Status")
 
-    # @classmethod
-    # def default(cls):
-    #     """Create a default instance of the class."""
-    #     return cls(
-    #         position=create_position_example(),
-    #         sog=10.0,
-    #         cog=45.0,
-    #         heading=45.2,
-    #         nav_status=AISNavStatus.UNDER_WAY_USING_ENGINE,
-    #     )
-
 
 class DataPoint(BaseModelConfig):
-    value: Optional[float] = Field(None, description="the value of the data at the current timestep", examples=[12.3])
-    m_before_leg_change: float = Field(
-        None, description="meters before the waypoint to start interpolating to the new value", examples=[10]
+    value: Optional[float] = Field(
+        None,
+        description="the value of the data at the current timestep",
+        examples=[12.3],
+    )
+    m_before_leg_change: Optional[float] = Field(
+        None,
+        description="meters before the waypoint to start interpolating to the new value",
+        examples=[10],
     )
     m_after_leg_change: Optional[float] = Field(
-        None, description="meters after the waypoint to finish interpolating to the new value", examples=[10]
+        None,
+        description="meters after the waypoint to finish interpolating to the new value",
+        examples=[10],
     )
     interp_method: Optional[Union[InterpolationMethod, str]] = Field(None, description="Method used for interpolation")
 
 
 class Data(BaseModelConfig):
-    sog: Optional[DataPoint] = Field(
-        None,
-        description="Speed data point",
-        examples=[DataPoint(value=12.3, m_before_leg_change=100, m_after_leg_change=100, interp_method="linear")],
-    )
-    heading: Optional[DataPoint] = Field(
-        None,
-        description="Heading data point",
-        examples=[DataPoint(value=180, m_before_leg_change=100, m_after_leg_change=100, interp_method="linear")],
-    )
     model_config = ConfigDict(
         extra="allow",
         json_schema_extra={
             "additionalProperties": {
                 "type": "object",
                 "properties": {
                     "value": {"type": "number"},
                     "mBeforeLegChange": {"type": "number"},
                     "mAfterLegChange": {"type": "number"},
                     "interpMethod": {"type": "string"},
                 },
-                "required": ["value", "mBeforeLegChange", "mAfterLegChange", "interpMethod"],
+                "required": [],
                 "description": "The 'data' field can include additional properties. All additional properties should be DataPoint objects.",
-            }
+            },
+            "sog": {
+                "type": "object",
+                "properties": {
+                    "value": {"type": "number"},
+                    "mBeforeLegChange": {"type": "number"},
+                    "mAfterLegChange": {"type": "number"},
+                    "interpMethod": {"type": "string"},
+                },
+                "required": [],
+                "description": "Speed data point",
+                "examples": [
+                    {
+                        "value": 12.3,
+                        "mBeforeLegChange": 100,
+                        "mAfterLegChange": 100,
+                        "interpMethod": "linear",
+                    }
+                ],
+            },
+            "heading": {
+                "type": "object",
+                "properties": {
+                    "value": {"type": "number"},
+                    "mBeforeLegChange": {"type": "number"},
+                    "mAfterLegChange": {"type": "number"},
+                    "interpMethod": {"type": "string"},
+                },
+                "required": [],
+                "description": "Heading data point",
+                "examples": [
+                    {
+                        "value": 180,
+                        "mBeforeLegChange": 100,
+                        "mAfterLegChange": 100,
+                        "interpMethod": "linear",
+                    }
+                ],
+            },
         },
     )
 
 
 class Waypoint(BaseModelConfig):
     position: Position = Field(
-        description="A geographical coordinate", examples=[Position(latitude=51.2123, longitude=11.2313)]
+        description="A geographical coordinate",
+        examples=[Position(latitude=51.2123, longitude=11.2313)],
     )
     turn_radius: Optional[float] = Field(
-        None, description="Orthodrome turn radius as defined in RTZ format", examples=[200]
+        None,
+        description="Orthodrome turn radius as defined in RTZ format",
+        examples=[200],
     )
     data: Optional[Data] = Field(
-        None, description="A `Data` object that includes `speed`, `course`, and `heading` data points"
+        None,
+        description="A `Data` object that includes `speed`, `course`, and `heading` data points",
     )
 
 
 class Ship(BaseModelConfig):
-    static: Optional[ShipStatic] = Field(
+    static: ShipStatic = Field(
         None,
         description="Static ship information which does not change during a scenario.",
         examples=[create_ship_static_example()],
     )
-    initial: Optional[Initial] = Field(None, title="Initial own ship Initial", examples=[create_initial_example()])
+    initial: Optional[Initial] = Field(None, examples=[create_initial_example()])
     waypoints: Optional[List[Waypoint]] = Field(
         None,
         description="An array of `Waypoint` objects. Each waypoint object must have a `position` property. <br /> If no turn radius is provided, it will be assumed to be `0`. <br /> Additional data can be added to each waypoint leg. This allows varying parameters on a per-leg basis, such as speed and heading, or navigational status ",
         examples=[create_waypoint_example()],
     )
 
     def __init__(self, **data: Any):
         super().__init__(**data)
         if not self.waypoints:
             self.waypoints = self.generate_waypoints()
 
-    def generate_waypoints(self) -> List[Waypoint]:
+    def generate_waypoints(self) -> Union[List[Waypoint], None]:
         """Generate waypoints if they don't exist."""
         waypoints = []
-        if (
-            self.initial is not None
-            and self.initial.position is not None
-            and self.initial.position.longitude is not None
-            and self.initial.position.latitude is not None
-            and self.initial.cog is not None
-        ):
+
+        if self.initial:
             # Create waypoints from initial position
             geod = Geod(ellps="WGS84")
             lon, lat, _ = geod.fwd(
                 self.initial.position.longitude,
                 self.initial.position.latitude,
                 self.initial.cog,
                 10000,  # distance in meters
             )
             position1 = Position(latitude=lat, longitude=lon)
             waypoint1 = Waypoint(position=position1)
-            sog_0 = DataPoint(value=self.initial.sog, m_before_leg_change=0, m_after_leg_change=0, interp_method=None)
-            cog_0 = DataPoint(value=self.initial.cog, m_before_leg_change=0, m_after_leg_change=0, interp_method=None)
-            data_0 = Data(sog=sog_0, cog=cog_0)
 
             position0 = Position(
-                latitude=self.initial.position.latitude, longitude=self.initial.position.longitude, data=data_0
+                latitude=self.initial.position.latitude,
+                longitude=self.initial.position.longitude,
             )
-            waypoint0 = Waypoint(position=position0)
+            waypoint0 = Waypoint(position=position0, data=None)
 
             waypoints = [waypoint0, waypoint1]
-        return waypoints
+            return waypoints
+
+        else:
+            return None
 
 
 class OwnShip(Ship):
     pass
 
 
 class TargetShip(Ship):
     pass
 
 
 class TrafficSituation(BaseModelConfig):
-    title: Optional[str] = Field(None, description="The title of the traffic situation", examples=["overtaking_18"])
+    title: str = Field(
+        None,
+        description="The title of the traffic situation",
+        examples=["overtaking_18"],
+    )
     description: Optional[str] = Field(
         None,
         description="A description of the traffic situation",
         examples=["Crossing situation with 3 target vessels in the Oslofjord"],
     )
     start_time: Optional[datetime] = Field(
         None,
-        title="Situation starting time",
         description="Starting time of the situation in `ISO 8601` format `YYYY-MM-DDThh:mm:ssZ`",
         examples=[datetime.now()],
     )
-    own_ship: OwnShip = Field(title="Own Ship data", description="Own Ship data", examples=[create_ship_example()])
+    own_ship: OwnShip = Field(
+        title="Own Ship data",
+        description="Own Ship data",
+        examples=[create_ship_example()],
+    )
     target_ships: List[TargetShip] = Field(
-        None, title="Target Ship data", description="Target Ship data", examples=[[create_ship_example()]]
+        None,
+        title="Target Ship data",
+        description="Target Ship data",
+        examples=[[create_ship_example()]],
     )
     environment: Optional[Environment] = Field(
-        None, description="environmental parameters", examples=[create_environment_example()]
+        None,
+        description="environmental parameters",
+        examples=[create_environment_example()],
     )
 
     model_config = ConfigDict(
         extra="allow",
         title="Test Input Schema",
         json_schema_extra={"additionalProperties": True, "omit_default": True},
     )
 
 
 class SoftwareConfig(BaseModelConfig):
     name: str = Field(..., description="The name of the system", examples=["AutoNavigation-System 1"])
-    version: str = Field(..., description="The software version", examples=["1.2.3"])
     vendor: str = Field(..., description="The name of the system vendor", examples=["CompanyABC"])
+    version: str = Field(..., description="The software version", examples=["1.2.3"])
 
     model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
 
 
-class CagaConfiguration(SoftwareConfig):
-    vendor_minimum_distance_to_targets: float = Field(
-        None, description="Minimum distance in meters that the system will keep to other Vessels", examples=[100]
-    )
-    vendor_critical_TCPA: float = Field(  # noqa: N815
-        None,
-        description="If the projected CPA is less than minimumDistanceToTargets, and TCPA falls below criticalTCPA, a new manoeuver should be calculated",
-        examples=[1000],
-    )
-    vendor_manoeuver_delay: float = Field(
-        None,
-        description="Time given in seconds to the navigator / system, before the proposed manoeuver is no longer able to be excecuted",
-        examples=[20],
-    )
-    vendor_safety_depth: float = Field(None, description="Minimum safety depth", examples=[30])
-    vendor_automatic_manoeuver_acceptance_time: float = Field(
-        None,
-        description="If automatic maneuver acceptance is enabled, the new route will be activated after a specified number of seconds",
-        examples=[20],
+class CagaConfiguration(BaseModelConfig):
+    name: str = Field(..., description="The name of the system", examples=["AutoNavigation-System 1"])
+    vendor: str = Field(..., description="The name of the system vendor", examples=["CompanyABC"])
+    version: str = Field(..., description="The software version", examples=["1.2.3"])
+    model_config = ConfigDict(
+        json_schema_extra={
+            "additionalProperties": True,
+            "properties": {
+                "vendor_minimum_distance_to_targets": {
+                    "type": "number",
+                    "description": "Minimum distance in meters that the system will keep to other Vessels",
+                    "examples": [100],
+                },
+                "vendor_critical_TCPA": {
+                    "type": "number",
+                    "description": "If the projected CPA is less than minimumDistanceToTargets, and TCPA falls below criticalTCPA, a new manoeuver should be calculated",
+                    "examples": [1000],
+                },
+                "vendor_manoeuver_delay": {
+                    "type": "number",
+                    "description": "Time given in seconds to the navigator / system, before the proposed manoeuver is no longer able to be excecuted",
+                    "examples": [20],
+                },
+                "vendor_safety_depth": {"type": "number", "description": "Minimum safety depth", "examples": [30]},
+                "vendor_automatic_manoeuver_acceptance_time": {
+                    "type": "number",
+                    "description": "If automatic maneuver acceptance is enabled, the new route will be activated after a specified number of seconds",
+                    "examples": [20],
+                },
+            },
+        }
     )
 
-    model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
-
 
 class EncounterType(str, Enum):
     OVERTAKING_STAND_ON = "Overtaking stand-on"
     OVERTAKING_GIVE_WAY = "Overtaking give-way"
     HEAD_ON = "Head-on"
     CROSSING_GIVE_WAY = "Crossing give-way"
     CROSSING_STAND_ON = "Crossing stand-on"
@@ -385,129 +440,145 @@
 class PredictedPoint(BaseModelConfig):
     time: Union[datetime, int] = Field(
         ...,
         description="Date and Time of the predicted value `ISO 8601` format `YYYY-MM-DDThh:mm:ssZ`",
         examples=[datetime.now()],
     )
     value: Union[float, Any] = Field(
-        ..., description="Value of the prediction", examples=[create_position_example(), 100]
+        ...,
+        description="Value of the prediction",
+        examples=[create_position_example(), 100],
     )
 
 
 class DetectedShip(BaseModelConfig):
     id: UUID = Field(..., description="Unique Identifier", examples=[uuid4()])
 
     position: Position = Field(
         ...,
-        title="Longitude and Latitude Values",
         description="A geographical coordinate",
         examples=[Position(latitude=51.2123, longitude=11.2313)],
     )
     sog: float = Field(
         ...,
         ge=0,
-        title="ship speed over ground",
         description="Initial ship speed over ground in knots",
         examples=[10.0],
     )
     cog: float = Field(
         ...,
         ge=0,
         le=360,
-        title="ship course over ground",
         description="Initial ship course over ground in degrees",
         examples=[45.0],
     )
-    heading: Optional[float] = Field(
-        None, ge=0, le=360, title="ship heading", description="Initial ship heading in degrees", examples=[45.2]
-    )
+    heading: Optional[float] = Field(None, ge=0, le=360, description="Initial ship heading in degrees", examples=[45.2])
     nav_status: AISNavStatus = Field(None, description="AIS Navigational Status")
 
     encounter_type: Optional[EncounterType] = Field(
         None, description="COLREG encounter type", examples=["Overtaking stand-on"]
     )
     colreg_rules_applied: List[int] = Field(
         None,
         description="COLREG rules the system is applying to the vessel. Each item in the list must be of type `int` corresponding to the COLREG rule number",
         examples=[[16, 17]],
     )
     distance_to_target: float = Field(
-        None, description="Calculated distance from the own ship to the target vessel", examples=[1900.2]
+        None,
+        description="Calculated distance from the own ship to the target vessel",
+        examples=[1900.2],
     )
     dcpa: Optional[float] = Field(None, description="Calculated closest point of approach", examples=[100.3])
     tcpa: Optional[float] = Field(
-        None, description="calculated time to closest point of approach in seconds", examples=[2131]
+        None,
+        description="calculated time to closest point of approach in seconds",
+        examples=[2131],
     )
 
-    predictions: Dict[str, List[PredictedPoint]] = Field(
+    predictions: Optional[Dict[str, List[PredictedPoint]]] = Field(
         None,
         description="List of predicted future values. This can be used to store data like a predicted path for each target vessel. The `value` field supports both numbers and objects",
         examples=[
-            [create_predicted_point_example(), create_predicted_point_example(), create_predicted_point_example()]
+            [
+                create_predicted_point_example(),
+                create_predicted_point_example(),
+                create_predicted_point_example(),
+            ]
         ],
     )
 
     model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
 
 
 class SimulatedShip(BaseModelConfig):
     id: UUID = Field(..., description="Unique Identifier", examples=[uuid4()])
 
     position: Position = Field(
         ...,
-        title="Longitude and Latitude Values",
         description="A geographical coordinate",
         examples=[Position(latitude=51.2123, longitude=11.2313)],
     )
     sog: float = Field(
         ...,
         ge=0,
-        title="ship speed over ground",
         description="Initial ship speed over ground in knots",
         examples=[10.0],
     )
     cog: float = Field(
         ...,
         ge=0,
         le=360,
-        title="ship course over ground",
         description="Initial ship course over ground in degrees",
         examples=[45.0],
     )
     heading: Optional[float] = Field(
-        None, ge=0, le=360, title="ship heading", description="Initial ship heading in degrees", examples=[45.2]
+        None,
+        ge=0,
+        le=360,
+        title="ship heading",
+        description="Initial ship heading in degrees",
+        examples=[45.2],
     )
     nav_status: AISNavStatus = Field(..., description="AIS Navigational Status")
 
     acceleration: float = Field(None, description="Ship acceleration in `ms^-2`", examples=[0.01])
     rate_of_turn: float = Field(None, description="Ship rate of turn in `deg/s`", examples=[1.8])
 
     model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
 
 
-class CagaTimeFrame(BaseModelConfig):
+class CagaTimeStep(BaseModelConfig):
     time: Union[datetime, int] = Field(
         ...,
         description="Date and Time of the predicted value `ISO 8601` format `YYYY-MM-DDThh:mm:ssZ`",
         examples=[datetime.now()],
     )
     target_ships: List[DetectedShip] = Field(
-        ..., description="list of target ships detected by the CAGA system", examples=[[create_detected_ship_example()]]
+        ...,
+        description="list of target ships detected by the CAGA system",
+        examples=[[create_detected_ship_example()]],
     )
     internal_status: Any = Field(
-        None, description="Dictionary containing additional internal  information about the system (health, status..)"
+        None,
+        description="Dictionary containing additional internal  information about the system (health, status..)",
     )
 
 
 class CagaEvent(BaseModelConfig):
     time: Union[datetime, int] = Field(..., description="Date and Time of the event", examples=[datetime.now()])
     route: List[Waypoint] = Field(
         None,
         description="Planned CAGA Route",
-        examples=[[create_waypoint_example(), create_waypoint_example(), create_waypoint_example()]],
+        examples=[
+            [
+                create_waypoint_example(),
+                create_waypoint_example(),
+                create_waypoint_example(),
+            ]
+        ],
     )
 
     calculation_time: Optional[float] = Field(None, description="Time to calculate new route")
 
     model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
 
 
@@ -517,19 +588,23 @@
     model_config = ConfigDict(json_schema_extra={"additionalProperties": True})
 
 
 class CagaData(BaseModelConfig):
     configuration: CagaConfiguration = Field(
         ..., description="System Configuration", examples=[create_caga_config_example()]
     )
-    time_series_data: List[CagaTimeFrame] = Field(
-        ..., description="Time series data from the system", examples=[[create_caga_time_frame_example()]]
+    time_series_data: List[CagaTimeStep] = Field(
+        ...,
+        description="Time series data from the system",
+        examples=[[create_caga_time_frame_example()]],
     )
     event_data: List[CagaEvent] = Field(
-        None, description="Event data from the system", examples=[[create_caga_event_example()]]
+        None,
+        description="Event data from the system",
+        examples=[[create_caga_event_example()]],
     )
 
 
 class SimulationTimeFrame(BaseModelConfig):
     time: Union[datetime, int] = Field(
         ...,
         description="Date and Time of the predicted value `ISO 8601` format `YYYY-MM-DDThh:mm:ssZ`",
@@ -537,20 +612,27 @@
     )
     own_ship: SimulatedShip
     target_ships: List[SimulatedShip]
 
 
 class SimulationData(BaseModelConfig):
     configuration: SoftwareConfig = Field(
-        ..., description="Simulator software configuration", examples=[create_software_config_example()]
+        ...,
+        description="Simulator software configuration",
+        examples=[create_software_config_example()],
     )
     time_series_data: List[SimulationTimeFrame] = Field(
         ...,
         description="TimeSeries data originating from the Simulator",
-        examples=[[create_simulation_timeframe_example(), create_simulation_timeframe_example()]],
+        examples=[
+            [
+                create_simulation_timeframe_example(),
+                create_simulation_timeframe_example(),
+            ]
+        ],
     )
     event_data: List[SimulatorEvent] = Field(None, description="Event data from the simulator")
 
 
 class OutputSchema(BaseModelConfig):
     creation_time: datetime = Field(
         ...,
@@ -613,14 +695,15 @@
     docs_dir = docs_dir if isinstance(docs_dir, Path) else Path(docs_dir)
 
     # Generate input schema
     generate_schema(
         model=TrafficSituation,
         name="input_schema",
         schema_dir=schema_dir,
+        by_alias=True,
     )
 
     # Generate output schema
     generate_schema(
         model=OutputSchema,
         name="output_schema",
         schema_dir=schema_dir,
```

### Comparing `maritime-schema-0.0.5/src/maritime_schema/types/caga_examples.py` & `maritime-schema-0.0.6/src/maritime_schema/types/caga_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     from maritime_schema.types.caga import GeneralShipType, ShipStatic
 
     return ShipStatic(
         id=generate_uuid(),
         length=230.0,
         width=30.0,
         height=15.0,
+        speed_max=20.0,
         mmsi=123456789,
         name="RMS Titanic",
         ship_type=GeneralShipType.FISHING,
         imo=1000001,
     )
 
 
@@ -68,15 +69,15 @@
 
 def create_waypoint_example():
     from maritime_schema.types.caga import Data, Waypoint
 
     return Waypoint(
         position=create_position_example(),
         turn_radius=500,
-        data=Data(sog=create_data_point_example(), heading=create_data_point_example()),
+        data=Data(sog=create_data_point_example(), heading=create_data_point_example()),  # type:ignore
     )
 
 
 def create_ship_example():
     from maritime_schema.types.caga import Ship
 
     return Ship(
@@ -124,19 +125,14 @@
 
     software_config = create_software_config_example()
 
     return CagaConfiguration(
         name=software_config.name,
         version=software_config.version,
         vendor=software_config.vendor,
-        vendor_minimum_distance_to_targets=100,
-        vendor_critical_TCPA=1000,
-        vendor_manoeuver_delay=20,
-        vendor_safety_depth=20,
-        vendor_automatic_manoeuver_acceptance_time=7,
     )
 
 
 def create_predicted_point_example():
     from maritime_schema.types.caga import PredictedPoint
 
     return PredictedPoint(time=datetime.now(), value=create_position_example())
@@ -179,17 +175,17 @@
         nav_status=AISNavStatus.ENGAGED_IN_FISHING,
         acceleration=0.01,
         rate_of_turn=1,
     )
 
 
 def create_caga_time_frame_example():
-    from maritime_schema.types.caga import CagaTimeFrame
+    from maritime_schema.types.caga import CagaTimeStep
 
-    return CagaTimeFrame(time=datetime.now(), target_ships=[create_detected_ship_example()], internal_status=None)
+    return CagaTimeStep(time=datetime.now(), target_ships=[create_detected_ship_example()], internal_status=None)
 
 
 def create_caga_event_example():
     from maritime_schema.types.caga import CagaEvent
 
     return CagaEvent(
         time=datetime.now(),
```

### Comparing `maritime-schema-0.0.5/src/maritime_schema/utils/logging.py` & `maritime-schema-0.0.6/src/maritime_schema/utils/logging.py`

 * *Files identical despite different names*

### Comparing `maritime-schema-0.0.5/src/maritime_schema/utils/publish.py` & `maritime-schema-0.0.6/src/maritime_schema/utils/publish.py`

 * *Files identical despite different names*

### Comparing `maritime-schema-0.0.5/src/maritime_schema.egg-info/SOURCES.txt` & `maritime-schema-0.0.6/src/maritime_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

