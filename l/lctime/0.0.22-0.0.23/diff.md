# Comparing `tmp/lctime-0.0.22.tar.gz` & `tmp/lctime-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctime-0.0.22.tar", last modified: Thu Feb 22 10:44:08 2024, max compression
+gzip compressed data, was "lctime-0.0.23.tar", last modified: Thu Apr  4 21:15:50 2024, max compression
```

## Comparing `lctime-0.0.22.tar` & `lctime-0.0.23.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.282893 lctime-0.0.22/
--rw-r--r--   0 user      (1000) user      (1000)     5815 2024-02-22 10:44:08.282893 lctime-0.0.22/PKG-INFO
--rw-r-----   0 user      (1000) user      (1000)     4759 2024-01-25 11:27:18.000000 lctime-0.0.22/README.md
--rw-r--r--   0 user      (1000) user      (1000)     1855 2024-02-22 10:43:34.000000 lctime-0.0.22/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-02-22 10:44:08.282893 lctime-0.0.22/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.266893 lctime-0.0.22/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.274893 lctime-0.0.22/src/lctime/
--rw-r--r--   0 user      (1000) user      (1000)      983 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     4077 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/cell_types.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.274893 lctime-0.0.22/src/lctime/characterization/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/__init__.py
--rw-r-----   0 user      (1000) user      (1000)    11796 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/input_capacitance.py
--rw-r--r--   0 user      (1000) user      (1000)    64459 2024-02-22 10:39:09.000000 lctime-0.0.22/src/lctime/characterization/main_lctime.py
--rw-r-----   0 user      (1000) user      (1000)     7311 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/main_sp2bool.py
--rw-r-----   0 user      (1000) user      (1000)     4926 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/ngspice_simulation.py
--rw-r-----   0 user      (1000) user      (1000)    24981 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/ngspice_subprocess.py
--rw-r-----   0 user      (1000) user      (1000)    14444 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/piece_wise_linear.py
--rw-r-----   0 user      (1000) user      (1000)     4810 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/test_ngspice_shared.py
--rw-r-----   0 user      (1000) user      (1000)     5414 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/test_ngspice_subprocess.py
--rw-r--r--   0 user      (1000) user      (1000)    15265 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/timing_combinatorial.py
--rw-r--r--   0 user      (1000) user      (1000)    61091 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/timing_sequential.py
--rw-r--r--   0 user      (1000) user      (1000)    16441 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/characterization/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.278893 lctime-0.0.22/src/lctime/lccommon/
--rw-r-----   0 user      (1000) user      (1000)      128 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/lccommon/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     1955 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/lccommon/data_types.py
--rw-r--r--   0 user      (1000) user      (1000)    10475 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/lccommon/net_util.py
--rw-r-----   0 user      (1000) user      (1000)     5094 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/lccommon/spice_parser.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.278893 lctime-0.0.22/src/lctime/liberty/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/liberty/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     4870 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/liberty/merge.py
--rw-r-----   0 user      (1000) user      (1000)     5853 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/liberty/util.py
--rw-r-----   0 user      (1000) user      (1000)     3919 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/liberty/visualize.py
--rw-r--r--   0 user      (1000) user      (1000)      472 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/licence.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.282893 lctime-0.0.22/src/lctime/logic/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     6513 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/cmos_sim.py
--rw-r-----   0 user      (1000) user      (1000)    10591 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/cmos_synth.py
--rw-r-----   0 user      (1000) user      (1000)    49051 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/functional_abstraction.py
--rw-r-----   0 user      (1000) user      (1000)     2365 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/graph_enumeration.py
--rw-r-----   0 user      (1000) user      (1000)    21778 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/seq_recognition.py
--rw-r-----   0 user      (1000) user      (1000)     1845 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/smt_4value_logic_scratch.py
--rw-r-----   0 user      (1000) user      (1000)     1690 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/types.py
--rw-r-----   0 user      (1000) user      (1000)     2657 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/logic/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.282893 lctime-0.0.22/src/lctime/transistor_sizing/
--rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/transistor_sizing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     9277 2024-01-25 11:27:22.000000 lctime-0.0.22/src/lctime/transistor_sizing/width_opt.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-22 10:44:08.282893 lctime-0.0.22/src/lctime.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     5815 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1505 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      216 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      128 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2024-02-22 10:44:08.000000 lctime-0.0.22/src/lctime.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.275904 lctime-0.0.23/
+-rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-04 21:15:50.275904 lctime-0.0.23/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     4983 2024-04-04 21:13:38.000000 lctime-0.0.23/README.md
+-rw-r--r--   0 user      (1000) user      (1000)     1855 2024-04-04 21:14:50.000000 lctime-0.0.23/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-04 21:15:50.275904 lctime-0.0.23/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.255904 lctime-0.0.23/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.255904 lctime-0.0.23/src/lctime/
+-rw-r--r--   0 user      (1000) user      (1000)      983 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     4077 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/cell_types.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.263904 lctime-0.0.23/src/lctime/characterization/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    11792 2024-04-03 14:36:44.000000 lctime-0.0.23/src/lctime/characterization/input_capacitance.py
+-rw-r--r--   0 user      (1000) user      (1000)    64459 2024-02-22 10:39:09.000000 lctime-0.0.23/src/lctime/characterization/main_lctime.py
+-rw-r-----   0 user      (1000) user      (1000)     7311 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/main_sp2bool.py
+-rw-r-----   0 user      (1000) user      (1000)     4926 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/ngspice_simulation.py
+-rw-r--r--   0 user      (1000) user      (1000)    24914 2024-04-03 14:36:44.000000 lctime-0.0.23/src/lctime/characterization/ngspice_subprocess.py
+-rw-r-----   0 user      (1000) user      (1000)    14444 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/piece_wise_linear.py
+-rw-r-----   0 user      (1000) user      (1000)     4810 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/test_ngspice_shared.py
+-rw-r-----   0 user      (1000) user      (1000)     5414 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/test_ngspice_subprocess.py
+-rw-r--r--   0 user      (1000) user      (1000)    15265 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/timing_combinatorial.py
+-rw-r--r--   0 user      (1000) user      (1000)    61091 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/timing_sequential.py
+-rw-r--r--   0 user      (1000) user      (1000)    16441 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/characterization/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.267904 lctime-0.0.23/src/lctime/lccommon/
+-rw-r-----   0 user      (1000) user      (1000)      128 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     1955 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/data_types.py
+-rw-r--r--   0 user      (1000) user      (1000)    10475 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/net_util.py
+-rw-r-----   0 user      (1000) user      (1000)     5094 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/lccommon/spice_parser.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.267904 lctime-0.0.23/src/lctime/liberty/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     4870 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/merge.py
+-rw-r-----   0 user      (1000) user      (1000)     5853 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/util.py
+-rw-r-----   0 user      (1000) user      (1000)     3919 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/liberty/visualize.py
+-rw-r--r--   0 user      (1000) user      (1000)      472 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/licence.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.271904 lctime-0.0.23/src/lctime/logic/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     6513 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/cmos_sim.py
+-rw-r-----   0 user      (1000) user      (1000)    10591 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/cmos_synth.py
+-rw-r-----   0 user      (1000) user      (1000)    49051 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/functional_abstraction.py
+-rw-r-----   0 user      (1000) user      (1000)     2365 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/graph_enumeration.py
+-rw-r-----   0 user      (1000) user      (1000)    21778 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/seq_recognition.py
+-rw-r-----   0 user      (1000) user      (1000)     1845 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/smt_4value_logic_scratch.py
+-rw-r-----   0 user      (1000) user      (1000)     1690 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/types.py
+-rw-r-----   0 user      (1000) user      (1000)     2657 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/logic/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.271904 lctime-0.0.23/src/lctime/transistor_sizing/
+-rw-r-----   0 user      (1000) user      (1000)      150 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/transistor_sizing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     9277 2024-01-25 11:27:22.000000 lctime-0.0.23/src/lctime/transistor_sizing/width_opt.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 21:15:50.275904 lctime-0.0.23/src/lctime.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     6039 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1505 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      216 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      128 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2024-04-04 21:15:50.000000 lctime-0.0.23/src/lctime.egg-info/top_level.txt
```

### Comparing `lctime-0.0.22/PKG-INFO` & `lctime-0.0.23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctime
-Version: 0.0.22
+Version: 0.0.23
 Summary: CMOS standard-cell characterization kit.
 Author-email: "T. Kramer" <code@tkramer.ch>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://codeberg.org/librecell/lctime
 Project-URL: Repository, https://codeberg.org/librecell/lctime
 Project-URL: Issue Tracker, https://codeberg.org/librecell/lctime/issues
 Keywords: cmos,cell,characterization,vlsi,asic
@@ -161,9 +161,11 @@
 sp2bool --spice ~/FreePDK45/osu_soc/lib/files/cells.sp --cell DFFSR
 ```
 
 For cells with *differential* inputs the `--diff` argument must be used to specify differential pairs.
 
 
 ## Debugging
-
-Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
+Options for increasing debugging information:
+* `--debug`: increase verbosity. Will also show the path to generated SPICE files.
+* `--debug-plots` plot the waveforms of all simulations to a file. Slow but sometimes useful.
+* Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
```

### Comparing `lctime-0.0.22/README.md` & `lctime-0.0.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,9 +134,11 @@
 sp2bool --spice ~/FreePDK45/osu_soc/lib/files/cells.sp --cell DFFSR
 ```
 
 For cells with *differential* inputs the `--diff` argument must be used to specify differential pairs.
 
 
 ## Debugging
-
-Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
+Options for increasing debugging information:
+* `--debug`: increase verbosity. Will also show the path to generated SPICE files.
+* `--debug-plots` plot the waveforms of all simulations to a file. Slow but sometimes useful.
+* Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
```

### Comparing `lctime-0.0.22/pyproject.toml` & `lctime-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Thomas Kramer
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 
 [project]
 name = "lctime"
-version = "0.0.22"
+version = "0.0.23"
 description='CMOS standard-cell characterization kit.'
 readme = {file = "README.md", content-type="text/markdown"}
 license = {text = "AGPL-3.0-or-later"}
 
 requires-python = ">=3.7"
 
 keywords= ["cmos", "cell", "characterization", "vlsi", "asic"]
```

### Comparing `lctime-0.0.22/src/lctime/__init__.py` & `lctime-0.0.23/src/lctime/__init__.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/cell_types.py` & `lctime-0.0.23/src/lctime/cell_types.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/input_capacitance.py` & `lctime-0.0.23/src/lctime/characterization/input_capacitance.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             # Get the breakpoint condition.
             if input_rising:
                 breakpoint_statement = f"stop when v({active_pin}) > {vdd * 0.9}"
             else:
                 breakpoint_statement = f"stop when v({active_pin}) < {vdd * 0.1}"
 
             static_supply_voltage_statements = "\n".join(
-                (f"Vinput_{net} {cell_conf.ground_net} {net} {voltage}" for net, voltage in input_voltages.items()))
+                (f"Vinput_{net} {net} {cell_conf.ground_net} {voltage}" for net, voltage in input_voltages.items()))
 
             # Initial node voltages.
             initial_conditions = {
                 active_pin: initial_voltage,
                 cell_conf.supply_net: cfg.supply_voltage
             }
             # Add static input voltages
@@ -192,15 +192,15 @@
 set filetype=ascii
 set wr_vecnames
 
 * Breakpoints
 {breakpoint_statement}
 
 * Transient simulation, use initial conditions.
-tran {cfg.time_step} {time_max} uic
+tran {cfg.time_step} {time_max}
 wrdata {sim_output_file} v({active_pin}) {" ".join((f"v({p})" for p in output_pins))}
 exit
 .endc
 
 .end
 """
```

### Comparing `lctime-0.0.22/src/lctime/characterization/main_lctime.py` & `lctime-0.0.23/src/lctime/characterization/main_lctime.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/main_sp2bool.py` & `lctime-0.0.23/src/lctime/characterization/main_sp2bool.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/ngspice_simulation.py` & `lctime-0.0.23/src/lctime/characterization/ngspice_simulation.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/ngspice_subprocess.py` & `lctime-0.0.23/src/lctime/characterization/ngspice_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,16 +212,16 @@
 
 set filetype=ascii
 set wr_vecnames
 
 * Breakpoints
 {breakpoint_statements}
 
-* Transient simulation, use initial conditions.
-tran {time_step} {max_simulation_time} uic
+* Transient simulation.
+tran {time_step} {max_simulation_time}
 * Write selected signals to the output file.
 wrdata {simulation_output_file} {output_voltage_defs} {output_current_defs} 
 * Exit ngspice.
 exit
 .endc
 
 .end
@@ -625,16 +625,16 @@
 
 set filetype=ascii
 set wr_vecnames
 
 * Breakpoints
 {breakpoint_statements}
 
-* Transient simulation, use initial conditions.
-* tran {time_step} {max_simulation_time} uic
+* Transient simulation.
+* tran {time_step} {max_simulation_time}
 * Write selected signals to the output file.
 * wrdata {simulation_output_file} {output_voltage_defs} {output_current_defs} 
 * Exit ngspice.
 *exit
 .endc
 
 .end
@@ -651,15 +651,15 @@
     logger.debug("Run simulation.")
     # stdout, stderr = run_simulation(simulation_file)
     ns = NgSpiceInteractive()
     ns.start()
 
     # ns.source(simulation_file)
     ns.load_circuit(sim_netlist)
-    nrows = ns.tran(t_step=time_step, t_stop=max_simulation_time, uic='uic')
+    nrows = ns.tran(t_step=time_step, t_stop=max_simulation_time)
     measure_currents_at = [f'v{c}' for c in output_currents]
     sim_data = ns.get_data(num_rows=nrows, voltages=output_voltages, currents=measure_currents_at)
     ns.cmd('quit')
     ns.stop()
 
     # # Retrieve data.
     # logger.debug("Load simulation output.")
```

### Comparing `lctime-0.0.22/src/lctime/characterization/piece_wise_linear.py` & `lctime-0.0.23/src/lctime/characterization/piece_wise_linear.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/test_ngspice_shared.py` & `lctime-0.0.23/src/lctime/characterization/test_ngspice_shared.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/test_ngspice_subprocess.py` & `lctime-0.0.23/src/lctime/characterization/test_ngspice_subprocess.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/timing_combinatorial.py` & `lctime-0.0.23/src/lctime/characterization/timing_combinatorial.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/timing_sequential.py` & `lctime-0.0.23/src/lctime/characterization/timing_sequential.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/characterization/util.py` & `lctime-0.0.23/src/lctime/characterization/util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/lccommon/data_types.py` & `lctime-0.0.23/src/lctime/lccommon/data_types.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/lccommon/net_util.py` & `lctime-0.0.23/src/lctime/lccommon/net_util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/lccommon/spice_parser.py` & `lctime-0.0.23/src/lctime/lccommon/spice_parser.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/liberty/merge.py` & `lctime-0.0.23/src/lctime/liberty/merge.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/liberty/util.py` & `lctime-0.0.23/src/lctime/liberty/util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/liberty/visualize.py` & `lctime-0.0.23/src/lctime/liberty/visualize.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/cmos_sim.py` & `lctime-0.0.23/src/lctime/logic/cmos_sim.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/cmos_synth.py` & `lctime-0.0.23/src/lctime/logic/cmos_synth.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/functional_abstraction.py` & `lctime-0.0.23/src/lctime/logic/functional_abstraction.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/graph_enumeration.py` & `lctime-0.0.23/src/lctime/logic/graph_enumeration.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/seq_recognition.py` & `lctime-0.0.23/src/lctime/logic/seq_recognition.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/smt_4value_logic_scratch.py` & `lctime-0.0.23/src/lctime/logic/smt_4value_logic_scratch.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/types.py` & `lctime-0.0.23/src/lctime/logic/types.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/logic/util.py` & `lctime-0.0.23/src/lctime/logic/util.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime/transistor_sizing/width_opt.py` & `lctime-0.0.23/src/lctime/transistor_sizing/width_opt.py`

 * *Files identical despite different names*

### Comparing `lctime-0.0.22/src/lctime.egg-info/PKG-INFO` & `lctime-0.0.23/src/lctime.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctime
-Version: 0.0.22
+Version: 0.0.23
 Summary: CMOS standard-cell characterization kit.
 Author-email: "T. Kramer" <code@tkramer.ch>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://codeberg.org/librecell/lctime
 Project-URL: Repository, https://codeberg.org/librecell/lctime
 Project-URL: Issue Tracker, https://codeberg.org/librecell/lctime/issues
 Keywords: cmos,cell,characterization,vlsi,asic
@@ -161,9 +161,11 @@
 sp2bool --spice ~/FreePDK45/osu_soc/lib/files/cells.sp --cell DFFSR
 ```
 
 For cells with *differential* inputs the `--diff` argument must be used to specify differential pairs.
 
 
 ## Debugging
-
-Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
+Options for increasing debugging information:
+* `--debug`: increase verbosity. Will also show the path to generated SPICE files.
+* `--debug-plots` plot the waveforms of all simulations to a file. Slow but sometimes useful.
+* Enable very verbose trace log: set the `DEBUG_LCTIME` environment variable to `yes`
```

### Comparing `lctime-0.0.22/src/lctime.egg-info/SOURCES.txt` & `lctime-0.0.23/src/lctime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

