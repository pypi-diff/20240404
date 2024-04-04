# Comparing `tmp/py_ballisticcalc-2.0.0b2.tar.gz` & `tmp/py_ballisticcalc-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc-2.0.0b2.tar", last modified: Tue Apr  2 04:25:27 2024, max compression
+gzip compressed data, was "py_ballisticcalc-2.0.0b3.tar", last modified: Thu Apr  4 18:32:36 2024, max compression
```

## Comparing `py_ballisticcalc-2.0.0b2.tar` & `py_ballisticcalc-2.0.0b3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/py_ballisticcalc/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22165 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/multiple_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/munition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22701 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 04:25:27.000000 py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:25:27.645088 py_ballisticcalc-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:27.641088 py_ballisticcalc-2.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_danger_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_mbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-02 04:25:17.000000 py_ballisticcalc-2.0.0b2/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.713611 py_ballisticcalc-2.0.0b3/py_ballisticcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/munition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24075 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22793 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 18:32:36.000000 py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:36.717611 py_ballisticcalc-2.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_danger_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_mbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-04 18:32:26.000000 py_ballisticcalc-2.0.0b3/tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.0b2/LICENSE` & `py_ballisticcalc-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b2/PKG-INFO` & `py_ballisticcalc-2.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -184,16 +184,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b2; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b3; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
 
@@ -251,20 +252,20 @@
 from py_ballisticcalc import Weapon, Shot, Calculator
 from py_ballisticcalc import Settings as Set
 from py_ballisticcalc.unit import *
 ```
 
 ## Simple Zero
 ```python
-# Establish 100-yard zero for a standard .308, G7 BC=0.22, muzzle velocity 2600fps
+# Establish 100-yard zero for a standard .308, G7 bc=0.22, muzzle velocity 2600fps
 zero = Shot(weapon=Weapon(sight_height=2), ammo=Ammo(DragModel(0.22, TableG7), mv=Velocity.FPS(2600)))
 calc = Calculator()
 zero_distance = Distance.Yard(100)
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 ```
 
     Barrel elevation for 100.0yd zero: 1.33mil
 
 ## Plot Trajectory with Danger Space
 ```python
 # Plot trajectory out to 500 yards
@@ -314,36 +315,36 @@
 ammo.calc_powder_sens(Velocity.MPS(820), Temperature.Celsius(0))
 weapon = Weapon(sight_height=Distance.Centimeter(9), twist=15)
 atmo = Atmo(altitude=Distance.Foot(1000), temperature=Unit.CELSIUS(5), humidity=.5)
 zero = Shot(weapon=weapon, ammo=ammo, atmo=atmo)
 zero_distance = Distance.Meter(500)
 calc = Calculator()
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 print(f'Muzzle velocity at zero temperature {atmo.temperature} is {ammo.get_velocity_for_temp(atmo.temperature) << Velocity.MPS}')
 ```
 
     Barrel elevation for 500.0m zero: 4.69mil
     Muzzle velocity at zero temperature 5.0°C is 830.0m/s
 
 ## Units
 
 ```python
 from py_ballisticcalc.unit import *
 
 # Print default units
-from py_ballisticcalc import Settings
+from py_ballisticcalc import Settings, PreferredUnits
 print(str(Settings.Units))
 
 # Change default
-Set.Units.distance = Unit.FOOT
-print(f'Default distance unit: {Set.Units.distance.name}')
+PreferredUnits.distance = Unit.FOOT
+print(f'Default distance unit: {PreferredUnits.distance.name}')
 # Can create value in default unit with either float or another unit of same type
-print(f'\tInstantiated from float (5): {Set.Units.distance(5)}')
-print(f'\tInstantiated from Distance.Line(200): {Set.Units.distance(Distance.Line(200))}')
+print(f'\tInstantiated from float (5): {PreferredUnits.distance(5)}')
+print(f'\tInstantiated from Distance.Line(200): {PreferredUnits.distance(Distance.Line(200))}')
 
 # Ways to define value in units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
```

### Comparing `py_ballisticcalc-2.0.0b2/README.md` & `py_ballisticcalc-2.0.0b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,20 @@
 from py_ballisticcalc import Weapon, Shot, Calculator
 from py_ballisticcalc import Settings as Set
 from py_ballisticcalc.unit import *
 ```
 
 ## Simple Zero
 ```python
-# Establish 100-yard zero for a standard .308, G7 BC=0.22, muzzle velocity 2600fps
+# Establish 100-yard zero for a standard .308, G7 bc=0.22, muzzle velocity 2600fps
 zero = Shot(weapon=Weapon(sight_height=2), ammo=Ammo(DragModel(0.22, TableG7), mv=Velocity.FPS(2600)))
 calc = Calculator()
 zero_distance = Distance.Yard(100)
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 ```
 
     Barrel elevation for 100.0yd zero: 1.33mil
 
 ## Plot Trajectory with Danger Space
 ```python
 # Plot trajectory out to 500 yards
@@ -115,36 +115,36 @@
 ammo.calc_powder_sens(Velocity.MPS(820), Temperature.Celsius(0))
 weapon = Weapon(sight_height=Distance.Centimeter(9), twist=15)
 atmo = Atmo(altitude=Distance.Foot(1000), temperature=Unit.CELSIUS(5), humidity=.5)
 zero = Shot(weapon=weapon, ammo=ammo, atmo=atmo)
 zero_distance = Distance.Meter(500)
 calc = Calculator()
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 print(f'Muzzle velocity at zero temperature {atmo.temperature} is {ammo.get_velocity_for_temp(atmo.temperature) << Velocity.MPS}')
 ```
 
     Barrel elevation for 500.0m zero: 4.69mil
     Muzzle velocity at zero temperature 5.0°C is 830.0m/s
 
 ## Units
 
 ```python
 from py_ballisticcalc.unit import *
 
 # Print default units
-from py_ballisticcalc import Settings
+from py_ballisticcalc import Settings, PreferredUnits
 print(str(Settings.Units))
 
 # Change default
-Set.Units.distance = Unit.FOOT
-print(f'Default distance unit: {Set.Units.distance.name}')
+PreferredUnits.distance = Unit.FOOT
+print(f'Default distance unit: {PreferredUnits.distance.name}')
 # Can create value in default unit with either float or another unit of same type
-print(f'\tInstantiated from float (5): {Set.Units.distance(5)}')
-print(f'\tInstantiated from Distance.Line(200): {Set.Units.distance(Distance.Line(200))}')
+print(f'\tInstantiated from float (5): {PreferredUnits.distance(5)}')
+print(f'\tInstantiated from Distance.Line(200): {PreferredUnits.distance(Distance.Line(200))}')
 
 # Ways to define value in units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/__init__.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,14 @@
     "Copyright 2024 David Bookstaber (https://github.com/dbookstaber)"
 )
 
 __credits__ = ["o-murphy", "dbookstaber"]
 
 from .backend import *
 from .drag_tables import *
+from .drag_model import *
 from .settings import *
-from .multiple_bc import *
 from .interface import *
 from .trajectory_data import *
 from .conditions import *
 from .munition import *
 from .unit import *
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/conditions.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/conditions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,142 +1,145 @@
 """Classes to define zeroing or current environment conditions"""
 
 import math
 from dataclasses import dataclass, field
 
-from .settings import Settings as Set
-from .unit import Distance, Velocity, Temperature, Pressure, TypedUnits, Angular
 from .munition import Weapon, Ammo
+# from .settings import Settings as Set
+from .unit import Distance, Velocity, Temperature, Pressure, Angular, Dimension, PreferredUnits
 
 __all__ = ('Atmo', 'Wind', 'Shot')
 
-cStandardHumidity: float = 0.0            # Relative Humidity
-cPressureExponent: float = 5.255876     # =g*M/R*L
+cStandardHumidity: float = 0.0  # Relative Humidity
+cPressureExponent: float = 5.255876  # =g*M/R*L
 cA0: float = 1.24871
 cA1: float = 0.0988438
 cA2: float = 0.00152907
 cA3: float = -3.07031e-06
 cA4: float = 4.21329e-07
 cA5: float = 3.342e-04
-# ISA, metric units: (https://www.engineeringtoolbox.com/international-standard-atmosphere-d_985.html)
-cDegreesCtoK: float = 273.15              # °K = °C + 273.15
-cStandardTemperatureC: float = 15.0       # °C
-cLapseRateMetric: float = -6.5e-03        # Lapse Rate, °C/m
+# ISA, metric prefer_units: (https://www.engineeringtoolbox.com/international-standard-atmosphere-d_985.html)
+cDegreesCtoK: float = 273.15  # °K = °C + 273.15
+cStandardTemperatureC: float = 15.0  # °C
+cLapseRateMetric: float = -6.5e-03  # Lapse Rate, °C/m
 cStandardPressureMetric: float = 1013.25  # hPa
-cSpeedOfSoundMetric: float = 331.3        # Mach1 in m/s = cSpeedOfSound * sqrt(°K)
-cStandardDensityMetric: float = 1.2250    # kg/m^3
-cDensityImperialToMetric: float = 16.0185 # lb/ft^3 to kg/m^3
+cSpeedOfSoundMetric: float = 331.3  # Mach1 in m/s = cSpeedOfSound * sqrt(°K)
+cStandardDensityMetric: float = 1.2250  # kg/m^3
+cDensityImperialToMetric: float = 16.0185  # lb/ft^3 to kg/m^3
 # ICAO standard atmosphere:
-cDegreesFtoR: float = 459.67              # °R = °F + 459.67
-cStandardTemperatureF: float = 59.0       # °F
+cDegreesFtoR: float = 459.67  # °R = °F + 459.67
+cStandardTemperatureF: float = 59.0  # °F
 cLapseRateImperial: float = -3.56616e-03  # Lapse rate, °F/ft
-cStandardPressure: float = 29.92          # InHg
-cSpeedOfSoundImperial: float = 49.0223    # Mach1 in fps = cSpeedOfSound * sqrt(°R)
-cStandardDensity: float = 0.076474        # lb/ft^3
+cStandardPressure: float = 29.92  # InHg
+cSpeedOfSoundImperial: float = 49.0223  # Mach1 in fps = cSpeedOfSound * sqrt(°R)
+cStandardDensity: float = 0.076474  # lb/ft^3
+
 
 @dataclass
-class Atmo(TypedUnits):  # pylint: disable=too-many-instance-attributes
+class Atmo(PreferredUnits.Mixin):  # pylint: disable=too-many-instance-attributes
     """Atmospheric conditions and density calculations"""
-    altitude: [float, Distance] = field(default_factory=Set.Units.distance)
-    pressure: [float, Pressure] = field(default_factory=Set.Units.pressure)
-    temperature: [float, Temperature] = field(default_factory=Set.Units.temperature)
-    humidity: float = 0.0           # Relative humidity [0% to 100%]
+
+    altitude: [float, Pressure] = Dimension(prefer_units="distance")
+    pressure: [float, Pressure] = Dimension(prefer_units="pressure")
+    temperature: [float, Temperature] = Dimension(prefer_units="temperature")
+
+    humidity: float = 0.0  # Relative humidity [0% to 100%]
     density_ratio: float = field(init=False)  # Density / cStandardDensity
     mach: Velocity = field(init=False)  # Mach 1 in reference atmosphere
     _mach1: float = field(init=False)  # Mach 1 in reference atmosphere in fps
     _a0: float = field(init=False)  # Initial reference altitude (ft)
     _t0: float = field(init=False)  # Temperature given at reference altitude °F
     _p0: float = field(init=False)  # Barometric pressure (sea level)
     _ta: float = field(init=False)  # Standard temperature at reference altitude °F
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.humidity > 1:
             self.humidity = self.humidity / 100.0
         if not 0 <= self.humidity <= 1:
             self.humidity = 0.0
         if not self.altitude:
             self.altitude = Distance.Foot(0)
         if not self.temperature:
             self.temperature = Atmo.standard_temperature(self.altitude)
         if not self.pressure:
-            self.pressure =  Atmo.standard_pressure(self.altitude)
+            self.pressure = Atmo.standard_pressure(self.altitude)
 
         self._t0 = self.temperature >> Temperature.Fahrenheit
         self._p0 = self.pressure >> Pressure.InHg
         self._a0 = self.altitude >> Distance.Foot
         self._ta = self._a0 * cLapseRateImperial + cStandardTemperatureF
         self.density_ratio = self.calculate_density(self._t0, self._p0) / cStandardDensity
         self._mach1 = Atmo.machF(self._t0)
         self.mach = Velocity.FPS(self._mach1)
 
     @staticmethod
     def standard_temperature(altitude: Distance) -> Temperature:
         """ICAO standard temperature for altitude"""
         return Temperature.Fahrenheit(cStandardTemperatureF
-                    + (altitude >> Distance.Foot) * cLapseRateImperial)
+                                      + (altitude >> Distance.Foot) * cLapseRateImperial)
 
     @staticmethod
     def standard_pressure(altitude: Distance) -> Pressure:
         """ICAO standard pressure for altitude"""
         return Pressure.InHg(0.02953
-            * math.pow(3.73145 - (2.56555e-05) * (altitude >> Distance.Foot),
-                       cPressureExponent)
-            )
+                             * math.pow(3.73145 - 2.56555e-05 * (altitude >> Distance.Foot),
+                                        cPressureExponent)
+                             )
         # # Metric formula
         # Pressure.hPa(cStandardPressureMetric
         #     * math.pow(1 - cLapseRateMetric * (altitude >> Distance.Meter) / (cStandardTemperatureC + cDegreesCtoK),
         #                cPressureExponent))
 
     @staticmethod
-    def standard(altitude: [float, Distance] = 0, temperature: Temperature=None):
+    def standard(altitude: [float, Distance] = 0, temperature: Temperature = None) -> 'Atmo':
         """Creates standard ICAO atmosphere at given altitude.
             If temperature not specified uses standard temperature.
         """
         return Atmo.icao(altitude, temperature)
 
     @staticmethod
-    def icao(altitude: [float, Distance] = 0, temperature: Temperature=None):
+    def icao(altitude: [float, Distance] = 0, temperature: Temperature = None) -> 'Atmo':
         """Creates standard ICAO atmosphere at given altitude.
             If temperature not specified uses standard temperature.
         """
-        altitude = Set.Units.distance(altitude)
+        altitude = PreferredUnits.distance(altitude)
         if temperature is None:
             temperature = Atmo.standard_temperature(altitude)
         pressure = Atmo.standard_pressure(altitude)
 
         return Atmo(
-            altitude >> Set.Units.distance,
-            pressure >> Set.Units.pressure,
-            temperature >> Set.Units.temperature,
+            altitude >> PreferredUnits.distance,
+            pressure >> PreferredUnits.pressure,
+            temperature >> PreferredUnits.temperature,
             cStandardHumidity
         )
 
     @staticmethod
     def machF(fahrenheit: float) -> float:
         """:return: Mach 1 in fps for Fahrenheit temperature"""
         return math.sqrt(fahrenheit + cDegreesFtoR) * cSpeedOfSoundImperial
 
     @staticmethod
     def machC(celsius: float) -> float:
         """:return: Mach 1 in m/s for Celsius temperature"""
-        return math.sqrt(1+celsius / cDegreesCtoK) * cSpeedOfSoundMetric
+        return math.sqrt(1 + celsius / cDegreesCtoK) * cSpeedOfSoundMetric
 
     @staticmethod
     def air_density(t: Temperature, p: Pressure, humidity: float) -> float:
         """Source: https://en.wikipedia.org/wiki/Density_of_air#Humid_air
         :return: Density in Imperial units (lb/ft^3)
         """
         tC = t >> Temperature.Celsius
         pM = (p >> Pressure.hPa) * 100  # Pressure in Pascals
         # Tetens approximation to saturation vapor pressure:
-        psat = 6.1078*math.pow(10, 17.27 * tC / (tC + 237.3))
-        pv = humidity*psat  # Pressure of water vapor in Pascals
-        pd = pM - pv    # Partial pressure of dry air in Pascals
+        psat = 6.1078 * math.pow(10, 17.27 * tC / (tC + 237.3))
+        pv = humidity * psat  # Pressure of water vapor in Pascals
+        pd = pM - pv  # Partial pressure of dry air in Pascals
         # Density in metric units kg/m^3
-        density = (pd*0.0289652 + pv*0.018016)/(8.31446 *(tC + cDegreesCtoK))
+        density = (pd * 0.0289652 + pv * 0.018016) / (8.31446 * (tC + cDegreesCtoK))
         return density / cDensityImperialToMetric
 
     @property
     def density_metric(self) -> float:
         """Returns density in kg/m^3"""
         return self.density_ratio * cStandardDensityMetric
 
@@ -166,91 +169,94 @@
             hc = 1.0
 
         density = cStandardDensity * (
                 (cStandardTemperatureF + cDegreesFtoR) / (t + cDegreesFtoR)
         ) * hc
         return density
 
-    def get_density_factor_and_mach_for_altitude(self, altitude: float):
+    def get_density_factor_and_mach_for_altitude(self, altitude: float) -> (float, float):
         """
         :param altitude: ASL in units of feet
         :return: density ratio and Mach 1 (fps) for the specified altitude
         """
         # Within 30 ft of initial altitude use initial values
         if math.fabs(self._a0 - altitude) < 30:
             density_ratio = self.density_ratio
             mach = self._mach1
         else:
             # https://en.wikipedia.org/wiki/Density_of_air#Exponential_approximation
-            density_ratio = math.exp(-altitude/34112.0)
+            density_ratio = math.exp(-altitude / 34112.0)
             t = self.temperature_at_altitude(altitude)
             mach = Atmo.machF(t)
         return density_ratio, mach
 
 
 @dataclass
-class Wind(TypedUnits):
+class Wind(PreferredUnits.Mixin):
     """
     Wind direction and velocity by down-range distance.
     direction_from = 0 is blowing from behind shooter. 
     direction_from = 90 degrees is blowing from shooter's left towards right.
     """
-    velocity: [float, Velocity] = field(default_factory=Set.Units.velocity)
-    direction_from: [float, Angular] = field(default_factory=Set.Units.angular)
-    until_distance: [float, Distance] = field(default_factory=Set.Units.distance)
+
+    velocity: [float, Velocity] = Dimension(prefer_units='velocity')
+    direction_from: [float, Angular] = Dimension(prefer_units='angular')
+    until_distance: [float, Distance] = Dimension(prefer_units='distance')
     MAX_DISTANCE_FEET = 1e8
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if not self.until_distance:
             self.until_distance = Distance.Foot(Wind.MAX_DISTANCE_FEET)
         if not self.direction_from or not self.velocity:
             self.direction_from = 0
             self.velocity = 0
 
 
 @dataclass
-class Shot(TypedUnits):
+class Shot(PreferredUnits.Mixin):
     """
     Stores shot parameters for the trajectory calculation.
     
     :param look_angle: Angle of sight line relative to horizontal.
-        If look_angle != 0 then any target in sight crosshairs will be at a different altitude:
+        If the look_angle != 0 then any target in sight crosshairs will be at a different altitude:
             With target_distance = sight distance to a target (i.e., as through a rangefinder):
                 * Horizontal distance X to target = cos(look_angle) * target_distance
                 * Vertical distance Y to target = sin(look_angle) * target_distance
     :param relative_angle: Elevation adjustment added to weapon.zero_elevation for a particular shot.
     :param cant_angle: Tilt of gun from vertical, which shifts any barrel elevation
         from the vertical plane into the horizontal plane by sine(cant_angle)
     """
-    look_angle: [float, Angular] = field(default_factory=Set.Units.angular)
-    relative_angle: [float, Angular] = field(default_factory=Set.Units.angular)
-    cant_angle: [float, Angular] = field(default_factory=Set.Units.angular)
+
+    look_angle: [float, Angular] = Dimension(prefer_units='angular')
+    relative_angle: [float, Angular] = Dimension(prefer_units='angular')
+    cant_angle: [float, Angular] = Dimension(prefer_units='angular')
 
     weapon: Weapon = field(default=None)
     ammo: Ammo = field(default=None)
     atmo: Atmo = field(default=None)
     winds: list[Wind] = field(default=None)
+
     # NOTE: Calculator assumes that winds are sorted by Wind.until_distance (ascending)
 
     @property
     def barrel_elevation(self) -> Angular:
         """Barrel elevation in vertical plane from horizontal"""
         return Angular.Radian((self.look_angle >> Angular.Radian)
                               + math.cos(self.cant_angle >> Angular.Radian)
                               * ((self.weapon.zero_elevation >> Angular.Radian)
-                               + (self.relative_angle >> Angular.Radian)))
+                                 + (self.relative_angle >> Angular.Radian)))
 
     @property
     def barrel_azimuth(self) -> Angular:
         """Horizontal angle of barrel relative to sight line"""
         return Angular.Radian(math.sin(self.cant_angle >> Angular.Radian)
                               * ((self.weapon.zero_elevation >> Angular.Radian)
-                               + (self.relative_angle >> Angular.Radian)))
+                                 + (self.relative_angle >> Angular.Radian)))
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if not self.look_angle:
             self.look_angle = 0
         if not self.relative_angle:
             self.relative_angle = 0
         if not self.cant_angle:
             self.cant_angle = 0
         if not self.atmo:
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/drag_tables.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/drag_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Templates of the common used drag tables"""
 
+
 TableG1 = [
     {'Mach': 0.00, 'CD': 0.2629},
     {'Mach': 0.05, 'CD': 0.2558},
     {'Mach': 0.10, 'CD': 0.2487},
     {'Mach': 0.15, 'CD': 0.2413},
     {'Mach': 0.20, 'CD': 0.2344},
     {'Mach': 0.25, 'CD': 0.2278},
@@ -662,9 +663,7 @@
     {'Mach': 3.75, 'CD': 0.9355},
     {'Mach': 3.80, 'CD': 0.9340},
     {'Mach': 3.85, 'CD': 0.9325},
     {'Mach': 3.90, 'CD': 0.9310},
     {'Mach': 3.95, 'CD': 0.9295},
     {'Mach': 4.00, 'CD': 0.9280},
 ]
-
-DragTablesSet = [value for key, value in globals().items() if key.startswith("Table")]
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/example.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Example of library usage"""
 
+# pylint: disable=wildcard-import,unused-wildcard-import
 from py_ballisticcalc import *
 from py_ballisticcalc import Settings as Set
 
-# Modify default units
-Set.Units.velocity = Velocity.FPS
-Set.Units.temperature = Temperature.Celsius
-Set.Units.distance = Distance.Meter
-Set.Units.sight_height = Distance.Centimeter
+# Modify default prefer_units
+PreferredUnits.velocity = Velocity.FPS
+PreferredUnits.temperature = Temperature.Celsius
+PreferredUnits.distance = Distance.Meter
+PreferredUnits.sight_height = Distance.Centimeter
 
 Set.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
 
 # Define ammunition parameters
 weight, diameter = 168, 0.308  # Numbers will be assumed to use default Settings.Units
-length = Distance.Inch(1.282)  # Or declare units explicitly
+length = Distance.Inch(1.282)  # Or declare prefer_units explicitly
 dm = DragModel(0.223, TableG7, weight, diameter, length)
 ammo = Ammo(dm, 2750, 15)
 ammo.calc_powder_sens(2723, 0)
 gun = Weapon(sight_height=9, twist=12)
 current_atmo = Atmo(110, 29.8, 15, 72)
 current_winds = [Wind(2, 90)]
 shot = Shot(weapon=gun, ammo=ammo, atmo=current_atmo, winds=current_winds)
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/interface.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Implements basic interface for the ballistics calculator"""
 from dataclasses import dataclass, field
 
 from .conditions import Shot
 # pylint: disable=import-error,no-name-in-module,wildcard-import,unused-wildcard-import
 from .backend import *
 from .trajectory_data import HitResult
-from .unit import Angular, Distance
-from .settings import Settings
+from .unit import Angular, Distance, PreferredUnits
+
 
 __all__ = ('Calculator',)
 
 
 @dataclass
 class Calculator:
     """Basic interface for the ballistics calculator"""
@@ -20,46 +20,47 @@
     @property
     def cdm(self):
         """returns custom drag function based on input data"""
         return self._calc._table_data
 
     def barrel_elevation_for_target(self, shot: Shot, target_distance: [float, Distance]) -> Angular:
         """Calculates barrel elevation to hit target at zero_distance.
-
+        :param shot: Shot instance for which calculate barrel elevation is
         :param target_distance: Look-distance to "zero," which is point we want to hit.
             This is the distance that a rangefinder would return with no ballistic adjustment.
             NB: Some rangefinders offer an adjusted distance based on inclinometer measurement.
                 However, without a complete ballistic model these can only approximate the effects
                 on ballistic trajectory of shooting uphill or downhill.  Therefore:
                 For maximum accuracy, use the raw sight distance and look_angle as inputs here.
         """
         self._calc = TrajectoryCalc(shot.ammo)
-        target_distance = Settings.Units.distance(target_distance)
+        target_distance = PreferredUnits.distance(target_distance)
         total_elevation = self._calc.zero_angle(shot, target_distance)
-        return Angular.Radian((total_elevation >> Angular.Radian)
-                                 - (shot.look_angle >> Angular.Radian))
+        return Angular.Radian(
+            (total_elevation >> Angular.Radian) - (shot.look_angle >> Angular.Radian)
+        )
 
     def set_weapon_zero(self, shot: Shot, zero_distance: [float, Distance]) -> Angular:
         """Sets shot.weapon.zero_elevation so that it hits a target at zero_distance.
-
-        :param target_distance: Look-distance to "zero," which is point we want to hit.
+        :param shot: Shot instance from which we take a zero
+        :param zero_distance: Look-distance to "zero," which is point we want to hit.
         """
         shot.weapon.zero_elevation = self.barrel_elevation_for_target(shot, zero_distance)
         return shot.weapon.zero_elevation
 
     def fire(self, shot: Shot, trajectory_range: [float, Distance],
              trajectory_step: [float, Distance] = 0,
              extra_data: bool = False) -> HitResult:
         """Calculates trajectory
         :param shot: shot parameters (initial position and barrel angle)
-        :param range: Downrange distance at which to stop computing trajectory
+        :param trajectory_range: Downrange distance at which to stop computing trajectory
         :param trajectory_step: step between trajectory points to record
         :param extra_data: True => store TrajectoryData for every calculation step;
             False => store TrajectoryData only for each trajectory_step
         """
-        trajectory_range = Settings.Units.distance(trajectory_range)
+        trajectory_range = PreferredUnits.distance(trajectory_range)
         if not trajectory_step:
             trajectory_step = trajectory_range.unit_value / 10.0
-        step = Settings.Units.distance(trajectory_step)
+        step = PreferredUnits.distance(trajectory_step)
         self._calc = TrajectoryCalc(shot.ammo)
         data = self._calc.trajectory(shot, trajectory_range, step, extra_data)
         return HitResult(shot, data, extra_data)
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/munition.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/munition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 """Module for Weapon and Ammo properties definitions"""
 import math
 from dataclasses import dataclass, field
 
 from .drag_model import DragModel
-from .settings import Settings as Set
-from .unit import TypedUnits, Velocity, Temperature, Distance, Angular
+from .unit import Velocity, Temperature, Distance, Angular, PreferredUnits, Dimension
 
 __all__ = ('Weapon', 'Ammo')
 
 
 @dataclass
-class Weapon(TypedUnits):
+class Weapon(PreferredUnits.Mixin):
     """
     :param sight_height: Vertical distance from center of bore line to center of sight line.
     :param twist: Distance for barrel rifling to complete one complete turn.
         Positive value => right-hand twist, negative value => left-hand twist.
     :param zero_elevation: Angle of barrel relative to sight line when sight is set to "zero."
         (Typically computed by ballistic Calculator.)
     """
-    sight_height: [float, Distance] = field(default_factory=Set.Units.sight_height)
-    twist: [float, Distance] = field(default_factory=Set.Units.twist)
-    zero_elevation: [float, Angular] = field(default_factory=Set.Units.angular)
+    sight_height: [float, Distance] = Dimension(prefer_units='sight_height')
+    twist: [float, Distance] = Dimension(prefer_units='twist')
+    zero_elevation: [float, Angular] = Dimension(prefer_units='angular')
 
     def __post_init__(self):
         if not self.sight_height:
             self.sight_height = 0
         if not self.twist:
             self.twist = 0
         if not self.zero_elevation:
             self.zero_elevation = 0
 
 
 @dataclass
-class Ammo(TypedUnits):
+class Ammo(PreferredUnits.Mixin):
     """
     :param dm: DragModel for projectile
     :param mv: Muzzle Velocity
     :param powder_temp: Baseline temperature that produces the given mv
     :param temp_modifier: Change in velocity w temperature: % per 15°C.
         Can be computed with .calc_powder_sens().  Only applies if:
             Settings.USE_POWDER_SENSITIVITY = True
     """
     dm: DragModel = field(default=None)
-    mv: [float, Velocity] = field(default_factory=Set.Units.velocity)
-    powder_temp: [float, Temperature] = field(default_factory=Set.Units.temperature)
+    mv: [float, Velocity] = Dimension(prefer_units='velocity')
+    powder_temp: [float, Temperature] = Dimension(prefer_units='temperature')
     temp_modifier: float = field(default=0)
 
     def __post_init__(self):
         if not self.powder_temp:
             self.powder_temp = Temperature.Celsius(15)
 
     def calc_powder_sens(self, other_velocity: [float, Velocity],
@@ -55,16 +54,16 @@
         """Calculates velocity correction by temperature change; assigns to self.temp_modifier
         :param other_velocity: other velocity at other_temperature
         :param other_temperature: other temperature
         :return: temperature modifier in terms %v_delta/15°C
         """
         v0 = self.mv >> Velocity.MPS
         t0 = self.powder_temp >> Temperature.Celsius
-        v1 = Set.Units.velocity(other_velocity) >> Velocity.MPS
-        t1 = Set.Units.temperature(other_temperature) >> Temperature.Celsius
+        v1 = PreferredUnits.velocity(other_velocity) >> Velocity.MPS
+        t1 = PreferredUnits.temperature(other_temperature) >> Temperature.Celsius
 
         v_delta = math.fabs(v0 - v1)
         t_delta = math.fabs(t0 - t1)
         v_lower = v1 if v1 < v0 else v0
 
         if v_delta == 0 or t_delta == 0:
             raise ValueError(
@@ -77,11 +76,11 @@
     def get_velocity_for_temp(self, current_temp: [float, Temperature]) -> Velocity:
         """Calculates muzzle velocity at temperature, based on temp_modifier.
         :param current_temp: Temperature of cartridge powder
         :return: Muzzle velocity corrected to current_temp
         """
         v0 = self.mv >> Velocity.MPS
         t0 = self.powder_temp >> Temperature.Celsius
-        t1 = Set.Units.temperature(current_temp) >> Temperature.Celsius
+        t1 = PreferredUnits.temperature(current_temp) >> Temperature.Celsius
         t_delta = t1 - t0
         muzzle_velocity = self.temp_modifier / (15 / v0) * t_delta + v0
         return Velocity.MPS(muzzle_velocity)
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_calc.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# pylint: disable=missing-class-docstring,missing-function-docstring,line-too-long,invalid-name,attribute-defined-outside-init
+# pylint: disable=missing-class-docstring,missing-function-docstring
+# pylint: disable=line-too-long,invalid-name,attribute-defined-outside-init
 """pure python trajectory calculation backend"""
 
 import math
 from dataclasses import dataclass
 from typing import NamedTuple
 
+from .drag_model import DragDataPoint
 from .conditions import Atmo, Shot, Wind
 from .munition import Ammo
 from .settings import Settings
 from .trajectory_data import TrajectoryData, TrajFlag
 from .unit import Distance, Angular, Velocity, Weight, Energy, Pressure, Temperature
 
-__all__ = ('TrajectoryCalc', )
+__all__ = ('TrajectoryCalc',)
 
 cZeroFindingAccuracy = 0.000005
 cMinimumVelocity = 50.0
 cMaximumDrop = -15000
 cMaxIterations = 20
 cGravityConstant = -32.17405
 
 
 class CurvePoint(NamedTuple):
+    """Coefficients for quadratic interpolation"""
     a: float
     b: float
     c: float
 
 
 @dataclass
 class Vector:
@@ -97,15 +100,16 @@
     def __init__(self, ammo: Ammo):
         self.ammo = ammo
         self._bc = self.ammo.dm.BC
         self._table_data = ammo.dm.drag_table
         self._curve = calculate_curve(self._table_data)
         self.gravity_vector = Vector(.0, cGravityConstant, .0)
 
-    def get_calc_step(self, step: float = 0):
+    @staticmethod
+    def get_calc_step(step: float = 0):
         """Keep step under max_calc_step_size
         :param step: proposed step size
         :return: step size for calculations (in feet)
         """
         if step == 0:
             return Settings.get_max_calc_step_size() / 2.0
         return min(step, Settings.get_max_calc_step_size()) / 2.0
@@ -146,15 +150,15 @@
         :param distance: Zero distance
         :return: Barrel elevation to hit height zero at zero distance
         """
         self._init_trajectory(shot_info)
 
         zero_distance = math.cos(self.look_angle) * (distance >> Distance.Foot)
         height_at_zero = math.sin(self.look_angle) * (distance >> Distance.Foot)
-        maximum_range = zero_distance - 1.5*self.calc_step
+        maximum_range = zero_distance - 1.5 * self.calc_step
         self.barrel_azimuth = 0.0
         self.barrel_elevation = math.atan(height_at_zero / zero_distance)
         self.twist = 0
 
         iterations_count = 0
         zero_finding_error = cZeroFindingAccuracy * 2
         # x = horizontal distance down range, y = drop, z = windage
@@ -175,53 +179,53 @@
             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
         return Angular.Radian(self.barrel_elevation)
 
     def _trajectory(self, shot_info: Shot, maximum_range: float, step: float,
                     filter_flags: TrajFlag) -> list[TrajectoryData]:
         """Calculate trajectory for specified shot
         :param maximum_range: Feet down range to stop calculation
-        :param dist_step: Frequency (in feet down range) to record TrajectoryData
+        :param step: Frequency (in feet down range) to record TrajectoryData
         :return: list of TrajectoryData, one for each dist_step, out to max_range
         """
         ranges = []  # Record of TrajectoryData points to return
         ranges_length = int(maximum_range / step) + 1
         time = 0
         previous_mach = .0
         drag = 0
 
-        #region Initialize wind-related variables to first wind reading (if any)
+        # region Initialize wind-related variables to first wind reading (if any)
         len_winds = len(shot_info.winds)
         current_wind = 0
         current_item = 0
         next_range_distance = .0
         next_wind_range = Wind.MAX_DISTANCE_FEET
         if len_winds < 1:
             wind_vector = Vector(.0, .0, .0)
         else:
             wind_vector = wind_to_vector(shot_info.winds[0])
             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot
-        #endregion
+        # endregion
 
-        #region Initialize velocity and position of projectile
+        # region Initialize velocity and position of projectile
         velocity = self.muzzle_velocity
         # x: downrange distance, y: drop, z: windage
-        range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
+        range_vector = Vector(.0, -self.cant_cosine * self.sight_height, -self.cant_sine * self.sight_height)
         velocity_vector = Vector(math.cos(self.barrel_elevation) * math.cos(self.barrel_azimuth),
                                  math.sin(self.barrel_elevation),
                                  math.cos(self.barrel_elevation) * math.sin(self.barrel_azimuth)) * velocity
-        #endregion
+        # endregion
 
         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
-        seen_zero = TrajFlag.NONE  # Record when we see each zero crossing so we only register one
+        seen_zero = TrajFlag.NONE  # Record when we see each zero crossing, so we only register one
         if range_vector.y >= 0:
             seen_zero |= TrajFlag.ZERO_UP  # We're starting above zero; we can only go down
         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
             seen_zero |= TrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
 
-        #region Trajectory Loop
+        # region Trajectory Loop
         while range_vector.x <= maximum_range + self.calc_step:
             _flag = TrajFlag.NONE
 
             # Update wind reading at current point in trajectory
             if range_vector.x >= next_wind_range:
                 current_wind += 1
                 if current_wind >= len_winds:  # No more winds listed after this range
@@ -231,15 +235,15 @@
                     wind_vector = wind_to_vector(shot_info.winds[current_wind])
                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
 
             # Update air density at current point in trajectory
             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(
                 self.alt0 + range_vector.y)
 
-            #region Check whether to record TrajectoryData row at current point
+            # region Check whether to record TrajectoryData row at current point
             if filter_flags:
                 # Zero-crossing checks
                 if range_vector.x > 0:
                     # Zero reference line is the sight line defined by look_angle
                     reference_height = range_vector.x * math.tan(self.look_angle)
                     # If we haven't seen ZERO_UP, we look for that first
                     if not seen_zero & TrajFlag.ZERO_UP:
@@ -267,19 +271,19 @@
                     ranges.append(create_trajectory_row(
                         time, range_vector, velocity_vector,
                         velocity, mach, self.spin_drift(time), self.look_angle,
                         density_factor, drag, self.weight, _flag.value
                     ))
                     if current_item == ranges_length:
                         break
-            #endregion
+            # endregion
 
             previous_mach = velocity / mach
 
-            #region Ballistic calculation step (point-mass)
+            # region Ballistic calculation step (point-mass)
             # Time step is set to advance bullet calc_step distance along x axis
             delta_time = self.calc_step / velocity_vector.x
             # Air resistance seen by bullet is ground velocity minus wind velocity relative to ground
             velocity_adjusted = velocity_vector - wind_vector
             velocity = velocity_adjusted.magnitude()  # Velocity relative to air
             # Drag is a function of air density and velocity relative to the air
             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
@@ -292,45 +296,45 @@
             # Update the bullet position
             range_vector += delta_range_vector
             velocity = velocity_vector.magnitude()  # Velocity relative to ground
             time += delta_range_vector.magnitude() / velocity
 
             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:
                 break
-            #endregion
-        #endregion
+            # endregion
+        # endregion
         # If filter_flags == 0 then all we want is the ending value
         if not filter_flags:
             ranges.append(create_trajectory_row(
-                        time, range_vector, velocity_vector,
-                        velocity, mach, self.spin_drift(time), self.look_angle,
-                        density_factor, drag, self.weight, _flag.value))
+                time, range_vector, velocity_vector,
+                velocity, mach, self.spin_drift(time), self.look_angle,
+                density_factor, drag, self.weight, _flag.value))
         return ranges
 
     def drag_by_mach(self, mach: float) -> float:
         """ Drag force = V^2 * Cd * AirDensity * S / 2m where:
                 cStandardDensity of Air = 0.076474 lb/ft^3
                 S is cross-section = d^2 pi/4, where d is bullet diameter in inches
                 m is bullet mass in pounds
-            BC contains m/d^2 in units lb/in^2, which we multiply by 144 to convert to lb/ft^2
+            bc contains m/d^2 in units lb/in^2, which we multiply by 144 to convert to lb/ft^2
             Thus: The magic constant found here = StandardDensity * pi / (4 * 2 * 144)
         :return: Drag coefficient at the given mach number
         """
         cd = calculate_by_curve(self._table_data, self._curve, mach)
         return cd * 2.08551e-04 / self._bc
 
     def spin_drift(self, time) -> float:
         """Litz spin-drift approximation
         :param time: Time of flight
         :return: windage due to spin drift, in feet
         """
         if self.twist != 0:
             sign = 1 if self.twist > 0 else -1
             return sign * (1.25 * (self.stability_coefficient + 1.2)
-                        * math.pow(time, 1.83) ) / 12
+                           * math.pow(time, 1.83)) / 12
         return 0
 
     def calc_stability_coefficient(self, atmo: Atmo) -> float:
         """Miller stability coefficient"""
         if self.twist and self.length and self.diameter:
             twist_rate = math.fabs(self.twist) / self.diameter
             length = self.length / self.diameter
@@ -363,36 +367,53 @@
     cross_component = (wind.velocity >> Velocity.FPS) * math.sin(wind.direction_from >> Angular.Radian)
     return Vector(range_component, 0, cross_component)
 
 
 def create_trajectory_row(time: float, range_vector: Vector, velocity_vector: Vector,
                           velocity: float, mach: float, spin_drift: float, look_angle: float,
                           density_factor: float, drag: float, weight: float, flag: int) -> TrajectoryData:
+    """
+    Create a TrajectoryData object representing a single row of trajectory data.
+
+    :param time: Time of flight.
+    :param range_vector: Vector representing range.
+    :param velocity_vector: Vector representing velocity.
+    :param velocity: Velocity value.
+    :param mach: Mach number.
+    :param spin_drift: Spin drift value.
+    :param look_angle: Look angle value.
+    :param density_factor: Density factor.
+    :param drag: Drag value.
+    :param weight: Weight value.
+    :param flag: Flag value.
+
+    :return: A TrajectoryData object representing the trajectory data.
+    """
     windage = range_vector.z + spin_drift
     drop_adjustment = get_correction(range_vector.x, range_vector.y)
     windage_adjustment = get_correction(range_vector.x, windage)
     trajectory_angle = math.atan(velocity_vector.y / velocity_vector.x)
 
     return TrajectoryData(
-        time= time,
-        distance= Distance.Foot(range_vector.x),
-        velocity= Velocity.FPS(velocity),
-        mach= velocity / mach,
-        height= Distance.Foot(range_vector.y),
-        target_drop= Distance.Foot((range_vector.y - range_vector.x * math.tan(look_angle))*math.cos(look_angle)),
-        drop_adj= Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
-        windage= Distance.Foot(windage),
-        windage_adj= Angular.Radian(windage_adjustment),
-        look_distance= Distance.Foot(range_vector.x / math.cos(look_angle)),
-        angle = Angular.Radian(trajectory_angle),
-        density_factor = density_factor-1,
-        drag = drag,
-        energy = Energy.FootPound(calculate_energy(weight, velocity)),
-        ogw = Weight.Pound(calculate_ogw(weight, velocity)),
-        flag = flag
+        time=time,
+        distance=Distance.Foot(range_vector.x),
+        velocity=Velocity.FPS(velocity),
+        mach=velocity / mach,
+        height=Distance.Foot(range_vector.y),
+        target_drop=Distance.Foot((range_vector.y - range_vector.x * math.tan(look_angle)) * math.cos(look_angle)),
+        drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
+        windage=Distance.Foot(windage),
+        windage_adj=Angular.Radian(windage_adjustment),
+        look_distance=Distance.Foot(range_vector.x / math.cos(look_angle)),
+        angle=Angular.Radian(trajectory_angle),
+        density_factor=density_factor - 1,
+        drag=drag,
+        energy=Energy.FootPound(calculate_energy(weight, velocity)),
+        ogw=Weight.Pound(calculate_ogw(weight, velocity)),
+        flag=flag
     )
 
 
 def get_correction(distance: float, offset: float) -> float:
     """:return: Sight adjustment in radians"""
     if distance != 0:
         return math.atan(offset / distance)
@@ -405,70 +426,72 @@
 
 
 def calculate_ogw(bullet_weight: float, velocity: float) -> float:
     """:return: Optimal Game Weight in pounds"""
     return math.pow(bullet_weight, 2) * math.pow(velocity, 3) * 1.5e-12
 
 
-def calculate_curve(data_points) -> list[CurvePoint]:
-    """
-    :param DragTable: data_points
+def calculate_curve(data_points: list[DragDataPoint]) -> list[CurvePoint]:
+    """Piecewise quadratic interpolation of drag curve
+    :param data_points: List[{Mach, CD}] data_points in ascending Mach order
     :return: List[CurvePoints] to interpolate drag coefficient
     """
     # rate, x1, x2, x3, y1, y2, y3, a, b, c
     # curve = []
     # curve_point
     # num_points, len_data_points, len_data_range
 
-    rate = (data_points[1]['CD'] - data_points[0]['CD']) \
-           / (data_points[1]['Mach'] - data_points[0]['Mach'])
-    curve = [CurvePoint(0, rate, data_points[0]['CD'] - data_points[0]['Mach'] * rate)]
+    rate = (data_points[1].CD - data_points[0].CD
+            ) / (data_points[1].Mach - data_points[0].Mach)
+    curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
     len_data_points = int(len(data_points))
     len_data_range = len_data_points - 1
 
     for i in range(1, len_data_range):
-        x1 = data_points[i - 1]['Mach']
-        x2 = data_points[i]['Mach']
-        x3 = data_points[i + 1]['Mach']
-        y1 = data_points[i - 1]['CD']
-        y2 = data_points[i]['CD']
-        y3 = data_points[i + 1]['CD']
+        x1 = data_points[i - 1].Mach
+        x2 = data_points[i].Mach
+        x3 = data_points[i + 1].Mach
+        y1 = data_points[i - 1].CD
+        y2 = data_points[i].CD
+        y3 = data_points[i + 1].CD
         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
         c = y1 - (a * x1 * x1 + b * x1)
         curve_point = CurvePoint(a, b, c)
         curve.append(curve_point)
 
     num_points = len_data_points
-    rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \
-           (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
+    rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
+           (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
     curve_point = CurvePoint(
-        0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate
+        0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate
     )
     curve.append(curve_point)
     return curve
 
 
 def calculate_by_curve(data: list, curve: list, mach: float) -> float:
-    """Binary search for drag coefficient based on Mach number
-    :param DragTable: data
-    :param List: Output of calculate_curve(data)
+    """
+    Binary search for drag coefficient based on Mach number
+    :param data: data
+    :param curve: Output of calculate_curve(data)
+    :param mach: Mach value for which we're searching for CD
     :return float: drag coefficient
     """
     num_points = int(len(curve))
     mlo = 0
     mhi = num_points - 2
 
     while mhi - mlo > 1:
         mid = int(math.floor(mhi + mlo) / 2.0)
-        if data[mid]['Mach'] < mach:
+        if data[mid].Mach < mach:
             mlo = mid
         else:
             mhi = mid
 
-    if data[mhi]['Mach'] - mach > mach - data[mlo]['Mach']:
+    if data[mhi].Mach - mach > mach - data[mlo].Mach:
         m = mlo
     else:
         m = mhi
     curve_m = curve[m]
     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/trajectory_data.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/trajectory_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import logging
 import math
 import typing
 from dataclasses import dataclass, field
 from enum import Flag
 from typing import NamedTuple
 
-from .settings import Settings as Set
-from .unit import Angular, Distance, Weight, Velocity, Energy, AbstractUnit, Unit
+from .unit import Angular, Distance, Weight, Velocity, Energy, AbstractUnit, Unit, PreferredUnits
 from .conditions import Shot
 
 try:
     import pandas as pd
 except ImportError as error:
     logging.warning("Install pandas to convert trajectory to dataframe")
     pd = None
@@ -21,15 +20,14 @@
     from matplotlib import patches
 except ImportError as error:
     logging.warning("Install matplotlib to get results as a plot")
     matplotlib = None
 
 __all__ = ('TrajectoryData', 'HitResult', 'TrajFlag')
 
-
 PLOT_FONT_HEIGHT = 72
 PLOT_FONT_SIZE = 552 / PLOT_FONT_HEIGHT
 
 
 class TrajFlag(Flag):
     """Flags for marking trajectory row if Zero or Mach crossing
     Also uses to set a filters for a trajectory calculation loop
@@ -48,28 +46,28 @@
     """
     Data for one point in ballistic trajectory
 
     Attributes:
         time (float): bullet flight time
         distance (Distance): x-axis coordinate
         velocity (Velocity): velocity
-        mach (float): velocity in Mach units
+        mach (float): velocity in Mach prefer_units
         height (Distance): y-axis coordinate
         target_drop (Distance): drop relative to sight-line
         drop_adj (Angular): sight adjustment to zero target_drop at this distance
         windage (Distance):
         windage_adj (Angular):
         look_distance (Distance): sight-line distance = .distance/cosine(look_angle)
-        look_height (Distance): y-coordinate of sight-line = .distance*tan(look_angle)
-        angle (Angular): Angle of velocity vector relative to x axis
+        # look_height (Distance): y-coordinate of sight-line = .distance*tan(look_angle)
+        angle (Angular): Angle of velocity vector relative to x-axis
         density_factor (float): Ratio of air density here to standard density
         drag (float): Current drag coefficient
         energy (Energy):
         ogw (Weight): optimal game weight
-        rtype (int): row type
+        flag (int): row type
     """
 
     time: float
     distance: Distance
     velocity: Velocity
     mach: float
     height: Distance
@@ -83,122 +81,121 @@
     drag: float
     energy: Energy
     ogw: Weight
     flag: typing.Union[TrajFlag, int]
 
     def formatted(self) -> tuple:
         """
-        :return: matrix of formatted strings for each value of trajectory in default units
+        :return: matrix of formatted strings for each value of trajectory in default prefer_units
         """
 
         def _fmt(v: AbstractUnit, u: Unit):
             """simple formatter"""
             return f"{v >> u:.{u.accuracy}f} {u.symbol}"
 
         return (
             f'{self.time:.3f} s',
-            _fmt(self.distance, Set.Units.distance),
-            _fmt(self.velocity, Set.Units.velocity),
+            _fmt(self.distance, PreferredUnits.distance),
+            _fmt(self.velocity, PreferredUnits.velocity),
             f'{self.mach:.2f} mach',
-            _fmt(self.height, Set.Units.drop),
-            _fmt(self.target_drop, Set.Units.drop),
-            _fmt(self.drop_adj, Set.Units.adjustment),
-            _fmt(self.windage, Set.Units.drop),
-            _fmt(self.windage_adj, Set.Units.adjustment),
-            _fmt(self.look_distance, Set.Units.distance),
-            _fmt(self.angle, Set.Units.angular),
+            _fmt(self.height, PreferredUnits.drop),
+            _fmt(self.target_drop, PreferredUnits.drop),
+            _fmt(self.drop_adj, PreferredUnits.adjustment),
+            _fmt(self.windage, PreferredUnits.drop),
+            _fmt(self.windage_adj, PreferredUnits.adjustment),
+            _fmt(self.look_distance, PreferredUnits.distance),
+            _fmt(self.angle, PreferredUnits.angular),
             f'{self.density_factor:.3e}',
             f'{self.drag:.3f}',
-            _fmt(self.energy, Set.Units.energy),
-            _fmt(self.ogw, Set.Units.ogw),
+            _fmt(self.energy, PreferredUnits.energy),
+            _fmt(self.ogw, PreferredUnits.ogw),
 
             self.flag
         )
 
     def in_def_units(self) -> tuple:
         """
-        :return: matrix of floats of the trajectory in default units
+        :return: matrix of floats of the trajectory in default prefer_units
         """
         return (
             self.time,
-            self.distance >> Set.Units.distance,
-            self.velocity >> Set.Units.velocity,
+            self.distance >> PreferredUnits.distance,
+            self.velocity >> PreferredUnits.velocity,
             self.mach,
-            self.height >> Set.Units.drop,
-            self.target_drop >> Set.Units.drop,
-            self.drop_adj >> Set.Units.adjustment,
-            self.windage >> Set.Units.drop,
-            self.windage_adj >> Set.Units.adjustment,
-            self.look_distance >> Set.Units.distance,
-            self.angle >> Set.Units.angular,
+            self.height >> PreferredUnits.drop,
+            self.target_drop >> PreferredUnits.drop,
+            self.drop_adj >> PreferredUnits.adjustment,
+            self.windage >> PreferredUnits.drop,
+            self.windage_adj >> PreferredUnits.adjustment,
+            self.look_distance >> PreferredUnits.distance,
+            self.angle >> PreferredUnits.angular,
             self.density_factor,
             self.drag,
-            self.energy >> Set.Units.energy,
-            self.ogw >> Set.Units.ogw,
+            self.energy >> PreferredUnits.energy,
+            self.ogw >> PreferredUnits.ogw,
             TrajFlag(self.flag)
         )
 
 
 class DangerSpace(NamedTuple):
     """Stores the danger space data for distance specified"""
     at_range: TrajectoryData
     target_height: Distance
     begin: TrajectoryData
     end: TrajectoryData
     look_angle: Angular
 
     def __str__(self) -> str:
-        return f'Danger space at {self.at_range.distance << Set.Units.distance} '\
-          + f'for {self.target_height << Set.Units.drop} tall target '\
-          + (f'at {self.look_angle << Angular.Degree} look-angle ' if self.look_angle != 0 else '')\
-          + f'ranges from {self.begin.distance << Set.Units.distance} '\
-          + f'to {self.end.distance << Set.Units.distance}'
+        return f'Danger space at {self.at_range.distance << PreferredUnits.distance} ' \
+            + f'for {self.target_height << PreferredUnits.drop} tall target ' \
+            + (f'at {self.look_angle << Angular.Degree} look-angle ' if self.look_angle != 0 else '') \
+            + f'ranges from {self.begin.distance << PreferredUnits.distance} ' \
+            + f'to {self.end.distance << PreferredUnits.distance}'
 
-    def overlay(self, ax: 'Axes', label: str=None):
+    def overlay(self, ax: 'Axes', label: str = None):
         """Highlights danger-space region on plot"""
         if matplotlib is None:
             raise ImportError("Install matplotlib to get results as a plot")
 
         cosine = math.cos(self.look_angle >> Angular.Radian)
-        begin_dist = (self.begin.distance >> Set.Units.distance) * cosine
-        begin_drop = (self.begin.height >> Set.Units.drop) * cosine
-        end_dist = (self.end.distance >> Set.Units.distance) * cosine
-        end_drop = (self.end.height >> Set.Units.drop) * cosine
-        range_dist = (self.at_range.distance >> Set.Units.distance) * cosine
-        range_drop = (self.at_range.height >> Set.Units.drop) * cosine
-        h = self.target_height >> Set.Units.drop
+        begin_dist = (self.begin.distance >> PreferredUnits.distance) * cosine
+        begin_drop = (self.begin.height >> PreferredUnits.drop) * cosine
+        end_dist = (self.end.distance >> PreferredUnits.distance) * cosine
+        end_drop = (self.end.height >> PreferredUnits.drop) * cosine
+        range_dist = (self.at_range.distance >> PreferredUnits.distance) * cosine
+        range_drop = (self.at_range.height >> PreferredUnits.drop) * cosine
+        h = self.target_height >> PreferredUnits.drop
 
         # Target position and height:
         ax.plot((range_dist, range_dist), (range_drop + h / 2, range_drop - h / 2),
                 color='r', linestyle=':')
         # Shaded danger-space region:
         vertices = (
             (begin_dist, begin_drop), (end_dist, begin_drop),
             (end_dist, end_drop), (begin_dist, end_drop)
         )
         polygon = patches.Polygon(vertices, closed=True,
                                   edgecolor='none', facecolor='r', alpha=0.3)
         ax.add_patch(polygon)
         if label is None:  # Add default label
-            label = f"Danger space\nat {self.at_range.distance << Set.Units.distance}"
+            label = f"Danger space\nat {self.at_range.distance << PreferredUnits.distance}"
         if label != '':
-            ax.text(begin_dist + (end_dist-begin_dist)/2, end_drop, label,
+            ax.text(begin_dist + (end_dist - begin_dist) / 2, end_drop, label,
                     linespacing=1.2, fontsize=PLOT_FONT_SIZE, ha='center', va='top')
 
 
 @dataclass(frozen=True)
 class HitResult:
     """Results of the shot"""
     shot: Shot
     trajectory: list[TrajectoryData] = field(repr=False)
     extra: bool = False
 
     def __iter__(self):
-        for row in self.trajectory:
-            yield row
+        yield from self.trajectory
 
     def __getitem__(self, item):
         return self.trajectory[item]
 
     def __check_extra__(self):
         if not self.extra:
             raise AttributeError(
@@ -217,23 +214,23 @@
     def index_at_distance(self, d: Distance) -> int:
         """
         :param d: Distance for which we want Trajectory Data
         :return: Index of first trajectory row with .distance >= d; otherwise -1
         """
         # Get index of first trajectory point with distance >= at_range
         return next((i for i in range(len(self.trajectory))
-                  if self.trajectory[i].distance >= d), -1)
+                     if self.trajectory[i].distance >= d), -1)
 
     def get_at_distance(self, d: Distance) -> TrajectoryData:
         """
         :param d: Distance for which we want Trajectory Data
         :return: First trajectory row with .distance >= d
         """
-        i = self.index_at_distance(d)
-        if i < 0:
+
+        if i := self.index_at_distance(d) < 0:
             raise ArithmeticError(
                 f"Calculated trajectory doesn't reach requested distance {d}"
             )
         return self.trajectory[i]
 
     def danger_space(self,
                      at_range: [float, Distance],
@@ -249,66 +246,63 @@
 
         :param at_range: Danger space is calculated for a target centered at this sight distance
         :param target_height: Target height (*h*) determines danger space
         :param look_angle: Ranging errors occur along the look angle to the target
         """
         self.__check_extra__()
 
-        at_range = Set.Units.distance(at_range)
-        target_height = Set.Units.distance(target_height)
+        at_range = PreferredUnits.distance(at_range)
+        target_height = PreferredUnits.distance(target_height)
         target_height_half = target_height.raw_value / 2.0
         if look_angle is None:
             look_angle = self.shot.look_angle
         else:
-            look_angle = Set.Units.angular(look_angle)
+            look_angle = PreferredUnits.angular(look_angle)
 
         # Get index of first trajectory point with distance >= at_range
-        i = self.index_at_distance(at_range)
-        if i < 0:
+        if (index := self.index_at_distance(at_range)) < 0:
             raise ArithmeticError(
                 f"Calculated trajectory doesn't reach requested distance {at_range}"
             )
 
         def find_begin_danger(row_num: int) -> TrajectoryData:
             """
-            Beginning of danger space is last .distance' < .distance where 
+            Beginning of danger space is last .distance' < .distance where
                 (.drop' - target_center) >= target_height/2
             :param row_num: Index of the trajectory point for which we are calculating danger space
             :return: Distance marking beginning of danger space
             """
             center_row = self.trajectory[row_num]
-            for i in range(row_num - 1, 0, -1):
-                prime_row = self.trajectory[i]
+            for prime_row in reversed(self.trajectory[:row_num]):
                 if (prime_row.target_drop.raw_value - center_row.target_drop.raw_value) >= target_height_half:
-                    return self.trajectory[i]
+                    return prime_row
             return self.trajectory[0]
 
         def find_end_danger(row_num: int) -> TrajectoryData:
             """
             End of danger space is first .distance' > .distance where
                 (target_center - .drop') >= target_height/2
             :param row_num: Index of the trajectory point for which we are calculating danger space
             :return: Distance marking end of danger space
             """
             center_row = self.trajectory[row_num]
-            for i in range(row_num + 1, len(self.trajectory)):
-                prime_row = self.trajectory[i]
+            for prime_row in self.trajectory[row_num + 1:]:
                 if (center_row.target_drop.raw_value - prime_row.target_drop.raw_value) >= target_height_half:
                     return prime_row
             return self.trajectory[-1]
 
-        return DangerSpace(self.trajectory[i],
+        return DangerSpace(self.trajectory[index],
                            target_height,
-                           find_begin_danger(i),
-                           find_end_danger(i),
+                           find_begin_danger(index),
+                           find_end_danger(index),
                            look_angle)
 
-    def dataframe(self, formatted: bool = False):
+    def dataframe(self, formatted: bool = False) -> 'DataFrame':
         """
-        :param formatted: False for values as floats; True for strings with units
+        :param formatted: False for values as floats; True for strings with prefer_units
         :return: the trajectory table as a DataFrame
         """
         if pd is None:
             raise ImportError("Install pandas to get trajectory as dataframe")
         col_names = list(TrajectoryData._fields)
         if formatted:
             trajectory = [p.formatted() for p in self]
@@ -324,56 +318,56 @@
         if matplotlib is None:
             raise ImportError("Install matplotlib to plot results")
         if not self.extra:
             logging.warning("HitResult.plot: To show extended data"
                             "Use Calculator.fire(..., extra_data=True)")
         font_size = PLOT_FONT_SIZE
         df = self.dataframe()
-        ax = df.plot(x='distance', y=['height'], ylabel=Set.Units.drop.symbol)
-        max_range = self.trajectory[-1].distance >> Set.Units.distance
+        ax = df.plot(x='distance', y=['height'], ylabel=PreferredUnits.drop.symbol)
+        max_range = self.trajectory[-1].distance >> PreferredUnits.distance
 
         for p in self.trajectory:
             if TrajFlag(p.flag) & TrajFlag.ZERO:
-                ax.plot([p.distance >> Set.Units.distance, p.distance >> Set.Units.distance],
-                        [df['height'].min(), p.height >> Set.Units.drop], linestyle=':')
-                ax.text((p.distance >> Set.Units.distance) + max_range/100, df['height'].min(),
+                ax.plot([p.distance >> PreferredUnits.distance, p.distance >> PreferredUnits.distance],
+                        [df['height'].min(), p.height >> PreferredUnits.drop], linestyle=':')
+                ax.text((p.distance >> PreferredUnits.distance) + max_range / 100, df['height'].min(),
                         f"{(TrajFlag(p.flag) & TrajFlag.ZERO).name}",
                         fontsize=font_size, rotation=90)
             if TrajFlag(p.flag) & TrajFlag.MACH:
-                ax.plot([p.distance >> Set.Units.distance, p.distance >> Set.Units.distance],
-                        [df['height'].min(), p.height >> Set.Units.drop], linestyle=':')
-                ax.text((p.distance >> Set.Units.distance) + max_range/100, df['height'].min(),
+                ax.plot([p.distance >> PreferredUnits.distance, p.distance >> PreferredUnits.distance],
+                        [df['height'].min(), p.height >> PreferredUnits.drop], linestyle=':')
+                ax.text((p.distance >> PreferredUnits.distance) + max_range / 100, df['height'].min(),
                         "Mach 1", fontsize=font_size, rotation=90)
 
-        max_range_in_drop_units = self.trajectory[-1].distance >> Set.Units.drop
+        max_range_in_drop_units = self.trajectory[-1].distance >> PreferredUnits.drop
         # Sight line
         x_sight = [0, df.distance.max()]
         y_sight = [0, max_range_in_drop_units * math.tan(look_angle >> Angular.Radian)]
-        ax.plot(x_sight, y_sight, linestyle='--', color=[.3,0,.3,.5])
+        ax.plot(x_sight, y_sight, linestyle='--', color=[.3, 0, .3, .5])
         # Barrel pointing line
         x_bbl = [0, df.distance.max()]
-        y_bbl = [-(self.shot.weapon.sight_height >> Set.Units.drop),
-                    max_range_in_drop_units * math.tan(self.trajectory[0].angle >> Angular.Radian)
-                    -(self.shot.weapon.sight_height >> Set.Units.drop)]
-        ax.plot(x_bbl, y_bbl, linestyle=':', color=[0,0,0,.5])
+        y_bbl = [-(self.shot.weapon.sight_height >> PreferredUnits.drop),
+                 max_range_in_drop_units * math.tan(self.trajectory[0].angle >> Angular.Radian)
+                 - (self.shot.weapon.sight_height >> PreferredUnits.drop)]
+        ax.plot(x_bbl, y_bbl, linestyle=':', color=[0, 0, 0, .5])
         # Line labels
-        sight_above_bbl = True if y_sight[1] > y_bbl[1] else False
-        angle = math.degrees(math.atan((y_sight[1]-y_sight[0])/(x_sight[1]-x_sight[0])))
+        sight_above_bbl = y_sight[1] > y_bbl[1]
+        angle = math.degrees(math.atan((y_sight[1] - y_sight[0]) / (x_sight[1] - x_sight[0])))
         ax.text(x_sight[1], y_sight[1], "Sight line", linespacing=1.2,
-                 rotation=angle, rotation_mode='anchor', transform_rotates_text=True,
-                 fontsize=font_size, color=[.3,0,.3,1], ha='right',
-                 va='bottom' if sight_above_bbl else 'top')
-        angle = math.degrees(math.atan((y_bbl[1]-y_bbl[0])/(x_bbl[1]-x_bbl[0])))
+                rotation=angle, rotation_mode='anchor', transform_rotates_text=True,
+                fontsize=font_size, color=[.3, 0, .3, 1], ha='right',
+                va='bottom' if sight_above_bbl else 'top')
+        angle = math.degrees(math.atan((y_bbl[1] - y_bbl[0]) / (x_bbl[1] - x_bbl[0])))
         ax.text(x_bbl[1], y_bbl[1], "Barrel pointing", linespacing=1.2,
-                 rotation=angle, rotation_mode='anchor', transform_rotates_text=True,
-                 fontsize=font_size, color='k', ha='right',
-                 va='top' if sight_above_bbl else 'bottom')
+                rotation=angle, rotation_mode='anchor', transform_rotates_text=True,
+                fontsize=font_size, color='k', ha='right',
+                va='top' if sight_above_bbl else 'bottom')
         # Plot velocity (on secondary axis)
-        df.plot(x='distance', xlabel=Set.Units.distance.symbol,
-                y=['velocity'], ylabel=Set.Units.velocity.symbol,
-                secondary_y=True, color=[0,.3,0,.5],
+        df.plot(x='distance', xlabel=PreferredUnits.distance.symbol,
+                y=['velocity'], ylabel=PreferredUnits.velocity.symbol,
+                secondary_y=True, color=[0, .3, 0, .5],
                 ylim=[0, df['velocity'].max()], ax=ax)
         # Let secondary shine through
         ax.set_zorder(1)
-        ax.set_facecolor([0,0,0,0])
+        ax.set_facecolor([0, 0, 0, 0])
 
         return ax
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc/unit.py` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc/unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 """
-Useful types for units of measurement conversion for ballistics calculations
+Useful types for prefer_units of measurement conversion for ballistics calculations
 """
-
-import typing
+import os
+import sys
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, MISSING, Field
 from enum import IntEnum
 from math import pi, atan, tan
-from typing import NamedTuple
-from dataclasses import dataclass
+from typing import NamedTuple, Union, TypeVar
+
+from py_ballisticcalc.logger import logger
+
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
 
 __all__ = ('Unit', 'AbstractUnit', 'UnitProps', 'UnitPropsDict', 'Distance',
            'Velocity', 'Angular', 'Temperature', 'Pressure',
-           'Energy', 'Weight', 'TypedUnits')
+           'Energy', 'Weight', 'Dimension', 'PreferredUnits', 'basicConfig')
+
+
+AbstractUnitType = TypeVar('AbstractUnitType', bound='AbstractUnit')
 
 
 # pylint: disable=invalid-name
 class Unit(IntEnum):
     """
     Usage of IntEnum simplify data serializing for using it with databases etc.
     """
@@ -59,15 +70,15 @@
     MPH = 63
     KT = 64
 
     Grain = 70
     Ounce = 71
     Gram = 72
     Pound = 73
-    Kilgram = 74
+    Kilogram = 74
     Newton = 75
 
     @property
     def key(self) -> str:
         """
         :return: readable name of the unit of measure
         """
@@ -86,22 +97,23 @@
         :return: short symbol of the unit of measure in CI
         """
         return UnitPropsDict[self].symbol
 
     def __repr__(self) -> str:
         return UnitPropsDict[self].name
 
-    def __call__(self: 'Unit', value: [int, float, 'AbstractUnit'] = None) -> ['AbstractUnit', 'Unit']:
+    def __call__(self: 'Unit', value: [int, float, AbstractUnitType] = None) -> AbstractUnitType:
         """Creates new unit instance by dot syntax
         :param self: unit as Unit enum
         :param value: numeric value of the unit
         :return: AbstractUnit instance
         """
-        if value is None:
-            return self
+
+        # if value is None:
+        #     return self
 
         if isinstance(value, AbstractUnit):
             return value << self
         if 0 <= self < 10:
             obj = Angular(value, self)
         elif 10 <= self < 20:
             obj = Distance(value, self)
@@ -169,22 +181,22 @@
     Unit.MPH: UnitProps('mph', 1, 'mph'),
     Unit.KT: UnitProps('knot', 1, 'kt'),
 
     Unit.Grain: UnitProps('grain', 1, 'gr'),
     Unit.Ounce: UnitProps('ounce', 1, 'oz'),
     Unit.Gram: UnitProps('gram', 1, 'g'),
     Unit.Pound: UnitProps('pound', 0, 'lb'),
-    Unit.Kilgram: UnitProps('kilogram', 3, 'kg'),
+    Unit.Kilogram: UnitProps('kilogram', 3, 'kg'),
     Unit.Newton: UnitProps('newton', 3, 'N'),
 }
 
 
 class AbstractUnit:
     """Abstract class for unit of measure instance definition
-    Stores defined unit and value, applies conversions to other units
+    Stores defined unit and value, applies conversions to other prefer_units
     """
     __slots__ = ('_value', '_defined_units')
 
     def __init__(self, value: [float, int], units: Unit):
         """
         :param units: unit as Unit enum
         :param value: numeric value of the unit
@@ -231,68 +243,68 @@
     def __rshift__(self, other: Unit):
         return self.get_in(other)
 
     def __rlshift__(self, other: Unit):
         return self.convert(other)
 
     def _unit_support_error(self, value: float, units: Unit):
-        """Validates the units
-        :param value: value of the unit
+        """Validates the prefer_units
+        :param value: value of the instance
         :param units: Unit enum type
-        :return: value in specified units
+        :return: value in specified prefer_units
         """
         if not isinstance(units, Unit):
             err_msg = f"Type expected: {Unit}, {type(Unit).__name__} " \
                       f"found: {type(units).__name__} ({value})"
             raise TypeError(err_msg)
         if units not in self.__dict__.values():
             raise ValueError(f'{self.__class__.__name__}: unit {units} is not supported')
         return 0
 
     def to_raw(self, value: float, units: Unit) -> float:
-        """Converts value with specified units to raw value
-        :param value: value of the unit
+        """Converts value with specified prefer_units to raw value
+        :param value: value of the instance
         :param units: Unit enum type
-        :return: value in specified units
+        :return: value in specified prefer_units
         """
         return self._unit_support_error(value, units)
 
     def from_raw(self, value: float, units: Unit) -> float:
-        """Converts raw value to specified units
+        """Converts raw value to specified prefer_units
         :param value: raw value of the unit
         :param units: Unit enum type
-        :return: value in specified units
+        :return: value in specified prefer_units
         """
         return self._unit_support_error(value, units)
 
     def convert(self, units: Unit) -> 'AbstractUnit':
-        """Returns new unit instance in specified units
+        """Returns new unit instance in specified prefer_units
         :param units: Unit enum type
-        :return: new unit instance in specified units
+        :return: new unit instance in specified prefer_units
         """
         value = self.get_in(units)
         return self.__class__(value, units)
 
     def get_in(self, units: Unit) -> float:
         """
         :param units: Unit enum type
-        :return: value in specified units
+        :return: value in specified prefer_units
         """
         return self.from_raw(self._value, units)
 
     @property
     def units(self) -> Unit:
         """
-        :return: defined units
+        :return: defined prefer_units
         """
         return self._defined_units
 
     @property
     def unit_value(self) -> float:
-        """Returns float value in defined units"""
+        """Returns float value in defined prefer_units"""
         return self.get_in(self.units)
 
     @property
     def raw_value(self) -> float:
         """Raw unit value getter
         :return: raw unit value
         """
@@ -441,15 +453,15 @@
             return super().from_raw(value, units)
         return result
 
     Grain = Unit.Grain
     Ounce = Unit.Ounce
     Gram = Unit.Gram
     Pound = Unit.Pound
-    Kilogram = Unit.Kilgram
+    Kilogram = Unit.Kilogram
     Newton = Unit.Newton
 
 
 class Temperature(AbstractUnit):
     """Temperature unit"""
 
     def to_raw(self, value: float, units: Unit):
@@ -504,16 +516,16 @@
             result = atan(value / 3600)
         elif units == Angular.CmPer100M:
             result = atan(value / 10000)
         elif units == Angular.OClock:
             result = value / 6 * pi
         else:
             return super().to_raw(value, units)
-        if result > 2*pi:
-            result = result % (2*pi)
+        if result > 2 * pi:
+            result = result % (2 * pi)
         return result
 
     def from_raw(self, value: float, units: Unit):
         if units == Angular.Radian:
             return value
         if units == Angular.Degree:
             result = value * 180 / pi
@@ -599,44 +611,172 @@
             return value / 0.737562149277
         return super().from_raw(value, units)
 
     FootPound = Unit.FootPound
     Joule = Unit.Joule
 
 
+class PreferredUnitsMeta(type):
+    """Provide representation method for static dataclasses."""
+
+    def __repr__(cls):
+        return '\n'.join(f'{field} = {getattr(cls, field)!r}'
+                         for field in getattr(cls, '__dataclass_fields__'))
+
+
 @dataclass
-class TypedUnits:  # pylint: disable=too-few-public-methods
-    """
-    Abstract class to apply auto-conversion values to
-    specified units by type-hints in inherited dataclasses
-    """
+class PreferredUnits(metaclass=PreferredUnitsMeta):  # pylint: disable=too-many-instance-attributes
+    """Default prefer_units for specified measures"""
+
+    angular: Unit = Unit.Degree
+    distance: Unit = Unit.Yard
+    velocity: Unit = Unit.FPS
+    pressure: Unit = Unit.InHg
+    temperature: Unit = Unit.Fahrenheit
+    diameter: Unit = Unit.Inch
+    length: Unit = Unit.Inch
+    weight: Unit = Unit.Grain
+    adjustment: Unit = Unit.Mil
+    drop: Unit = Unit.Inch
+    energy: Unit = Unit.FootPound
+    ogw: Unit = Unit.Pound
+    sight_height: Unit = Unit.Inch
+    target_height: Unit = Unit.Inch
+    twist: Unit = Unit.Inch
+
+    @dataclass
+    class Mixin(ABC):  # pylint: disable=too-few-public-methods
+        """
+        TODO: move it to Units, use it instead of TypedUnits
+        Abstract class to apply auto-conversion values to
+        specified prefer_units by type-hints in inherited dataclasses
+        """
+
+        def __setattr__(self, key, value):
+            """
+            converts value to specified prefer_units by type-hints in inherited dataclass
+            """
+
+            _fields = self.__getattribute__('__dataclass_fields__')
+
+            if (_field := _fields.get(key)) and value is not None and not isinstance(value, AbstractUnit):
+
+                if units := _field.metadata.get('prefer_units'):
+
+                    if isinstance(units, Unit):
+                        value = units(value)
+                    elif isinstance(units, str):
+                        value = PreferredUnits.__dict__[units](value)
+                    else:
+                        raise TypeError(f"Unsupported unit or dimension use one of {PreferredUnits}")
+
+            super().__setattr__(key, value)
+
+    @classmethod
+    def set(cls, **kwargs):
+        """set preferred units from Mapping"""
+        for attribute, value in kwargs.items():
+            try:
+                if hasattr(PreferredUnits, attribute):
+                    setattr(PreferredUnits, attribute, Unit[value])
+                else:
+                    logger.warning(f"{attribute=} not found in preferred_units")
+            except KeyError:
+                logger.warning(f"{value=} not found in preferred_units")
+
+    @classmethod
+    def _load_config(cls, filepath=None):
+
+        def find_pybc_toml(start_dir=os.path.dirname(__file__)):
+            """
+            Search for the pyproject.toml file starting from the specified directory.
+            :param start_dir: (str) The directory to start searching from. Default is the current working directory.
+            :return: str: The absolute path to the pyproject.toml file if found, otherwise None.
+            """
+            current_dir = os.path.abspath(start_dir)
+            while True:
+                # Check if pybc.toml or .pybc.toml exists in the current directory
+                pybc_paths = [
+                    os.path.join(current_dir, '.pybc.toml'),
+                    os.path.join(current_dir, 'pybc.toml'),
+                ]
+                for pypc_path in pybc_paths:
+                    if os.path.exists(pypc_path):
+                        return os.path.abspath(pypc_path)
+
+                # Move to the parent directory
+                parent_dir = os.path.dirname(current_dir)
+
+                # If we have reached the root directory, stop searching
+                if parent_dir == current_dir:
+                    return None
+
+                current_dir = parent_dir
+
+        if filepath is None:
+            filepath = find_pybc_toml()
+
+        with open(filepath, "rb") as fp:
+            _config = tomllib.load(fp)
+
+            if _pybc := _config.get('pybc'):
+                if preferred_units := _pybc.get('preferred_units'):
+                    cls.set(**preferred_units)
+                else:
+                    logger.warning("Config has not `pybc.preferred_units` section")
+            else:
+                logger.warning("Config has not `pybc` section")
 
-    def __setattr__(self, key, value):
+    @classmethod
+    def basic_config(cls, filename=None, **preferred_units):
         """
-        converts value to specified units by type-hints in inherited dataclass
+        Method to load preferred units from file or Mapping
         """
+        if filename and preferred_units:
+            raise ValueError("Can't use preferred_units and config file at same time")
+        if preferred_units:
+            cls.set(**preferred_units)
+        else:
+            # trying to load definitions from pybc.toml
+            cls._load_config(filename)
 
-        _fields = self.__getattribute__('__dataclass_fields__')
-        # fields(self.__class__)[0].name
-        if key in _fields and not isinstance(value, AbstractUnit):
-            default_factory = _fields[key].default_factory
-            if isinstance(default_factory, typing.Callable):
-                if isinstance(value, Unit):
-                    value = None
-                else:
-                    value = default_factory()(value)
 
-        super().__setattr__(key, value)
+# pylint: disable=redefined-builtin,too-few-public-methods,too-many-arguments
+class Dimension(Field):
+    """
+    Definition of measure units specified field for
+    PreferredUnits.Mixin based dataclasses
+    """
+
+    def __init__(self, prefer_units: Union[str, Unit], init=True, repr_=True,
+                 hash_=None, compare=True, metadata=None):
+        if metadata is None:
+            metadata = {}
+        metadata['prefer_units'] = prefer_units
+
+        major, minor = sys.version_info.major, sys.version_info.minor
+
+        if major >= 3 and minor > 9:
+            extra = {'kw_only': MISSING}
+        elif major >= 3 and minor == 9:
+            extra = {}
+        else:
+            raise RuntimeError("Unsupported python version")
+
+        super().__init__(default=None, default_factory=MISSING,
+                         init=init, repr=repr_,
+                         hash=hash_, compare=compare,
+                         metadata=metadata, **extra)
+
+    @abstractmethod
+    def __rshift__(self, other):
+        ...
+
+    @abstractmethod
+    def __lshift__(self, other):
+        ...
+
 
+PreferredUnits.basic_config()  # init PreferredUnits
 
-# def is_unit(obj: [AbstractUnit, float, int]):
-#     """
-#     Check if obj is inherited by AbstractUnit
-#     :return: False - if float or int
-#     """
-#     if isinstance(obj, AbstractUnit):
-#         return True
-#     if isinstance(obj, (float, int)):
-#         return False
-#     if obj is None:
-#         return None
-#     raise TypeError(f"Expected Unit, int, or float, found {obj.__class__.__name__}")
+# export method globally
+basicConfig = PreferredUnits.basic_config
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/PKG-INFO` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -184,16 +184,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tomli; python_version < "3.11"
 Provides-Extra: exts
-Requires-Dist: py_ballisticcalc.exts==2.0.0b2; extra == "exts"
+Requires-Dist: py_ballisticcalc.exts==2.0.0b3; extra == "exts"
 Provides-Extra: lint
 Requires-Dist: pylint; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Provides-Extra: charts
 Requires-Dist: matplotlib; extra == "charts"
 Requires-Dist: pandas; extra == "charts"
 
@@ -251,20 +252,20 @@
 from py_ballisticcalc import Weapon, Shot, Calculator
 from py_ballisticcalc import Settings as Set
 from py_ballisticcalc.unit import *
 ```
 
 ## Simple Zero
 ```python
-# Establish 100-yard zero for a standard .308, G7 BC=0.22, muzzle velocity 2600fps
+# Establish 100-yard zero for a standard .308, G7 bc=0.22, muzzle velocity 2600fps
 zero = Shot(weapon=Weapon(sight_height=2), ammo=Ammo(DragModel(0.22, TableG7), mv=Velocity.FPS(2600)))
 calc = Calculator()
 zero_distance = Distance.Yard(100)
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 ```
 
     Barrel elevation for 100.0yd zero: 1.33mil
 
 ## Plot Trajectory with Danger Space
 ```python
 # Plot trajectory out to 500 yards
@@ -314,36 +315,36 @@
 ammo.calc_powder_sens(Velocity.MPS(820), Temperature.Celsius(0))
 weapon = Weapon(sight_height=Distance.Centimeter(9), twist=15)
 atmo = Atmo(altitude=Distance.Foot(1000), temperature=Unit.CELSIUS(5), humidity=.5)
 zero = Shot(weapon=weapon, ammo=ammo, atmo=atmo)
 zero_distance = Distance.Meter(500)
 calc = Calculator()
 zero_elevation = calc.set_weapon_zero(zero, zero_distance)
-print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << Set.Units.adjustment}')
+print(f'Barrel elevation for {zero_distance} zero: {zero_elevation << PreferredUnits.adjustment}')
 print(f'Muzzle velocity at zero temperature {atmo.temperature} is {ammo.get_velocity_for_temp(atmo.temperature) << Velocity.MPS}')
 ```
 
     Barrel elevation for 500.0m zero: 4.69mil
     Muzzle velocity at zero temperature 5.0°C is 830.0m/s
 
 ## Units
 
 ```python
 from py_ballisticcalc.unit import *
 
 # Print default units
-from py_ballisticcalc import Settings
+from py_ballisticcalc import Settings, PreferredUnits
 print(str(Settings.Units))
 
 # Change default
-Set.Units.distance = Unit.FOOT
-print(f'Default distance unit: {Set.Units.distance.name}')
+PreferredUnits.distance = Unit.FOOT
+print(f'Default distance unit: {PreferredUnits.distance.name}')
 # Can create value in default unit with either float or another unit of same type
-print(f'\tInstantiated from float (5): {Set.Units.distance(5)}')
-print(f'\tInstantiated from Distance.Line(200): {Set.Units.distance(Distance.Line(200))}')
+print(f'\tInstantiated from float (5): {PreferredUnits.distance(5)}')
+print(f'\tInstantiated from Distance.Line(200): {PreferredUnits.distance(Distance.Line(200))}')
 
 # Ways to define value in units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
```

### Comparing `py_ballisticcalc-2.0.0b2/py_ballisticcalc.egg-info/SOURCES.txt` & `py_ballisticcalc-2.0.0b3/py_ballisticcalc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 py_ballisticcalc/backend.py
 py_ballisticcalc/conditions.py
 py_ballisticcalc/drag_model.py
 py_ballisticcalc/drag_tables.py
 py_ballisticcalc/example.py
 py_ballisticcalc/interface.py
 py_ballisticcalc/logger.py
-py_ballisticcalc/multiple_bc.py
 py_ballisticcalc/munition.py
 py_ballisticcalc/settings.py
 py_ballisticcalc/trajectory_calc.py
 py_ballisticcalc/trajectory_data.py
 py_ballisticcalc/unit.py
 py_ballisticcalc.egg-info/PKG-INFO
 py_ballisticcalc.egg-info/SOURCES.txt
 py_ballisticcalc.egg-info/dependency_links.txt
 py_ballisticcalc.egg-info/requires.txt
 py_ballisticcalc.egg-info/top_level.txt
 tests/test_.py
 tests/test_atmosphere.py
 tests/test_computer.py
+tests/test_config_loader.py
 tests/test_danger_space.py
 tests/test_mbc.py
 tests/test_trajectory.py
 tests/test_units.py
```

### Comparing `py_ballisticcalc-2.0.0b2/pyproject.toml` & `py_ballisticcalc-2.0.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc"
-version = "2.0.0b2"
+version = "2.0.0b3"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dependencies = []
+dependencies = ["tomli; python_version<'3.11'"]
 #dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/o-murphy/py_ballisticcalc"
 "Bug Reports" = "https://github.com/o-murphy/py_ballisticcalc/issues"
 #"Funding" = "https://donate.pypi.org"
 #"Say Thanks!" = ""
@@ -49,15 +49,11 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["py_ballisticcalc*"]  # alternatively: `exclude = ["additional*"]`
 exclude = ["py_ballisticcalc_exts*"]
 
 
-#[tool.setuptools.dynamic]
-#version = {attr = "py_ballisticcalc.__version__"}
-
-
 [project.optional-dependencies]
-exts = ['py_ballisticcalc.exts==2.0.0b2']
+exts = ['py_ballisticcalc.exts==2.0.0b3']
 lint = ['pylint', 'flake8']
 charts = ['matplotlib', 'pandas']
```

### Comparing `py_ballisticcalc-2.0.0b2/tests/test_atmosphere.py` & `py_ballisticcalc-2.0.0b3/tests/test_atmosphere.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
 from py_ballisticcalc import Atmo
-from py_ballisticcalc import Settings as Set
 from py_ballisticcalc.unit import *
 
 class TestAtmosphere(unittest.TestCase):
     """Unittests of the Atmosphere class"""
 
     def setUp(self):
         self.standard = Atmo.standard()
```

### Comparing `py_ballisticcalc-2.0.0b2/tests/test_computer.py` & `py_ballisticcalc-2.0.0b3/tests/test_computer.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         shot = Shot(weapon=self.weapon, ammo=self.ammo, atmo=thin)
         t = self.calc.fire(shot=shot, trajectory_range=self.range, trajectory_step=self.step)
         self.assertGreater(t.trajectory[5].height, self.baseline_trajectory[5].height)
 #endregion Atmo
 
 #region Ammo
     def test_ammo_drag(self):
-        """Increasing ballistic coefficient (BC) should decrease drop"""
+        """Increasing ballistic coefficient (bc) should decrease drop"""
         tdm = DragModel(self.dm.BC+0.5, self.dm.drag_table, self.dm.weight, self.dm.diameter, self.dm.length)
         slick = Ammo(tdm, self.ammo.mv)
         shot = Shot(weapon=self.weapon, ammo=slick, atmo=self.atmosphere)
         t = self.calc.fire(shot=shot, trajectory_range=self.range, trajectory_step=self.step)
         self.assertGreater(t.trajectory[5].height, self.baseline_trajectory[5].height)
 
     def test_ammo_optional(self):
```

### Comparing `py_ballisticcalc-2.0.0b2/tests/test_danger_space.py` & `py_ballisticcalc-2.0.0b3/tests/test_danger_space.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b2/tests/test_trajectory.py` & `py_ballisticcalc-2.0.0b3/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc-2.0.0b2/tests/test_units.py` & `py_ballisticcalc-2.0.0b3/tests/test_units.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,46 @@
+import typing
 import unittest
+import warnings
+from dataclasses import field, dataclass
+
+from py_ballisticcalc import Settings
 from py_ballisticcalc.unit import *
 
 
 def back_n_forth(test, value, units):
     u = test.unit_class(value, units)
     v = u >> units
     test.assertAlmostEqual(v, value, 7, f'Read back failed for {units}')
 
 
+class TestPrefUnits(unittest.TestCase):
+
+    def test_pref(self):
+
+        @dataclass
+        class TestClass(PreferredUnits.Mixin):
+            as_metadata_str: [float, Distance] = Dimension(prefer_units='sight_height')
+            as_metadata_unit: [float, Distance] = Dimension(prefer_units=Unit.Meter)
+
+        tc1 = TestClass(1, 1)
+        self.assertEqual(tc1.as_metadata_str.units, Unit.Inch)
+        self.assertEqual(tc1.as_metadata_unit.units, Unit.Meter)
+
+        tc2 = TestClass(Unit.Meter(1), Unit.Meter(1))
+        self.assertEqual(tc2.as_metadata_str.units, Unit.Meter)
+        self.assertEqual(tc2.as_metadata_unit.units, Unit.Meter)
+
+        PreferredUnits.sight_height = Unit.Centimeter
+
+        tc3 = TestClass(1, 1)
+        self.assertEqual(tc3.as_metadata_str.units, Unit.Centimeter)
+        self.assertEqual(tc3.as_metadata_unit.units, Unit.Meter)
+
+
 class TestAngular(unittest.TestCase):
 
     def setUp(self) -> None:
         self.unit_class = Angular
         self.unit_list = [
             Angular.Degree,
             Angular.MOA,
```

