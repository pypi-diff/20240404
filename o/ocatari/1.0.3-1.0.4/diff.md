# Comparing `tmp/ocatari-1.0.3.tar.gz` & `tmp/ocatari-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-1.0.3.tar", last modified: Wed Mar 20 15:36:45 2024, max compression
+gzip compressed data, was "ocatari-1.0.4.tar", last modified: Thu Apr  4 12:45:31 2024, max compression
```

## Comparing `ocatari-1.0.3.tar` & `ocatari-1.0.4.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.194520 ocatari-1.0.3/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.3/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-03-20 15:36:45.194520 ocatari-1.0.3/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.3/README.md
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.178520 ocatari-1.0.3/ocatari/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.3/ocatari/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    22811 2024-03-19 14:31:16.000000 ocatari-1.0.3/ocatari/core.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/environments.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.186520 ocatari-1.0.3/ocatari/ram/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.3/ocatari/ram/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15652 2024-03-19 14:28:41.000000 ocatari-1.0.3/ocatari/ram/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.3/ocatari/ram/asterix_old.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.3/ocatari/ram/asterix_old2.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14228 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5593 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    29613 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4745 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/ram/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.3/ocatari/ram/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15746 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5885 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10776 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14452 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9441 2024-03-18 13:29:46.000000 ocatari-1.0.3/ocatari/ram/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12471 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.3/ocatari/ram/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.3/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10737 2024-03-18 11:06:15.000000 ocatari-1.0.3/ocatari/utils.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.190520 ocatari-1.0.3/ocatari/vision/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.3/ocatari/vision/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.3/ocatari/vision/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.3/ocatari/vision/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.3/ocatari/vision/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.3/ocatari/vision/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.3/ocatari/vision/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.3/ocatari/vision/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.3/ocatari/vision/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.3/ocatari/vision/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.3/ocatari/vision/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.3/ocatari/vision/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.3/ocatari/vision/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.3/ocatari/vision/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.3/ocatari/vision/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.3/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.3/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.3/ocatari/vision/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.3/ocatari/vision/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.3/ocatari/vision/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.3/ocatari/vision/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.3/ocatari/vision/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.3/ocatari/vision/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.3/ocatari/vision/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.3/ocatari/vision/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.3/ocatari/vision/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.3/ocatari/vision/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.3/ocatari/vision/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.3/ocatari/vision/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.3/ocatari/vision/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.3/ocatari/vision/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.3/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.178520 ocatari-1.0.3/ocatari.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-03-20 15:36:45.000000 ocatari-1.0.3/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-03-20 15:36:45.000000 ocatari-1.0.3/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-03-20 15:36:45.000000 ocatari-1.0.3/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-03-20 15:36:45.000000 ocatari-1.0.3/ocatari.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-03-20 15:36:45.000000 ocatari-1.0.3/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-03-20 15:36:45.194520 ocatari-1.0.3/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1024 2024-03-20 15:14:02.000000 ocatari-1.0.3/setup.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-03-20 15:36:45.194520 ocatari-1.0.3/tests/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.3/tests/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.3/tests/display_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.3/tests/display_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.3/tests/get_metrics.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.3/tests/metrics_utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.3/tests/plot_speed_results.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.3/tests/pong_test.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.3/tests/test_explanation.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.3/tests/test_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.3/tests/test_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.3/tests/test_game_both_interactive.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.3/tests/test_speed.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.4/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-04 12:45:31.534425 ocatari-1.0.4/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.4/README.md
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.522425 ocatari-1.0.4/ocatari/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.4/ocatari/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    22811 2024-03-19 14:31:16.000000 ocatari-1.0.4/ocatari/core.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/environments.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.526425 ocatari-1.0.4/ocatari/ram/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.4/ocatari/ram/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/ram/_helper_methods.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15652 2024-03-19 14:28:41.000000 ocatari-1.0.4/ocatari/ram/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.4/ocatari/ram/asterix_old.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.4/ocatari/ram/asterix_old2.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14228 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5593 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    29613 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/extract_ram_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/extract_ram_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4745 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/ram/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.4/ocatari/ram/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15746 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-03-23 11:45:59.000000 ocatari-1.0.4/ocatari/ram/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10776 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14452 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9441 2024-03-18 13:29:46.000000 ocatari-1.0.4/ocatari/ram/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12471 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.4/ocatari/ram/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/yarsrevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10737 2024-03-18 11:06:15.000000 ocatari-1.0.4/ocatari/utils.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/ocatari/vision/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.4/ocatari/vision/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.4/ocatari/vision/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.4/ocatari/vision/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.4/ocatari/vision/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.4/ocatari/vision/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.4/ocatari/vision/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.4/ocatari/vision/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.4/ocatari/vision/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.4/ocatari/vision/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.4/ocatari/vision/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.4/ocatari/vision/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.4/ocatari/vision/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.4/ocatari/vision/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.4/ocatari/vision/extract_vision_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.4/ocatari/vision/extract_vision_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.4/ocatari/vision/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.4/ocatari/vision/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.4/ocatari/vision/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.4/ocatari/vision/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.4/ocatari/vision/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.4/ocatari/vision/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.4/ocatari/vision/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.4/ocatari/vision/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.4/ocatari/vision/yarsrevenge.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.522425 ocatari-1.0.4/ocatari.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-04-04 12:45:31.534425 ocatari-1.0.4/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-04-04 12:45:17.000000 ocatari-1.0.4/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/tests/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.4/tests/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/display_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.4/tests/display_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.4/tests/get_metrics.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.4/tests/metrics_utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.4/tests/plot_speed_results.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/pong_test.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_explanation.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.4/tests/test_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.4/tests/test_game_both_interactive.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_speed.py
```

### Comparing `ocatari-1.0.3/LICENSE` & `ocatari-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/PKG-INFO` & `ocatari-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.3
+Version: 1.0.4
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.3/README.md` & `ocatari-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/core.py` & `ocatari-1.0.4/ocatari/core.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/environments.py` & `ocatari-1.0.4/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/_helper_methods.py` & `ocatari-1.0.4/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/adventure.py` & `ocatari-1.0.4/ocatari/ram/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/alien.py` & `ocatari-1.0.4/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/amidar.py` & `ocatari-1.0.4/ocatari/ram/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/assault.py` & `ocatari-1.0.4/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/asterix.py` & `ocatari-1.0.4/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/asterix_old.py` & `ocatari-1.0.4/ocatari/ram/asterix_old.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/asterix_old2.py` & `ocatari-1.0.4/ocatari/ram/asterix_old2.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/asteroids.py` & `ocatari-1.0.4/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/atlantis.py` & `ocatari-1.0.4/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/bankheist.py` & `ocatari-1.0.4/ocatari/ram/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/battlezone.py` & `ocatari-1.0.4/ocatari/ram/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/beamrider.py` & `ocatari-1.0.4/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/berzerk.py` & `ocatari-1.0.4/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/bowling.py` & `ocatari-1.0.4/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/boxing.py` & `ocatari-1.0.4/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/breakout.py` & `ocatari-1.0.4/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/carnival.py` & `ocatari-1.0.4/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/centipede.py` & `ocatari-1.0.4/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/choppercommand.py` & `ocatari-1.0.4/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/crazyclimber.py` & `ocatari-1.0.4/ocatari/ram/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/demonattack.py` & `ocatari-1.0.4/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/donkeykong.py` & `ocatari-1.0.4/ocatari/ram/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/enduro.py` & `ocatari-1.0.4/ocatari/ram/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/extract_ram_info.py` & `ocatari-1.0.4/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/extract_ram_info_short.py` & `ocatari-1.0.4/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/fishingderby.py` & `ocatari-1.0.4/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/freeway.py` & `ocatari-1.0.4/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/frostbite.py` & `ocatari-1.0.4/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/game_objects.py` & `ocatari-1.0.4/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/gopher.py` & `ocatari-1.0.4/ocatari/ram/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/hero.py` & `ocatari-1.0.4/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/icehockey.py` & `ocatari-1.0.4/ocatari/ram/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/jamesbond.py` & `ocatari-1.0.4/ocatari/ram/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/kangaroo.py` & `ocatari-1.0.4/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/krull.py` & `ocatari-1.0.4/ocatari/ram/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/montezumarevenge.py` & `ocatari-1.0.4/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/mspacman.py` & `ocatari-1.0.4/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/pacman.py` & `ocatari-1.0.4/ocatari/ram/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/pitfall.py` & `ocatari-1.0.4/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/pong.py` & `ocatari-1.0.4/ocatari/ram/pong.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     player, ball, enemy = objects[:3]
 
     # ball
     if ram_state[54] != 0:  # otherwise no ball
         ball.xy = ram_state[49]-49, ram_state[54]-14
 
     # enemy
-    if ram_state[50] > 18:  # otherwise no enemy
+    if ram_state[50] > 18:  # otherwise no enemy # could be ram pos 21 as well
         if ram_state[50] - 15 < 34:
             enemy.xy = 16, 34
             enemy.wh = 4, ram_state[50]-33
         elif ram_state[50] > 194:
             enemy.xy = 16, ram_state[50]-15
             enemy.wh = 4, 209 - ram_state[50]
         else:
```

### Comparing `ocatari-1.0.3/ocatari/ram/privateeye.py` & `ocatari-1.0.4/ocatari/ram/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/qbert.py` & `ocatari-1.0.4/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/riverraid.py` & `ocatari-1.0.4/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/roadrunner.py` & `ocatari-1.0.4/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/seaquest.py` & `ocatari-1.0.4/ocatari/ram/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/skiing.py` & `ocatari-1.0.4/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/spaceinvaders.py` & `ocatari-1.0.4/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/tennis.py` & `ocatari-1.0.4/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/timepilot.py` & `ocatari-1.0.4/ocatari/ram/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/upndown.py` & `ocatari-1.0.4/ocatari/ram/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/utils.py` & `ocatari-1.0.4/ocatari/ram/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/venture.py` & `ocatari-1.0.4/ocatari/ram/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/videopinball.py` & `ocatari-1.0.4/ocatari/ram/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/ram/yarsrevenge.py` & `ocatari-1.0.4/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/utils.py` & `ocatari-1.0.4/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/adventure.py` & `ocatari-1.0.4/ocatari/vision/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/alien.py` & `ocatari-1.0.4/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/amidar.py` & `ocatari-1.0.4/ocatari/vision/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/assault.py` & `ocatari-1.0.4/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/asterix.py` & `ocatari-1.0.4/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/asteroids.py` & `ocatari-1.0.4/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/atlantis.py` & `ocatari-1.0.4/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/bankheist.py` & `ocatari-1.0.4/ocatari/vision/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/battlezone.py` & `ocatari-1.0.4/ocatari/vision/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/beamrider.py` & `ocatari-1.0.4/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/berzerk.py` & `ocatari-1.0.4/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/bowling.py` & `ocatari-1.0.4/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/boxing.py` & `ocatari-1.0.4/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/breakout.py` & `ocatari-1.0.4/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/carnival.py` & `ocatari-1.0.4/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/centipede.py` & `ocatari-1.0.4/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/choppercommand.py` & `ocatari-1.0.4/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/crazyclimber.py` & `ocatari-1.0.4/ocatari/vision/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/demonattack.py` & `ocatari-1.0.4/ocatari/vision/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/donkeykong.py` & `ocatari-1.0.4/ocatari/vision/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/enduro.py` & `ocatari-1.0.4/ocatari/vision/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/extract_vision_info.py` & `ocatari-1.0.4/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/extract_vision_info_short.py` & `ocatari-1.0.4/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/fishingderby.py` & `ocatari-1.0.4/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/freeway.py` & `ocatari-1.0.4/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/frostbite.py` & `ocatari-1.0.4/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/game_objects.py` & `ocatari-1.0.4/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/gopher.py` & `ocatari-1.0.4/ocatari/vision/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/hero.py` & `ocatari-1.0.4/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/icehockey.py` & `ocatari-1.0.4/ocatari/vision/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/jamesbond.py` & `ocatari-1.0.4/ocatari/vision/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/kangaroo.py` & `ocatari-1.0.4/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/krull.py` & `ocatari-1.0.4/ocatari/vision/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/montezumarevenge.py` & `ocatari-1.0.4/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/mspacman.py` & `ocatari-1.0.4/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/pacman.py` & `ocatari-1.0.4/ocatari/vision/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/pitfall.py` & `ocatari-1.0.4/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/pong.py` & `ocatari-1.0.4/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/privateeye.py` & `ocatari-1.0.4/ocatari/vision/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/qbert.py` & `ocatari-1.0.4/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/riverraid.py` & `ocatari-1.0.4/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/roadrunner.py` & `ocatari-1.0.4/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/seaquest.py` & `ocatari-1.0.4/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/skiing.py` & `ocatari-1.0.4/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/spaceinvaders.py` & `ocatari-1.0.4/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/tennis.py` & `ocatari-1.0.4/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/timepilot.py` & `ocatari-1.0.4/ocatari/vision/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/upndown.py` & `ocatari-1.0.4/ocatari/vision/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/utils.py` & `ocatari-1.0.4/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/venture.py` & `ocatari-1.0.4/ocatari/vision/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/videopinball.py` & `ocatari-1.0.4/ocatari/vision/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari/vision/yarsrevenge.py` & `ocatari-1.0.4/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/ocatari.egg-info/PKG-INFO` & `ocatari-1.0.4/ocatari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.3
+Version: 1.0.4
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.3/ocatari.egg-info/SOURCES.txt` & `ocatari-1.0.4/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/setup.py` & `ocatari-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
@@ -35,8 +35,8 @@
         "tqdm",
         "pygame",
         "pyfiglet",
     ]
 )
 
 print("Please install gymnasium atari dependencies, using:\n", 
-      "pip install gymnasium[atari, accept-rom-license]")
+      "pip install gymnasium[atari, accept-rom-license]")
```

### Comparing `ocatari-1.0.3/tests/display_game.py` & `ocatari-1.0.4/tests/display_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/display_game_both.py` & `ocatari-1.0.4/tests/display_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/get_metrics.py` & `ocatari-1.0.4/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/metrics_utils.py` & `ocatari-1.0.4/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/plot_speed_results.py` & `ocatari-1.0.4/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/pong_test.py` & `ocatari-1.0.4/tests/pong_test.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/test_explanation.py` & `ocatari-1.0.4/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/test_game.py` & `ocatari-1.0.4/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/test_game_both.py` & `ocatari-1.0.4/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/test_game_both_interactive.py` & `ocatari-1.0.4/tests/test_game_both_interactive.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.3/tests/test_speed.py` & `ocatari-1.0.4/tests/test_speed.py`

 * *Files identical despite different names*

