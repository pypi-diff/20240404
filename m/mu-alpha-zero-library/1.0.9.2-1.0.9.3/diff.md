# Comparing `tmp/mu_alpha_zero_library-1.0.9.2.tar.gz` & `tmp/mu_alpha_zero_library-1.0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mu_alpha_zero_library-1.0.9.2.tar", last modified: Thu Mar 28 15:16:07 2024, max compression
+gzip compressed data, was "mu_alpha_zero_library-1.0.9.3.tar", last modified: Thu Apr  4 12:34:29 2024, max compression
```

## Comparing `mu_alpha_zero_library-1.0.9.2.tar` & `mu_alpha_zero_library-1.0.9.3.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.649665 mu_alpha_zero_library-1.0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-28 15:16:07.649665 mu_alpha_zero_library-1.0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.641665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.641665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.641665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/players.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.641665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/az_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/nnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    16702 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/alpha_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/asteroids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/tictactoe_game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/az_game.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/mz_game.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/JavaGateway/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/JavaGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/JavaGateway/java_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/JavaGateway/java_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_Arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_Arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_Arena/arena.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.645665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/Network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/Network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/Network/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/lazy_arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/muzero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/pickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/mem_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/prepare_for_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/root.root
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/save_best_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/start_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:16:07.649665 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-28 15:16:07.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-28 15:16:07.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:16:07.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-28 15:16:07.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 15:16:07.000000 mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:16:07.649665 mu_alpha_zero_library-1.0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-28 15:13:29.000000 mu_alpha_zero_library-1.0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4931 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/arena.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8548 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/players.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5473 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9589 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7370 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/nnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16326 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4501 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/alpha_zero.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5294 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/checkpointer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2593 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4590 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10972 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1349 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/asteroids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17301 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/tictactoe_game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/arena.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3070 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/az_game.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/mz_game.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3006 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/search_tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1685 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_callables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3004 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      321 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2982 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/arena.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7609 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10649 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/networks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      767 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/lazy_arrays.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4936 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/muzero.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/pickler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5023 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7017 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11244 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/mem_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/prepare_for_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5549 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/root.root
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/save_best_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/start_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/setup.py
```

### Comparing `mu_alpha_zero_library-1.0.9.2/LICENSE` & `mu_alpha_zero_library-1.0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/PKG-INFO` & `mu_alpha_zero_library-1.0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mu_alpha_zero_library
-Version: 1.0.9.2
+Version: 1.0.9.3
 Summary: Library for running and training MuZero and AlphaZero models.
 Home-page: https://github.com/Skirlax/MuAlphaZeroLibrary
 Author: Skyr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MuAlphaZeroLibrary
```

### Comparing `mu_alpha_zero_library-1.0.9.2/README.md` & `mu_alpha_zero_library-1.0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/arena.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/arena.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import time
 from typing import Type
 
 from mu_alpha_zero.AlphaZero.Arena.players import Player
 from mu_alpha_zero.Game.tictactoe_game import TicTacToeGameManager as GameManager
 from mu_alpha_zero.General.arena import GeneralArena
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.config import AlphaZeroConfig
 
 
 class Arena(GeneralArena):
-    def __init__(self, game_manager: GameManager, alpha_zero_config: AlphaZeroConfig, device):
+    def __init__(self, game_manager: GameManager, alpha_zero_config: AlphaZeroConfig, device,
+                 hook_manager: HookManager or None = None):
         self.game_manager = game_manager
         self.device = device
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         self.alpha_zero_config = alpha_zero_config
 
-    def pit(self, player1: Type[Player], player2: Type[Player],
-            num_games_to_play: int, num_mc_simulations: int, one_player: bool = False,
-            start_player: int = 1, add_to_kwargs: dict or None = None, debug: bool = False) -> tuple[int, int, int]:
+    def pit(self, player1: Type[Player], player2: Type[Player], num_games_to_play: int, num_mc_simulations: int,
+            one_player: bool = False, start_player: int = 1, add_to_kwargs: dict or None = None, debug: bool = False) -> \
+            tuple[int, int, int]:
         """
         Pit two players against each other for a given number of games and gather the results.
         :param start_player: Which player should start the game.
         :param one_player: If True always only the first player will start the game.
         :param player1:
         :param player2:
         :param num_games_to_play:
@@ -51,20 +55,20 @@
             if player2.name == "NetworkPlayer":
                 player2.monte_carlo_tree_search.step_root(None)
             # time.sleep(0.01)
             while True:
                 self.game_manager.render()
                 if current_player == 1:
                     # p1_time = time.time()
-                    move = player1.choose_move(state, **kwargs)
-                    # net_player_times.append(time.time() - p1_time)
+                    move = player1.choose_move(state, **kwargs)  # net_player_times.append(time.time() - p1_time)
                 else:
                     # p2_time = time.time()
-                    move = player2.choose_move(state, **kwargs)
-                    # minimax_player_times.append(time.time() - p2_time)
+                    move = player2.choose_move(state, **kwargs)  # minimax_player_times.append(time.time() - p2_time)
+                self.hook_manager.process_hook_executes(self, self.pit.__name__, __file__, HookAt.MIDDLE,
+                                                        args=(move, kwargs,current_player))
                 self.game_manager.play(current_player, move)
                 state = self.game_manager.get_board()
                 status = self.game_manager.game_result(current_player, state)
                 self.game_manager.render()
 
                 if status is not None:
                     # time.sleep(3)
@@ -93,10 +97,11 @@
                 kwargs["current_player"] = current_player
         # print(f"Average net player time: {sum(net_player_times) / len(net_player_times)}")
         # print(f"Average minimax player time: {sum(minimax_player_times) / len(minimax_player_times)}")
         # print(f"Net player times: {net_player_times}")
         # print(f"Minimax player times: {minimax_player_times}")
         return results["wins_p1"], results["wins_p2"], results["draws"]
 
+
     def wait_keypress(self):
         inpt = input("Press any key to continue...")
         return inpt
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Arena/players.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/players.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/az_node.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_node.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
 from mu_alpha_zero.AlphaZero.MCTS.az_node import AlphaZeroNode
 from mu_alpha_zero.AlphaZero.utils import augment_experience_with_symmetries, mask_invalid_actions
 from mu_alpha_zero.Game.tictactoe_game import TicTacToeGameManager
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralNetwork
 from mu_alpha_zero.General.search_tree import SearchTree
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.config import AlphaZeroConfig
 
 
 class McSearchTree(SearchTree):
-    def __init__(self, game_manager: TicTacToeGameManager, alpha_zero_config: AlphaZeroConfig):
+    def __init__(self, game_manager: TicTacToeGameManager, alpha_zero_config: AlphaZeroConfig,
+                 hook_manager: HookManager or None = None):
         self.game_manager = game_manager
         self.alpha_zero_config = alpha_zero_config
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         self.root_node = None
 
     def play_one_game(self, network: GeneralNetwork, device: th.device) -> tuple[list, int, int, int]:
         """
         Plays a single game using the Monte Carlo Tree Search algorithm.
 
         Args:
@@ -62,14 +66,16 @@
                 else:
                     game_history = [(x[0], x[1], r * current_player * x[3], x[3]) for x in game_history]
                 break
             current_player *= -1
 
         # game_history = make_channels(game_history)
         game_history = augment_experience_with_symmetries(game_history, self.game_manager.board_size)
+        self.hook_manager.process_hook_executes(self, self.play_one_game.__name__, __file__, HookAt.TAIL,
+                                                args=(game_history, results))
         return game_history, results["1"], results["-1"], results["D"]
 
     def search(self, network, state, current_player, device, tau=None):
         """
         Perform a Monte Carlo Tree Search on the current state starting with the current player.
         :param tau:
         :param network:
@@ -116,14 +122,16 @@
                 probabilities = mask_invalid_actions(probabilities, next_state, self.game_manager.board_size)
                 v = v.flatten().tolist()[0]
                 probabilities = probabilities.flatten().tolist()
                 current_node.expand(next_state, probabilities)
 
             self.backprop(v, path)
 
+        self.hook_manager.process_hook_executes(self, self.search.__name__, __file__, HookAt.TAIL,
+                                                args=(tau, self.root_node))
         return self.root_node.get_self_action_probabilities(tau=tau), None
 
     def backprop(self, v, path):
         """
         Backpropagates the value `v` through the search tree, updating the relevant nodes.
 
         Args:
@@ -168,26 +176,20 @@
 
     @staticmethod
     def parallel_self_play(nets: list, trees: list, memory: GeneralMemoryBuffer, device: th.device, num_games: int,
                            num_jobs: int):
         with Pool(num_jobs) as p:
             if not memory.is_disk:
                 results = p.starmap(p_self_play,
-                                    [(
-                                        nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs,
-                                        None)
-                                        for i in
-                                        range(len(nets))])
+                                    [(nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, None) for i in
+                                     range(len(nets))])
             else:
-                results = p.starmap(p_self_play,
-                                    [(
-                                        nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs,
-                                        copy.deepcopy(memory))
-                                        for i in
-                                        range(len(nets))])
+                results = p.starmap(p_self_play, [
+                    (nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, copy.deepcopy(memory)) for i in
+                    range(len(nets))])
         wins_p1, wins_p2, draws = 0, 0, 0
         for result in results:
             wins_p1 += result[0]
             wins_p2 += result[1]
             draws += result[2]
             if not memory.is_disk:
                 memory.add_list(result[3])
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/nnet.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/nnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 import numpy as np
 import torch as th
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.functional import mse_loss
 
 from mu_alpha_zero.General.network import GeneralAlphZeroNetwork
-from mu_alpha_zero.mem_buffer import MemBuffer
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.config import AlphaZeroConfig
+from mu_alpha_zero.mem_buffer import MemBuffer
 
 
 class AlphaZeroNet(nn.Module, GeneralAlphZeroNetwork):
-    def __init__(self, in_channels: int, num_channels: int, dropout: float, action_size: int, linear_input_size: int):
+    def __init__(self, in_channels: int, num_channels: int, dropout: float, action_size: int, linear_input_size: int,
+                 hook_manager: HookManager or None = None):
         super(AlphaZeroNet, self).__init__()
         self.in_channels = in_channels
         self.num_channels = num_channels
         self.dropout_p = dropout
         self.action_size = action_size
         self.linear_input_size = linear_input_size
-
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         # Convolutional layers
         self.conv1 = nn.Conv2d(in_channels, num_channels, 3, padding=1)
         self.bn1 = nn.BatchNorm2d(num_channels)
         self.conv2 = nn.Conv2d(num_channels, num_channels, 3, padding=1)
         self.bn2 = nn.BatchNorm2d(num_channels)
         self.conv3 = nn.Conv2d(num_channels, num_channels, 3, padding=1)
         self.bn3 = nn.BatchNorm2d(num_channels)
@@ -88,17 +91,17 @@
             os.remove(trace_file)
 
     def make_fresh_instance(self):
         return AlphaZeroNet(self.in_channels, self.num_channels, self.dropout_p, self.action_size,
                             self.linear_input_size)
 
     @staticmethod
-    def make_from_config(config: AlphaZeroConfig):
+    def make_from_config(config: AlphaZeroConfig, hook_manager: HookManager or None = None):
         return AlphaZeroNet(config.num_net_in_channels, config.num_net_channels, config.net_dropout,
-                            config.net_action_size, config.az_net_linear_input_size)
+                            config.net_action_size, config.az_net_linear_input_size, hook_manager=hook_manager)
 
     def train_net(self, memory_buffer: MemBuffer, alpha_zero_config: AlphaZeroConfig):
         from mu_alpha_zero.AlphaZero.utils import mask_invalid_actions_batch
         device = th.device("cuda" if th.cuda.is_available() else "cpu")
         losses = []
         optimizer = th.optim.Adam(self.parameters(), lr=alpha_zero_config.lr)
         memory_buffer.shuffle()
@@ -115,26 +118,32 @@
                 loss = mse_loss(v_pred, v) + self.pi_loss(pi_pred, pi, masks, device)
                 losses.append(loss.item())
                 # self.summary_writer.add_scalar("Loss", loss.item(), i * epochs + epoch)
 
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
+                self.hook_manager.process_hook_executes(self, self.train_net.__name__, __file__, HookAt.MIDDLE,
+                                                        args=(experience_batch, loss.item(), epoch))
 
+        self.hook_manager.process_hook_executes(self, self.train_net.__name__, __file__, HookAt.TAIL, args=(losses,))
         return sum(losses) / len(losses), losses
 
     def pi_loss(self, y_hat, y, masks, device: th.device):
         masks = masks.reshape(y_hat.shape).to(device)
         masked_y_hat = masks * y_hat
         return -th.sum(y * masked_y_hat) / y.size()[0]
 
     def to_shared_memory(self):
         for param in self.parameters():
             param.share_memory_()
 
+    def run_at_training_end(self):
+        self.hook_manager.process_hook_executes(self, self.run_at_training_end.__name__, __file__, HookAt.ALL)
+
 
 class TicTacToeNetNoNorm(nn.Module):
     def __init__(self, in_channels, num_channels, dropout, action_size):
         super(TicTacToeNetNoNorm, self).__init__()
         self.conv1 = nn.Conv2d(in_channels, num_channels, 3, padding=1)
         self.conv2 = nn.Conv2d(num_channels, num_channels, 3, padding=1)
         self.conv3 = nn.Conv2d(num_channels, num_channels, 3, padding=1)
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/Network/trainer.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,125 +6,113 @@
 from copy import deepcopy
 
 from typing import Type
 
 import torch as th
 from tqdm import tqdm
 from mu_alpha_zero.AlphaZero.Arena.arena import Arena
-from mu_alpha_zero.AlphaZero.Arena.players import RandomPlayer, Player,NetPlayer
+from mu_alpha_zero.AlphaZero.Arena.players import RandomPlayer, Player, NetPlayer
 from mu_alpha_zero.AlphaZero.MCTS.az_search_tree import McSearchTree
 from mu_alpha_zero.AlphaZero.Network.nnet import AlphaZeroNet
 from mu_alpha_zero.AlphaZero.checkpointer import CheckPointer
 from mu_alpha_zero.AlphaZero.logger import LoggingMessageTemplates, Logger
 from mu_alpha_zero.AlphaZero.utils import build_all_from_config
 from mu_alpha_zero.General.arena import GeneralArena
 from mu_alpha_zero.General.az_game import AlphaZeroGame
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralNetwork
 from mu_alpha_zero.General.search_tree import SearchTree
 from mu_alpha_zero.MuZero.JavaGateway.java_manager import JavaManager
 from mu_alpha_zero.config import Config
 from mu_alpha_zero.mem_buffer import MemBuffer
-
-
-# joblib.parallel.BACKENDS['multiprocessing'].use_dill = True
+from mu_alpha_zero.Hooks.hook_manager import HookManager
 
 
 class Trainer:
-    def __init__(self, network: GeneralNetwork, game: AlphaZeroGame,
-                 optimizer: th.optim, memory: GeneralMemoryBuffer,
-                 muzero_alphazero_config: Config, checkpointer: CheckPointer,
-                 search_tree: SearchTree, net_player: Player,
-                 device, headless: bool = True,
-                 opponent_network_override: th.nn.Module or None = None,
-                 arena_override: GeneralArena or None = None,
+    def __init__(self, network: GeneralNetwork, game: AlphaZeroGame, optimizer: th.optim, memory: GeneralMemoryBuffer,
+                 muzero_alphazero_config: Config, checkpointer: CheckPointer, search_tree: SearchTree,
+                 net_player: Player, hook_manager: HookManager or None, device, headless: bool = True,
+                 opponent_network_override: th.nn.Module or None = None, arena_override: GeneralArena or None = None,
                  java_manager: JavaManager = None) -> None:
         self.muzero_alphazero_config = muzero_alphazero_config
         self.device = device
         self.headless = headless
         self.game_manager = game
         self.mcts = search_tree
         self.net_player = net_player
         self.network = network
         self.opponent_network = self.network.make_fresh_instance() if opponent_network_override is None else opponent_network_override
         self.optimizer = optimizer
         self.memory = memory
         self.java_manager = java_manager
+        self.hook_manager = hook_manager
         self.arena = Arena(self.game_manager, self.muzero_alphazero_config,
-                           self.device) if arena_override is None else arena_override
+                           self.device,hook_manager=self.hook_manager) if arena_override is None else arena_override
         self.checkpointer = checkpointer
         self.logger = Logger(logdir=self.muzero_alphazero_config.log_dir,
                              token=self.muzero_alphazero_config.pushbullet_token)
         self.arena_win_frequencies = []
         self.losses = []
 
     @classmethod
     def from_checkpoint(cls, net_class: Type[GeneralNetwork], tree_class: Type[SearchTree],
-                        net_player_class: Type[Player],
-                        checkpoint_path: str, checkpoint_dir: str,
-                        game: AlphaZeroGame, headless: bool = True,
-                        checkpointer_verbose: bool = False,
-                        arena_override: GeneralArena or None = None,
+                        net_player_class: Type[Player], checkpoint_path: str, checkpoint_dir: str, game: AlphaZeroGame,
+                        headless: bool = True, hook_manager: HookManager or None = None,
+                        checkpointer_verbose: bool = False, arena_override: GeneralArena or None = None,
                         mem: GeneralMemoryBuffer or None = None):
         device = th.device("cuda" if th.cuda.is_available() else "cpu")
         checkpointer = CheckPointer(checkpoint_dir, verbose=checkpointer_verbose)
 
         network_dict, optimizer_dict, memory, lr, args, opponent_dict = checkpointer.load_checkpoint_from_path(
             checkpoint_path)
         conf = Config.from_args(args)
-        tree = tree_class(game.make_fresh_instance(), conf)
+        tree = tree_class(game.make_fresh_instance(), conf, hook_manager=hook_manager)
         if "fc1.weight" in network_dict:
             conf.az_net_linear_input_size = network_dict["fc1.weight"].shape[1]
-        network = net_class.make_from_config(conf).to(device)
+        network = net_class.make_from_config(conf, hook_manager=hook_manager).to(device)
         opponent_network = network.make_fresh_instance().to(device)
         optimizer = th.optim.Adam(network.parameters(), lr=lr)
         # opponent_network = build_net_from_args(args, device)
         net_player = net_player_class(game.make_fresh_instance(),
                                       **{"network": network, "monte_carlo_tree_search": tree})
         network.load_state_dict(network_dict)
         opponent_network.load_state_dict(opponent_dict)
 
         try:
             optimizer.load_state_dict(optimizer_dict)
         except ValueError:
             print("Couldn't load optimizer dict.")
         if memory is None:
             memory = mem
-        return cls(network, game, optimizer, memory, conf, checkpointer, tree, net_player, device, headless=headless,
-                   arena_override=arena_override)
+        return cls(network, game, optimizer, memory, conf, checkpointer, tree, net_player, hook_manager, device,
+                   headless=headless, arena_override=arena_override)
 
     @classmethod
     def create(cls, muzero_alphazero_config: Config, game: AlphaZeroGame, network: GeneralNetwork,
-               search_tree: SearchTree,
-               net_player: Player,
-               headless: bool = True,
-               checkpointer_verbose: bool = False,
-               arena_override: GeneralArena or None = None,
-               memory_override: GeneralMemoryBuffer or None = None,
-               java_manager: JavaManager or None = None):
+               search_tree: SearchTree, net_player: Player, headless: bool = True, checkpointer_verbose: bool = False,
+               hook_manager: HookManager or None = None, arena_override: GeneralArena or None = None,
+               memory_override: GeneralMemoryBuffer or None = None, java_manager: JavaManager or None = None):
         device = th.device("cuda" if th.cuda.is_available() else "cpu")
         _, optimizer, mem = build_all_from_config(muzero_alphazero_config, device)
         memory = mem if memory_override is None else memory_override
         checkpointer = CheckPointer(muzero_alphazero_config.checkpoint_dir, verbose=checkpointer_verbose)
         return cls(network, game, optimizer, memory, muzero_alphazero_config, checkpointer, search_tree, net_player,
-                   device,
-                   headless=headless, arena_override=arena_override, java_manager=java_manager)
+                   hook_manager, device, headless=headless, arena_override=arena_override, java_manager=java_manager)
 
     @classmethod
     def from_state_dict(cls, path: str, muzero_alphazero_config: Config, game: AlphaZeroGame, search_tree: SearchTree,
-                        headless: bool = True,
+                        headless: bool = True, hook_manager: HookManager or None = None,
                         checkpointer_verbose: bool = False, java_manager: JavaManager or None = None):
         device = th.device("cuda" if th.cuda.is_available() else "cpu")
         net, optimizer, memory = build_all_from_config(muzero_alphazero_config, device)
         checkpointer = CheckPointer(muzero_alphazero_config.checkpoint_dir, verbose=checkpointer_verbose)
         net.load_state_dict(th.load(path))
         net_player = NetPlayer(game.make_fresh_instance(), **{"network": net, "monte_carlo_tree_search": search_tree})
-        return cls(net, game, optimizer, memory, muzero_alphazero_config, checkpointer, search_tree, net_player, device,
-                   headless=headless,
-                   java_manager=java_manager)
+        return cls(net, game, optimizer, memory, muzero_alphazero_config, checkpointer, search_tree, net_player,
+                   hook_manager, device, headless=headless, java_manager=java_manager)
 
     def train(self) -> AlphaZeroNet:
         self.opponent_network.to(self.device)
         self.logger.log(LoggingMessageTemplates.TRAINING_START(self.muzero_alphazero_config.num_iters))
         self.opponent_network.load_state_dict(self.network.state_dict())
         # self.checkpointer.save_state_dict_checkpoint(self.network, "h_search_network")
         num_iters = self.muzero_alphazero_config.num_iters
@@ -138,18 +126,16 @@
                 self.muzero_alphazero_config.arena_tau = 0
             with th.no_grad():
                 n_jobs = self.muzero_alphazero_config.num_workers
                 self.logger.log(LoggingMessageTemplates.SELF_PLAY_START(self_play_games))
 
                 if self.muzero_alphazero_config.num_workers > 1:
                     wins_p1, wins_p2, game_draws = self.mcts.parallel_self_play(self.make_n_networks(n_jobs),
-                                                                                self.make_n_trees(n_jobs),
-                                                                                self.memory, self.device,
-                                                                                self_play_games,
-                                                                                n_jobs)
+                                                                                self.make_n_trees(n_jobs), self.memory,
+                                                                                self.device, self_play_games, n_jobs)
                     if isinstance(self.memory, MemBuffer) and self.memory.is_disk and self.memory.full_disk:
                         self.memory = self.memory.make_fresh_instance()
                 else:
                     wins_p1, wins_p2, game_draws = self.mcts.self_play(self.network, self.device, self_play_games,
                                                                        self.memory)
                 self.logger.log(LoggingMessageTemplates.SELF_PLAY_END(wins_p1, wins_p2, game_draws, not_zero))
                 self.logger.pushbullet_log("Finished self-play.")
@@ -171,23 +157,21 @@
 
             num_games = self.muzero_alphazero_config.num_pit_games
             update_threshold = self.muzero_alphazero_config.update_threshold
             p1_wins, p2_wins, draws, wins_total = self.run_pitting(num_simulations, num_games)
             self.check_model(p1_wins, wins_total, update_threshold, i)
             self.run_pitting_random(num_simulations, num_games, i)
 
-        important_args = {
-            "numIters": self.muzero_alphazero_config.num_iters,
-            "numSelfPlayGames": self.muzero_alphazero_config.self_play_games,
-            "tau": self.muzero_alphazero_config.tau,
-            "updateThreshold": self.muzero_alphazero_config.update_threshold,
-            "mcSimulations": self.muzero_alphazero_config.num_simulations,
-            "c": self.muzero_alphazero_config.c,
-            "numPitGames": self.muzero_alphazero_config.num_pit_games
-        }
+        important_args = {"numIters": self.muzero_alphazero_config.num_iters,
+                          "numSelfPlayGames": self.muzero_alphazero_config.self_play_games,
+                          "tau": self.muzero_alphazero_config.tau,
+                          "updateThreshold": self.muzero_alphazero_config.update_threshold,
+                          "mcSimulations": self.muzero_alphazero_config.num_simulations,
+                          "c": self.muzero_alphazero_config.c,
+                          "numPitGames": self.muzero_alphazero_config.num_pit_games}
 
         self.logger.log(LoggingMessageTemplates.TRAINING_END(important_args))
         self.logger.pushbullet_log(LoggingMessageTemplates.TRAINING_END_PSB())
         return self.network
 
     def make_n_networks(self, n: int) -> list[AlphaZeroNet]:
         """
@@ -214,22 +198,17 @@
     def get_arena_win_frequencies_mean(self):
         return sum(self.arena_win_frequencies) / not_zero(len(self.arena_win_frequencies))
 
     def save_latest(self, path):
         state_dict = self.network.state_dict()
         opponent_state_dict = self.opponent_network.state_dict()
         optimizer_state_dict = self.optimizer.state_dict()
-        th.save({
-            'optimizer': optimizer_state_dict,
-            'memory': self.memory,
-            'lr': self.muzero_alphazero_config.lr,
-            'net': state_dict,
-            'opponent_state_dict': opponent_state_dict,
-            'args': self.muzero_alphazero_config.to_dict()
-        }, path)
+        th.save({'optimizer': optimizer_state_dict, 'memory': self.memory, 'lr': self.muzero_alphazero_config.lr,
+                 'net': state_dict, 'opponent_state_dict': opponent_state_dict,
+                 'args': self.muzero_alphazero_config.to_dict()}, path)
         print("Saved latest model data to {}".format(path))
 
     def make_tqdm_bar(self, iterable, desc, position, leave=True):
         if self.muzero_alphazero_config.show_tqdm:
             return tqdm(iterable, desc=desc, position=position, leave=leave)
         else:
             return iterable
@@ -250,16 +229,15 @@
         p1.set_network(self.network)
         p2 = self.net_player.make_fresh_instance()
         p2.set_network(self.opponent_network)
         self.logger.log(LoggingMessageTemplates.PITTING_START(p1.name, p2.name, num_games))
         p1_wins, p2_wins, draws = self.arena.pit(p1, p2, num_games, num_mc_simulations=num_simulations,
                                                  one_player=False)
         wins_total = not_zero(p1_wins + p2_wins)
-        self.logger.log(LoggingMessageTemplates.PITTING_END(p1.name, p2.name, p1_wins,
-                                                            p2_wins, wins_total, draws))
+        self.logger.log(LoggingMessageTemplates.PITTING_END(p1.name, p2.name, p1_wins, p2_wins, wins_total, draws))
         self.arena_win_frequencies.append(p1_wins / num_games)
         return p1_wins, p2_wins, draws, wins_total
 
     def run_pitting_random(self, num_simulations: int, num_games: int, i: int):
         if i % self.muzero_alphazero_config.random_pit_freq != 0:
             return
         self.network.eval()
@@ -269,35 +247,31 @@
             p1 = self.net_player.make_fresh_instance()
             p1.set_network(self.network)
             self.logger.log(LoggingMessageTemplates.PITTING_START(p1.name, random_player.name, num_games))
             p1_wins_random, p2_wins_random, draws_random = self.arena.pit(p1, random_player, num_games,
                                                                           num_mc_simulations=num_simulations)
             wins_total = not_zero(p1_wins_random + p2_wins_random)
             self.logger.log(
-                LoggingMessageTemplates.PITTING_END(p1.name, random_player.name, p1_wins_random,
-                                                    p2_wins_random, wins_total, draws_random))
+                LoggingMessageTemplates.PITTING_END(p1.name, random_player.name, p1_wins_random, p2_wins_random,
+                                                    wins_total, draws_random))
 
     def check_model(self, p1_wins: int, wins_total: int, update_threshold: float, i: int):
         if p1_wins / wins_total > update_threshold:
-            self.logger.log(LoggingMessageTemplates.MODEL_ACCEPT(p1_wins / wins_total,
-                                                                 update_threshold))
+            self.logger.log(LoggingMessageTemplates.MODEL_ACCEPT(p1_wins / wins_total, update_threshold))
             self.checkpointer.save_checkpoint(self.network, self.opponent_network, self.optimizer,
-                                              self.muzero_alphazero_config.lr, i,
-                                              self.muzero_alphazero_config)
-            self.logger.log(LoggingMessageTemplates.SAVED("accepted model checkpoint",
-                                                          self.checkpointer.get_checkpoint_dir()))
+                                              self.muzero_alphazero_config.lr, i, self.muzero_alphazero_config)
+            self.logger.log(
+                LoggingMessageTemplates.SAVED("accepted model checkpoint", self.checkpointer.get_checkpoint_dir()))
         else:
-            self.logger.log(LoggingMessageTemplates.MODEL_REJECT(p1_wins / wins_total,
-                                                                 update_threshold))
+            self.logger.log(LoggingMessageTemplates.MODEL_REJECT(p1_wins / wins_total, update_threshold))
             self.checkpointer.load_temp_net_checkpoint(self.network)
-            self.logger.log(LoggingMessageTemplates.LOADED("previous version checkpoint",
-                                                           self.checkpointer.get_temp_path()))
+            self.logger.log(
+                LoggingMessageTemplates.LOADED("previous version checkpoint", self.checkpointer.get_temp_path()))
         self.logger.pushbullet_log(LoggingMessageTemplates.ITER_FINISHED_PSB(i))
 
     def self_play_get_r_mean(self):
         self.network.eval()
         self.mcts.parallel_self_play(self.make_n_networks(self.muzero_alphazero_config.num_workers),
-                                     self.make_n_trees(self.muzero_alphazero_config.num_workers),
-                                     self.memory, self.device,
-                                     self.muzero_alphazero_config.self_play_games,
+                                     self.make_n_trees(self.muzero_alphazero_config.num_workers), self.memory,
+                                     self.device, self.muzero_alphazero_config.self_play_games,
                                      self.muzero_alphazero_config.num_workers)
         return sum([x[2][0] for x in self.memory.buffer]) / not_zero(len(self.memory.buffer))
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/alpha_zero.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/alpha_zero.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,58 +8,59 @@
 from mu_alpha_zero.AlphaZero.Arena.players import NetPlayer
 from mu_alpha_zero.AlphaZero.MCTS.az_search_tree import McSearchTree
 from mu_alpha_zero.AlphaZero.Network.trainer import Trainer
 from mu_alpha_zero.General.az_game import AlphaZeroGame
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralNetwork
 from mu_alpha_zero.General.utils import net_not_none, find_project_root
+from mu_alpha_zero.Hooks.hook_manager import HookManager
 from mu_alpha_zero.config import AlphaZeroConfig
 
 
 class AlphaZero:
     def __init__(self, game_instance: AlphaZeroGame):
         self.trainer = None
         self.net = None
         self.game = game_instance
         self.device = th.device("cuda" if th.cuda.is_available() else "cpu")
         self.alpha_zero_config: AlphaZeroConfig = None
         self.tree: McSearchTree = None
 
     def create_new(self, alpha_zero_config: AlphaZeroConfig, network_class: Type[GeneralNetwork],
-                   memory: GeneralMemoryBuffer,
-                   headless: bool = True,
+                   memory: GeneralMemoryBuffer, headless: bool = True, hook_manager: HookManager or None = None,
                    checkpointer_verbose: bool = False):
-        network = network_class.make_from_config(alpha_zero_config).to(self.device)
+        network = network_class.make_from_config(alpha_zero_config,hook_manager=hook_manager).to(self.device)
         tree = McSearchTree(self.game.make_fresh_instance(), alpha_zero_config)
         self.tree = tree
         net_player = NetPlayer(self.game.make_fresh_instance(), **{"network": network, "monte_carlo_tree_search": tree})
         self.alpha_zero_config = alpha_zero_config
         self.trainer = Trainer.create(alpha_zero_config, self.game, network, tree, net_player, headless=headless,
-                                      checkpointer_verbose=checkpointer_verbose, memory_override=memory)
+                                      checkpointer_verbose=checkpointer_verbose, memory_override=memory,
+                                      hook_manager=hook_manager)
         self.net = self.trainer.get_network()
 
     def load_checkpoint(self, network_class: Type[GeneralNetwork], path: str, checkpoint_dir: str,
-                        headless: bool = True,
+                        headless: bool = True, hook_manager: HookManager or None = None,
                         checkpointer_verbose: bool = False):
         self.trainer = Trainer.from_checkpoint(network_class, McSearchTree, NetPlayer, path, checkpoint_dir, self.game,
-                                               headless=headless,
+                                               headless=headless, hook_manager=hook_manager,
                                                checkpointer_verbose=checkpointer_verbose)
         self.net = self.trainer.get_network()
         self.tree = self.trainer.get_tree()
         self.args = self.trainer.get_args()
 
     def train(self):
         net_not_none(self.net)
         self.trainer.train()
 
     def predict(self, x: np.ndarray, tau: float = 0) -> int:
         net_not_none(self.net)
-        assert x.shape == (self.args["board_size"], self.args["board_size"], self.args["num_net_in_channels"]), \
-            "Input shape is not correct. Expected (board_size, board_size, num_net_in_channels)." \
-            "Got: " + str(x.shape)
+        assert x.shape == (self.args["board_size"], self.args["board_size"], self.args[
+            "num_net_in_channels"]), "Input shape is not correct. Expected (board_size, board_size, num_net_in_channels)." \
+                                     "Got: " + str(x.shape)
         pi, _ = self.tree.search(self.net, x, 1, self.device, tau=tau)
         return self.game.select_move(pi)
 
     def play(self, p1_name: str, p2_name: str, num_games: int, alpha_zero_config: AlphaZeroConfig, starts: int = 1,
              switch_players: bool = True):
         net_not_none(self.net)
         self.net.to(self.device)
@@ -73,8 +74,7 @@
         p2 = sys.modules[f"{path_prefix}.AlphaZero.Arena.players"].__dict__[p2_name](manager, **kwargs)
         arena_manager = self.game.make_fresh_instance()
         arena_manager.set_headless(False)
         arena = Arena(arena_manager, alpha_zero_config, self.device)
         p1_w, p2_w, ds = arena.pit(p1, p2, num_games, alpha_zero_config.num_simulations, one_player=not switch_players,
                                    start_player=starts, add_to_kwargs=kwargs)
         print(f"Results: Player 1 wins: {p1_w}, Player 2 wins: {p2_w}, Draws: {ds}")
-
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/checkpointer.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/checkpointer.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/constants.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/constants.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/logger.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/logger.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/AlphaZero/utils.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/utils.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/asteroids.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/asteroids.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/Game/tictactoe_game.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/tictactoe_game.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/az_game.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/az_game.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/memory.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/memory.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/mz_game.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/mz_game.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/network.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from abc import ABC, abstractmethod
+
+from mu_alpha_zero.Hooks.hook_manager import HookManager
 from mu_alpha_zero.config import Config
 import torch as th
 
 
 class GeneralNetwork(ABC):
     @abstractmethod
     def make_fresh_instance(self):
         """
         Returns a fresh instance of the network
         """
         pass
 
     @classmethod
     @abstractmethod
-    def make_from_config(cls, config: Config):
+    def make_from_config(cls, config: Config,hook_manager: HookManager or None = None):
         """
         Builds the network from the given arguments dict.
         """
         pass
 
     @abstractmethod
     def train_net(self, memory_buffer, muzero_alphazero_config: Config) -> tuple[float, list[float]]:
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/search_tree.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/search_tree.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/General/utils.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/utils.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/JavaGateway/java_manager.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_manager.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_Arena/arena.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/arena.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 from typing import Type
 
 import torch as th
 
 from mu_alpha_zero.AlphaZero.Arena.players import Player
 from mu_alpha_zero.General.arena import GeneralArena
 from mu_alpha_zero.General.mz_game import MuZeroGame
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.MuZero.utils import resize_obs, scale_state
 from mu_alpha_zero.config import MuZeroConfig
 
 
 class MzArena(GeneralArena):
-    def __init__(self, game_manager: MuZeroGame, muzero_config: MuZeroConfig, device: th.device):
+    def __init__(self, game_manager: MuZeroGame, muzero_config: MuZeroConfig, device: th.device,
+                 hook_manager: HookManager or None = None):
         self.game_manager = game_manager
         self.muzero_config = muzero_config
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         self.device = device
 
     def pit(self, player1: Type[Player], player2: Type[Player], num_games_to_play: int, num_mc_simulations: int,
             one_player: bool = False, start_player: int = 1):
         tau = self.muzero_config.arena_tau
         rewards = {1: [], -1: []}
         if one_player:
@@ -28,16 +32,15 @@
         players = {"1": player1, "-1": player2}
         for player in [1, -1]:
             kwargs = {"num_simulations": num_mc_simulations, "current_player": player, "device": self.device,
                       "tau": tau, "unravel": False}
             for game in range(num_games_per_player):
                 self.game_manager.reset()
 
-                state, _, _ = self.game_manager.frame_skip_step(self.game_manager.get_noop(), None,
-                                                                frame_skip=noop_num)
+                state, _, _ = self.game_manager.frame_skip_step(self.game_manager.get_noop(), None, frame_skip=noop_num)
                 state = resize_obs(state, self.muzero_config.target_resolution)
                 state = scale_state(state)
                 for step in range(self.muzero_config.num_steps):
                     self.game_manager.render()
                     move = players[str(player)].choose_move(state, **kwargs)
 
                     state, reward, done = self.game_manager.frame_skip_step(move, None)
@@ -48,8 +51,12 @@
                     except AttributeError:
                         # Player is probably not net player and doesn't have monte_carlo_tree_search.
                         pass
                     rewards[player].append(reward)
                     if done:
                         break
 
+        self.hook_manager.process_hook_executes(self, self.pit.__name__, __file__, HookAt.TAIL, (rewards, kwargs))
         return sum(rewards[1]), sum(rewards[-1]), 0
+
+    def run_on_training_end(self):
+        self.hook_manager.process_hook_executes(self, self.run_on_training_end.__name__, __file__, HookAt.ALL)
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import copy
 import gc
-from multiprocessing import Pool
+from torch.multiprocessing import Pool
 
 import numpy as np
 import torch as th
 
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.mz_game import MuZeroGame
 from mu_alpha_zero.General.search_tree import SearchTree
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.MuZero.MZ_MCTS.mz_node import MzAlphaZeroNode
 from mu_alpha_zero.MuZero.Network.networks import MuZeroNet
 from mu_alpha_zero.MuZero.lazy_arrays import LazyArray
-from mu_alpha_zero.MuZero.utils import match_action_with_obs, resize_obs, scale_action, scale_reward, scale_state
+from mu_alpha_zero.MuZero.utils import match_action_with_obs, resize_obs, scale_action, scale_reward, scale_state,scale_hidden_state
 from mu_alpha_zero.config import MuZeroConfig
 from mu_alpha_zero.mem_buffer import MuZeroFrameBuffer
 
 
 class MuZeroSearchTree(SearchTree):
 
-    def __init__(self, game_manager: MuZeroGame, muzero_config: MuZeroConfig):
+    def __init__(self, game_manager: MuZeroGame, muzero_config: MuZeroConfig, hook_manager: HookManager or None = None):
         self.game_manager = game_manager
         self.muzero_config = muzero_config
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         self.buffer = MuZeroFrameBuffer(self.muzero_config.frame_buffer_size, self.game_manager.get_noop(),
                                         self.muzero_config.net_action_size)
         self.min_max_q = [float("inf"), -float("inf")]
 
     def play_one_game(self, network_wrapper: MuZeroNet, device: th.device, dir_path: str or None = None) -> list:
         num_steps = self.muzero_config.num_steps
         frame_skip = self.muzero_config.frame_skip
@@ -59,14 +62,15 @@
         num_simulations = self.muzero_config.num_simulations
         if tau is None:
             tau = self.muzero_config.tau
 
         root_node = MzAlphaZeroNode()
         state_ = network_wrapper.representation_forward(
             self.buffer.concat_frames().permute(2, 0, 1).unsqueeze(0)).squeeze(0)
+        state_ = scale_hidden_state(state_)
         pi, v = network_wrapper.prediction_forward(state_.unsqueeze(0), predict=True)
         pi = pi.flatten().tolist()
         root_node.expand_node(state_, pi, 0)
         for simulation in range(num_simulations):
             current_node = root_node
             path = [current_node]
             action = None
@@ -75,25 +79,28 @@
                 path.append(current_node)
 
             action = scale_action(action, self.game_manager.get_num_actions())
 
             current_node_state_with_action = match_action_with_obs(current_node.parent().state, action)
             next_state, reward = network_wrapper.dynamics_forward(current_node_state_with_action.unsqueeze(0),
                                                                   predict=True)
+            next_state = scale_hidden_state(next_state)
             reward = reward[0][0]
             v = self.game_manager.game_result(current_node.current_player)
             if v is None or not v:
                 pi, v = network_wrapper.prediction_forward(next_state.unsqueeze(0), predict=True)
                 pi = pi.flatten().tolist()
                 v = v.flatten().tolist()[0]
                 current_node.expand_node(next_state, pi, reward)
             self.backprop(v, path)
 
         action_probs = root_node.get_self_action_probabilities(tau=tau)
         root_val_latent = (root_node.get_self_value(), root_node.get_latent())
+        self.hook_manager.process_hook_executes(self, self.search.__name__, __file__, HookAt.TAIL,
+                                                args=(action_probs, root_val_latent, root_node))
         root_node = None
         return action_probs, root_val_latent
 
     def backprop(self, v, path):
         G = 0
         gamma = self.muzero_config.gamma
         for node in reversed(path):
@@ -110,15 +117,16 @@
         for game in range(num_games):
             game_results = self.play_one_game(net, device)
             memory.add_list(game_results)
 
         return None, None, None
 
     def make_fresh_instance(self):
-        return MuZeroSearchTree(self.game_manager.make_fresh_instance(), copy.deepcopy(self.muzero_config))
+        return MuZeroSearchTree(self.game_manager.make_fresh_instance(), copy.deepcopy(self.muzero_config),
+                                hook_manager=self.hook_manager)
 
     def step_root(self, action: int or None):
         # I am never reusing the tree in MuZero.
         pass
 
     def update_min_max_q(self, q):
         self.min_max_q[0] = min(self.min_max_q[0], q)
@@ -126,25 +134,28 @@
 
     @staticmethod
     def parallel_self_play(nets: list, trees: list, memory: GeneralMemoryBuffer, device: th.device, num_games: int,
                            num_jobs: int):
         with Pool(num_jobs) as p:
             if memory.is_disk and memory.full_disk:
                 results = p.starmap(p_self_play, [
-                    (nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, copy.deepcopy(memory),None) for i in
-                    range(len(nets))])
+                    (nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, copy.deepcopy(memory), None) for i
+                    in range(len(nets))])
             else:
-                results = p.starmap(p_self_play,
-                                    [(nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, None,memory.dir_path) for i in
-                                     range(len(nets))])
+                results = p.starmap(p_self_play, [
+                    (nets[i], trees[i], copy.deepcopy(device), num_games // num_jobs, None, memory.dir_path) for i in
+                    range(len(nets))])
         for result in results:
             memory.add_list(result)
 
         return None, None, None
 
+    def run_on_training_end(self):
+        self.hook_manager.process_hook_executes(self, self.run_on_training_end.__name__, __file__, HookAt.ALL)
+
 
 def p_self_play(net, tree, dev, num_g, mem, dir_path: str or None = None):
     data = []
     for _ in range(num_g):
         game_results = tree.play_one_game(net, dev, dir_path=dir_path)
         if mem is not None:
             mem.add_list(game_results)
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/Network/networks.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/networks.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,43 +5,46 @@
 import torch.nn.functional as F
 from torch import nn
 from torch.nn.functional import mse_loss
 
 from mu_alpha_zero.AlphaZero.Network.nnet import AlphaZeroNet as PredictionNet
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralMuZeroNetwork
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.MuZero.utils import match_action_with_obs_batch, scale_reward_value
 from mu_alpha_zero.config import MuZeroConfig
 
 
 class MuZeroNet(th.nn.Module, GeneralMuZeroNetwork):
     def __init__(self, input_channels: int, dropout: float, action_size: int, num_channels: int, latent_size: int,
-                 num_out_channels: int, linear_input_size: int):
+                 num_out_channels: int, linear_input_size: int, hook_manager: HookManager or None = None):
         super(MuZeroNet, self).__init__()
         self.input_channels = input_channels
         self.dropout = dropout
         self.device = th.device("cuda" if th.cuda.is_available() else "cpu")
         self.action_size = action_size
         self.num_channels = num_channels
         self.latent_size = latent_size
         self.num_out_channels = num_out_channels
         self.linear_input_size = linear_input_size
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         # self.action_embedding = th.nn.Embedding(action_size, 256)
         self.representation_network = RepresentationNet()
         self.dynamics_network = DynamicsNet(in_channels=257, num_channels=num_channels, dropout=dropout,
                                             latent_size=latent_size, out_channels=num_out_channels)
         # prediction outputs 6x6 latent state
         self.prediction_network = PredictionNet(in_channels=256, num_channels=num_channels, dropout=dropout,
                                                 action_size=action_size, linear_input_size=linear_input_size)
 
     @classmethod
-    def make_from_config(cls, config: MuZeroConfig):
-        return cls(config.num_net_in_channels, config.net_dropout, config.net_action_size,
-                   config.num_net_channels, config.net_latent_size, config.num_net_out_channels,
-                   config.az_net_linear_input_size)
+    def make_from_config(cls, config: MuZeroConfig, hook_manager: HookManager or None = None):
+        return cls(config.num_net_in_channels, config.net_dropout, config.net_action_size, config.num_net_channels,
+                   config.net_latent_size, config.num_net_out_channels, config.az_net_linear_input_size,
+                   hook_manager=hook_manager)
 
     def dynamics_forward(self, x: th.Tensor, predict: bool = False):
         if predict:
             return self.dynamics_network.predict(x)
         state, reward = self.dynamics_network(x)
         reward = scale_reward_value(reward)
         return state, reward
@@ -57,21 +60,22 @@
 
     def representation_forward(self, x: th.Tensor):
         x = self.representation_network(x)
         return x
 
     def make_fresh_instance(self):
         return MuZeroNet(self.input_channels, self.dropout, self.action_size, self.num_channels, self.latent_size,
-                         self.num_out_channels, self.linear_input_size)
+                         self.num_out_channels, self.linear_input_size, hook_manager=self.hook_manager)
 
     def train_net(self, memory_buffer: GeneralMemoryBuffer, muzero_config: MuZeroConfig) -> tuple[float, list[float]]:
         device = th.device("cuda" if th.cuda.is_available() else "cpu")
         losses = []
         K = muzero_config.K
         optimizer = th.optim.Adam(self.parameters(), lr=muzero_config.lr)
+        iteration = 0
         for experience_batch, priorities in memory_buffer.batch_with_priorities(muzero_config.epochs,
                                                                                 muzero_config.batch_size, K,
                                                                                 alpha=muzero_config.alpha):
             if len(experience_batch) <= 1:
                 continue
             pis, vs, rews_moves, states = zip(*experience_batch)
             rews = [x[0] for x in rews_moves]
@@ -95,22 +99,31 @@
             loss_pi = self.muzero_pi_loss(pred_pis, pis) * balance_term * w
             loss_r = mse_loss(pred_rews, rews) * balance_term * w
             loss = loss_v.sum() + loss_pi.sum() + loss_r.sum()
             losses.append(loss.item())
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
+            self.hook_manager.process_hook_executes(self, self.train_net.__name__, __file__, HookAt.MIDDLE, args=(
+                experience_batch, loss.item(), loss_v, loss_pi, loss_r,
+                iteration))
+            iteration += 1
+        self.hook_manager.process_hook_executes(self, self.train_net.__name__, __file__, HookAt.TAIL,
+                                                args=(memory_buffer, losses))
         return sum(losses) / len(losses), losses
 
     def muzero_pi_loss(self, y_hat, y):
         return -th.sum(y * y_hat) / y.size()[0]
 
     def to_pickle(self, path: str):
         th.save(self, path)
 
+    def run_on_training_end(self):
+        self.hook_manager.process_hook_executes(self, self.run_on_training_end.__name__, __file__, HookAt.ALL)
+
 
 class RepresentationNet(th.nn.Module):
     def __init__(self):
         super(RepresentationNet, self).__init__()
         self.device = th.device("cuda" if th.cuda.is_available() else "cpu")
         self.conv1 = th.nn.Conv2d(in_channels=128, out_channels=128, kernel_size=3, stride=2, padding=1)
         self.residuals1 = th.nn.ModuleList([ResidualBlock(128) for _ in range(2)])
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/muzero.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/muzero.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from mu_alpha_zero.General.mz_game import MuZeroGame
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralNetwork
 from mu_alpha_zero.MuZero.MZ_Arena.arena import MzArena
 from mu_alpha_zero.MuZero.MZ_MCTS.mz_search_tree import MuZeroSearchTree
 from mu_alpha_zero.mem_buffer import PickleMemBuffer
 from mu_alpha_zero.config import MuZeroConfig
-
+from mu_alpha_zero.Hooks.hook_manager import HookManager
 
 class MuZero:
     """
     Class for managing the training and creation of a MuZero model.
 
     Attributes:
         game_manager (MuZeroGame): The game manager instance.
@@ -46,43 +46,47 @@
         self.net = None
         self.trainer = None
         self.device = th.device("cuda" if th.cuda.is_available() else "cpu")
         self.tree = None
         self.muzero_config = None
 
     def create_new(self, muzero_config: MuZeroConfig, network_class: Type[GeneralNetwork], memory: GeneralMemoryBuffer,
+                   hook_manager: HookManager or None = None,
                    headless: bool = True,
                    checkpointer_verbose: bool = False):
         muzero_config.net_action_size = int(self.game_manager.get_num_actions())
         if not os.path.isabs(muzero_config.pickle_dir):
             muzero_config.pickle_dir = find_project_root() + "/" + muzero_config.pickle_dir
         self.muzero_config = muzero_config
-        network = network_class.make_from_config(muzero_config).to(self.device)
+        network = network_class.make_from_config(muzero_config,hook_manager=hook_manager).to(self.device)
         self.tree = MuZeroSearchTree(self.game_manager.make_fresh_instance(), muzero_config)
 
         net_player = NetPlayer(self.game_manager.make_fresh_instance(),
                                **{"network": network, "monte_carlo_tree_search": self.tree})
 
         arena = MzArena(self.game_manager.make_fresh_instance(), self.muzero_config, self.device)
         java_manager = None
         self.trainer = Trainer.create(self.muzero_config, self.game_manager.make_fresh_instance(), network, self.tree,
                                       net_player,
                                       headless=headless,
                                       checkpointer_verbose=checkpointer_verbose, arena_override=arena,
+                                      hook_manager=hook_manager,
                                       memory_override=memory, java_manager=java_manager)
         self.net = self.trainer.get_network()
 
     def from_checkpoint(self, network_class: Type[GeneralNetwork], memory: GeneralMemoryBuffer, path: str,
                         checkpoint_dir: str,
                         headless: bool = True,
+                        hook_manager: HookManager or None = None,
                         checkpointer_verbose: bool = False):
         self.trainer = Trainer.from_checkpoint(network_class, MuZeroSearchTree, NetPlayer, path,
                                                checkpoint_dir,
                                                self.game_manager,
                                                headless=headless,
+                                               hook_manager=hook_manager,
                                                checkpointer_verbose=checkpointer_verbose,
                                                mem=memory)
         self.net = self.trainer.get_network()
         self.tree = self.trainer.get_tree()
         self.args = self.trainer.get_args()
 
     def train(self):
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/pickler.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/pickler.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/MuZero/utils.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import math
 
 import numpy as np
 import optuna
 import torch as th
 from PIL import Image
-
 from mu_alpha_zero.config import MuZeroConfig
 
 
 def add_actions_to_obs(observations: th.Tensor, actions: th.Tensor, dim=0):
     return th.cat((observations, actions), dim=dim)
 
 
@@ -37,14 +36,18 @@
     return state / 255
 
 
 def scale_action(action: int, num_actions: int):
     return action / (num_actions - 1)
 
 
+def scale_hidden_state(hidden_state: th.Tensor):
+    return (hidden_state - th.min(hidden_state)) / (th.max(hidden_state) - th.min(hidden_state))
+
+
 def scale_reward_value(value: th.Tensor, e: float = 0.001):
     if isinstance(value, float) or isinstance(value, np.float32):
         scaled_v = np.sign(value) * (np.sqrt(np.abs(value) + 1) - 1 + value * e)
         return np.array([scaled_v])
     return th.sign(value) * (th.sqrt(th.abs(value) + 1) - 1 + value * e)
 
 
@@ -98,14 +101,15 @@
     from mu_alpha_zero.MuZero.MZ_Arena.arena import MzArena
     from mu_alpha_zero.MuZero.MZ_MCTS.mz_search_tree import MuZeroSearchTree
     from mu_alpha_zero.MuZero.Network.networks import MuZeroNet
     from mu_alpha_zero.AlphaZero.Network.trainer import Trainer
     from mu_alpha_zero.AlphaZero.Arena.players import NetPlayer
     from mu_alpha_zero.mem_buffer import MemBuffer
 
+
     muzero_config.show_tqdm = False
     if in_memory:
         study = optuna.create_study(study_name=study_name, direction=direction)
     else:
         if storage is None:
             raise ValueError("Storage can't be None if in_memory is False.")
         study = optuna.load_study(study_name=study_name, storage=storage)
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/__init__.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/__init__.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/config.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/config.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/main.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/main.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/mem_buffer.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/mem_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,46 @@
+import itertools
 import random
 from collections import deque
 from itertools import chain
 
 import numpy as np
 import pymongo
 import torch as th
 from diskcache import Deque
 from torch.utils.data import Dataset, DataLoader
-from mu_alpha_zero.MuZero.lazy_arrays import LazyArray
+
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.utils import find_project_root
-from mu_alpha_zero.MuZero.utils import scale_action
+from mu_alpha_zero.Hooks.hook_manager import HookManager
+from mu_alpha_zero.Hooks.hook_point import HookAt
+from mu_alpha_zero.MuZero.lazy_arrays import LazyArray
 from mu_alpha_zero.MuZero.pickler import DataPickler
-import itertools
+from mu_alpha_zero.MuZero.utils import scale_action
+
 
 class MemDataset(Dataset):
     def __init__(self, mem_buffer):
         self.mem_buffer = list(mem_buffer)
 
     def __len__(self):
         return len(self.mem_buffer)
 
     def __getitem__(self, idx):
         return self.mem_buffer[idx]
 
 
 class MemBuffer(GeneralMemoryBuffer):
-    def __init__(self, max_size, disk: bool = False, full_disk: bool = False, dir_path: str = None):
+    def __init__(self, max_size, disk: bool = False, full_disk: bool = False, dir_path: str = None,
+                 hook_manager: HookManager or None = None):
         self.max_size = max_size
         self.disk = disk
         self.full_disk = full_disk
         self.dir_path = dir_path
+        self.hook_manager = hook_manager if hook_manager is not None else HookManager()
         self.buffer = self.init_buffer(dir_path)
         self.last_buffer_size = 0
         self.priorities = None
         self.is_disk = disk
 
     def add(self, experience):
         if not isinstance(experience, tuple):
@@ -85,32 +91,38 @@
             if self.last_buffer_size < len(self.buffer):
                 priorities = self.calculate_priorities(batch_size, alpha, K)
                 self.priorities = priorities
                 self.last_buffer_size = len(self.buffer)
             random_indexes = np.random.choice(np.arange(len(self.buffer)),
                                               size=min(len(self.priorities) // K, max(batch_size // K, 1)),
                                               replace=False, p=self.priorities).tolist()
-            batch = [list(itertools.islice(self.buffer,i,i+K)) for i in random_indexes]
+            batch = [list(itertools.islice(self.buffer, i, i + K)) for i in random_indexes]
             pris = [self.priorities[i:i + K] for i in random_indexes]
+            self.hook_manager.process_hook_executes(self, self.batch_with_priorities.__name__, __file__, HookAt.ALL,
+                                                    args=(batch, pris))
             yield list(chain.from_iterable(batch)), th.tensor(list(chain.from_iterable(pris)), dtype=th.float32)
 
     def calculate_priorities(self, batch_size, alpha, K):
-        ps = [abs(self.buffer[i][1] - self.buffer[i][2][2]) for i in
-              range(len(self.buffer))]
+        ps = [abs(self.buffer[i][1] - self.buffer[i][2][2]) for i in range(len(self.buffer))]
         ps = np.array(ps)
         ps = ps ** alpha
         ps = ps / ps.sum()
+        self.hook_manager.process_hook_executes(self, self.calculate_priorities.__name__, __file__, HookAt.ALL,
+                                                args=(ps,))
         return ps
 
     def make_fresh_instance(self):
         return MemBuffer(self.max_size, self.disk, self.dir_path)
 
     def to_dataloader(self, batch_size):
         return DataLoader(MemDataset(self.buffer), batch_size=batch_size, shuffle=True, collate_fn=lambda x: x)
 
+    def run_on_training_end(self):
+        self.hook_manager.process_hook_executes(self, self.run_on_training_end.__name__, __file__, HookAt.ALL)
+
     def save(self):
         if not self.disk:
             buffer = list(self.buffer)
             th.save(buffer, f"{find_project_root()}/Pickles/memory_buffer.pt")
             return f"{find_project_root()}/Pickles/memory_buffer.pt"
         else:
             return self.buffer.directory
@@ -184,16 +196,15 @@
             indexes = np.random.choice(np.arange(self.db.game_data.count_documents({})),
                                        size=min(self.calculated_buffer_size, batch_size // K), replace=False,
                                        p=priorities).tolist()
             items = [list(self.db.game_data.find({}).skip(x).limit(K)) for x in indexes]
             items = list(chain.from_iterable(items))
             items = tuple(
                 [(x["probabilities"], x["vs"], (x["t_reward"], x["game_move"], x["pred_reward"]), x["game_state"]) for x
-                 in
-                 items])
+                 in items])
             yield items, th.tensor(priorities, dtype=th.float32)
 
     def get_last_greatest_id(self):
         return self.db.game_data.find_one(sort=[("_id", pymongo.DESCENDING)])["_id"]
 
     def __len__(self):
         return self.db.game_data.count_documents({})
@@ -214,16 +225,15 @@
         self.pickler = DataPickler(pickle_dir)
 
     def add(self, experience):
         raise NotImplementedError("Single experience addition shouldn't be performed in PickleMemBuffer, please add "
                                   "entire bach with add_list method")
 
     def add_list(self, experience_list):
-        self.pickler.pickle_buffer(experience_list)
-        # self.pickler.push_to_consumer(experience_list)
+        self.pickler.pickle_buffer(experience_list)  # self.pickler.push_to_consumer(experience_list)
 
     def batch(self, batch_size):
         raise NotImplementedError("Batch method not implemented for PickleMemBuffer, please use batch_with_priorities")
 
     def calculate_priorities(self, batch_size, alpha, K):
         vs = self.pickler.load_index(1)
         rews = self.pickler.load_index(2)
@@ -233,16 +243,16 @@
         return {p[1]: p[0] for p in ps}
 
     def batch_with_priorities(self, epochs, batch_size, K, alpha=1):
         priorities = self.calculate_priorities(batch_size, alpha, K)
         ps_probs = np.array(list(priorities.values()))
         for _ in range(epochs):
             random_indexes = np.random.choice(np.arange(len(priorities)),
-                                              size=min(len(priorities) // K, max(batch_size // K, 1)),
-                                              replace=False, p=list(ps_probs)).tolist()
+                                              size=min(len(priorities) // K, max(batch_size // K, 1)), replace=False,
+                                              p=list(ps_probs)).tolist()
             batch = self.pickler.load_all(batch_size, random_indexes, K)
             pris = [list(priorities.values())[i:i + K] for i in random_indexes]
             tmp = list(chain.from_iterable(pris))
             yield batch, th.tensor(tmp, dtype=th.float32)
 
     def save(self):
         print("Load using datapickler.load_all(float(inf),...)")
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/root.root` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/root.root`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero/start_jobs.py` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/start_jobs.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/PKG-INFO` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mu-alpha-zero-library
-Version: 1.0.9.2
+Version: 1.0.9.3
 Summary: Library for running and training MuZero and AlphaZero models.
 Home-page: https://github.com/Skirlax/MuAlphaZeroLibrary
 Author: Skyr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MuAlphaZeroLibrary
```

### Comparing `mu_alpha_zero_library-1.0.9.2/mu_alpha_zero_library.egg-info/SOURCES.txt` & `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 mu_alpha_zero/General/arena.py
 mu_alpha_zero/General/az_game.py
 mu_alpha_zero/General/memory.py
 mu_alpha_zero/General/mz_game.py
 mu_alpha_zero/General/network.py
 mu_alpha_zero/General/search_tree.py
 mu_alpha_zero/General/utils.py
+mu_alpha_zero/Hooks/__init__.py
+mu_alpha_zero/Hooks/hook_callables.py
+mu_alpha_zero/Hooks/hook_manager.py
+mu_alpha_zero/Hooks/hook_point.py
 mu_alpha_zero/MuZero/__init__.py
 mu_alpha_zero/MuZero/lazy_arrays.py
 mu_alpha_zero/MuZero/muzero.py
 mu_alpha_zero/MuZero/pickler.py
 mu_alpha_zero/MuZero/utils.py
 mu_alpha_zero/MuZero/JavaGateway/__init__.py
 mu_alpha_zero/MuZero/JavaGateway/java_manager.py
```

### Comparing `mu_alpha_zero_library-1.0.9.2/setup.py` & `mu_alpha_zero_library-1.0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name="mu_alpha_zero_library",
-    version="1.0.9.2",
+    version="1.0.9.3",
     description="Library for running and training MuZero and AlphaZero models.",
     author="Skyr",
     install_requires=open("requirements.txt").read().strip().split("\n"),
     long_description=open('README.md',encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     package_data={
         "mu_alpha_zero": ["*.txt", "*.root"]
     },
     url="https://github.com/Skirlax/MuAlphaZeroLibrary",
 
-)
+)
```

