# Comparing `tmp/pgtg-0.1.0.tar.gz` & `tmp/pgtg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgtg-0.1.0.tar", max compression
+gzip compressed data, was "pgtg-0.2.0.tar", max compression
```

## Comparing `pgtg-0.1.0.tar` & `pgtg-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      181 2024-02-08 09:36:01.597292 pgtg-0.1.0/pgtg/__init__.py
--rw-r--r--   0        0        0      706 2024-02-19 20:30:42.064128 pgtg-0.1.0/pgtg/constants.py
--rw-r--r--   0        0        0    30762 2024-02-19 22:32:51.716786 pgtg-0.1.0/pgtg/environment.py
--rw-r--r--   0        0        0    12292 2024-02-05 17:28:34.890738 pgtg-0.1.0/pgtg/evaluator.py
--rw-r--r--   0        0        0     5717 2024-02-05 17:28:34.946434 pgtg-0.1.0/pgtg/example_maps/tile_map_big_with_obstacles.json
--rw-r--r--   0        0        0     4494 2024-02-05 17:28:34.950214 pgtg-0.1.0/pgtg/example_maps/tile_map_big_without_obstacles.json
--rw-r--r--   0        0        0     1422 2024-02-05 17:28:34.951563 pgtg-0.1.0/pgtg/example_maps/tile_map_medium_with_obstacles.json
--rw-r--r--   0        0        0      716 2024-02-05 17:28:34.955022 pgtg-0.1.0/pgtg/example_maps/tile_map_medium_without_obstacles.json
--rw-r--r--   0        0        0      254 2024-02-05 17:28:34.958061 pgtg-0.1.0/pgtg/example_maps/tile_map_minimal_without_obstacles.json
--rw-r--r--   0        0        0    10624 2024-02-16 18:30:41.191869 pgtg-0.1.0/pgtg/graphic.py
--rw-r--r--   0        0        0     5857 2024-02-18 11:53:48.767912 pgtg-0.1.0/pgtg/map.py
--rw-r--r--   0        0        0    10757 2024-02-15 16:57:54.076545 pgtg-0.1.0/pgtg/map_generator.py
--rw-r--r--   0        0        0    85827 2024-02-19 20:35:05.226457 pgtg-0.1.0/pgtg/map_tiles_data.py
--rw-r--r--   0        0        0    10153 2024-02-19 21:41:05.467239 pgtg-0.1.0/pgtg/parser.py
--rw-r--r--   0        0        0    12838 2024-02-05 17:28:34.960343 pgtg-0.1.0/pgtg/pics/beginning.png
--rw-r--r--   0        0        0    13575 2024-02-05 17:28:34.961338 pgtg-0.1.0/pgtg/pics/road_break.png
--rw-r--r--   0        0        0     8739 2024-02-05 17:28:34.962345 pgtg-0.1.0/pgtg/pics/road_left.png
--rw-r--r--   0        0        0      336 2024-02-05 17:28:34.963344 pgtg-0.1.0/pgtg/pics/test.png
--rw-r--r--   0        0        0      974 2024-02-19 22:28:04.526022 pgtg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3819 2024-02-19 22:35:43.680297 pgtg-0.1.0/README.md
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 pgtg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      181 2024-04-04 18:03:29.163895 pgtg-0.2.0/pgtg/__init__.py
+-rw-r--r--   0        0        0      706 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/constants.py
+-rw-r--r--   0        0        0    31146 2024-04-04 17:13:49.100300 pgtg-0.2.0/pgtg/environment.py
+-rw-r--r--   0        0        0    12292 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/evaluator.py
+-rw-r--r--   0        0        0     5717 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_big_with_obstacles.json
+-rw-r--r--   0        0        0     4494 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_big_without_obstacles.json
+-rw-r--r--   0        0        0     1422 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_medium_with_obstacles.json
+-rw-r--r--   0        0        0      716 2024-03-25 09:00:18.472318 pgtg-0.2.0/pgtg/example_maps/tile_map_medium_without_obstacles.json
+-rw-r--r--   0        0        0      254 2024-03-25 09:00:18.485270 pgtg-0.2.0/pgtg/example_maps/tile_map_minimal_without_obstacles.json
+-rw-r--r--   0        0        0    10624 2024-03-25 09:00:18.486753 pgtg-0.2.0/pgtg/graphic.py
+-rw-r--r--   0        0        0     5857 2024-03-25 09:00:18.497055 pgtg-0.2.0/pgtg/map.py
+-rw-r--r--   0        0        0    10757 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/map_generator.py
+-rw-r--r--   0        0        0    85827 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/map_tiles_data.py
+-rw-r--r--   0        0        0    10153 2024-03-25 09:00:18.497293 pgtg-0.2.0/pgtg/parser.py
+-rw-r--r--   0        0        0    12838 2024-03-25 09:00:18.502311 pgtg-0.2.0/pgtg/pics/beginning.png
+-rw-r--r--   0        0        0    13575 2024-03-25 09:00:18.502883 pgtg-0.2.0/pgtg/pics/road_break.png
+-rw-r--r--   0        0        0     8739 2024-03-25 09:00:18.504371 pgtg-0.2.0/pgtg/pics/road_left.png
+-rw-r--r--   0        0        0      336 2024-03-25 09:00:18.505409 pgtg-0.2.0/pgtg/pics/test.png
+-rw-r--r--   0        0        0      974 2024-04-04 18:02:17.309218 pgtg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3924 2024-04-04 17:44:46.079919 pgtg-0.2.0/README.md
+-rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 pgtg-0.2.0/PKG-INFO
```

### Comparing `pgtg-0.1.0/pgtg/constants.py` & `pgtg-0.2.0/pgtg/constants.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/environment.py` & `pgtg-0.2.0/pgtg/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         sum_subgoals_reward: int = 100,
         final_goal_bonus: int = 0,
         crash_penalty: int = 100,
         standing_still_penalty: int = 0,
         already_visited_position_penalty: int = 0,
         ice_probability: float = 0.1,
         street_damage_probability: float = 0.1,
+        sand_probability: float = 0.2,
         traffic_density: float = 0.0,
         ignore_traffic_collisions: bool = False,
     ):
         """initializes an object of the class with the given arguments.
 
         Args:
             map_name: Default None. Path to map file, either absolute or relative to the current working directory. If it is None a random map is generated instead.
@@ -62,14 +63,15 @@
             sum_subgoals_reward: Default 100. The sum of all subgoal rewards. Gets split evenly among all subgoals.
             final_goal_bonus: Default 0. Bonus for the final goal that gets added to the subgoal reward.
             crash_penalty: Default 100. Penalty for driving into a wall or out of the map. The value will get negated so a positive value should be used.
             standing_still_penalty: Default 0. Penalty for not moving. Gets applied every step. The value will get negated so a positive value should be used.
             already_visited_position_penalty: Default 0. Penalty for moving to a position that was visited before. Gets applied every step for the final position of that step. Standing still does not result in penalty. The value will get negated so a positive value should be used.
             ice_probability: Default 0.1. Probability of the ice effect happening when the agent drives over it.
             street_damage_probability: Default  0.1. Probability of the broken road effect happening when the agent drives over it.
+            sand_probability: Default 0.2. Probability of the sand effect happening when the agent drives over it.
             traffic_density: Default 0.0. The density of the traffic as fraction of the number of traffic cars and the number of positions where traffic could be. For a value of 0 no traffic is generated.
             ignore_traffic_collisions: Default False. If true collisions with traffic are ignored. For testing purposes.
         """
 
         # There are 8 different directions to accelerate into and the option to stand still.
         self.action_space = spaces.Discrete(9)
 
@@ -113,14 +115,15 @@
         self.final_goal_bonus = final_goal_bonus
         self.crash_penalty = crash_penalty
         self.standing_still_penalty = standing_still_penalty
         self.already_visited_position_penalty = already_visited_position_penalty
 
         self.ice_probability = ice_probability
         self.street_damage_probability = street_damage_probability
+        self.sand_probability = sand_probability
         self.traffic_density = traffic_density
 
         self.ignore_traffic_collisions = ignore_traffic_collisions
 
         self.window_size = 720
         self.window = None
         self.clock = None
@@ -138,15 +141,16 @@
 
         # define one random number generator for each random element
         (
             self.map_rng,
             self.car_rng,
             self.ice_rng,
             self.broken_road_rng,
-        ) = self.np_random.spawn(4)
+            self.sand_rng,
+        ) = self.np_random.spawn(5)
 
         if (
             not self.map_path == None
         ):  # if a map_path is provided load the map from that path
             if self.map_plan == None:  # only load the file on the first reset
                 self.map_plan = json_file_to_map_plan(self.map_path)
             self.map = EpisodeMap(self.map_plan)
@@ -516,32 +520,39 @@
                 self.map.set_subgoals_to_used(current_position_x, current_position_y)
 
             # if the last step -> only checking for goal and wall, skip the rest
             if velocity_part is None:
                 continue
 
             # case ice
-            if self.map.feature_at(current_position_x, current_position_y, "ice"):
-                if self.ice_rng.random() < self.ice_probability:
-                    # pick a random action
-                    ice_action = self.ice_rng.choice(list(range(9)))
-                    ice_velocity = np.array(ACTIONS_TO_ACCELERATION[ice_action])
-                    velocity_part = ice_velocity
-                    self.noise_path.append(list(current_position))
+            if (
+                self.map.feature_at(current_position_x, current_position_y, "ice")
+                and self.ice_rng.random() < self.ice_probability
+            ):
+                # pick a random action
+                ice_action = self.ice_rng.choice(list(range(9)))
+                ice_velocity = np.array(ACTIONS_TO_ACCELERATION[ice_action])
+                velocity_part = ice_velocity
+                self.noise_path.append(list(current_position))
 
             # case road_break
-            if self.map.feature_at(
-                current_position_x, current_position_y, "broken road"
+            if (
+                self.map.feature_at(
+                    current_position_x, current_position_y, "broken road"
+                )
+                and self.broken_road_rng.random() < self.street_damage_probability
             ):
-                if self.broken_road_rng.random() < self.street_damage_probability:
-                    self.flat_tire = True
-                    self.noise_path.append(list(current_position))
+                self.flat_tire = True
+                self.noise_path.append(list(current_position))
 
             # case sand
-            if self.map.feature_at(current_position_x, current_position_y, "sand"):
+            if (
+                self.map.feature_at(current_position_x, current_position_y, "sand")
+                and self.sand_rng.random() < self.sand_probability
+            ):
                 self.noise_path.append(list(current_position))
                 current_position += velocity_part
                 self.tile_path.append(list(current_position))
                 self.velocity = np.array([0, 0])
                 break
 
             current_position += velocity_part
```

### Comparing `pgtg-0.1.0/pgtg/evaluator.py` & `pgtg-0.2.0/pgtg/evaluator.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/example_maps/tile_map_big_with_obstacles.json` & `pgtg-0.2.0/pgtg/example_maps/tile_map_big_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/example_maps/tile_map_big_without_obstacles.json` & `pgtg-0.2.0/pgtg/example_maps/tile_map_big_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/example_maps/tile_map_medium_with_obstacles.json` & `pgtg-0.2.0/pgtg/example_maps/tile_map_medium_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/example_maps/tile_map_medium_without_obstacles.json` & `pgtg-0.2.0/pgtg/example_maps/tile_map_medium_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/graphic.py` & `pgtg-0.2.0/pgtg/graphic.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/map.py` & `pgtg-0.2.0/pgtg/map.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/map_generator.py` & `pgtg-0.2.0/pgtg/map_generator.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/map_tiles_data.py` & `pgtg-0.2.0/pgtg/map_tiles_data.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/parser.py` & `pgtg-0.2.0/pgtg/parser.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/pics/beginning.png` & `pgtg-0.2.0/pgtg/pics/beginning.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/pics/road_break.png` & `pgtg-0.2.0/pgtg/pics/road_break.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pgtg/pics/road_left.png` & `pgtg-0.2.0/pgtg/pics/road_left.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.1.0/pyproject.toml` & `pgtg-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "Operating System :: OS Independent",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 description = "Python simulation of a driving challange. Compatible with the Gymnasium API standard."
 name = "pgtg"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 Pillow = "^8.4.0"
 matplotlib = "^3.4.3"
 numpy = "^1.26.3"
 python = ">=3.10,<3.11"
 jupyter = "^1.0.0"
```

### Comparing `pgtg-0.1.0/README.md` & `pgtg-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# ProgGrid Traffic Gym (pgtg)
+# ProcGrid Traffic Gym (pgtg)
 
 A driving simulation on a grid with procedural generated maps and traffic. Compatible with the Gymnasium API standard.
 
 ### Installation
 
 ```bash
 pip install pgtg
 ```
 
 ### Usage
 The easiest way to use pgtg is to create the environment with gymnasium:
 ```python
 import pgtg
-env = gymnasium.make("pgtg-v0")
+env = gymnasium.make("pgtg-v1")
 ```
 The package relies on ```import``` side-effects to register the environment
 name so, even though the package is never explicitly used, its import is
 necessary to access the environment.  
 
 If you want to access the environment constructor directly this is also possible:
 ```python
 from pgtg import PGTGEnv
 env = PGTGEnv()
 ```
 
 ## Environment
-ProgGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
+ProcGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
 
 The environment is highly customizable, see the constructor documentation for more info.
 
 ### Action Space
-ProgGrid Traffic Gym has a `Discrete(9)` action space.
+ProcGrid Traffic Gym has a `Discrete(9)` action space.
 
 | Value | Meaning                   |
 |-------|---------------------------|
 | 0     | accelerate left and up    |
 | 1     | accelerate left           |
 | 2     | accelerate left and down  |
 | 3     | accelerate up             |
 | 4     | don't accelerate          |
 | 5     | accelerate down           |
 | 6     | accelerate right and up   |
 | 7     | accelerate right          |
 | 8     | accelerate right and down |
 
 ### Observation Space
-ProgGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
+ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
 | Key | Type | Explanation |
 |-----|------|-------------|
 | "position" | `MultiDiscrete` | The x and y position of the agent within the observation window. |
 | "velocity" | `Box` | The velocity of the agent is x and y direction. |
 | "map" | `Dict` | The 9x9 are of the map the agent is currently inside. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
 
 Most reinforcement learning implementations can't deal with `Dict` observations, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
@@ -68,12 +68,13 @@
 | rgb_array | `render()` returns a `np.array` representing a image. |
 | pil_image| `render()` returns a `PIL.Image.Image`, useful for displaying inside jupiter notebooks. |
 
 ### Obstacles
 | Name | Effect |
 |------|--------|
 | Ice | When driving over a square with ice, there is a chance the agent moves in a random direction instead of the expected one. |
-| Sand | When driving over sand the agent is slowed, as the velocity is reset to 0 every step. |
+| Sand | When driving over sand, there is a chance that the agent is slowed, as the velocity is reset to 0. |
 | Broken road | When driving over broken road, there is a chance for the agent to get a flat tire. This slows the agent down, as the velocity is reset to 0 every step. A flat tire lasts until the end of the episode.|
 
 ## Version History
-- v0: initial release
+- v0: initial release
+- v1: Sand now slows down with a customizable probability (default 20%) instead of always.
```

### Comparing `pgtg-0.1.0/PKG-INFO` & `pgtg-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgtg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python simulation of a driving challange. Compatible with the Gymnasium API standard.
 Author: Timo P. Gros
 Author-email: timopgros@cs.uni-saarland.de
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -16,62 +16,62 @@
 Requires-Dist: gymnasium (>=0.28.1,<0.29.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pygame (>=2.5.2,<3.0.0)
 Description-Content-Type: text/markdown
 
-# ProgGrid Traffic Gym (pgtg)
+# ProcGrid Traffic Gym (pgtg)
 
 A driving simulation on a grid with procedural generated maps and traffic. Compatible with the Gymnasium API standard.
 
 ### Installation
 
 ```bash
 pip install pgtg
 ```
 
 ### Usage
 The easiest way to use pgtg is to create the environment with gymnasium:
 ```python
 import pgtg
-env = gymnasium.make("pgtg-v0")
+env = gymnasium.make("pgtg-v1")
 ```
 The package relies on ```import``` side-effects to register the environment
 name so, even though the package is never explicitly used, its import is
 necessary to access the environment.  
 
 If you want to access the environment constructor directly this is also possible:
 ```python
 from pgtg import PGTGEnv
 env = PGTGEnv()
 ```
 
 ## Environment
-ProgGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
+ProcGrid Traffic Gym procedurally generates a map consisting of multiple preconstructed tiles or loads a map from a file. The goal is to drive from the start of the map to the end. The navigation task is not part of this environment, instead a shortest path is provided and marked on the map.  
 
 The environment is highly customizable, see the constructor documentation for more info.
 
 ### Action Space
-ProgGrid Traffic Gym has a `Discrete(9)` action space.
+ProcGrid Traffic Gym has a `Discrete(9)` action space.
 
 | Value | Meaning                   |
 |-------|---------------------------|
 | 0     | accelerate left and up    |
 | 1     | accelerate left           |
 | 2     | accelerate left and down  |
 | 3     | accelerate up             |
 | 4     | don't accelerate          |
 | 5     | accelerate down           |
 | 6     | accelerate right and up   |
 | 7     | accelerate right          |
 | 8     | accelerate right and down |
 
 ### Observation Space
-ProgGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
+ProcGrid Traffic Gym has a `Dict` observation space that shows the 9x9 area the agent currently is inside.
 | Key | Type | Explanation |
 |-----|------|-------------|
 | "position" | `MultiDiscrete` | The x and y position of the agent within the observation window. |
 | "velocity" | `Box` | The velocity of the agent is x and y direction. |
 | "map" | `Dict` | The 9x9 are of the map the agent is currently inside. The keys are the name of the features (`"walls"`, `"goals"`, `"ice"`, `"broken road"`, `"sand"`, and `"traffic"`). Each item is a `MultiBinary` that encodes that feature as a hot one encoding. |
 
 Most reinforcement learning implementations can't deal with `Dict` observations, thus it might be necessary to flatten the observations. This is easily doable with the `gymnasium.wrappers.FlattenObservation` wrapper:
@@ -90,12 +90,13 @@
 | rgb_array | `render()` returns a `np.array` representing a image. |
 | pil_image| `render()` returns a `PIL.Image.Image`, useful for displaying inside jupiter notebooks. |
 
 ### Obstacles
 | Name | Effect |
 |------|--------|
 | Ice | When driving over a square with ice, there is a chance the agent moves in a random direction instead of the expected one. |
-| Sand | When driving over sand the agent is slowed, as the velocity is reset to 0 every step. |
+| Sand | When driving over sand, there is a chance that the agent is slowed, as the velocity is reset to 0. |
 | Broken road | When driving over broken road, there is a chance for the agent to get a flat tire. This slows the agent down, as the velocity is reset to 0 every step. A flat tire lasts until the end of the episode.|
 
 ## Version History
 - v0: initial release
+- v1: Sand now slows down with a customizable probability (default 20%) instead of always.
```

