# Comparing `tmp/gym_gui_tictactoe-0.1.tar.gz` & `tmp/gym_gui_tictactoe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_gui_tictactoe-0.1.tar", last modified: Tue Apr  2 20:18:32 2024, max compression
+gzip compressed data, was "gym_gui_tictactoe-0.1.1.tar", last modified: Thu Apr  4 15:40:18 2024, max compression
```

## Comparing `gym_gui_tictactoe-0.1.tar` & `gym_gui_tictactoe-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/gym_gui_tictactoe/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/gym_gui_tictactoe/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe/envs/tictactoe_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/gym_gui_tictactoe/example/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe/example/play_game.py
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe/example/play_game_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-02 20:18:32.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 20:18:32.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:18:32.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:18:32.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 20:18:32.000000 gym_gui_tictactoe-0.1/gym_gui_tictactoe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:18:32.018743 gym_gui_tictactoe-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-02 20:18:17.000000 gym_gui_tictactoe-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:18.526905 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/envs/tictactoe_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/example/play_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/example/play_game_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-04 15:40:18.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 15:40:18.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:40:18.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 15:40:18.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 15:40:18.000000 gym_gui_tictactoe-0.1.1/gym_gui_tictactoe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:40:18.530905 gym_gui_tictactoe-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-04 15:40:12.000000 gym_gui_tictactoe-0.1.1/setup.py
```

### Comparing `gym_gui_tictactoe-0.1/LICENSE.md` & `gym_gui_tictactoe-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gym_gui_tictactoe-0.1/gym_gui_tictactoe/envs/tictactoe_env.py` & `gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/envs/tictactoe_env.py`

 * *Files identical despite different names*

### Comparing `gym_gui_tictactoe-0.1/gym_gui_tictactoe/example/play_game_gui.py` & `gym_gui_tictactoe-0.1.1/gym_gui_tictactoe/example/play_game_gui.py`

 * *Files identical despite different names*

### Comparing `gym_gui_tictactoe-0.1/pyproject.toml` & `gym_gui_tictactoe-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym_gui_tictactoe"
-version = "0.1"
+version = "0.1.1"
 description = "An OpenAI gym environment for playing Tic Tac Toe with GUI"
 readme = "README.md"
 authors = [{ name = "AI Trafic Project" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["tictactoe", "gym"]
-dependencies = ["gym"]
-requires-python = ">=3.10"
+keywords = ["tictactoe", "gym", "pygame"]
+dependencies = ["gym", "pygame"]
+requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/fauzisho/T3_Env.git"
```

