# Comparing `tmp/paladium-1.0.5.tar.gz` & `tmp/paladium-1.0.6.tar.gz`

## Comparing `paladium-1.0.5.tar` & `paladium-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 paladium-1.0.5/.DS_Store
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 paladium-1.0.5/example.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 paladium-1.0.5/src/paladium/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 paladium-1.0.5/src/paladium/faction.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 paladium-1.0.5/src/paladium/paladium.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 paladium-1.0.5/src/paladium/player.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 paladium-1.0.5/src/paladium/rank.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paladium-1.0.5/tests/.gitkeep
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 paladium-1.0.5/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 paladium-1.0.5/README.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 paladium-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 paladium-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 paladium-1.0.6/example.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/faction.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/paladium.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/player.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/rank.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paladium-1.0.6/tests/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 paladium-1.0.6/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 paladium-1.0.6/README.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 paladium-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 paladium-1.0.6/PKG-INFO
```

### Comparing `paladium-1.0.5/example.py` & `paladium-1.0.6/example.py`

 * *Files identical despite different names*

### Comparing `paladium-1.0.5/src/paladium/faction.py` & `paladium-1.0.6/src/paladium/faction.py`

 * *Files identical despite different names*

### Comparing `paladium-1.0.5/src/paladium/paladium.py` & `paladium-1.0.6/src/paladium/paladium.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from typing import List, Dict
-from player import Player
-from faction import Faction, FactionLeaderboard
-from rank import PlayerRank, Leaderboard, PlayerLeaderboard
+from .player import Player
+from .faction import Faction, FactionLeaderboard
+from .rank import PlayerRank, Leaderboard, PlayerLeaderboard
 import uuid
 
 PALADIUM_API_URL = 'https://api.paladium-pvp.fr/'
 
 class Paladium:
     def __init__(self, key: str = None):
         self.key = key
```

### Comparing `paladium-1.0.5/src/paladium/player.py` & `paladium-1.0.6/src/paladium/player.py`

 * *Files identical despite different names*

### Comparing `paladium-1.0.5/src/paladium/rank.py` & `paladium-1.0.6/src/paladium/rank.py`

 * *Files identical despite different names*

