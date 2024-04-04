# Comparing `tmp/nonebot_plugin_chikari_economy-0.0.1.tar.gz` & `tmp/nonebot_plugin_chikari_economy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.1.tar", last modified: Thu Apr  4 11:56:32 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.2.tar", last modified: Thu Apr  4 12:05:25 2024, max compression
```

## Comparing `nonebot_plugin_chikari_economy-0.0.1.tar` & `nonebot_plugin_chikari_economy-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:32.508445 nonebot_plugin_chikari_economy-0.0.1/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4464 2024-04-04 11:56:32.507469 nonebot_plugin_chikari_economy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3873 2024-04-04 11:51:08.000000 nonebot_plugin_chikari_economy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:32.499661 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/
--rw-rw-rw-   0        0        0     1196 2024-04-04 11:36:07.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/__init__.py
--rw-rw-rw-   0        0        0     4327 2024-04-04 11:30:58.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/data_handles.py
--rw-rw-rw-   0        0        0     1206 2024-04-04 11:35:25.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/handles.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:56:32.507469 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/
--rw-rw-rw-   0        0        0     4464 2024-04-04 11:56:32.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-04 11:56:32.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:56:32.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-04 11:56:32.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-04 11:56:32.000000 nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-04 11:56:32.509422 nonebot_plugin_chikari_economy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-04-04 11:55:52.000000 nonebot_plugin_chikari_economy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.114381 nonebot_plugin_chikari_economy-0.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4464 2024-04-04 12:05:25.114381 nonebot_plugin_chikari_economy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3873 2024-04-04 11:51:08.000000 nonebot_plugin_chikari_economy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.100718 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/
+-rw-rw-rw-   0        0        0     1192 2024-04-04 12:02:17.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/data_handles.py
+-rw-rw-rw-   0        0        0     1206 2024-04-04 11:35:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/handles.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.113406 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/
+-rw-rw-rw-   0        0        0     4464 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-04 12:05:25.115874 nonebot_plugin_chikari_economy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      795 2024-04-04 12:02:20.000000 nonebot_plugin_chikari_economy-0.0.2/setup.py
```

### Comparing `nonebot_plugin_chikari_economy-0.0.1/LICENSE` & `nonebot_plugin_chikari_economy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.1/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.1
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.2
 Summary: A economy plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_economy Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_economy-0.0.1/README.md` & `nonebot_plugin_chikari_economy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/__init__.py` & `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="Chikari_economy",
     description="一个经济插件（库），可由其他插件调用，以便插件间的经济联动",
     usage="",
-    type="application",
+    type="library",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     supported_adapters={"~onebot.v11"}
 )
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from .data_handles import def_money_type as def_money_type
 from .data_handles import set_money as set_money
 from .data_handles import add_money as add_money
 from .data_handles import inquire_money as inquire_money
 
 from .handles import message_Handles
```

### Comparing `nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/data_handles.py` & `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/data_handles.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,18 @@
         uid (str): 用户id
         key (str): 数据键值
         value (_type_): 数据
     """
     
     global data
     if uid not in data.keys:
-        data[uid] = {key: value}
-    else:
-        data[uid][key] = value
+        data[uid] = {
+            "defaultmoney": 0.0
+        }
+    data[uid][key] = value
     file_save()
     return
 
 def configdata_set(key: str,value):
     """设置配置文件
 
     Args:
@@ -148,10 +149,10 @@
 
     Returns:
         float: 货币当前数量
     """
     global data
     if id not in configdata["money_types"].keys:
         raise NameError(f"Undefined money type:{id}")
-    if id not in data[uid]:
-        return 0
+    if id not in data[uid].keys:
+        return 0.0
     return data[uid][id]
```

### Comparing `nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy/handles.py` & `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.1/nonebot_plugin_chikari_economy.egg-info/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.1
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.2
 Summary: A economy plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_economy Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_economy-0.0.1/setup.py` & `nonebot_plugin_chikari_economy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_economy",
-    version="0.0.1",
+    version="0.0.2",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A economy plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     packages=setuptools.find_packages(),
```

