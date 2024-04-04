# Comparing `tmp/pyweatherfr-1.4.4.tar.gz` & `tmp/pyweatherfr-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpmgxoz0rb/tmp1hu1rvvs/pyweatherfr-1.4.4.tar", last modified: Sun Nov 21 13:53:34 2021, max compression
+gzip compressed data, was "pyweatherfr-2.0.0.tar", last modified: Thu Apr  4 19:42:12 2024, max compression
```

## Comparing `pyweatherfr-1.4.4.tar` & `pyweatherfr-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24618 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3519 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/pyweatherfr/update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-11-21 13:53:24.000000 pyweatherfr-1.4.4/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-21 13:53:33.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-11-21 13:53:34.000000 pyweatherfr-1.4.4/pyweatherfr.egg-info/entry_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31075 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyweatherfr-1.4.4/pyweatherfr/args.py` & `pyweatherfr-2.0.0/pyweatherfr/args.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,27 @@
         "town",
         metavar="VILLE",
         type=str,
         nargs="?",
         help="affichage des données météo par nom de ville -si absent, la VILLE est déduite de l'ip-",
     )
     my_parser.add_argument(
+        "-n",
+        "--now",
+        action="store_true",
+        help="affichage des données météo détaillées actuelles",
+    )    
+    my_parser.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
         default=-1,
-        choices=range(0, 5),
+        choices=range(0, 4),
         help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ...)",
     ) 
     my_group.add_argument(
         "-p",
         "--post",
         action="store",
         metavar="CODE_POSTAL",
@@ -79,15 +85,14 @@
         "--search",
         action="store",
         metavar="RECHERCHE",
         type=str,
         help="ville ou code postal à rechercher",
     )        
     my_parser.add_argument(
-        "-n",
         "--nocolor",
         action="store_true",
         help="désactiver couleur et emojis en sortie -à utiliser en cas de problème d'affichage-",
     )
     my_parser.add_argument(
         "-c",
         "--condensate",
```

### Comparing `pyweatherfr-1.4.4/README.md` & `pyweatherfr-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # :sunny: :umbrella: :cloud: pyweatherfr
 
-pyweatherfr affiche les prévisions méteo pour les communes françaises dans votre terminal. Il utilise les API https://www.prevision-meteo.ch et https://geolocation-db.com/json.
+pyweatherfr affiche les prévisions méteo pour les communes françaises dans votre terminal. Il utilise les API de méteoFrance, https://www.prevision-meteo.ch et https://geolocation-db.com/json.
 
 
 # 🚀 Comment utiliser **pyweatherfr**
 
 pyweatherfr \[VILLE\]
 
-exemple : ``pyweatherfr Grenoble`` affiche les prévisions météo pour Grenoble
+exemple : ``pyweatherfr Grenoble`` affiche les prévisions météo pour Grenoble sur 4 jours
 
-pyweatherfr \[TOWN\] -j [INT(0-4)]
+pyweatherfr -n \[VILLE\]
+
+exemple : ``pyweatherfr -n Grenoble`` affiche les données météo pour Grenoble 
+
+pyweatherfr \[TOWN\] -j [INT(0-3)]
 
 exemple : ``pyweatherfr Grenoble -j 1`` affiche les prévisions météo détaillées pour Grenoble à J+1
 
 pyweatherfr -p \[CODE_POSTAL\]
 
 exemple : ``pyweatherfr -p  38700`` affiche les prévisions météo pour le code postal 38700
 
@@ -23,15 +27,15 @@
 
 
 ## Autres options
 
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
-  - ``-n/--nocolor``  désactive les couleurs et les emojis en sortie
+  - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``-C/--cache``  met à jour le cache du nom des villes (cache par défaut 30j)
   
 # Démo
 
 ![image](./demo_01.png)
```

### Comparing `pyweatherfr-1.4.4/setup.py` & `pyweatherfr-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="1.4.4",
+    version="2.0.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
-    install_requires=["columnar","termcolor", "colorama","unidecode","requests"],
+    install_requires=["columnar","termcolor", "colorama","unidecode","requests","openmeteo_requests","requests_cache","pandas","retry_requests"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "pyweatherfr=pyweatherfr.__init__:pyweatherfr"
         ],
     },
     classifiers=[
```

### Comparing `pyweatherfr-1.4.4/LICENSE.txt` & `pyweatherfr-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

