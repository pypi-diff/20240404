# Comparing `tmp/aixblock_converter-0.0.4.tar.gz` & `tmp/aixblock_converter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_converter-0.0.4.tar", max compression
+gzip compressed data, was "aixblock_converter-0.0.5.tar", max compression
```

## Comparing `aixblock_converter-0.0.4.tar` & `aixblock_converter-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.4/README.md
--rw-r--r--   0        0        0      232 2024-04-03 08:01:32.692474 aixblock_converter-0.0.4/aixblock_converter/__init__.py
--rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.4/aixblock_converter/audio.py
--rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.4/aixblock_converter/brush.py
--rw-r--r--   0        0        0     3829 2024-04-03 07:46:25.567052 aixblock_converter-0.0.4/aixblock_converter/cli.py
--rw-r--r--   0        0        0    57486 2024-04-03 06:07:40.400484 aixblock_converter-0.0.4/aixblock_converter/converter.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.4/aixblock_converter/exports/__init__.py
--rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.4/aixblock_converter/exports/csv.py
--rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.4/aixblock_converter/funsd.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.4/aixblock_converter/imports/__init__.py
--rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.4/aixblock_converter/imports/coco.py
--rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.4/aixblock_converter/imports/colors.py
--rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.4/aixblock_converter/imports/label_config.py
--rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.4/aixblock_converter/imports/pathtrack.py
--rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.4/aixblock_converter/imports/yolo.py
--rw-r--r--   0        0        0     5734 2024-04-03 07:46:53.775888 aixblock_converter-0.0.4/aixblock_converter/main.py
--rw-r--r--   0        0        0    11769 2024-04-03 07:47:01.646870 aixblock_converter-0.0.4/aixblock_converter/utils.py
--rw-r--r--   0        0        0      270 2024-04-03 08:01:48.101795 aixblock_converter-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.5/README.md
+-rw-r--r--   0        0        0      232 2024-04-03 08:01:32.692474 aixblock_converter-0.0.5/aixblock_converter/__init__.py
+-rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.5/aixblock_converter/audio.py
+-rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.5/aixblock_converter/brush.py
+-rw-r--r--   0        0        0     3835 2024-04-03 08:23:41.957286 aixblock_converter-0.0.5/aixblock_converter/cli.py
+-rw-r--r--   0        0        0    57482 2024-04-03 08:23:03.374515 aixblock_converter-0.0.5/aixblock_converter/converter.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.5/aixblock_converter/exports/__init__.py
+-rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.5/aixblock_converter/exports/csv.py
+-rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.5/aixblock_converter/funsd.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.5/aixblock_converter/imports/__init__.py
+-rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.5/aixblock_converter/imports/coco.py
+-rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.5/aixblock_converter/imports/colors.py
+-rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.5/aixblock_converter/imports/label_config.py
+-rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.5/aixblock_converter/imports/pathtrack.py
+-rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.5/aixblock_converter/imports/yolo.py
+-rw-r--r--   0        0        0     5741 2024-04-03 08:23:41.978844 aixblock_converter-0.0.5/aixblock_converter/main.py
+-rw-r--r--   0        0        0    12915 2024-04-03 08:24:37.345094 aixblock_converter-0.0.5/aixblock_converter/utils.py
+-rw-r--r--   0        0        0      270 2024-04-03 08:25:00.788102 aixblock_converter-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.5/PKG-INFO
```

### Comparing `aixblock_converter-0.0.4/aixblock_converter/audio.py` & `aixblock_converter-0.0.5/aixblock_converter/audio.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/brush.py` & `aixblock_converter-0.0.5/aixblock_converter/brush.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/cli.py` & `aixblock_converter-0.0.5/aixblock_converter/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         '--project-dir',
         dest='project_dir',
         default=None,
         help='Label Studio project directory path',
     )
     parser.add_argument(
         '--heartex-format',
-        dest='heartex_format',
+        dest='PLATFORM_format',
         action='store_true',
         help='Set this flag if your completions are coming from Heartex platform instead of Label Studio',
     )
     args = parser.parse_args()
 
     with io.open(args.config) as f:
         config_str = f.read()
@@ -94,33 +94,33 @@
         header = not args.csv_no_header
         sep = args.csv_separator
         c.convert_to_csv(
             args.input,
             args.output,
             sep=sep,
             header=header,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.CONLL2003:
-        c.convert_to_conll2003(args.input, args.output, is_dir=not args.heartex_format)
+        c.convert_to_conll2003(args.input, args.output, is_dir=not args.PLATFORM_format)
     elif args.format == Format.COCO:
         c.convert_to_coco(
             args.input,
             args.output,
             output_image_dir=args.image_dir,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.VOC:
         c.convert_to_voc(
             args.input,
             args.output,
             output_image_dir=args.image_dir,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.YOLO:
-        c.convert_to_yolo(args.input, args.output, is_dir=not args.heartex_format)
+        c.convert_to_yolo(args.input, args.output, is_dir=not args.PLATFORM_format)
 
     print('Congratulations! Now check:\n' + args.output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aixblock_converter-0.0.4/aixblock_converter/converter.py` & `aixblock_converter-0.0.5/aixblock_converter/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -927,15 +927,15 @@
                             'iscrowd': 0,
                             'area': get_polygon_area(x, y),
                         }
                     )
                 else:
                     raise ValueError("Unknown label type")
 
-                if os.getenv('LABEL_STUDIO_FORCE_ANNOTATOR_EXPORT'):
+                if os.getenv('AIXBLOCK_FORCE_ANNOTATOR_EXPORT'):
                     annotations[-1].update({'annotator': _get_annotator(item)})
 
         with io.open(output_file, mode='w', encoding='utf8') as fout:
             json.dump(
                 {
                     'images': images,
                     'categories': categories,
```

### Comparing `aixblock_converter-0.0.4/aixblock_converter/exports/csv.py` & `aixblock_converter-0.0.5/aixblock_converter/exports/csv.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/funsd.py` & `aixblock_converter-0.0.5/aixblock_converter/funsd.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/imports/coco.py` & `aixblock_converter-0.0.5/aixblock_converter/imports/coco.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/imports/colors.py` & `aixblock_converter-0.0.5/aixblock_converter/imports/colors.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/imports/label_config.py` & `aixblock_converter-0.0.5/aixblock_converter/imports/label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/imports/pathtrack.py` & `aixblock_converter-0.0.5/aixblock_converter/imports/pathtrack.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/imports/yolo.py` & `aixblock_converter-0.0.5/aixblock_converter/imports/yolo.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.4/aixblock_converter/main.py` & `aixblock_converter-0.0.5/aixblock_converter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         '--project-dir',
         dest='project_dir',
         default=None,
         help='Label Studio project directory path',
     )
     parser.add_argument(
         '--heartex-format',
-        dest='heartex_format',
+        dest='PLATFORM_format',
         action='store_true',
         default=True,
         help='Set this flag if your annotations are in one JSON file instead of multiple JSON files from directory',
     )
 
 
 def get_all_args():
@@ -111,15 +111,15 @@
         header = not args.csv_no_header
         sep = args.csv_separator
         c.convert_to_csv(
             args.input,
             args.output,
             sep=sep,
             header=header,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.CSV_OLD:
         header = not args.csv_no_header
         sep = args.csv_separator
         ExportToCSV(args.input).to_file(
             args.output, sep=sep, header=header, index=False
         )
@@ -127,34 +127,34 @@
         header = not args.csv_no_header
         sep = '\t'
         c.convert_to_csv(
             args.input,
             args.output,
             sep=sep,
             header=header,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.CONLL2003:
-        c.convert_to_conll2003(args.input, args.output, is_dir=not args.heartex_format)
+        c.convert_to_conll2003(args.input, args.output, is_dir=not args.PLATFORM_format)
     elif args.format == Format.COCO:
         c.convert_to_coco(
             args.input,
             args.output,
             output_image_dir=args.image_dir,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.VOC:
         c.convert_to_voc(
             args.input,
             args.output,
             output_image_dir=args.image_dir,
-            is_dir=not args.heartex_format,
+            is_dir=not args.PLATFORM_format,
         )
     elif args.format == Format.YOLO:
-        c.convert_to_yolo(args.input, args.output, is_dir=not args.heartex_format)
+        c.convert_to_yolo(args.input, args.output, is_dir=not args.PLATFORM_format)
     else:
         raise FormatNotSupportedError()
 
 
 def imports(args):
     if args.import_format == 'yolo':
         import_yolo.convert_yolo_to_ls(
```

### Comparing `aixblock_converter-0.0.4/aixblock_converter/utils.py` & `aixblock_converter-0.0.5/aixblock_converter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,49 @@
 
 from operator import itemgetter
 from PIL import Image
 from urllib.parse import urlparse
 from nltk.tokenize.treebank import TreebankWordTokenizer
 from lxml import etree
 from collections import defaultdict
-from aixblock_tools.core.utils.params import get_env
+# from aixblock_tools.core.utils.params import get_env
+def bool_from_request(params, key, default):
+    """Get boolean value from request GET, POST, etc
+    :param params: dict POST, GET, etc
+    :param key: key to find
+    :param default: default value
+    :return: boolean
+    """
+    value = params.get(key, default)
+
+    if isinstance(value, str):
+        value = cast_bool_from_str(value)
+
+    return bool(int(value))
+def cast_bool_from_str(value):
+    if isinstance(value, str):
+        if value.lower() in ['true', 'yes', 'on', '1']:
+            value = True
+        elif value.lower() in ['false', 'no', 'not', 'off', '0']:
+            value = False
+        else:
+            raise ValueError(
+                f'Incorrect bool value "{value}". '
+                f'It should be one of [1, 0, true, false, yes, no]'
+            )
+    return value
+def get_env(name, default=None, is_bool=False):
+    for env_key in ['AIXBLOCK_' + name, 'PLATFORM_' + name, name]:
+        value = os.environ.get(env_key)
+        if value is not None:
+            if is_bool:
+                return bool_from_request(os.environ, env_key, default)
+            else:
+                return value
+    return default
 
 logger = logging.getLogger(__name__)
 
 _LABEL_TAGS = {'Label', 'Choice'}
 _NOT_CONTROL_TAGS = {
     'Filter',
 }
```

