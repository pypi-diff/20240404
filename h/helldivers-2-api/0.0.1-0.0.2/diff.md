# Comparing `tmp/helldivers-2-api-0.0.1.tar.gz` & `tmp/helldivers-2-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helldivers-2-api-0.0.1.tar", last modified: Wed Apr  3 07:01:48 2024, max compression
+gzip compressed data, was "helldivers-2-api-0.0.2.tar", last modified: Thu Apr  4 13:54:03 2024, max compression
```

## Comparing `helldivers-2-api-0.0.1.tar` & `helldivers-2-api-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 07:01:48.650018 helldivers-2-api-0.0.1/
--rw-r--r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2372 2024-04-03 07:01:48.650018 helldivers-2-api-0.0.1/PKG-INFO
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2379 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/README.md
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     1686 2024-04-03 06:59:15.000000 helldivers-2-api-0.0.1/README_PYPI.md
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      777 2024-04-03 07:01:10.000000 helldivers-2-api-0.0.1/pyproject.toml
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       38 2024-04-03 07:01:48.650018 helldivers-2-api-0.0.1/setup.cfg
-drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 07:01:48.646018 helldivers-2-api-0.0.1/src/
-drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 07:01:48.650018 helldivers-2-api-0.0.1/src/helldivers2_api/
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/__init__.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     5214 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/api_client.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      178 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/api_version.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      165 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/campaign.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      162 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/endpoint_map.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      119 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/faction.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      459 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/global_event.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      156 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/planet.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      119 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/planet_attack.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)   136603 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/planet_info_table.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      277 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/planet_status.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     1265 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/sector.py
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      891 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.1/src/helldivers2_api/war_status.py
-drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 07:01:48.650018 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/
--rw-r--r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2372 2024-04-03 07:01:48.000000 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/PKG-INFO
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      703 2024-04-03 07:01:48.000000 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/SOURCES.txt
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)        1 2024-04-03 07:01:48.000000 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/dependency_links.txt
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       17 2024-04-03 07:01:48.000000 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/requires.txt
--rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       16 2024-04-03 07:01:48.000000 helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/top_level.txt
+drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-04 13:54:03.720764 helldivers-2-api-0.0.2/
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      478 2024-04-03 07:04:46.000000 helldivers-2-api-0.0.2/LICENCE.md
+-rw-r--r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2539 2024-04-04 13:54:03.716764 helldivers-2-api-0.0.2/PKG-INFO
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2276 2024-04-04 07:07:06.000000 helldivers-2-api-0.0.2/README.md
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     1739 2024-04-04 05:37:08.000000 helldivers-2-api-0.0.2/README_PYPI.md
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      866 2024-04-03 07:23:48.000000 helldivers-2-api-0.0.2/pyproject.toml
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       38 2024-04-04 13:54:03.720764 helldivers-2-api-0.0.2/setup.cfg
+drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-04 13:54:03.704764 helldivers-2-api-0.0.2/src/
+drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-04 13:54:03.716764 helldivers-2-api-0.0.2/src/helldivers2_api/
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/__init__.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2505 2024-04-04 07:00:42.000000 helldivers-2-api-0.0.2/src/helldivers2_api/api_client.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      242 2024-04-04 05:15:52.000000 helldivers-2-api-0.0.2/src/helldivers2_api/api_version.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      165 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/campaign.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      416 2024-04-04 06:35:42.000000 helldivers-2-api-0.0.2/src/helldivers2_api/endpoint_map.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      119 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/faction.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      459 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/global_event.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      142 2024-04-04 05:59:07.000000 helldivers-2-api-0.0.2/src/helldivers2_api/joint_operation.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     9731 2024-04-04 06:59:51.000000 helldivers-2-api-0.0.2/src/helldivers2_api/mapping_strategy.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      207 2024-04-04 06:39:22.000000 helldivers-2-api-0.0.2/src/helldivers2_api/news.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      156 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/planet.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      119 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/planet_attack.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      554 2024-04-04 06:11:26.000000 helldivers-2-api-0.0.2/src/helldivers2_api/planet_event.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)   137348 2024-04-04 05:38:01.000000 helldivers-2-api-0.0.2/src/helldivers2_api/planet_info_table.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      277 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/planet_status.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     1265 2024-04-03 06:48:13.000000 helldivers-2-api-0.0.2/src/helldivers2_api/sector.py
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      950 2024-04-04 06:07:09.000000 helldivers-2-api-0.0.2/src/helldivers2_api/war_status.py
+drwxrwxr-x   0 drodenkirchen  (1000) drodenkirchen  (1000)        0 2024-04-04 13:54:03.716764 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/
+-rw-r--r--   0 drodenkirchen  (1000) drodenkirchen  (1000)     2539 2024-04-04 13:54:03.000000 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/PKG-INFO
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)      857 2024-04-04 13:54:03.000000 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)        1 2024-04-04 13:54:03.000000 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       17 2024-04-04 13:54:03.000000 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/requires.txt
+-rw-rw-r--   0 drodenkirchen  (1000) drodenkirchen  (1000)       16 2024-04-04 13:54:03.000000 helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/top_level.txt
```

### Comparing `helldivers-2-api-0.0.1/PKG-INFO` & `helldivers-2-api-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: helldivers-2-api
-Version: 0.0.1
-Summary: TBD
+Version: 0.0.2
+Summary: A Python abstraction layer for the unofficial Helldivers 2 API from HellDiversTrainingManual
 Author-email: David Rodenkirchen <davidr.develop@gmail.com>
 Project-URL: Repository, https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api
 Project-URL: Discord, https://discord.gg/kKuxparXWT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENCE.md
 Requires-Dist: requests>=2.31.0
 
 # Helldivers 2 Python API
 
 A Python abstraction layer for the [unofficial Helldivers 2 API](https://helldiverstrainingmanual.com/api)
 
 ## Key Features
@@ -40,28 +41,29 @@
 
 Make sure to check out the [examples](https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/-/tree/main/examples).
 
 ### Minimal usage example
 
 ```python
 from helldivers2_api.api_client import ApiClient
+from helldivers2_api.planet_info_table import get_planet_by_id
 
 my_client = ApiClient()
 
 war_status = my_client.get_war_status()
 
 print(war_status.planet_attacks)
 
 #  [
 #    PlanetAttack(source_planet_id=125, target_planet_id=34), 
 #    PlanetAttack(source_planet_id=168, target_planet_id=34),
 #    ...
 #  ]
 
-planet_name = my_client.get_planet_by_id(34).name
+planet_name = get_planet_by_id(34).name
 print(planet_name)
 
 #  Hellmire
 ```
 
 
 ## Credits
```

### Comparing `helldivers-2-api-0.0.1/README.md` & `helldivers-2-api-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 <div align="center">
 <h1>
-  <br>
   <a href="https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/"><img src="https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/-/raw/main/static/logo.png" alt="HD2API" width="200"></a>
   <br>
   Helldivers 2 Python API
   <br>
 </h1>
 
 <h4 align="center">A Python abstraction layer for the [unofficial Helldivers 2 API](https://helldiverstrainingmanual.com/api)</h4>
 
 <p>
   <a href="http://www.wtfpl.net/">
     <img src="https://img.shields.io/badge/licence-WTFPL-green?style=flat" alt="WTFPL">
   </a>
-  <a href=https://www.python.org/downloads/""><img src="https://img.shields.io/badge/Python-3.11%20%7C%203.12-blue?style=flat"></a>
-  <a href="https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/">
-    <img src="https://img.shields.io/badge/version-0.0.1-orange?style=flat">
+  <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Python-3.11%20%7C%203.12-blue?style=flat"></a>
+  <a href="https://pypi.org/project/helldivers-2-api/">
+    <img src="https://img.shields.io/badge/version-0.0.2-orange?style=flat">
   </a>
 </p>
 
-<p>
-  <a href="#key-features">Key Features</a> •
-  <a href="#how-to-use">How To Use</a> •
-  <a href="#credits">Credits</a> •
-  <a href="#license">License</a>
-</p>
-
 </div>
 
 ## Key Features
 
 * Fully typed data model
   - Planets
   - Sectors
   - Factions
-  - Events
+  - GlobalEvents and PlanetEvents
   - Campaigns
   - Attacks
+  - News Feed
+  - Joint Operations
 * Simple to use
   - Use your IDE's autocompletion to simply traverse the data model tree
 * Easy Install
   - Only dependency is [requests](https://pypi.org/project/requests/)!
 
 ## How To Use
 
-Simply install [the PyPI package via pip]().
+Simply install [the PyPI package via pip](https://pypi.org/project/helldivers-2-api/).
 
 Checkout the examples in the subdirectory `examples` for a primer on how to use this package.
 
 ## Credits
 
 This software uses the following open source packages:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-                                    ************
-                                   _[[_HH_DD_22_AA_PP_II_]]
+                                ************ _[[_HH_DD_22_AA_PP_II_]]
                             HHeellllddiivveerrss 22 PPyytthhoonn AAPPII
                                      ************
  ****** AA PPyytthhoonn aabbssttrraaccttiioonn llaayyeerr ffoorr tthhee [[uunnooffffiicciiaall HHeellllddiivveerrss 22 AAPPII]]((hhttttppss::////
                      hheellllddiivveerrssttrraaiinniinnggmmaannuuaall..ccoomm//aappii)) ******
 _[_W_T_F_P_L_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_y_t_h_o_n_-_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_?_s_t_y_l_e_=_f_l_a_t_]
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-_0_._0_._1_-_o_r_a_n_g_e_?_s_t_y_l_e_=_f_l_a_t_]
-              _K_e_y_ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _C_r_e_d_i_t_s â¢ _L_i_c_e_n_s_e
+        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_v_e_r_s_i_o_n_-_0_._0_._2_-_o_r_a_n_g_e_?_s_t_y_l_e_=_f_l_a_t_]
 ## Key Features * Fully typed data model - Planets - Sectors - Factions -
-Events - Campaigns - Attacks * Simple to use - Use your IDE's autocompletion to
-simply traverse the data model tree * Easy Install - Only dependency is
-[requests](https://pypi.org/project/requests/)! ## How To Use Simply install
-[the PyPI package via pip](). Checkout the examples in the subdirectory
-`examples` for a primer on how to use this package. ## Credits This software
-uses the following open source packages: - [Python](https://www.python.org/) -
-[requests](https://pypi.org/project/requests/) ## License ``` DO WHAT THE FUCK
-YOU WANT TO PUBLIC LICENSE Version 2, December 2004 Copyright (C) 2024 David
-Rodenkirchen
+GlobalEvents and PlanetEvents - Campaigns - Attacks - News Feed - Joint
+Operations * Simple to use - Use your IDE's autocompletion to simply traverse
+the data model tree * Easy Install - Only dependency is [requests](https://
+pypi.org/project/requests/)! ## How To Use Simply install [the PyPI package via
+pip](https://pypi.org/project/helldivers-2-api/). Checkout the examples in the
+subdirectory `examples` for a primer on how to use this package. ## Credits
+This software uses the following open source packages: - [Python](https://
+www.python.org/) - [requests](https://pypi.org/project/requests/) ## License
+``` DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE Version 2, December 2004
+Copyright (C) 2024 David Rodenkirchen
 gmail.com> Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long as the name
 is changed. DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE TERMS AND CONDITIONS
 FOR COPYING, DISTRIBUTION AND MODIFICATION 0. You just DO WHAT THE FUCK YOU
 WANT TO. ``` --- > [jdrodenkirchen.de](https://jdrodenkirchen.de/)  ·  > Git:
 [@drodenkirchen](https://git.jdrodenkirchen.de/drodenkirchen)  ·  > Steam:
 [Typhus](https://steamcommunity.com/id/originaltyphus/)
```

### Comparing `helldivers-2-api-0.0.1/README_PYPI.md` & `helldivers-2-api-0.0.2/README_PYPI.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 
 Make sure to check out the [examples](https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/-/tree/main/examples).
 
 ### Minimal usage example
 
 ```python
 from helldivers2_api.api_client import ApiClient
+from helldivers2_api.planet_info_table import get_planet_by_id
 
 my_client = ApiClient()
 
 war_status = my_client.get_war_status()
 
 print(war_status.planet_attacks)
 
 #  [
 #    PlanetAttack(source_planet_id=125, target_planet_id=34), 
 #    PlanetAttack(source_planet_id=168, target_planet_id=34),
 #    ...
 #  ]
 
-planet_name = my_client.get_planet_by_id(34).name
+planet_name = get_planet_by_id(34).name
 print(planet_name)
 
 #  Hellmire
 ```
 
 
 ## Credits
```

### Comparing `helldivers-2-api-0.0.1/pyproject.toml` & `helldivers-2-api-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helldivers-2-api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="David Rodenkirchen", email="davidr.develop@gmail.com" },
 ]
-description = "TBD"
+description = "A Python abstraction layer for the unofficial Helldivers 2 API from HellDiversTrainingManual"
 readme = "README_PYPI.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `helldivers-2-api-0.0.1/src/helldivers2_api/planet_info_table.py` & `helldivers-2-api-0.0.2/src/helldivers2_api/planet_info_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from typing import Union
+
+from helldivers2_api.planet import Planet
+from helldivers2_api.sector import Sector
+
 PLANET_INFO_TABLE: dict = {
     "0": {
         "name": "Super Earth",
         "sector": "Sol",
         "biome": None,
         "environmentals": []
     },
@@ -4134,7 +4139,28 @@
             {
                 "name": "Tremors",
                 "description": "Frequent earthquakes stun players and enemies alike."
             }
         ]
     }
 }
+
+
+def get_planet_by_id(planet_id: Union[str, int]) -> Planet:
+    """
+    Retrieves a planet from the database by its ID
+    :param planet_id: Planet ID or planet index
+    :return: The found planet
+    :raises: KeyError if the planet could not been found
+    """
+    if isinstance(planet_id, int):
+        planet_id = str(planet_id)
+
+    try:
+        planet_info = PLANET_INFO_TABLE[planet_id]
+    except KeyError:
+        raise KeyError(f"Planet with ID '{planet_id}' is not on the database.")
+    return Planet(
+        planet_id=int(planet_id),
+        name=planet_info["name"],
+        sector=Sector(planet_info["sector"])
+    )
```

### Comparing `helldivers-2-api-0.0.1/src/helldivers2_api/sector.py` & `helldivers-2-api-0.0.2/src/helldivers2_api/sector.py`

 * *Files identical despite different names*

### Comparing `helldivers-2-api-0.0.1/src/helldivers2_api/war_status.py` & `helldivers-2-api-0.0.2/src/helldivers2_api/war_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from dataclasses import dataclass
 
 from helldivers2_api.campaign import Campaign
 from helldivers2_api.global_event import GlobalEvent
+from helldivers2_api.joint_operation import JointOperation
 from helldivers2_api.planet_attack import PlanetAttack
+from helldivers2_api.planet_event import PlanetEvent
 from helldivers2_api.planet_status import PlanetStatus
 
 
 @dataclass
 class WarStatus:
     active_election_policy_effects: list
     campaigns: list[Campaign]
     community_targets: list  # ToDo: Unclear how to parse this value
     global_events: list[GlobalEvent]
     impact_multiplier: float
-    joint_operations: list  # ToDo: Unclear how to parse this value
+    joint_operations: list[JointOperation]
     planet_active_effects: list  # ToDo: Unclear how to parse this value
     planet_attacks: list[PlanetAttack]
-    planet_events: list  # ToDo: Unclear how to parse this value
+    planet_events: list[PlanetEvent]
     planet_status: list[PlanetStatus]
     story_beat_id: int
     super_earth_war_results: list  # ToDo: Unclear how to parse this value
     time: int
     war_id: int
```

### Comparing `helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/PKG-INFO` & `helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: helldivers-2-api
-Version: 0.0.1
-Summary: TBD
+Version: 0.0.2
+Summary: A Python abstraction layer for the unofficial Helldivers 2 API from HellDiversTrainingManual
 Author-email: David Rodenkirchen <davidr.develop@gmail.com>
 Project-URL: Repository, https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api
 Project-URL: Discord, https://discord.gg/kKuxparXWT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENCE.md
 Requires-Dist: requests>=2.31.0
 
 # Helldivers 2 Python API
 
 A Python abstraction layer for the [unofficial Helldivers 2 API](https://helldiverstrainingmanual.com/api)
 
 ## Key Features
@@ -40,28 +41,29 @@
 
 Make sure to check out the [examples](https://git.jdrodenkirchen.de/drodenkirchen/helldivers-2-python-api/-/tree/main/examples).
 
 ### Minimal usage example
 
 ```python
 from helldivers2_api.api_client import ApiClient
+from helldivers2_api.planet_info_table import get_planet_by_id
 
 my_client = ApiClient()
 
 war_status = my_client.get_war_status()
 
 print(war_status.planet_attacks)
 
 #  [
 #    PlanetAttack(source_planet_id=125, target_planet_id=34), 
 #    PlanetAttack(source_planet_id=168, target_planet_id=34),
 #    ...
 #  ]
 
-planet_name = my_client.get_planet_by_id(34).name
+planet_name = get_planet_by_id(34).name
 print(planet_name)
 
 #  Hellmire
 ```
 
 
 ## Credits
```

### Comparing `helldivers-2-api-0.0.1/src/helldivers_2_api.egg-info/SOURCES.txt` & `helldivers-2-api-0.0.2/src/helldivers_2_api.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+LICENCE.md
 README.md
 README_PYPI.md
 pyproject.toml
 src/helldivers2_api/__init__.py
 src/helldivers2_api/api_client.py
 src/helldivers2_api/api_version.py
 src/helldivers2_api/campaign.py
 src/helldivers2_api/endpoint_map.py
 src/helldivers2_api/faction.py
 src/helldivers2_api/global_event.py
+src/helldivers2_api/joint_operation.py
+src/helldivers2_api/mapping_strategy.py
+src/helldivers2_api/news.py
 src/helldivers2_api/planet.py
 src/helldivers2_api/planet_attack.py
+src/helldivers2_api/planet_event.py
 src/helldivers2_api/planet_info_table.py
 src/helldivers2_api/planet_status.py
 src/helldivers2_api/sector.py
 src/helldivers2_api/war_status.py
 src/helldivers_2_api.egg-info/PKG-INFO
 src/helldivers_2_api.egg-info/SOURCES.txt
 src/helldivers_2_api.egg-info/dependency_links.txt
```

