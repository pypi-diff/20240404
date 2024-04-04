# Comparing `tmp/geojson-shave-0.1.0.tar.gz` & `tmp/geojson-shave-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson-shave-0.1.0.tar", last modified: Fri Mar 29 08:09:58 2024, max compression
+gzip compressed data, was "geojson-shave-0.1.1.tar", last modified: Thu Apr  4 01:18:42 2024, max compression
```

## Comparing `geojson-shave-0.1.0.tar` & `geojson-shave-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-03-29 08:09:58.880683 geojson-shave-0.1.0/
--rw-rw-r--   0 benjaminnour   (501) staff       (20)     1067 2024-03-29 06:27:46.000000 geojson-shave-0.1.0/LICENSE
--rw-r--r--   0 benjaminnour   (501) staff       (20)     2404 2024-03-29 08:09:58.880599 geojson-shave-0.1.0/PKG-INFO
--rw-rw-r--   0 benjaminnour   (501) staff       (20)     1559 2024-03-29 07:56:16.000000 geojson-shave-0.1.0/README.md
-drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-03-29 08:09:58.877453 geojson-shave-0.1.0/geojson_shave/
--rw-rw-r--   0 benjaminnour   (501) staff       (20)      127 2024-03-29 06:27:46.000000 geojson-shave-0.1.0/geojson_shave/__init__.py
--rw-rw-r--   0 benjaminnour   (501) staff       (20)     7584 2024-03-29 07:55:02.000000 geojson-shave-0.1.0/geojson_shave/geojson_shave.py
-drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-03-29 08:09:58.880293 geojson-shave-0.1.0/geojson_shave.egg-info/
--rw-r--r--   0 benjaminnour   (501) staff       (20)     2404 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/PKG-INFO
--rw-r--r--   0 benjaminnour   (501) staff       (20)      337 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminnour   (501) staff       (20)        1 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminnour   (501) staff       (20)       67 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/entry_points.txt
--rw-r--r--   0 benjaminnour   (501) staff       (20)       24 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/requires.txt
--rw-r--r--   0 benjaminnour   (501) staff       (20)       14 2024-03-29 08:09:58.000000 geojson-shave-0.1.0/geojson_shave.egg-info/top_level.txt
--rw-r--r--   0 benjaminnour   (501) staff       (20)      897 2024-03-29 08:09:58.881124 geojson-shave-0.1.0/setup.cfg
--rw-r--r--   0 benjaminnour   (501) staff       (20)       69 2024-03-29 07:40:47.000000 geojson-shave-0.1.0/setup.py
-drwxr-xr-x   0 benjaminnour   (501) staff       (20)        0 2024-03-29 08:09:58.879758 geojson-shave-0.1.0/tests/
--rw-rw-r--   0 benjaminnour   (501) staff       (20)    20036 2024-03-29 06:27:46.000000 geojson-shave-0.1.0/tests/test_logic.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.423693 geojson-shave-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-04 00:47:11.000000 geojson-shave-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3325 2024-04-04 01:18:42.184688 geojson-shave-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-04-04 00:47:11.000000 geojson-shave-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.438691 geojson-shave-0.1.1/geojson_shave/
+-rw-rw-rw-   0        0        0      132 2024-04-04 01:02:05.000000 geojson-shave-0.1.1/geojson_shave/__init__.py
+-rw-rw-rw-   0        0        0     7746 2024-04-04 00:53:01.000000 geojson-shave-0.1.1/geojson_shave/geojson_shave.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.449692 geojson-shave-0.1.1/geojson_shave.egg-info/
+-rw-rw-rw-   0        0        0     3325 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-04 01:18:41.000000 geojson-shave-0.1.1/geojson_shave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-04 01:18:40.000000 geojson-shave-0.1.1/geojson_shave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      932 2024-04-04 01:18:42.241687 geojson-shave-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-04-04 00:47:12.000000 geojson-shave-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:18:41.456692 geojson-shave-0.1.1/tests/
+-rw-rw-rw-   0        0        0    20609 2024-04-04 00:47:12.000000 geojson-shave-0.1.1/tests/test_logic.py
```

### Comparing `geojson-shave-0.1.0/PKG-INFO` & `geojson-shave-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,93 @@
-Metadata-Version: 2.1
-Name: geojson-shave
-Version: 0.1.0
-Summary: A command-line tool for reducing the size of GeoJSON files.
-Home-page: https://github.com/ben-n93/geojson-shave
-Author: Ben Nour
-Author-email: hello@ben-nour.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress
-Requires-Dist: humanize
-
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
-    </a>
-</p>
-
----
-
-geojson-shave reduces the size of GeoJSON files by:
-
-- Truncating latitude/longitude coordinates to the specified decimal places.
-- Eliminating unnecessary whitespace.
-- (Optionally) replacing the properties key's value with null/empty dictionary.
-
-This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
-
-## Installation
-```
-$ pip install geojson-shave
-```
-
-## Usage
-
-Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
-
-```
-$ geojson-shave roads.geoson
-```
-
-Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
-
-```
-$ geojson-shave roads.geojson -d 3
-```
-
-You can also specify if you only want certain Geometry object types in the file to be processed:
-```
-$ geojson-shave roads.geojson -g LineString Polygon
-```
-
-Note that the -g option doesn't apply to objects nested within Geometry Collection.
-
-And to reduce the file size even further you can nullify the property value of Feature objects:
-
-```
-$ geojson-shave roads.geojson -p
-```
-
-Output to a directory other than the current working directory:
-```
-$ geojson-shave roads.geojson -o ../data/output.geojson
-```
-
-## TODO
-
-- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
+Metadata-Version: 2.1
+Name: geojson-shave
+Version: 0.1.1
+Summary: A command-line tool for reducing the size of GeoJSON files.
+Home-page: https://github.com/ben-n93/geojson-shave
+Author: Ben Nour
+Author-email: hello@ben-nour.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress
+Requires-Dist: humanize
+
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
+    </a>
+</p>
+
+<p align="center">
+     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
+     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
+    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
+    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
+</p>
+
+---
+
+geojson-shave reduces the size of GeoJSON files by:
+
+- Truncating latitude/longitude coordinates to the specified decimal places.
+- Eliminating unnecessary whitespace.
+- (Optionally) replacing the properties key's value with null/empty dictionary.
+
+This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
+
+## Installation
+```
+$ pip install geojson-shave
+```
+
+## Usage
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
+    </a>
+</p>
+
+Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
+
+```
+$ geojson-shave roads.geoson
+```
+
+Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
+
+```
+$ geojson-shave roads.geojson -d 3
+```
+
+You can also specify if you only want certain Geometry object types in the file to be processed:
+```
+$ geojson-shave roads.geojson -g LineString Polygon
+```
+
+Note that the -g option doesn't apply to objects nested within Geometry Collection.
+
+And to reduce the file size even further you can nullify the property value of Feature objects:
+
+```
+$ geojson-shave roads.geojson -p
+```
+
+Output to a directory other than the current working directory:
+```
+$ geojson-shave roads.geojson -o ../data/output.geojson
+```
+
+## TODO
+
+- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.0 Summary: A command-
+Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.1 Summary: A command-
 line tool for reducing the size of GeoJSON files. Home-page: https://
 github.com/ben-n93/geojson-shave Author: Ben Nour Author-email: hello@ben-
 nour.com License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: alive-progress Requires-
 Dist: humanize
                                 _[_G_e_o_J_S_O_N_-_s_h_a_v_e_]
+     _[_T_e_s_t_i_n_g_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_b_e_n_-_n_9_3_/_g_e_o_j_s_o_n_-_s_h_a_v_e_/_g_r_a_p_h_/
+                     _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_X_U_M_K_0_D_4_J_9_X_]_[_v_e_r_s_i_o_n_s_]
 --- geojson-shave reduces the size of GeoJSON files by: - Truncating latitude/
 longitude coordinates to the specified decimal places. - Eliminating
 unnecessary whitespace. - (Optionally) replacing the properties key's value
 with null/empty dictionary. This tool assumes that your GeoJSON file confirms
 to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946). ##
-Installation ``` $ pip install geojson-shave ``` ## Usage Simply pass the file
-path of your GeoJSON file and it will truncuate the coordinates to 5 decimal
-places, outputing to the current working directory: ``` $ geojson-shave
-roads.geoson ``` Alterntatively you can specify the number of decimal points
-you want the coordiantes truncuated to: ``` $ geojson-shave roads.geojson -d 3
-``` You can also specify if you only want certain Geometry object types in the
-file to be processed: ``` $ geojson-shave roads.geojson -g LineString Polygon
-``` Note that the -g option doesn't apply to objects nested within Geometry
-Collection. And to reduce the file size even further you can nullify the
-property value of Feature objects: ``` $ geojson-shave roads.geojson -p ```
-Output to a directory other than the current working directory: ``` $ geojson-
-shave roads.geojson -o ../data/output.geojson ``` ## TODO - [ ] Add support for
-passing the URL of a hosted GeoJSON file to the tool.
+Installation ``` $ pip install geojson-shave ``` ## Usage
+                             _[_G_e_o_J_S_O_N_-_s_h_a_v_e_-_d_e_m_o_]
+Simply pass the file path of your GeoJSON file and it will truncuate the
+coordinates to 5 decimal places, outputing to the current working directory:
+``` $ geojson-shave roads.geoson ``` Alterntatively you can specify the number
+of decimal points you want the coordiantes truncuated to: ``` $ geojson-shave
+roads.geojson -d 3 ``` You can also specify if you only want certain Geometry
+object types in the file to be processed: ``` $ geojson-shave roads.geojson -
+g LineString Polygon ``` Note that the -g option doesn't apply to objects
+nested within Geometry Collection. And to reduce the file size even further you
+can nullify the property value of Feature objects: ``` $ geojson-shave
+roads.geojson -p ``` Output to a directory other than the current working
+directory: ``` $ geojson-shave roads.geojson -o ../data/output.geojson ``` ##
+TODO - [ ] Add support for passing the URL of a hosted GeoJSON file to the
+tool.
```

### Comparing `geojson-shave-0.1.0/geojson_shave/geojson_shave.py` & `geojson-shave-0.1.1/geojson_shave/geojson_shave.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,220 +1,219 @@
-"""A command-line tool that reduces the size of GeoJSON files.
-"""
-
-import argparse
-import json
-import pathlib
-import re
-
-from alive_progress import alive_bar
-import humanize
-
-GEOMETRY_OBJECTS = {
-    "Point",
-    "MultiPoint",
-    "LineString",
-    "MultiLineString",
-    "Polygon",
-    "MultiPolygon",
-    "GeometryCollection",
-}
-
-
-def get_parser():
-    """Create the command-line interface."""
-    parser = argparse.ArgumentParser(
-        description="""Reduces the size of a GeoJSON file by lowering the
-        decimal point precision of the file's latitude/language 
-        coordinates.""",
-        epilog="""
-        EXAMPLES
-        --------
-        Truncuate a GeoJSON's file to 3 decimal points:
-            geojson_shave roads.geojson -d 3
-
-        Only truncuate the coordinates of LineString and Polygon objects:
-            geojson_shave roads.geojson -g LineString Polygon
-
-        Replace the properties value with a null value:
-            geojson_shave roads.geojson -p
-        """,
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-
-    parser.add_argument(
-        "input",
-        type=argparse.FileType("r"),
-        help="Input GeoJSON file to pass to the tool.",
-    )
-
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=argparse.FileType("w"),
-        help="""Name and path of the output GeoJSON file. Default path is the
-        current working directory.""",
-        default=pathlib.Path.cwd() / "output.geojson",
-        required=False,
-    )
-
-    parser.add_argument(
-        "-d",
-        "--decimal_points",
-        type=int,
-        help="Number of decimal points to keep when \
-                            truncating coordinates. Default is 5.",
-        required=False,
-        default=5,
-    )
-
-    parser.add_argument(
-        "-p",
-        "--properties",
-        help="Overwrite the properties with a null value.",
-        required=False,
-        action="store_true",
-    )
-
-    parser.add_argument(
-        "-g",
-        "--geometry_object",
-        type=str,
-        help="""The types of Geometry Object to be processed.
-        Default is all objects.""",
-        required=False,
-        default=GEOMETRY_OBJECTS,
-        choices=GEOMETRY_OBJECTS,
-        metavar="GEOMETRY_OBJECT",
-        nargs="+",
-    )
-
-    return parser
-
-
-def _create_coordinates(coordinates, precision):
-    """Create truncuated coordinates."""
-    new_coordinates = []
-    for item in coordinates:
-        if isinstance(item, list):
-            new_coordinates.append(_create_coordinates(item, precision))
-        else:
-            item = re.search(rf"[\-]?[0-9]+\.[0-9]{{0,{precision}}}", str(item)).group()
-            new_coordinates.append(float(item))
-    return new_coordinates
-
-
-def _process_geometry_collection(geometry_collection, precision):
-    """Parse and truncuate the coordinates of each geometry
-    object nested within a geometry collection."""
-    new_geometry_collection = {"type": "GeometryCollection"}
-    processed_geometry_objects = []
-    for geometry_object in geometry_collection["geometries"]:
-        object_type = geometry_object["type"]
-        new_coordinates = _create_coordinates(geometry_object["coordinates"], precision)
-        processed_geometry_objects.append(
-            {"type": object_type, "coordinates": new_coordinates}
-        )
-
-    new_geometry_collection["geometries"] = processed_geometry_objects
-    return new_geometry_collection
-
-
-def _process_features(geojson, precision, geometry_to_include, nullify_property):
-    """Process Feature objects, truncuating coordinates and/or replacing
-    the properties member with a blank value."""
-    # Create new GeoJSON object.
-    if (total_features := geojson.get("features")) is None:
-        if geojson.get("type") == "Feature":
-            output_geojson = {"type": "Feature"}
-            length = 1
-        else:
-            raise SystemError("Error: there are no Feature objects in this file.")
-    else:
-        output_geojson = {"type": "FeatureCollection", "features": []}
-        length = len(total_features)
-
-    # Process Feature objects.
-    with alive_bar(length) as progress_bar:
-        progress_bar.title("Processing the input file:")
-        if geojson["type"] == "FeatureCollection":
-            for index, feature in enumerate(geojson["features"]):
-                output_geojson["features"].append(feature)
-                if nullify_property:
-                    output_geojson["features"][index]["properties"] = {}
-                try:
-                    if (geo_type := feature["geometry"]["type"]) in geometry_to_include:
-                        if geo_type == "GeometryCollection":
-                            output_geojson["features"][index]["geometry"] = (
-                                _process_geometry_collection(
-                                    feature["geometry"], precision
-                                )
-                            )
-                        else:
-                            new_coordinates = _create_coordinates(
-                                feature["geometry"]["coordinates"], precision
-                            )
-                            output_geojson["features"][index]["geometry"][
-                                "coordinates"
-                            ] = new_coordinates
-                except TypeError:  # Feature's "geometry" member has a null value.
-                    progress_bar()
-                    continue
-                progress_bar()
-
-        else:  # Only one Feature.
-            if geojson["geometry"]["type"] in geometry_to_include:
-                new_coordinates = _create_coordinates(
-                    geojson["geometry"]["coordinates"], precision
-                )
-                output_geojson["geometry"] = {
-                    "type": geojson["geometry"]["type"],
-                    "coordinates": new_coordinates,
-                }
-                if nullify_property:
-                    output_geojson["properties"] = {}
-                progress_bar()
-
-    # Including any non-standard (RFC) top-level keys in the output file.
-    for key in geojson.keys():
-        if key not in ("type", "features", "geometry"):
-            output_geojson[key] = geojson[key]
-    return output_geojson
-
-
-def main():
-    """Launch the command-line tool."""
-    parser = get_parser()
-    args = parser.parse_args()
-
-    if args.decimal_points < 0:
-        raise ValueError(
-            """Please only pass a positive number to the
-        decimal argument."""
-        )
-
-    # Process input file.
-    with open(args.input.name, "r") as input_file:
-        try:
-            input_geojson = json.load(input_file)
-        except json.decoder.JSONDecodeError as e:
-            raise SystemError("Error: please provide a valid GeoJSON file.") from e
-    output_geojson = _process_features(
-        input_geojson, args.decimal_points, args.geometry_object, args.properties
-    )
-
-    # Write to output file.
-    with open(args.output.name, "w", encoding="utf-8") as output_file:
-        print("Writing to output file...")
-        json.dump(output_geojson, output_file, separators=(",", ":"))
-
-    # Exit message to user.
-    size_before = pathlib.Path(args.input.name).stat().st_size
-    size_after = pathlib.Path(args.output.name).stat().st_size
-    difference = round(((size_before - size_after) / size_before) * 100)
-    print(f"Input file size: {humanize.naturalsize(size_before)}.")
-    print(f"Output file size: {humanize.naturalsize(size_after)}.")
-    print(f"File size reduction: {difference}%")
-
-
-if __name__ == "__main__":
-    main()
+"""A command-line tool that reduces the size of GeoJSON files.
+"""
+
+import argparse
+import json
+import pathlib
+
+from alive_progress import alive_bar
+import humanize
+
+GEOMETRY_OBJECTS = {
+    "Point",
+    "MultiPoint",
+    "LineString",
+    "MultiLineString",
+    "Polygon",
+    "MultiPolygon",
+    "GeometryCollection",
+}
+
+
+def get_parser():
+    """Create the command-line interface."""
+    parser = argparse.ArgumentParser(
+        description="""Reduces the size of a GeoJSON file by lowering the
+        decimal point precision of the file's latitude/language 
+        coordinates.""",
+        epilog="""
+        EXAMPLES
+        --------
+        Truncuate a GeoJSON's file to 3 decimal points:
+            geojson_shave roads.geojson -d 3
+
+        Only truncuate the coordinates of LineString and Polygon objects:
+            geojson_shave roads.geojson -g LineString Polygon
+
+        Replace the properties value with a null value:
+            geojson_shave roads.geojson -p
+        """,
+        formatter_class=argparse.RawTextHelpFormatter,
+    )
+
+    parser.add_argument(
+        "input",
+        type=argparse.FileType("r"),
+        help="Input GeoJSON file to pass to the tool.",
+    )
+
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=argparse.FileType("w"),
+        help="""Name and path of the output GeoJSON file. Default path is the
+        current working directory.""",
+        default=pathlib.Path.cwd() / "output.geojson",
+        required=False,
+    )
+
+    parser.add_argument(
+        "-d",
+        "--decimal_points",
+        type=int,
+        help="Number of decimal points to keep when \
+                            truncating coordinates. Default is 5.",
+        required=False,
+        default=5,
+    )
+
+    parser.add_argument(
+        "-p",
+        "--properties",
+        help="Overwrite the properties with a null value.",
+        required=False,
+        action="store_true",
+    )
+
+    parser.add_argument(
+        "-g",
+        "--geometry_object",
+        type=str,
+        help="""The types of Geometry Object to be processed.
+        Default is all objects.""",
+        required=False,
+        default=GEOMETRY_OBJECTS,
+        choices=GEOMETRY_OBJECTS,
+        metavar="GEOMETRY_OBJECT",
+        nargs="+",
+    )
+
+    return parser
+
+
+def _create_coordinates(coordinates, precision):
+    """Create truncuated coordinates."""
+    new_coordinates = []
+    for item in coordinates:
+        if isinstance(item, list):
+            new_coordinates.append(_create_coordinates(item, precision))
+        else:
+            item = round(item, precision)
+            new_coordinates.append(float(item))
+    return new_coordinates
+
+
+def _process_geometry_collection(geometry_collection, precision):
+    """Parse and truncuate the coordinates of each geometry
+    object nested within a geometry collection."""
+    new_geometry_collection = {"type": "GeometryCollection"}
+    processed_geometry_objects = []
+    for geometry_object in geometry_collection["geometries"]:
+        object_type = geometry_object["type"]
+        new_coordinates = _create_coordinates(geometry_object["coordinates"], precision)
+        processed_geometry_objects.append(
+            {"type": object_type, "coordinates": new_coordinates}
+        )
+
+    new_geometry_collection["geometries"] = processed_geometry_objects
+    return new_geometry_collection
+
+
+def _process_features(geojson, precision, geometry_to_include, nullify_property):
+    """Process Feature objects, truncuating coordinates and/or replacing
+    the properties member with a blank value."""
+    # Create new GeoJSON object.
+    if (total_features := geojson.get("features")) is None:
+        if geojson.get("type") == "Feature":
+            output_geojson = {"type": "Feature"}
+            length = 1
+        else:
+            raise SystemError("Error: there are no Feature objects in this file.")
+    else:
+        output_geojson = {"type": "FeatureCollection", "features": []}
+        length = len(total_features)
+
+    # Process Feature objects.
+    with alive_bar(length) as progress_bar:
+        progress_bar.title("Processing the input file:")
+        if geojson["type"] == "FeatureCollection":
+            for index, feature in enumerate(geojson["features"]):
+                output_geojson["features"].append(feature)
+                if nullify_property:
+                    output_geojson["features"][index]["properties"] = {}
+                try:
+                    if (geo_type := feature["geometry"]["type"]) in geometry_to_include:
+                        if geo_type == "GeometryCollection":
+                            output_geojson["features"][index]["geometry"] = (
+                                _process_geometry_collection(
+                                    feature["geometry"], precision
+                                )
+                            )
+                        else:
+                            new_coordinates = _create_coordinates(
+                                feature["geometry"]["coordinates"], precision
+                            )
+                            output_geojson["features"][index]["geometry"][
+                                "coordinates"
+                            ] = new_coordinates
+                except TypeError:  # Feature's "geometry" member has a null value.
+                    progress_bar()
+                    continue
+                progress_bar()
+
+        else:  # Only one Feature.
+            if geojson["geometry"]["type"] in geometry_to_include:
+                new_coordinates = _create_coordinates(
+                    geojson["geometry"]["coordinates"], precision
+                )
+                output_geojson["geometry"] = {
+                    "type": geojson["geometry"]["type"],
+                    "coordinates": new_coordinates,
+                }
+                if nullify_property:
+                    output_geojson["properties"] = {}
+                progress_bar()
+
+    # Including any non-standard (RFC) top-level keys in the output file.
+    for key in geojson.keys():
+        if key not in ("type", "features", "geometry"):
+            output_geojson[key] = geojson[key]
+    return output_geojson
+
+
+def main():
+    """Launch the command-line tool."""
+    parser = get_parser()
+    args = parser.parse_args()
+
+    if args.decimal_points < 0:
+        raise ValueError(
+            """Please only pass a positive number to the
+        decimal argument."""
+        )
+
+    # Process input file.
+    with open(args.input.name, "r") as input_file:
+        try:
+            input_geojson = json.load(input_file)
+        except json.decoder.JSONDecodeError as e:
+            raise SystemError("Error: please provide a valid GeoJSON file.") from e
+    output_geojson = _process_features(
+        input_geojson, args.decimal_points, args.geometry_object, args.properties
+    )
+
+    # Write to output file.
+    with open(args.output.name, "w", encoding="utf-8") as output_file:
+        print("Writing to output file...")
+        json.dump(output_geojson, output_file, separators=(",", ":"))
+
+    # Exit message to user.
+    size_before = pathlib.Path(args.input.name).stat().st_size
+    size_after = pathlib.Path(args.output.name).stat().st_size
+    difference = round(((size_before - size_after) / size_before) * 100)
+    print(f"Input file size: {humanize.naturalsize(size_before)}.")
+    print(f"Output file size: {humanize.naturalsize(size_after)}.")
+    print(f"File size reduction: {difference}%")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `geojson-shave-0.1.0/geojson_shave.egg-info/PKG-INFO` & `geojson-shave-0.1.1/geojson_shave.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,93 @@
-Metadata-Version: 2.1
-Name: geojson-shave
-Version: 0.1.0
-Summary: A command-line tool for reducing the size of GeoJSON files.
-Home-page: https://github.com/ben-n93/geojson-shave
-Author: Ben Nour
-Author-email: hello@ben-nour.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress
-Requires-Dist: humanize
-
-
-<p align="center">
-    <a href="https://pypi.python.org">
-        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
-    </a>
-</p>
-
----
-
-geojson-shave reduces the size of GeoJSON files by:
-
-- Truncating latitude/longitude coordinates to the specified decimal places.
-- Eliminating unnecessary whitespace.
-- (Optionally) replacing the properties key's value with null/empty dictionary.
-
-This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
-
-## Installation
-```
-$ pip install geojson-shave
-```
-
-## Usage
-
-Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
-
-```
-$ geojson-shave roads.geoson
-```
-
-Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
-
-```
-$ geojson-shave roads.geojson -d 3
-```
-
-You can also specify if you only want certain Geometry object types in the file to be processed:
-```
-$ geojson-shave roads.geojson -g LineString Polygon
-```
-
-Note that the -g option doesn't apply to objects nested within Geometry Collection.
-
-And to reduce the file size even further you can nullify the property value of Feature objects:
-
-```
-$ geojson-shave roads.geojson -p
-```
-
-Output to a directory other than the current working directory:
-```
-$ geojson-shave roads.geojson -o ../data/output.geojson
-```
-
-## TODO
-
-- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
+Metadata-Version: 2.1
+Name: geojson-shave
+Version: 0.1.1
+Summary: A command-line tool for reducing the size of GeoJSON files.
+Home-page: https://github.com/ben-n93/geojson-shave
+Author: Ben Nour
+Author-email: hello@ben-nour.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress
+Requires-Dist: humanize
+
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/geojson-shave.png" alt="GeoJSON-shave" style="width: 60%; height: auto;"/>
+    </a>
+</p>
+
+<p align="center">
+     <a href="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml"><img src="https://github.com/ben-n93/geojson-shave/actions/workflows/tests.yml/badge.svg"                 alt="Testing"></a>
+     <a href="https://github.com/ben-n93/geojson-shave/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/geojson-shave" alt="License"></a>
+    <a href="https://codecov.io/gh/ben-n93/geojson-shave" ><img src="https://codecov.io/gh/ben-n93/geojson-shave/graph/badge.svg?token=XUMK0D4J9X"/></a>
+    <a href="https://pypi.org/project/geojson-shave/"><img src="https://img.shields.io/pypi/pyversions/geojson-shave" alt="versions"></a>
+</p>
+
+---
+
+geojson-shave reduces the size of GeoJSON files by:
+
+- Truncating latitude/longitude coordinates to the specified decimal places.
+- Eliminating unnecessary whitespace.
+- (Optionally) replacing the properties key's value with null/empty dictionary.
+
+This tool assumes that your GeoJSON file confirms to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946).
+
+## Installation
+```
+$ pip install geojson-shave
+```
+
+## Usage
+
+<p align="center">
+    <a href="https://pypi.python.org">
+        <img src="https://ben-nour.com/images/demo.gif" alt="GeoJSON-shave-demo">
+    </a>
+</p>
+
+Simply pass the file path of your GeoJSON file and it will truncuate the coordinates to 5 decimal places, outputing to the current working directory:
+
+```
+$ geojson-shave roads.geoson
+```
+
+Alterntatively you can specify the number of decimal points you want the coordiantes truncuated to:
+
+```
+$ geojson-shave roads.geojson -d 3
+```
+
+You can also specify if you only want certain Geometry object types in the file to be processed:
+```
+$ geojson-shave roads.geojson -g LineString Polygon
+```
+
+Note that the -g option doesn't apply to objects nested within Geometry Collection.
+
+And to reduce the file size even further you can nullify the property value of Feature objects:
+
+```
+$ geojson-shave roads.geojson -p
+```
+
+Output to a directory other than the current working directory:
+```
+$ geojson-shave roads.geojson -o ../data/output.geojson
+```
+
+## TODO
+
+- [ ] Add support for passing the URL of a hosted GeoJSON file to the tool.
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.0 Summary: A command-
+Metadata-Version: 2.1 Name: geojson-shave Version: 0.1.1 Summary: A command-
 line tool for reducing the size of GeoJSON files. Home-page: https://
 github.com/ben-n93/geojson-shave Author: Ben Nour Author-email: hello@ben-
 nour.com License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Environment :: Console Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: alive-progress Requires-
 Dist: humanize
                                 _[_G_e_o_J_S_O_N_-_s_h_a_v_e_]
+     _[_T_e_s_t_i_n_g_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_b_e_n_-_n_9_3_/_g_e_o_j_s_o_n_-_s_h_a_v_e_/_g_r_a_p_h_/
+                     _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_X_U_M_K_0_D_4_J_9_X_]_[_v_e_r_s_i_o_n_s_]
 --- geojson-shave reduces the size of GeoJSON files by: - Truncating latitude/
 longitude coordinates to the specified decimal places. - Eliminating
 unnecessary whitespace. - (Optionally) replacing the properties key's value
 with null/empty dictionary. This tool assumes that your GeoJSON file confirms
 to the [RFC 7946](https://datatracker.ietf.org/doc/html/rfc7946). ##
-Installation ``` $ pip install geojson-shave ``` ## Usage Simply pass the file
-path of your GeoJSON file and it will truncuate the coordinates to 5 decimal
-places, outputing to the current working directory: ``` $ geojson-shave
-roads.geoson ``` Alterntatively you can specify the number of decimal points
-you want the coordiantes truncuated to: ``` $ geojson-shave roads.geojson -d 3
-``` You can also specify if you only want certain Geometry object types in the
-file to be processed: ``` $ geojson-shave roads.geojson -g LineString Polygon
-``` Note that the -g option doesn't apply to objects nested within Geometry
-Collection. And to reduce the file size even further you can nullify the
-property value of Feature objects: ``` $ geojson-shave roads.geojson -p ```
-Output to a directory other than the current working directory: ``` $ geojson-
-shave roads.geojson -o ../data/output.geojson ``` ## TODO - [ ] Add support for
-passing the URL of a hosted GeoJSON file to the tool.
+Installation ``` $ pip install geojson-shave ``` ## Usage
+                             _[_G_e_o_J_S_O_N_-_s_h_a_v_e_-_d_e_m_o_]
+Simply pass the file path of your GeoJSON file and it will truncuate the
+coordinates to 5 decimal places, outputing to the current working directory:
+``` $ geojson-shave roads.geoson ``` Alterntatively you can specify the number
+of decimal points you want the coordiantes truncuated to: ``` $ geojson-shave
+roads.geojson -d 3 ``` You can also specify if you only want certain Geometry
+object types in the file to be processed: ``` $ geojson-shave roads.geojson -
+g LineString Polygon ``` Note that the -g option doesn't apply to objects
+nested within Geometry Collection. And to reduce the file size even further you
+can nullify the property value of Feature objects: ``` $ geojson-shave
+roads.geojson -p ``` Output to a directory other than the current working
+directory: ``` $ geojson-shave roads.geojson -o ../data/output.geojson ``` ##
+TODO - [ ] Add support for passing the URL of a hosted GeoJSON file to the
+tool.
```

### Comparing `geojson-shave-0.1.0/setup.cfg` & `geojson-shave-0.1.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6765 6f6a 736f 6e2d 7368 6176 650a  = geojson-shave.
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 300a  version = 0.1.0.
-00000030: 6175 7468 6f72 203d 2042 656e 204e 6f75  author = Ben Nou
-00000040: 720a 6175 7468 6f72 5f65 6d61 696c 203d  r.author_email =
-00000050: 2068 656c 6c6f 4062 656e 2d6e 6f75 722e   hello@ben-nour.
-00000060: 636f 6d0a 6465 7363 7269 7074 696f 6e20  com.description 
-00000070: 3d20 4120 636f 6d6d 616e 642d 6c69 6e65  = A command-line
-00000080: 2074 6f6f 6c20 666f 7220 7265 6475 6369   tool for reduci
-00000090: 6e67 2074 6865 2073 697a 6520 6f66 2047  ng the size of G
-000000a0: 656f 4a53 4f4e 2066 696c 6573 2e0a 6c6f  eoJSON files..lo
-000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000c0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
-000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000e0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-000000f0: 2074 6578 742f 6d61 726b 646f 776e 0a6c   text/markdown.l
-00000100: 6963 656e 7365 203d 204d 4954 0a75 726c  icense = MIT.url
-00000110: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000120: 622e 636f 6d2f 6265 6e2d 6e39 332f 6765  b.com/ben-n93/ge
-00000130: 6f6a 736f 6e2d 7368 6176 650a 636c 6173  ojson-shave.clas
-00000140: 7369 6669 6572 7320 3d20 0a09 4465 7665  sifiers = ..Deve
-00000150: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000160: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
-00000170: 2f53 7461 626c 650a 0949 6e74 656e 6465  /Stable..Intende
-00000180: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000190: 7665 6c6f 7065 7273 0a09 4c69 6365 6e73  velopers..Licens
-000001a0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000001b0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000001c0: 0a09 456e 7669 726f 6e6d 656e 7420 3a3a  ..Environment ::
-000001d0: 2043 6f6e 736f 6c65 0a09 5072 6f67 7261   Console..Progra
-000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001f0: 3a20 5079 7468 6f6e 203a 3a20 330a 0950  : Python :: 3..P
-00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000220: 2033 2e38 0a09 5072 6f67 7261 6d6d 696e   3.8..Programmin
-00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000240: 7468 6f6e 203a 3a20 332e 390a 0950 726f  thon :: 3.9..Pro
-00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000270: 2e31 300a 0950 726f 6772 616d 6d69 6e67  .10..Programming
-00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000290: 686f 6e20 3a3a 2033 2e31 310a 0950 726f  hon :: 3.11..Pro
-000002a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002c0: 2e31 320a 0a5b 6f70 7469 6f6e 735d 0a69  .12..[options].i
-000002d0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-000002e0: 3d20 0a09 616c 6976 652d 7072 6f67 7265  = ..alive-progre
-000002f0: 7373 0a09 6875 6d61 6e69 7a65 0a0a 5b6f  ss..humanize..[o
-00000300: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-00000310: 6e74 735d 0a63 6f6e 736f 6c65 5f73 6372  nts].console_scr
-00000320: 6970 7473 203d 200a 0967 656f 6a73 6f6e  ipts = ..geojson
-00000330: 2d73 6861 7665 203d 2067 656f 6a73 6f6e  -shave = geojson
-00000340: 5f73 6861 7665 2e67 656f 6a73 6f6e 5f73  _shave.geojson_s
-00000350: 6861 7665 3a6d 6169 6e0a 0a5b 6567 675f  have:main..[egg_
-00000360: 696e 666f 5d0a 7461 675f 6275 696c 6420  info].tag_build 
-00000370: 3d20 0a74 6167 5f64 6174 6520 3d20 300a  = .tag_date = 0.
-00000380: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2067 656f 6a73 6f6e 2d73 6861 7665   = geojson-shave
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
+00000030: 310d 0a61 7574 686f 7220 3d20 4265 6e20  1..author = Ben 
+00000040: 4e6f 7572 0d0a 6175 7468 6f72 5f65 6d61  Nour..author_ema
+00000050: 696c 203d 2068 656c 6c6f 4062 656e 2d6e  il = hello@ben-n
+00000060: 6f75 722e 636f 6d0d 0a64 6573 6372 6970  our.com..descrip
+00000070: 7469 6f6e 203d 2041 2063 6f6d 6d61 6e64  tion = A command
+00000080: 2d6c 696e 6520 746f 6f6c 2066 6f72 2072  -line tool for r
+00000090: 6564 7563 696e 6720 7468 6520 7369 7a65  educing the size
+000000a0: 206f 6620 4765 6f4a 534f 4e20 6669 6c65   of GeoJSON file
+000000b0: 732e 0d0a 6c6f 6e67 5f64 6573 6372 6970  s...long_descrip
+000000c0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000d0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000e0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+000000f0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000100: 6b64 6f77 6e0d 0a6c 6963 656e 7365 203d  kdown..license =
+00000110: 204d 4954 0d0a 7572 6c20 3d20 6874 7470   MIT..url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+00000130: 656e 2d6e 3933 2f67 656f 6a73 6f6e 2d73  en-n93/geojson-s
+00000140: 6861 7665 0d0a 636c 6173 7369 6669 6572  have..classifier
+00000150: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
+00000160: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00000170: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00000180: 6c65 0d0a 0949 6e74 656e 6465 6420 4175  le...Intended Au
+00000190: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+000001a0: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
+000001b0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001c0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
+000001d0: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+000001e0: 6f6e 736f 6c65 0d0a 0950 726f 6772 616d  onsole...Program
+000001f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000200: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+00000210: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000220: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000230: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
+00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000280: 2033 2e31 300d 0a09 5072 6f67 7261 6d6d   3.10...Programm
+00000290: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002a0: 5079 7468 6f6e 203a 3a20 332e 3131 0d0a  Python :: 3.11..
+000002b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002d0: 3a3a 2033 2e31 320d 0a0d 0a5b 6f70 7469  :: 3.12....[opti
+000002e0: 6f6e 735d 0d0a 696e 7374 616c 6c5f 7265  ons]..install_re
+000002f0: 7175 6972 6573 203d 200d 0a09 616c 6976  quires = ...aliv
+00000300: 652d 7072 6f67 7265 7373 0d0a 0968 756d  e-progress...hum
+00000310: 616e 697a 650d 0a0d 0a5b 6f70 7469 6f6e  anize....[option
+00000320: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000330: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000340: 203d 200d 0a09 6765 6f6a 736f 6e2d 7368   = ...geojson-sh
+00000350: 6176 6520 3d20 6765 6f6a 736f 6e5f 7368  ave = geojson_sh
+00000360: 6176 652e 6765 6f6a 736f 6e5f 7368 6176  ave.geojson_shav
+00000370: 653a 6d61 696e 0d0a 0d0a 5b65 6767 5f69  e:main....[egg_i
+00000380: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000390: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000003a0: 0d0a 0d0a                                ....
```

### Comparing `geojson-shave-0.1.0/tests/test_logic.py` & `geojson-shave-0.1.1/tests/test_logic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,573 +1,573 @@
-"""Unit tests for geojson_shave.py"""
-
-import os
-import unittest
-import sys
-
-from geojson_shave.geojson_shave import (_create_coordinates,
- _process_geometry_collection,
-_process_features, 
-GEOMETRY_OBJECTS)
-
-
-class TestCreateCoordinates(unittest.TestCase):
-    """Tests for the _create_coordinates function.
-
-    Note that both LineStrings' and MultiPoints' coordinates both consist
-    of an array of Points, hence only the LineString being tested.
-    """
-
-    def setUp(self):
-        self.point = {
-            "type": "Point",
-            "coordinates": [-100.123456, 200.123456],
-            "properties": {"name": "Test Point"},
-        }
-
-        self.linestring = {
-            "type": "LineString",
-            "coordinates": [
-                [100.123456, 0.123456],
-                [101.123456, 1.123456],
-                [102.123456, 2.123456],
-            ],
-        }
-
-        self.multilinestring = {
-            "type": "MultiLineString",
-            "coordinates": [
-                [[-100.123456, 0.123456], [-101.123456, 1.123456]],
-                [[102.123456, 2.123456], [103.123456, 3.123456]],
-            ],
-        }
-
-        self.polygon = {
-            "type": "Polygon",
-            "coordinates": [
-                [
-                    [100.123456, 0.123456],
-                    [101.123456, 0.123456],
-                    [101.123456, 1.123456],
-                    [100.123456, 1.123456],
-                    [100.123456, 0.123456],
-                ]
-            ],
-        }
-
-        self.multipolygon = {
-            "type": "MultiPolygon",
-            "coordinates": [
-                [
-                    [
-                        [102.123456, 2.123456],
-                        [103.123456, 2.123456],
-                        [103.123456, 3.123456],
-                        [102.123456, 3.123456],
-                        [102.123456, 2.123456],
-                    ]
-                ],
-                [
-                    [
-                        [100.123456, 0.123456],
-                        [101.123456, 0.123456],
-                        [101.123456, 1.123456],
-                        [100.123456, 1.123456],
-                        [100.123456, 0.123456],
-                    ],
-                    [
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                        [100.123456, 0.123456],
-                    ],
-                ],
-            ],
-        }
-
-    # Point.
-    def test_truncuating_point_coordinates(self):
-        """Test that Point coordinates are truncuated succesfully."""
-        expected_return_value = [-100.123, 200.123]
-        precision = 3
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_point_same_precision(self):
-        """Test that Point coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.point["coordinates"]
-        precision = 6
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_point_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.point["coordinates"]
-        precision = 50
-        geometry_coordinates = self.point["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # LineString.
-    def test_truncuating_linestring_coordinates(self):
-        """Test that LineString coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [100.123, 0.123],
-            [101.123, 1.123],
-            [102.123, 2.123],
-        ]
-        precision = 3
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_linestring_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.linestring["coordinates"]
-        precision = 6
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_linestring_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.linestring["coordinates"]
-        precision = 50
-        geometry_coordinates = self.linestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # MultiLine strings.
-    def test_truncuating_multilinestring_coordinates(self):
-        """Test that MultiLineString coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [[-100.123, 0.123], [-101.123, 1.123]],
-            [[102.123, 2.123], [103.123, 3.123]],
-        ]
-        precision = 3
-        geometry_coordinates = self.multilinestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multilinestring_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.multilinestring["coordinates"]
-        precision = 50
-        geometry_coordinates = self.multilinestring["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multilinestring_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 6
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # Polygon.
-    def test_truncuating_polygon_coordinates(self):
-        """Test that Polygon coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [
-                [100.123, 0.123],
-                [101.123, 0.123],
-                [101.123, 1.123],
-                [100.123, 1.123],
-                [100.123, 0.123],
-            ]
-        ]
-        precision = 3
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_polygon_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = [
-            [
-                [100.123456, 0.123456],
-                [101.123456, 0.123456],
-                [101.123456, 1.123456],
-                [100.123456, 1.123456],
-                [100.123456, 0.123456],
-            ]
-        ]
-        precision = 50
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_polygon_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = [
-            [
-                [100.123456, 0.123456],
-                [101.123456, 0.123456],
-                [101.123456, 1.123456],
-                [100.123456, 1.123456],
-                [100.123456, 0.123456],
-            ]
-        ]
-        precision = 6
-        geometry_coordinates = self.polygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    # MultiPolygon.
-    def test_truncuating_multipolygon_coordinates(self):
-        """Test that MultiPolygon coordinates are truncuated succesfully."""
-        expected_return_value = [
-            [
-                [
-                    [102.123, 2.123],
-                    [103.123, 2.123],
-                    [103.123, 3.123],
-                    [102.123, 3.123],
-                    [102.123, 2.123],
-                ]
-            ],
-            [
-                [
-                    [100.123, 0.123],
-                    [101.123, 0.123],
-                    [101.123, 1.123],
-                    [100.123, 1.123],
-                    [100.123, 0.123],
-                ],
-                [
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                    [100.123, 0.123],
-                ],
-            ],
-        ]
-        precision = 3
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multipolygon_precision_larger_than_places(self):
-        """Test that when the precision argument is a value larger
-        than the number of coordinate decimnal points, the same coordinate values
-        are returned.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 50
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-    def test_multipolygon_same_precision(self):
-        """Test that LineString coordinates are not truncuated when
-        the coordinate decimal points matches what's passed
-        to the precision parameter.
-        """
-        expected_return_value = self.multipolygon["coordinates"]
-        precision = 6
-        geometry_coordinates = self.multipolygon["coordinates"]
-        self.assertEqual(
-            _create_coordinates(geometry_coordinates, precision), expected_return_value
-        )
-
-
-class TestProcessGeometryCollection(unittest.TestCase):
-    """Tests for the _process_geometry_collection function."""
-
-    def setUp(self):
-        self.geometry_collection = {
-            "type": "GeometryCollection",
-            "geometries": [
-                {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                {
-                    "type": "LineString",
-                    "coordinates": [
-                        [1.123456, 1.123456],
-                        [2.123456, 3.123456],
-                        [4.123456, 5.123456],
-                    ],
-                },
-                {
-                    "type": "Polygon",
-                    "coordinates": [
-                        [
-                            [6.123456, 6.123456],
-                            [8.123456, 8.123456],
-                            [10.123456, 10.123456],
-                            [6.123456, 6.123456],
-                        ]
-                    ],
-                },
-                {
-                    "type": "MultiPoint",
-                    "coordinates": [
-                        [12.123456, 12.123456],
-                        [14.123456, 14.123456],
-                        [16.123456, 16.123456],
-                    ],
-                },
-            ],
-        }
-
-    def test_truncuating_coordinates(self):
-        """Tests that the coordinates of each nested Geometry object
-        is truncuated correctly."""
-
-        expected_return_value = {
-            "type": "GeometryCollection",
-            "geometries": [
-                {"type": "Point", "coordinates": [0.123, 0.123]},
-                {
-                    "type": "LineString",
-                    "coordinates": [[1.123, 1.123], [2.123, 3.123], [4.123, 5.123]],
-                },
-                {
-                    "type": "Polygon",
-                    "coordinates": [
-                        [
-                            [6.123, 6.123],
-                            [8.123, 8.123],
-                            [10.123, 10.123],
-                            [6.123, 6.123],
-                        ]
-                    ],
-                },
-                {
-                    "type": "MultiPoint",
-                    "coordinates": [
-                        [12.123, 12.123],
-                        [14.123, 14.123],
-                        [16.123, 16.123],
-                    ],
-                },
-            ],
-        }
-
-        geo_collection = self.geometry_collection
-        precision = 3
-        self.assertEqual(
-            _process_geometry_collection(geo_collection, precision),
-            expected_return_value,
-        )
-
-
-class TestProcessFeatures(unittest.TestCase):
-    """Tests for the _process_features function."""
-
-    def setUp(self):
-        self.feature_collection = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123456, 5.123456],
-                                [15.123456, 5.123456],
-                                [15.123456, 15.123456],
-                                [5.123456, 15.123456],
-                                [5.123456, 5.123456],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-        self.blank_feature_collection = {}
-
-        self.feature = {
-            "type": "Feature",
-            "geometry": {"type": "Point", "coordinates": [100.123456, -0.123456]},
-            "properties": {"name": "Example Point"},
-        }
-
-    def test_feature_collection_truncuation(self):
-        """Test that the coordinates of each nested Geometry object is
-        truncuated."""
-        geometry_to_include = GEOMETRY_OBJECTS
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, geometry_to_include, False
-            ),
-            expected_return_value,
-        )
-
-    def test_feature_truncuation(self):
-        """Test that the Feature is processed (coordinates truncuated).
-        Note the distinction between Feature and FeatureCollection.
-        """
-        geometry_to_include = GEOMETRY_OBJECTS
-        precision = 3
-        expected_return_value = {
-            "type": "Feature",
-            "geometry": {"type": "Point", "coordinates": [100.123, -0.123]},
-            "properties": {"name": "Example Point"},
-        }
-
-        self.assertEqual(
-            _process_features(self.feature, precision, geometry_to_include, False),
-            expected_return_value,
-        )
-
-    def test_empty_gson_file(self):
-        """Test that an exception is raised when an empty
-        GeoJSON file is passed."""
-        with self.assertRaises(SystemError):
-            _process_features(self.blank_feature_collection, 3, ["Point"], False)
-
-    def test_properties_nullified(self):
-        """Test that the properties key returns a null/empty dictionary."""
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
-                    "properties": {},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, GEOMETRY_OBJECTS, True
-            ),
-            expected_return_value,
-        )
-
-    def test_geometry_to_include_parameter(self):
-        """Test that only the passed geometry objects are truncuated."""
-        geometry_to_include = ["Polygon"]
-        precision = 3
-        expected_return_value = {
-            "type": "FeatureCollection",
-            "features": [
-                {
-                    "type": "Feature",
-                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
-                    "properties": {"name": "Feature 1"},
-                },
-                {
-                    "type": "Feature",
-                    "geometry": {
-                        "type": "Polygon",
-                        "coordinates": [
-                            [
-                                [5.123, 5.123],
-                                [15.123, 5.123],
-                                [15.123, 15.123],
-                                [5.123, 15.123],
-                                [5.123, 5.123],
-                            ]
-                        ],
-                    },
-                    "properties": {"name": "Feature 2"},
-                },
-            ],
-        }
-
-        self.assertEqual(
-            _process_features(
-                self.feature_collection, precision, geometry_to_include, False
-            ),
-            expected_return_value,
-        )
-
-
-if __name__ == "__main__":
-    unittest.main(buffer=True)
+"""Unit tests for geojson_shave.py"""
+
+import os
+import unittest
+import sys
+
+from geojson_shave.geojson_shave import (_create_coordinates,
+ _process_geometry_collection,
+_process_features, 
+GEOMETRY_OBJECTS)
+
+
+class TestCreateCoordinates(unittest.TestCase):
+    """Tests for the _create_coordinates function.
+
+    Note that both LineStrings' and MultiPoints' coordinates both consist
+    of an array of Points, hence only the LineString being tested.
+    """
+
+    def setUp(self):
+        self.point = {
+            "type": "Point",
+            "coordinates": [-100.123456, 200.123456],
+            "properties": {"name": "Test Point"},
+        }
+
+        self.linestring = {
+            "type": "LineString",
+            "coordinates": [
+                [100.123456, 0.123456],
+                [101.123456, 1.123456],
+                [102.123456, 2.123456],
+            ],
+        }
+
+        self.multilinestring = {
+            "type": "MultiLineString",
+            "coordinates": [
+                [[-100.123456, 0.123456], [-101.123456, 1.123456]],
+                [[102.123456, 2.123456], [103.123456, 3.123456]],
+            ],
+        }
+
+        self.polygon = {
+            "type": "Polygon",
+            "coordinates": [
+                [
+                    [100.123456, 0.123456],
+                    [101.123456, 0.123456],
+                    [101.123456, 1.123456],
+                    [100.123456, 1.123456],
+                    [100.123456, 0.123456],
+                ]
+            ],
+        }
+
+        self.multipolygon = {
+            "type": "MultiPolygon",
+            "coordinates": [
+                [
+                    [
+                        [102.123456, 2.123456],
+                        [103.123456, 2.123456],
+                        [103.123456, 3.123456],
+                        [102.123456, 3.123456],
+                        [102.123456, 2.123456],
+                    ]
+                ],
+                [
+                    [
+                        [100.123456, 0.123456],
+                        [101.123456, 0.123456],
+                        [101.123456, 1.123456],
+                        [100.123456, 1.123456],
+                        [100.123456, 0.123456],
+                    ],
+                    [
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                        [100.123456, 0.123456],
+                    ],
+                ],
+            ],
+        }
+
+    # Point.
+    def test_truncuating_point_coordinates(self):
+        """Test that Point coordinates are truncuated succesfully."""
+        expected_return_value = [-100.123, 200.123]
+        precision = 3
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_point_same_precision(self):
+        """Test that Point coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.point["coordinates"]
+        precision = 6
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_point_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.point["coordinates"]
+        precision = 50
+        geometry_coordinates = self.point["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # LineString.
+    def test_truncuating_linestring_coordinates(self):
+        """Test that LineString coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [100.123, 0.123],
+            [101.123, 1.123],
+            [102.123, 2.123],
+        ]
+        precision = 3
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_linestring_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.linestring["coordinates"]
+        precision = 6
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_linestring_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.linestring["coordinates"]
+        precision = 50
+        geometry_coordinates = self.linestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # MultiLine strings.
+    def test_truncuating_multilinestring_coordinates(self):
+        """Test that MultiLineString coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [[-100.123, 0.123], [-101.123, 1.123]],
+            [[102.123, 2.123], [103.123, 3.123]],
+        ]
+        precision = 3
+        geometry_coordinates = self.multilinestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multilinestring_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.multilinestring["coordinates"]
+        precision = 50
+        geometry_coordinates = self.multilinestring["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multilinestring_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 6
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # Polygon.
+    def test_truncuating_polygon_coordinates(self):
+        """Test that Polygon coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [
+                [100.123, 0.123],
+                [101.123, 0.123],
+                [101.123, 1.123],
+                [100.123, 1.123],
+                [100.123, 0.123],
+            ]
+        ]
+        precision = 3
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_polygon_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = [
+            [
+                [100.123456, 0.123456],
+                [101.123456, 0.123456],
+                [101.123456, 1.123456],
+                [100.123456, 1.123456],
+                [100.123456, 0.123456],
+            ]
+        ]
+        precision = 50
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_polygon_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = [
+            [
+                [100.123456, 0.123456],
+                [101.123456, 0.123456],
+                [101.123456, 1.123456],
+                [100.123456, 1.123456],
+                [100.123456, 0.123456],
+            ]
+        ]
+        precision = 6
+        geometry_coordinates = self.polygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    # MultiPolygon.
+    def test_truncuating_multipolygon_coordinates(self):
+        """Test that MultiPolygon coordinates are truncuated succesfully."""
+        expected_return_value = [
+            [
+                [
+                    [102.123, 2.123],
+                    [103.123, 2.123],
+                    [103.123, 3.123],
+                    [102.123, 3.123],
+                    [102.123, 2.123],
+                ]
+            ],
+            [
+                [
+                    [100.123, 0.123],
+                    [101.123, 0.123],
+                    [101.123, 1.123],
+                    [100.123, 1.123],
+                    [100.123, 0.123],
+                ],
+                [
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                    [100.123, 0.123],
+                ],
+            ],
+        ]
+        precision = 3
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multipolygon_precision_larger_than_places(self):
+        """Test that when the precision argument is a value larger
+        than the number of coordinate decimnal points, the same coordinate values
+        are returned.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 50
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+    def test_multipolygon_same_precision(self):
+        """Test that LineString coordinates are not truncuated when
+        the coordinate decimal points matches what's passed
+        to the precision parameter.
+        """
+        expected_return_value = self.multipolygon["coordinates"]
+        precision = 6
+        geometry_coordinates = self.multipolygon["coordinates"]
+        self.assertEqual(
+            _create_coordinates(geometry_coordinates, precision), expected_return_value
+        )
+
+
+class TestProcessGeometryCollection(unittest.TestCase):
+    """Tests for the _process_geometry_collection function."""
+
+    def setUp(self):
+        self.geometry_collection = {
+            "type": "GeometryCollection",
+            "geometries": [
+                {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                {
+                    "type": "LineString",
+                    "coordinates": [
+                        [1.123456, 1.123456],
+                        [2.123456, 3.123456],
+                        [4.123456, 5.123456],
+                    ],
+                },
+                {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [6.123456, 6.123456],
+                            [8.123456, 8.123456],
+                            [10.123456, 10.123456],
+                            [6.123456, 6.123456],
+                        ]
+                    ],
+                },
+                {
+                    "type": "MultiPoint",
+                    "coordinates": [
+                        [12.123456, 12.123456],
+                        [14.123456, 14.123456],
+                        [16.123456, 16.123456],
+                    ],
+                },
+            ],
+        }
+
+    def test_truncuating_coordinates(self):
+        """Tests that the coordinates of each nested Geometry object
+        is truncuated correctly."""
+
+        expected_return_value = {
+            "type": "GeometryCollection",
+            "geometries": [
+                {"type": "Point", "coordinates": [0.123, 0.123]},
+                {
+                    "type": "LineString",
+                    "coordinates": [[1.123, 1.123], [2.123, 3.123], [4.123, 5.123]],
+                },
+                {
+                    "type": "Polygon",
+                    "coordinates": [
+                        [
+                            [6.123, 6.123],
+                            [8.123, 8.123],
+                            [10.123, 10.123],
+                            [6.123, 6.123],
+                        ]
+                    ],
+                },
+                {
+                    "type": "MultiPoint",
+                    "coordinates": [
+                        [12.123, 12.123],
+                        [14.123, 14.123],
+                        [16.123, 16.123],
+                    ],
+                },
+            ],
+        }
+
+        geo_collection = self.geometry_collection
+        precision = 3
+        self.assertEqual(
+            _process_geometry_collection(geo_collection, precision),
+            expected_return_value,
+        )
+
+
+class TestProcessFeatures(unittest.TestCase):
+    """Tests for the _process_features function."""
+
+    def setUp(self):
+        self.feature_collection = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123456, 5.123456],
+                                [15.123456, 5.123456],
+                                [15.123456, 15.123456],
+                                [5.123456, 15.123456],
+                                [5.123456, 5.123456],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+        self.blank_feature_collection = {}
+
+        self.feature = {
+            "type": "Feature",
+            "geometry": {"type": "Point", "coordinates": [100.123456, -0.123456]},
+            "properties": {"name": "Example Point"},
+        }
+
+    def test_feature_collection_truncuation(self):
+        """Test that the coordinates of each nested Geometry object is
+        truncuated."""
+        geometry_to_include = GEOMETRY_OBJECTS
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, geometry_to_include, False
+            ),
+            expected_return_value,
+        )
+
+    def test_feature_truncuation(self):
+        """Test that the Feature is processed (coordinates truncuated).
+        Note the distinction between Feature and FeatureCollection.
+        """
+        geometry_to_include = GEOMETRY_OBJECTS
+        precision = 3
+        expected_return_value = {
+            "type": "Feature",
+            "geometry": {"type": "Point", "coordinates": [100.123, -0.123]},
+            "properties": {"name": "Example Point"},
+        }
+
+        self.assertEqual(
+            _process_features(self.feature, precision, geometry_to_include, False),
+            expected_return_value,
+        )
+
+    def test_empty_gson_file(self):
+        """Test that an exception is raised when an empty
+        GeoJSON file is passed."""
+        with self.assertRaises(SystemError):
+            _process_features(self.blank_feature_collection, 3, ["Point"], False)
+
+    def test_properties_nullified(self):
+        """Test that the properties key returns a null/empty dictionary."""
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123, 0.123]},
+                    "properties": {},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, GEOMETRY_OBJECTS, True
+            ),
+            expected_return_value,
+        )
+
+    def test_geometry_to_include_parameter(self):
+        """Test that only the passed geometry objects are truncuated."""
+        geometry_to_include = ["Polygon"]
+        precision = 3
+        expected_return_value = {
+            "type": "FeatureCollection",
+            "features": [
+                {
+                    "type": "Feature",
+                    "geometry": {"type": "Point", "coordinates": [0.123456, 0.123456]},
+                    "properties": {"name": "Feature 1"},
+                },
+                {
+                    "type": "Feature",
+                    "geometry": {
+                        "type": "Polygon",
+                        "coordinates": [
+                            [
+                                [5.123, 5.123],
+                                [15.123, 5.123],
+                                [15.123, 15.123],
+                                [5.123, 15.123],
+                                [5.123, 5.123],
+                            ]
+                        ],
+                    },
+                    "properties": {"name": "Feature 2"},
+                },
+            ],
+        }
+
+        self.assertEqual(
+            _process_features(
+                self.feature_collection, precision, geometry_to_include, False
+            ),
+            expected_return_value,
+        )
+
+
+if __name__ == "__main__":
+    unittest.main(buffer=True)
```

