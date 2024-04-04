# Comparing `tmp/nonebot_plugin_chikari_economy-0.0.2.tar.gz` & `tmp/nonebot_plugin_chikari_economy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.2.tar", last modified: Thu Apr  4 12:05:25 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.3.tar", last modified: Thu Apr  4 12:12:51 2024, max compression
```

## Comparing `nonebot_plugin_chikari_economy-0.0.2.tar` & `nonebot_plugin_chikari_economy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.114381 nonebot_plugin_chikari_economy-0.0.2/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4464 2024-04-04 12:05:25.114381 nonebot_plugin_chikari_economy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3873 2024-04-04 11:51:08.000000 nonebot_plugin_chikari_economy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.100718 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/
--rw-rw-rw-   0        0        0     1192 2024-04-04 12:02:17.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/data_handles.py
--rw-rw-rw-   0        0        0     1206 2024-04-04 11:35:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/handles.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:05:25.113406 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/
--rw-rw-rw-   0        0        0     4464 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-04 12:05:25.000000 nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-04 12:05:25.115874 nonebot_plugin_chikari_economy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-04-04 12:02:20.000000 nonebot_plugin_chikari_economy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:12:51.124753 nonebot_plugin_chikari_economy-0.0.3/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4441 2024-04-04 12:12:51.124753 nonebot_plugin_chikari_economy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3873 2024-04-04 11:51:08.000000 nonebot_plugin_chikari_economy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:12:51.116945 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/
+-rw-rw-rw-   0        0        0     1192 2024-04-04 12:12:22.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/data_handles.py
+-rw-rw-rw-   0        0        0     1206 2024-04-04 11:35:25.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/handles.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:12:51.123777 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/
+-rw-rw-rw-   0        0        0     4441 2024-04-04 12:12:51.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-04 12:12:51.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:12:51.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-04 12:12:51.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-04 12:12:51.000000 nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-04 12:12:51.125729 nonebot_plugin_chikari_economy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-04-04 12:12:23.000000 nonebot_plugin_chikari_economy-0.0.3/setup.py
```

### Comparing `nonebot_plugin_chikari_economy-0.0.2/LICENSE` & `nonebot_plugin_chikari_economy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.2/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pillow
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.2
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.3
 Summary: A economy plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_economy Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
-Requires-Dist: nonebot-plugin-localstore
+nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot Requires-Dist: nonebot-
+plugin-localstore
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # nonebot-plugin-chikari-economy _â¨ NoneBot ç»æµæä»¶ï¼åºï¼ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç»
 ä¸ä¸ªç»æµæä»¶ï¼åºï¼ï¼å¯ç±å¶ä»æä»¶è°ç¨ï¼ä»¥ä¾¿æä»¶é´çç»æµèå¨
 ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
```

### Comparing `nonebot_plugin_chikari_economy-0.0.2/README.md` & `nonebot_plugin_chikari_economy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/__init__.py` & `nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     description="一个经济插件（库），可由其他插件调用，以便插件间的经济联动",
     usage="",
     type="library",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     supported_adapters={"~onebot.v11"}
 )
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from .data_handles import def_money_type as def_money_type
 from .data_handles import set_money as set_money
 from .data_handles import add_money as add_money
 from .data_handles import inquire_money as inquire_money
 
 from .handles import message_Handles
```

### Comparing `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/data_handles.py` & `nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/data_handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy/handles.py` & `nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy/handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.2/nonebot_plugin_chikari_economy.egg-info/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.3/nonebot_plugin_chikari_economy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pillow
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.2
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_economy Version: 0.0.3
 Summary: A economy plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_economy Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
-Requires-Dist: nonebot-plugin-localstore
+nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot Requires-Dist: nonebot-
+plugin-localstore
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # nonebot-plugin-chikari-economy _â¨ NoneBot ç»æµæä»¶ï¼åºï¼ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç»
 ä¸ä¸ªç»æµæä»¶ï¼åºï¼ï¼å¯ç±å¶ä»æä»¶è°ç¨ï¼ä»¥ä¾¿æä»¶é´çç»æµèå¨
 ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
```

### Comparing `nonebot_plugin_chikari_economy-0.0.2/setup.py` & `nonebot_plugin_chikari_economy-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_economy",
-    version="0.0.2",
+    version="0.0.3",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A economy plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     packages=setuptools.find_packages(),
-    install_requires=['pillow', 'nonebot2>=2.2.0','nonebot-adapter-onebot','nonebot-plugin-localstore'],
+    install_requires=['nonebot2>=2.2.0','nonebot-adapter-onebot','nonebot-plugin-localstore'],
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ),
 )
```

