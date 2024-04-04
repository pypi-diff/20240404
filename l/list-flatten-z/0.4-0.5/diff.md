# Comparing `tmp/list_flatten_z-0.4.tar.gz` & `tmp/list_flatten_z-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_flatten_z-0.4.tar", last modified: Thu Apr  4 07:12:42 2024, max compression
+gzip compressed data, was "list_flatten_z-0.5.tar", last modified: Thu Apr  4 07:42:21 2024, max compression
```

## Comparing `list_flatten_z-0.4.tar` & `list_flatten_z-0.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.066517 list_flatten_z-0.4/
--rw-rw-rw-   0        0        0      227 2024-04-04 07:12:42.066517 list_flatten_z-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.063517 list_flatten_z-0.4/list_flatten_z/
--rw-rw-rw-   0        0        0        0 2024-04-04 05:08:17.000000 list_flatten_z-0.4/list_flatten_z/__init__.py
--rw-rw-rw-   0        0        0      540 2024-04-04 04:42:03.000000 list_flatten_z-0.4/list_flatten_z/list_flatten_z.py
-drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.065517 list_flatten_z-0.4/list_flatten_z.egg-info/
--rw-rw-rw-   0        0        0      227 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 07:12:42.066517 list_flatten_z-0.4/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-04-04 07:11:50.000000 list_flatten_z-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:42:21.777684 list_flatten_z-0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 07:33:20.000000 list_flatten_z-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      691 2024-04-04 07:42:21.777684 list_flatten_z-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-04 07:30:54.000000 list_flatten_z-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 07:42:21.775684 list_flatten_z-0.5/list_flatten_z/
+-rw-rw-rw-   0        0        0      594 2024-04-04 07:41:32.000000 list_flatten_z-0.5/list_flatten_z/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:42:21.777684 list_flatten_z-0.5/list_flatten_z.egg-info/
+-rw-rw-rw-   0        0        0      691 2024-04-04 07:42:21.000000 list_flatten_z-0.5/list_flatten_z.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-04 07:42:21.000000 list_flatten_z-0.5/list_flatten_z.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 07:42:21.000000 list_flatten_z-0.5/list_flatten_z.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 07:42:21.000000 list_flatten_z-0.5/list_flatten_z.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 07:42:21.000000 list_flatten_z-0.5/list_flatten_z.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 07:42:21.777684 list_flatten_z-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      858 2024-04-04 07:42:14.000000 list_flatten_z-0.5/setup.py
```

### Comparing `list_flatten_z-0.4/list_flatten_z/list_flatten_z.py` & `list_flatten_z-0.5/list_flatten_z/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import pandas as pd
 
 def list_flatten(data, fill_value=''):
     # 创建一个 DataFrame
     df = pd.DataFrame({'data': data})
+    python
+    setup.py
+    sdist
+    bdist_wheel
 
     # 定义一个函数来处理每个元素
     def process_item(item):
         if isinstance(item, list) and item:
             return item[0]
         else:
             return fill_value
```

