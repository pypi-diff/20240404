# Comparing `tmp/vedicastro-0.2.0.tar.gz` & `tmp/vedicastro-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedicastro-0.2.0.tar", last modified: Wed Mar 27 14:55:17 2024, max compression
+gzip compressed data, was "vedicastro-0.2.1.tar", last modified: Thu Apr  4 13:00:06 2024, max compression
```

## Comparing `vedicastro-0.2.0.tar` & `vedicastro-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 14:55:17.984605 vedicastro-0.2.0/
--rw-rw-rw-   0        0        0     6718 2024-03-27 14:55:17.982756 vedicastro-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6035 2024-03-27 14:54:48.000000 vedicastro-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-27 14:55:17.987110 vedicastro-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1480 2024-03-27 14:54:48.000000 vedicastro-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:55:17.848631 vedicastro-0.2.0/vedicastro/
--rw-rw-rw-   0        0        0    27076 2024-03-24 18:58:15.000000 vedicastro-0.2.0/vedicastro/VedicAstro.py
--rw-rw-rw-   0        0        0        0 2024-03-03 15:49:54.000000 vedicastro-0.2.0/vedicastro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:55:17.976210 vedicastro-0.2.0/vedicastro/data/
--rw-rw-rw-   0        0        0    13692 2024-03-23 12:37:12.000000 vedicastro-0.2.0/vedicastro/data/KP_SL_Divisions.csv
--rw-rw-rw-   0        0        0     7621 2024-03-27 14:54:48.000000 vedicastro-0.2.0/vedicastro/horary_chart.py
--rw-rw-rw-   0        0        0     4342 2024-03-25 16:53:01.000000 vedicastro-0.2.0/vedicastro/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-27 14:55:17.980560 vedicastro-0.2.0/vedicastro.egg-info/
--rw-rw-rw-   0        0        0     6718 2024-03-27 14:55:17.000000 vedicastro-0.2.0/vedicastro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-03-27 14:55:17.000000 vedicastro-0.2.0/vedicastro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       64 2024-03-27 14:55:17.000000 vedicastro-0.2.0/vedicastro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-03-27 14:55:17.000000 vedicastro-0.2.0/vedicastro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-27 14:55:17.000000 vedicastro-0.2.0/vedicastro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 13:00:06.431669 vedicastro-0.2.1/
+-rw-rw-rw-   0        0        0     6718 2024-04-04 13:00:06.428672 vedicastro-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6035 2024-03-27 14:54:48.000000 vedicastro-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:00:06.431669 vedicastro-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2024-04-04 12:59:59.000000 vedicastro-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:00:06.370017 vedicastro-0.2.1/vedicastro/
+-rw-rw-rw-   0        0        0    26566 2024-04-04 12:54:29.000000 vedicastro-0.2.1/vedicastro/VedicAstro.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 15:49:54.000000 vedicastro-0.2.1/vedicastro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:00:06.424367 vedicastro-0.2.1/vedicastro/data/
+-rw-rw-rw-   0        0        0    13692 2024-03-23 12:37:12.000000 vedicastro-0.2.1/vedicastro/data/KP_SL_Divisions.csv
+-rw-rw-rw-   0        0        0     7621 2024-03-27 14:54:48.000000 vedicastro-0.2.1/vedicastro/horary_chart.py
+-rw-rw-rw-   0        0        0     4342 2024-03-25 16:53:01.000000 vedicastro-0.2.1/vedicastro/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:00:06.427370 vedicastro-0.2.1/vedicastro.egg-info/
+-rw-rw-rw-   0        0        0     6718 2024-04-04 13:00:06.000000 vedicastro-0.2.1/vedicastro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-04 13:00:06.000000 vedicastro-0.2.1/vedicastro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       64 2024-04-04 13:00:06.000000 vedicastro-0.2.1/vedicastro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-04 13:00:06.000000 vedicastro-0.2.1/vedicastro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 13:00:06.000000 vedicastro-0.2.1/vedicastro.egg-info/top_level.txt
```

### Comparing `vedicastro-0.2.0/PKG-INFO` & `vedicastro-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedicastro
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for Vedic Astrology, with a particular focus on the Krishnamurthi Paddhati system
 Home-page: https://github.com/diliprk/VedicAstro
 Author: Dilip Rajkumar
 Author-email: diliprajkumar@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vedicastro-0.2.0/README.md` & `vedicastro-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vedicastro-0.2.0/setup.py` & `vedicastro-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="vedicastro",
-    version="0.2.0",
+    version="0.2.1",
     author="Dilip Rajkumar",
     author_email="diliprajkumar@gmail.com",
     description="A python package for Vedic Astrology, with a particular focus on the Krishnamurthi Paddhati system",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/diliprk/VedicAstro",
```

### Comparing `vedicastro-0.2.0/vedicastro/VedicAstro.py` & `vedicastro-0.2.1/vedicastro/VedicAstro.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,22 @@
 ## Lords of the 12 Zodiac Signs
 SIGN_LORDS = ["Mars", "Venus", "Mercury", "Moon", "Sun", "Mercury", "Venus", "Mars", "Jupiter", "Saturn", "Saturn", "Jupiter"]          
 
 NAKSHATRAS = ['Ashwini','Bharani','Krittika','Rohini','Mrigashīrsha', 'Ardra', 'Punarvasu', 'Pushya', 'Āshleshā', 
 'Maghā', 'PūrvaPhalgunī', 'UttaraPhalgunī', 'Hasta', 'Chitra', 'Svati', 'Vishakha', 'Anuradha', 'Jyeshtha', 'Mula', 
 'PurvaAshadha','UttaraAshadha', 'Shravana', 'Dhanishta','Shatabhisha', 'PurvaBhādrapadā', 'UttaraBhādrapadā', 'Revati']
 
-AYANAMSA_MAPPING = { "Lahiri": const.AY_LAHIRI, "Krishnamurti": const.AY_KRISHNAMURTI, "Raman": const.AY_RAMAN,
-                    "FaganBradley": const.AY_FAGAN_BRADLEY, "Deluce": const.AY_DELUCE, "Sassanian": const.AY_SASSANIAN,
-                    "Aldebaran15Taurus": const.AY_ALDEBARAN_15TAU, "GalacticCenter_05_Sag": const.AY_GALCENTER_5SAG
+AYANAMSA_MAPPING = { "Lahiri": const.AY_LAHIRI, "Lahiri_1940" : const.AY_LAHIRI_1940, 
+                    "Lahiri_VP285": const.AY_LAHIRI_VP285, "Lahiri_ICRC" : const.AY_LAHIRI_ICRC, "Raman": const.AY_RAMAN,
+                    "Krishnamurti": const.AY_KRISHNAMURTI, "Krishnamurti_Senthilathiban": const.AY_KRISHNAMURTI_SENTHILATHIBAN,
                     }
 
 
-HOUSE_SYSTEM_MAPPING = { "Placidus": const.HOUSES_PLACIDUS, "Koch": const.HOUSES_EQUAL, 
-                        "Porphyrius": const.HOUSES_PORPHYRIUS, "Regiomontanus": const.HOUSES_REGIOMONTANUS, 
-                        "Campanus": const.HOUSES_CAMPANUS, "Equal": const.HOUSES_EQUAL,
-                        "Equal 2": const.HOUSES_EQUAL_2, "Vehlow Equal": const.HOUSES_VEHLOW_EQUAL, 
-                        "Whole Sign": const.HOUSES_WHOLE_SIGN, "Meridian": const.HOUSES_MERIDIAN, 
-                        "Azimuthal": const.HOUSES_AZIMUTHAL, "Polich Page": const.HOUSES_POLICH_PAGE,
-                        "Alcabitus": const.HOUSES_ALCABITUS, "Morinus": const.HOUSES_MORINUS
+HOUSE_SYSTEM_MAPPING = { "Placidus": const.HOUSES_PLACIDUS, "Equal": const.HOUSES_EQUAL,
+                        "Equal 2": const.HOUSES_EQUAL_2, "Whole Sign": const.HOUSES_WHOLE_SIGN,
                     }
 
 ASPECT_MAPPING = {  const.NO_ASPECT: "No Aspect", const.CONJUNCTION: "Conjunction", const.SEXTILE: "Sextile",
                     const.SQUARE: "Square", const.TRINE: "Trine", const.OPPOSITION: "Opposition", 
                     const.SEMISEXTILE: "Semi Sextile", const.SEMIQUINTILE: "Semi Quintile",
                     const.SEMISQUARE: "Semi Square", const.QUINTILE: "Quintile", 
                     const.SESQUIQUINTILE: "Sesqui Quintile", const.SESQUISQUARE: "Sesqui Square",
@@ -488,8 +483,8 @@
                 bhukti_length = dasa_length * bhukti_lengths[j] / 120  # The total length of all Bhuktis in a Maha Dasa is 120 years
                 bhukti_end_date = compute_new_date(start_date = tuple(bhukti_start_date.timetuple())[:5], diff_value = bhukti_length, direction="forward")
                 vimshottari_dasa[dasa]['bhuktis'][bhukti] = {'start':  dt_tuple_str(bhukti_start_date), 'end': dt_tuple_str(bhukti_end_date)}
                 # vimshottari_dasa[dasa]['bhuktis'][bhukti] = collections.OrderedDict([('start',  dt_tuple_str(bhukti_start_date)), ('end', dt_tuple_str(bhukti_end_date))])
                 bhukti_start_date = bhukti_end_date
             dasa_start_date = dasa_end_date
 
-        return vimshottari_dasa
+        return vimshottari_dasa
```

### Comparing `vedicastro-0.2.0/vedicastro/data/KP_SL_Divisions.csv` & `vedicastro-0.2.1/vedicastro/data/KP_SL_Divisions.csv`

 * *Files identical despite different names*

### Comparing `vedicastro-0.2.0/vedicastro/horary_chart.py` & `vedicastro-0.2.1/vedicastro/horary_chart.py`

 * *Files identical despite different names*

### Comparing `vedicastro-0.2.0/vedicastro/utils.py` & `vedicastro-0.2.1/vedicastro/utils.py`

 * *Files identical despite different names*

### Comparing `vedicastro-0.2.0/vedicastro.egg-info/PKG-INFO` & `vedicastro-0.2.1/vedicastro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedicastro
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for Vedic Astrology, with a particular focus on the Krishnamurthi Paddhati system
 Home-page: https://github.com/diliprk/VedicAstro
 Author: Dilip Rajkumar
 Author-email: diliprajkumar@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

