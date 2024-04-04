# Comparing `tmp/py_ballisticcalc.exts-2.0.0b2.tar.gz` & `tmp/py_ballisticcalc.exts-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ballisticcalc.exts-2.0.0b2.tar", last modified: Tue Apr  2 04:25:34 2024, max compression
+gzip compressed data, was "py_ballisticcalc.exts-2.0.0b3.tar", last modified: Thu Apr  4 18:32:43 2024, max compression
```

## Comparing `py_ballisticcalc.exts-2.0.0b2.tar` & `py_ballisticcalc.exts-2.0.0b3.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 04:25:34.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   575422 2024-04-02 04:25:33.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.c
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/drag_model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   894073 2024-04-02 04:25:33.000000 py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/trajectory_calc.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:25:34.021506 py_ballisticcalc.exts-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 04:25:16.000000 py_ballisticcalc.exts-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 18:32:43.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   885017 2024-04-04 18:32:42.000000 py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/trajectory_calc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:43.125635 py_ballisticcalc.exts-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-04 18:32:26.000000 py_ballisticcalc.exts-2.0.0b3/setup.py
```

### Comparing `py_ballisticcalc.exts-2.0.0b2/LICENSE` & `py_ballisticcalc.exts-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ballisticcalc.exts-2.0.0b2/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -264,15 +264,15 @@
 
 The library supports all the popular units of measurement, and adds different built-in methods to define and manipulate it
 #### Unit manipulation syntax:
 
 ```python
 from py_ballisticcalc.unit import *
 
-# ways to define value in units
+# ways to define value in prefer_units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
 unit_in_meter = Unit.Meter(100)
 
@@ -281,48 +281,48 @@
 # convert unit
 # 1. by method
 unit_in_yard = unit_in_meter.convert(Distance.Yard)
 # 2. using shift syntax
 unit_in_yards = unit_in_meter << Distance.Yard  # '<<=' operator also supports
 # >>> <Distance>: 109.36132983377078 yd (3937.0078740157483)
 
-# get value in specified units
+# get value in specified prefer_units
 # 1. by method
 value_in_km = unit_in_yards.get_in(Distance.Kilometer)
 # 2. by shift syntax
 value_in_km = unit_in_yards >> Distance.Kilometer  # '>>=' operator also supports
 # >>> 0.1
 
 # getting unit raw value:
 rvalue = Distance.Meter(10).raw_value
 rvalue = float(Distance.Meter(10))
 
-# units comparison:
+# prefer_units comparison:
 # supports operators like < > <= >= == !=
-Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two units by raw value
+Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two prefer_units by raw value
 Distance.Meter(100) > 10  # >>> True, compare unit with float by raw value
 ```
 
 #### An example of calculations
 
 ```python
 from py_ballisticcalc import *
-from py_ballisticcalc import Settings as Set
+from py_ballisticcalc import Settings, PreferredUnits
 
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
 
-Set.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
+Settings.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
 
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

### Comparing `py_ballisticcalc.exts-2.0.0b2/README.md` & `py_ballisticcalc.exts-2.0.0b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 The library supports all the popular units of measurement, and adds different built-in methods to define and manipulate it
 #### Unit manipulation syntax:
 
 ```python
 from py_ballisticcalc.unit import *
 
-# ways to define value in units
+# ways to define value in prefer_units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
 unit_in_meter = Unit.Meter(100)
 
@@ -90,48 +90,48 @@
 # convert unit
 # 1. by method
 unit_in_yard = unit_in_meter.convert(Distance.Yard)
 # 2. using shift syntax
 unit_in_yards = unit_in_meter << Distance.Yard  # '<<=' operator also supports
 # >>> <Distance>: 109.36132983377078 yd (3937.0078740157483)
 
-# get value in specified units
+# get value in specified prefer_units
 # 1. by method
 value_in_km = unit_in_yards.get_in(Distance.Kilometer)
 # 2. by shift syntax
 value_in_km = unit_in_yards >> Distance.Kilometer  # '>>=' operator also supports
 # >>> 0.1
 
 # getting unit raw value:
 rvalue = Distance.Meter(10).raw_value
 rvalue = float(Distance.Meter(10))
 
-# units comparison:
+# prefer_units comparison:
 # supports operators like < > <= >= == !=
-Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two units by raw value
+Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two prefer_units by raw value
 Distance.Meter(100) > 10  # >>> True, compare unit with float by raw value
 ```
 
 #### An example of calculations
 
 ```python
 from py_ballisticcalc import *
-from py_ballisticcalc import Settings as Set
+from py_ballisticcalc import Settings, PreferredUnits
 
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
 
-Set.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
+Settings.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
 
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

### Comparing `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc.exts.egg-info/PKG-INFO` & `py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc.exts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ballisticcalc.exts
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: LGPL library for small arms ballistic calculations (Python 3)
 Author-email: o-murphy <thehelixpg@gmail.com>, dbookstaber <bookstaber@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -264,15 +264,15 @@
 
 The library supports all the popular units of measurement, and adds different built-in methods to define and manipulate it
 #### Unit manipulation syntax:
 
 ```python
 from py_ballisticcalc.unit import *
 
-# ways to define value in units
+# ways to define value in prefer_units
 # 1. old syntax
 unit_in_meter = Distance(100, Distance.Meter)
 # 2. short syntax by Unit type class
 unit_in_meter = Distance.Meter(100)
 # 3. by Unit enum class
 unit_in_meter = Unit.Meter(100)
 
@@ -281,48 +281,48 @@
 # convert unit
 # 1. by method
 unit_in_yard = unit_in_meter.convert(Distance.Yard)
 # 2. using shift syntax
 unit_in_yards = unit_in_meter << Distance.Yard  # '<<=' operator also supports
 # >>> <Distance>: 109.36132983377078 yd (3937.0078740157483)
 
-# get value in specified units
+# get value in specified prefer_units
 # 1. by method
 value_in_km = unit_in_yards.get_in(Distance.Kilometer)
 # 2. by shift syntax
 value_in_km = unit_in_yards >> Distance.Kilometer  # '>>=' operator also supports
 # >>> 0.1
 
 # getting unit raw value:
 rvalue = Distance.Meter(10).raw_value
 rvalue = float(Distance.Meter(10))
 
-# units comparison:
+# prefer_units comparison:
 # supports operators like < > <= >= == !=
-Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two units by raw value
+Distance.Meter(100) == Distance.Centimeter(100)  # >>> False, compare two prefer_units by raw value
 Distance.Meter(100) > 10  # >>> True, compare unit with float by raw value
 ```
 
 #### An example of calculations
 
 ```python
 from py_ballisticcalc import *
-from py_ballisticcalc import Settings as Set
+from py_ballisticcalc import Settings, PreferredUnits
 
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
 
-Set.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
+Settings.USE_POWDER_SENSITIVITY = True  # Correct muzzle velocity for powder temperature
 
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

### Comparing `py_ballisticcalc.exts-2.0.0b2/py_ballisticcalc_exts/trajectory_calc.c` & `py_ballisticcalc.exts-2.0.0b3/py_ballisticcalc_exts/trajectory_calc.c`

 * *Files 2% similar despite different names*

```diff
@@ -1626,14 +1626,15 @@
  * cdef class TrajectoryCalc:             # <<<<<<<<<<<<<<
  *     cdef:
  *         object ammo
  */
 
 struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc {
   double (*get_calc_step)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args);
+  PyObject *(*_init_trajectory)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *);
   PyObject *(*_zero_angle)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, PyObject *);
   PyObject *(*_trajectory)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag);
   double (*drag_by_mach)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double);
   double (*spin_drift)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double);
   double (*calc_stability_coefficient)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *);
 };
 static struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
@@ -2466,14 +2467,15 @@
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_const(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, double __pyx_v_a); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_mul_by_vector(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_add(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_subtract(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_b); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_negate(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto*/
 static struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_6Vector_normalize(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args); /* proto*/
+static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__init_trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info); /* proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__zero_angle(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_distance); /* proto*/
 static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, double __pyx_v_maximum_range, double __pyx_v_step, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag __pyx_v_filter_flags); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_drag_by_mach(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, double __pyx_v_mach); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_spin_drift(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, double __pyx_v_time); /* proto*/
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_calc_stability_coefficient(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_atmo); /* proto*/
 
 /* Module declarations from "libc.math" */
@@ -2518,15 +2520,15 @@
 static const char __pyx_k_CD[] = "CD";
 static const char __pyx_k__6[] = ".";
 static const char __pyx_k__7[] = "*";
 static const char __pyx_k_dm[] = "dm";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_mv[] = "mv";
 static const char __pyx_k_FPS[] = "FPS";
-static const char __pyx_k__25[] = "?";
+static const char __pyx_k__23[] = "?";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_mul[] = "__mul__";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_ogw[] = "ogw";
 static const char __pyx_k_Ammo[] = "Ammo";
 static const char __pyx_k_Atmo[] = "Atmo";
 static const char __pyx_k_Foot[] = "Foot";
@@ -2546,15 +2548,14 @@
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_Grain[] = "Grain";
 static const char __pyx_k_Pound[] = "Pound";
-static const char __pyx_k_Units[] = "Units";
 static const char __pyx_k_angle[] = "angle";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_twist[] = "twist";
 static const char __pyx_k_winds[] = "winds";
 static const char __pyx_k_Energy[] = "Energy";
 static const char __pyx_k_Radian[] = "Radian";
@@ -2618,21 +2619,21 @@
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_sight_height[] = "sight_height";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_look_distance[] = "look_distance";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_PreferredUnits[] = "PreferredUnits";
 static const char __pyx_k_TrajectoryCalc[] = "TrajectoryCalc";
 static const char __pyx_k_TrajectoryData[] = "TrajectoryData";
 static const char __pyx_k_barrel_azimuth[] = "barrel_azimuth";
 static const char __pyx_k_density_factor[] = "density_factor";
 static const char __pyx_k_direction_from[] = "direction_from";
 static const char __pyx_k_until_distance[] = "until_distance";
-static const char __pyx_k_init_trajectory[] = "_init_trajectory";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_barrel_elevation[] = "barrel_elevation";
 static const char __pyx_k_MAX_DISTANCE_FEET[] = "MAX_DISTANCE_FEET";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Zero_vertical_error[] = "Zero vertical error ";
@@ -2645,15 +2646,14 @@
 static const char __pyx_k_TrajectoryCalc_trajectory[] = "TrajectoryCalc.trajectory";
 static const char __pyx_k_TrajectoryCalc_zero_angle[] = "TrajectoryCalc.zero_angle";
 static const char __pyx_k_py_ballisticcalc_munition[] = "py_ballisticcalc.munition";
 static const char __pyx_k_py_ballisticcalc_settings[] = "py_ballisticcalc.settings";
 static const char __pyx_k_py_ballisticcalc_conditions[] = "py_ballisticcalc.conditions";
 static const char __pyx_k_pyx_unpickle_TrajectoryCalc[] = "__pyx_unpickle_TrajectoryCalc";
 static const char __pyx_k_TrajectoryCalc___reduce_cython[] = "TrajectoryCalc.__reduce_cython__";
-static const char __pyx_k_TrajectoryCalc__init_trajectory[] = "TrajectoryCalc._init_trajectory";
 static const char __pyx_k_get_density_factor_and_mach_for[] = "get_density_factor_and_mach_for_altitude";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1a1505e, 0xaee47ca, 0x4420ce0) = (_bc, _curve, _table_data, alt0, ammo, barrel_azimuth, barrel_elevation, calc_step, cant_cosine, cant_sine, diameter, gravity_vector, length, look_angle, muzzle_velocity, sight_height, stability_coefficient, twist, weight))";
 static const char __pyx_k_No_value_specified_for_struct_at[] = "No value specified for struct attribute 'a'";
 static const char __pyx_k_TrajectoryCalc___setstate_cython[] = "TrajectoryCalc.__setstate_cython__";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_py_ballisticcalc_exts_trajectory[] = "py_ballisticcalc_exts.trajectory_calc";
 static const char __pyx_k_py_ballisticcalc_trajectory_data[] = "py_ballisticcalc.trajectory_data";
@@ -2673,17 +2673,16 @@
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_18__imul__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_20__neg__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_22__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_6Vector_24__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc___init__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_ammo); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_2zero_angle(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_distance); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info, PyObject *__pyx_v_max_range, PyObject *__pyx_v_dist_step, PyObject *__pyx_v_extra_data); /* proto */
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info); /* proto */
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc___pyx_unpickle_TrajectoryCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_21py_ballisticcalc_exts_15trajectory_calc_Vector(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2720,58 +2719,57 @@
   #endif
   PyTypeObject *__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector;
   PyTypeObject *__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
   PyObject *__pyx_n_s_Ammo;
   PyObject *__pyx_n_s_Angular;
   PyObject *__pyx_n_s_Atmo;
   PyObject *__pyx_n_s_BC;
-  PyObject *__pyx_n_u_CD;
+  PyObject *__pyx_n_s_CD;
   PyObject *__pyx_n_s_Distance;
   PyObject *__pyx_n_s_Energy;
   PyObject *__pyx_n_s_FPS;
   PyObject *__pyx_n_s_Fahrenheit;
   PyObject *__pyx_n_s_Foot;
   PyObject *__pyx_n_s_FootPound;
   PyObject *__pyx_n_s_Grain;
   PyObject *__pyx_n_s_InHg;
   PyObject *__pyx_n_s_Inch;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_n_s_KeyError;
   PyObject *__pyx_n_s_MAX_DISTANCE_FEET;
-  PyObject *__pyx_n_u_Mach;
+  PyObject *__pyx_n_s_Mach;
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at;
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at_2;
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at_3;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_Pound;
+  PyObject *__pyx_n_s_PreferredUnits;
   PyObject *__pyx_n_s_Pressure;
   PyObject *__pyx_n_s_Radian;
   PyObject *__pyx_n_s_Settings;
   PyObject *__pyx_n_s_Shot;
   PyObject *__pyx_n_s_Temperature;
   PyObject *__pyx_n_s_TrajectoryCalc;
   PyObject *__pyx_n_u_TrajectoryCalc;
   PyObject *__pyx_n_s_TrajectoryCalc___reduce_cython;
   PyObject *__pyx_n_s_TrajectoryCalc___setstate_cython;
-  PyObject *__pyx_n_s_TrajectoryCalc__init_trajectory;
   PyObject *__pyx_n_s_TrajectoryCalc_trajectory;
   PyObject *__pyx_n_s_TrajectoryCalc_zero_angle;
   PyObject *__pyx_n_s_TrajectoryData;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_USE_POWDER_SENSITIVITY;
-  PyObject *__pyx_n_s_Units;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_Vector;
   PyObject *__pyx_n_s_Vector___reduce_cython;
   PyObject *__pyx_n_s_Vector___setstate_cython;
   PyObject *__pyx_n_s_Velocity;
   PyObject *__pyx_n_s_Weight;
   PyObject *__pyx_n_s_Wind;
   PyObject *__pyx_kp_u_Zero_vertical_error;
-  PyObject *__pyx_n_s__25;
+  PyObject *__pyx_n_s__23;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_n_s__7;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_s_all;
   PyObject *__pyx_n_s_altitude;
   PyObject *__pyx_n_s_ammo;
   PyObject *__pyx_n_s_angle;
@@ -2806,15 +2804,14 @@
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get_density_factor_and_mach_for;
   PyObject *__pyx_n_s_get_max_calc_step_size;
   PyObject *__pyx_n_s_get_velocity_for_temp;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_height;
   PyObject *__pyx_n_s_import;
-  PyObject *__pyx_n_s_init_trajectory;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_kp_u_iterations;
   PyObject *__pyx_n_s_length;
   PyObject *__pyx_n_s_look_angle;
   PyObject *__pyx_n_s_look_distance;
   PyObject *__pyx_n_s_mach;
@@ -2892,24 +2889,22 @@
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
-  PyObject *__pyx_tuple__20;
-  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__21;
   PyObject *__pyx_codeobj__10;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__19;
-  PyObject *__pyx_codeobj__21;
+  PyObject *__pyx_codeobj__20;
   PyObject *__pyx_codeobj__22;
-  PyObject *__pyx_codeobj__24;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2952,58 +2947,57 @@
   Py_CLEAR(clear_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_CLEAR(clear_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_s_Ammo);
   Py_CLEAR(clear_module_state->__pyx_n_s_Angular);
   Py_CLEAR(clear_module_state->__pyx_n_s_Atmo);
   Py_CLEAR(clear_module_state->__pyx_n_s_BC);
-  Py_CLEAR(clear_module_state->__pyx_n_u_CD);
+  Py_CLEAR(clear_module_state->__pyx_n_s_CD);
   Py_CLEAR(clear_module_state->__pyx_n_s_Distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_Energy);
   Py_CLEAR(clear_module_state->__pyx_n_s_FPS);
   Py_CLEAR(clear_module_state->__pyx_n_s_Fahrenheit);
   Py_CLEAR(clear_module_state->__pyx_n_s_Foot);
   Py_CLEAR(clear_module_state->__pyx_n_s_FootPound);
   Py_CLEAR(clear_module_state->__pyx_n_s_Grain);
   Py_CLEAR(clear_module_state->__pyx_n_s_InHg);
   Py_CLEAR(clear_module_state->__pyx_n_s_Inch);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
   Py_CLEAR(clear_module_state->__pyx_n_s_MAX_DISTANCE_FEET);
-  Py_CLEAR(clear_module_state->__pyx_n_u_Mach);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Mach);
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at);
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_3);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pound);
+  Py_CLEAR(clear_module_state->__pyx_n_s_PreferredUnits);
   Py_CLEAR(clear_module_state->__pyx_n_s_Pressure);
   Py_CLEAR(clear_module_state->__pyx_n_s_Radian);
   Py_CLEAR(clear_module_state->__pyx_n_s_Settings);
   Py_CLEAR(clear_module_state->__pyx_n_s_Shot);
   Py_CLEAR(clear_module_state->__pyx_n_s_Temperature);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_u_TrajectoryCalc);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc__init_trajectory);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc_trajectory);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryCalc_zero_angle);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrajectoryData);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_USE_POWDER_SENSITIVITY);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Units);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vector);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vector___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Vector___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Velocity);
   Py_CLEAR(clear_module_state->__pyx_n_s_Weight);
   Py_CLEAR(clear_module_state->__pyx_n_s_Wind);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Zero_vertical_error);
-  Py_CLEAR(clear_module_state->__pyx_n_s__25);
+  Py_CLEAR(clear_module_state->__pyx_n_s__23);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_n_s__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_all);
   Py_CLEAR(clear_module_state->__pyx_n_s_altitude);
   Py_CLEAR(clear_module_state->__pyx_n_s_ammo);
   Py_CLEAR(clear_module_state->__pyx_n_s_angle);
@@ -3038,15 +3032,14 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_density_factor_and_mach_for);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_max_calc_step_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_velocity_for_temp);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_height);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
-  Py_CLEAR(clear_module_state->__pyx_n_s_init_trajectory);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_kp_u_iterations);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_look_angle);
   Py_CLEAR(clear_module_state->__pyx_n_s_look_distance);
   Py_CLEAR(clear_module_state->__pyx_n_s_mach);
@@ -3124,24 +3117,22 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
-  Py_CLEAR(clear_module_state->__pyx_tuple__20);
-  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__10);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3162,58 +3153,57 @@
   Py_VISIT(traverse_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_Vector);
   Py_VISIT(traverse_module_state->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_s_Ammo);
   Py_VISIT(traverse_module_state->__pyx_n_s_Angular);
   Py_VISIT(traverse_module_state->__pyx_n_s_Atmo);
   Py_VISIT(traverse_module_state->__pyx_n_s_BC);
-  Py_VISIT(traverse_module_state->__pyx_n_u_CD);
+  Py_VISIT(traverse_module_state->__pyx_n_s_CD);
   Py_VISIT(traverse_module_state->__pyx_n_s_Distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_Energy);
   Py_VISIT(traverse_module_state->__pyx_n_s_FPS);
   Py_VISIT(traverse_module_state->__pyx_n_s_Fahrenheit);
   Py_VISIT(traverse_module_state->__pyx_n_s_Foot);
   Py_VISIT(traverse_module_state->__pyx_n_s_FootPound);
   Py_VISIT(traverse_module_state->__pyx_n_s_Grain);
   Py_VISIT(traverse_module_state->__pyx_n_s_InHg);
   Py_VISIT(traverse_module_state->__pyx_n_s_Inch);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
   Py_VISIT(traverse_module_state->__pyx_n_s_MAX_DISTANCE_FEET);
-  Py_VISIT(traverse_module_state->__pyx_n_u_Mach);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Mach);
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at);
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_2);
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_3);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pound);
+  Py_VISIT(traverse_module_state->__pyx_n_s_PreferredUnits);
   Py_VISIT(traverse_module_state->__pyx_n_s_Pressure);
   Py_VISIT(traverse_module_state->__pyx_n_s_Radian);
   Py_VISIT(traverse_module_state->__pyx_n_s_Settings);
   Py_VISIT(traverse_module_state->__pyx_n_s_Shot);
   Py_VISIT(traverse_module_state->__pyx_n_s_Temperature);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_u_TrajectoryCalc);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc__init_trajectory);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc_trajectory);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryCalc_zero_angle);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrajectoryData);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_USE_POWDER_SENSITIVITY);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Units);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vector);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vector___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Vector___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Velocity);
   Py_VISIT(traverse_module_state->__pyx_n_s_Weight);
   Py_VISIT(traverse_module_state->__pyx_n_s_Wind);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Zero_vertical_error);
-  Py_VISIT(traverse_module_state->__pyx_n_s__25);
+  Py_VISIT(traverse_module_state->__pyx_n_s__23);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_n_s__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_all);
   Py_VISIT(traverse_module_state->__pyx_n_s_altitude);
   Py_VISIT(traverse_module_state->__pyx_n_s_ammo);
   Py_VISIT(traverse_module_state->__pyx_n_s_angle);
@@ -3248,15 +3238,14 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_density_factor_and_mach_for);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_max_calc_step_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_velocity_for_temp);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_height);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
-  Py_VISIT(traverse_module_state->__pyx_n_s_init_trajectory);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_kp_u_iterations);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_look_angle);
   Py_VISIT(traverse_module_state->__pyx_n_s_look_distance);
   Py_VISIT(traverse_module_state->__pyx_n_s_mach);
@@ -3334,24 +3323,22 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
-  Py_VISIT(traverse_module_state->__pyx_tuple__20);
-  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__10);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3386,58 +3373,57 @@
 #endif
 #define __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector __pyx_mstate_global->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector
 #define __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc __pyx_mstate_global->__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc
 #define __pyx_n_s_Ammo __pyx_mstate_global->__pyx_n_s_Ammo
 #define __pyx_n_s_Angular __pyx_mstate_global->__pyx_n_s_Angular
 #define __pyx_n_s_Atmo __pyx_mstate_global->__pyx_n_s_Atmo
 #define __pyx_n_s_BC __pyx_mstate_global->__pyx_n_s_BC
-#define __pyx_n_u_CD __pyx_mstate_global->__pyx_n_u_CD
+#define __pyx_n_s_CD __pyx_mstate_global->__pyx_n_s_CD
 #define __pyx_n_s_Distance __pyx_mstate_global->__pyx_n_s_Distance
 #define __pyx_n_s_Energy __pyx_mstate_global->__pyx_n_s_Energy
 #define __pyx_n_s_FPS __pyx_mstate_global->__pyx_n_s_FPS
 #define __pyx_n_s_Fahrenheit __pyx_mstate_global->__pyx_n_s_Fahrenheit
 #define __pyx_n_s_Foot __pyx_mstate_global->__pyx_n_s_Foot
 #define __pyx_n_s_FootPound __pyx_mstate_global->__pyx_n_s_FootPound
 #define __pyx_n_s_Grain __pyx_mstate_global->__pyx_n_s_Grain
 #define __pyx_n_s_InHg __pyx_mstate_global->__pyx_n_s_InHg
 #define __pyx_n_s_Inch __pyx_mstate_global->__pyx_n_s_Inch
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
 #define __pyx_n_s_MAX_DISTANCE_FEET __pyx_mstate_global->__pyx_n_s_MAX_DISTANCE_FEET
-#define __pyx_n_u_Mach __pyx_mstate_global->__pyx_n_u_Mach
+#define __pyx_n_s_Mach __pyx_mstate_global->__pyx_n_s_Mach
 #define __pyx_kp_s_No_value_specified_for_struct_at __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at
 #define __pyx_kp_s_No_value_specified_for_struct_at_2 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_2
 #define __pyx_kp_s_No_value_specified_for_struct_at_3 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_3
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_Pound __pyx_mstate_global->__pyx_n_s_Pound
+#define __pyx_n_s_PreferredUnits __pyx_mstate_global->__pyx_n_s_PreferredUnits
 #define __pyx_n_s_Pressure __pyx_mstate_global->__pyx_n_s_Pressure
 #define __pyx_n_s_Radian __pyx_mstate_global->__pyx_n_s_Radian
 #define __pyx_n_s_Settings __pyx_mstate_global->__pyx_n_s_Settings
 #define __pyx_n_s_Shot __pyx_mstate_global->__pyx_n_s_Shot
 #define __pyx_n_s_Temperature __pyx_mstate_global->__pyx_n_s_Temperature
 #define __pyx_n_s_TrajectoryCalc __pyx_mstate_global->__pyx_n_s_TrajectoryCalc
 #define __pyx_n_u_TrajectoryCalc __pyx_mstate_global->__pyx_n_u_TrajectoryCalc
 #define __pyx_n_s_TrajectoryCalc___reduce_cython __pyx_mstate_global->__pyx_n_s_TrajectoryCalc___reduce_cython
 #define __pyx_n_s_TrajectoryCalc___setstate_cython __pyx_mstate_global->__pyx_n_s_TrajectoryCalc___setstate_cython
-#define __pyx_n_s_TrajectoryCalc__init_trajectory __pyx_mstate_global->__pyx_n_s_TrajectoryCalc__init_trajectory
 #define __pyx_n_s_TrajectoryCalc_trajectory __pyx_mstate_global->__pyx_n_s_TrajectoryCalc_trajectory
 #define __pyx_n_s_TrajectoryCalc_zero_angle __pyx_mstate_global->__pyx_n_s_TrajectoryCalc_zero_angle
 #define __pyx_n_s_TrajectoryData __pyx_mstate_global->__pyx_n_s_TrajectoryData
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_USE_POWDER_SENSITIVITY __pyx_mstate_global->__pyx_n_s_USE_POWDER_SENSITIVITY
-#define __pyx_n_s_Units __pyx_mstate_global->__pyx_n_s_Units
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_Vector __pyx_mstate_global->__pyx_n_s_Vector
 #define __pyx_n_s_Vector___reduce_cython __pyx_mstate_global->__pyx_n_s_Vector___reduce_cython
 #define __pyx_n_s_Vector___setstate_cython __pyx_mstate_global->__pyx_n_s_Vector___setstate_cython
 #define __pyx_n_s_Velocity __pyx_mstate_global->__pyx_n_s_Velocity
 #define __pyx_n_s_Weight __pyx_mstate_global->__pyx_n_s_Weight
 #define __pyx_n_s_Wind __pyx_mstate_global->__pyx_n_s_Wind
 #define __pyx_kp_u_Zero_vertical_error __pyx_mstate_global->__pyx_kp_u_Zero_vertical_error
-#define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
+#define __pyx_n_s__23 __pyx_mstate_global->__pyx_n_s__23
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_s_all __pyx_mstate_global->__pyx_n_s_all
 #define __pyx_n_s_altitude __pyx_mstate_global->__pyx_n_s_altitude
 #define __pyx_n_s_ammo __pyx_mstate_global->__pyx_n_s_ammo
 #define __pyx_n_s_angle __pyx_mstate_global->__pyx_n_s_angle
@@ -3472,15 +3458,14 @@
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get_density_factor_and_mach_for __pyx_mstate_global->__pyx_n_s_get_density_factor_and_mach_for
 #define __pyx_n_s_get_max_calc_step_size __pyx_mstate_global->__pyx_n_s_get_max_calc_step_size
 #define __pyx_n_s_get_velocity_for_temp __pyx_mstate_global->__pyx_n_s_get_velocity_for_temp
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_height __pyx_mstate_global->__pyx_n_s_height
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
-#define __pyx_n_s_init_trajectory __pyx_mstate_global->__pyx_n_s_init_trajectory
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_kp_u_iterations __pyx_mstate_global->__pyx_kp_u_iterations
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
 #define __pyx_n_s_look_angle __pyx_mstate_global->__pyx_n_s_look_angle
 #define __pyx_n_s_look_distance __pyx_mstate_global->__pyx_n_s_look_distance
 #define __pyx_n_s_mach __pyx_mstate_global->__pyx_n_s_mach
@@ -3558,24 +3543,22 @@
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
-#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
-#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
 #define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
-#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
 /* #### Code section: module_code ### */
 
 /* "FromPyStructUtility":12
  * 
  * @cname("__pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint")
  * cdef struct_type __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(obj) except *:             # <<<<<<<<<<<<<<
  *     cdef struct_type result
@@ -6258,15 +6241,15 @@
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shot_info,&__pyx_n_s_max_range,&__pyx_n_s_dist_step,&__pyx_n_s_extra_data,0};
 
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":137
  * 
  *     def trajectory(self, shot_info: Shot, max_range: Distance, dist_step: Distance,
  *                    extra_data: bool = False):             # <<<<<<<<<<<<<<
  *         cdef:
- *             object step = Settings.Units.distance(dist_step)
+ *             object step = PreferredUnits.distance(dist_step)
  */
     values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_False));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -6392,65 +6375,62 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trajectory", 0);
   __Pyx_INCREF(__pyx_v_dist_step);
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":139
  *                    extra_data: bool = False):
  *         cdef:
- *             object step = Settings.Units.distance(dist_step)             # <<<<<<<<<<<<<<
+ *             object step = PreferredUnits.distance(dist_step)             # <<<<<<<<<<<<<<
  *             object atmo = shot_info.atmo
  *             list winds = shot_info.winds
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Settings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_PreferredUnits); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Units); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = NULL;
+  __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_4 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_dist_step};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_dist_step};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_step = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":140
  *         cdef:
- *             object step = Settings.Units.distance(dist_step)
+ *             object step = PreferredUnits.distance(dist_step)
  *             object atmo = shot_info.atmo             # <<<<<<<<<<<<<<
  *             list winds = shot_info.winds
  *             CTrajFlag filter_flags = CTrajFlag.RANGE
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_atmo = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":141
- *             object step = Settings.Units.distance(dist_step)
+ *             object step = PreferredUnits.distance(dist_step)
  *             object atmo = shot_info.atmo
  *             list winds = shot_info.winds             # <<<<<<<<<<<<<<
  *             CTrajFlag filter_flags = CTrajFlag.RANGE
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -6480,40 +6460,40 @@
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":145
  * 
  *         if extra_data:
  *             dist_step = Distance.Foot(0.2)             # <<<<<<<<<<<<<<
  *             filter_flags = CTrajFlag.ALL
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
+    if (unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_float_0_2};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_float_0_2};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_dist_step, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":146
  *         if extra_data:
  *             dist_step = Distance.Foot(0.2)
@@ -6535,66 +6515,44 @@
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":148
  *             filter_flags = CTrajFlag.ALL
  * 
  *         self._init_trajectory(shot_info)             # <<<<<<<<<<<<<<
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_init_trajectory); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
-  __pyx_t_4 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_shot_info};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":149
  * 
  *         self._init_trajectory(shot_info)
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)             # <<<<<<<<<<<<<<
  * 
- *     def _init_trajectory(self, shot_info: Shot):
+ *     cdef _init_trajectory(self, shot_info: Shot):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_v_max_range, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_v_max_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_v_dist_step, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_v_dist_step, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_trajectory(__pyx_v_self, __pyx_v_shot_info, __pyx_t_6, __pyx_t_7, __pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6623,117 +6581,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "py_ballisticcalc_exts/trajectory_calc.pyx":151
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
- *     def _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
+ *     cdef _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory, "TrajectoryCalc._init_trajectory(self, shot_info: Shot)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory = {"_init_trajectory", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory};
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_shot_info = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[1] = {0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_init_trajectory (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shot_info,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shot_info)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_init_trajectory") < 0)) __PYX_ERR(0, 151, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v_shot_info = values[0];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_init_trajectory", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 151, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc._init_trajectory", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self), __pyx_v_shot_info);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info) {
+static PyObject *__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__init_trajectory(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v_shot_info) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   double __pyx_t_4;
   int __pyx_t_5;
@@ -6742,15 +6603,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_init_trajectory", 1);
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":152
  * 
- *     def _init_trajectory(self, shot_info: Shot):
+ *     cdef _init_trajectory(self, shot_info: Shot):
  *         self.look_angle = shot_info.look_angle >> Angular.Radian             # <<<<<<<<<<<<<<
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_look_angle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Angular); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
@@ -6763,15 +6624,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->look_angle = __pyx_t_4;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":153
- *     def _init_trajectory(self, shot_info: Shot):
+ *     cdef _init_trajectory(self, shot_info: Shot):
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch             # <<<<<<<<<<<<<<
  *         self.length = shot_info.ammo.dm.length >> Distance.Inch
  *         self.diameter = shot_info.ammo.dm.diameter >> Distance.Inch
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_weapon); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -7142,29 +7003,29 @@
   __pyx_t_4 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->calc_stability_coefficient(__pyx_v_self, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_self->stability_coefficient = __pyx_t_4;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":151
  *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
  * 
- *     def _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
+ *     cdef _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
  *         self.look_angle = shot_info.look_angle >> Angular.Radian
  *         self.twist = shot_info.weapon.twist >> Distance.Inch
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc._init_trajectory", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "py_ballisticcalc_exts/trajectory_calc.pyx":170
@@ -7187,18 +7048,18 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   double __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  Py_ssize_t __pyx_t_9;
-  Py_UCS4 __pyx_t_10;
+  PyObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
+  Py_UCS4 __pyx_t_9;
+  int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_zero_angle", 1);
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":172
  *     cdef _zero_angle(TrajectoryCalc self, object shot_info, object distance):
@@ -7306,38 +7167,16 @@
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":178
  *             double zero_finding_error = cZeroFindingAccuracy * 2
  * 
  *         self._init_trajectory(shot_info)             # <<<<<<<<<<<<<<
  *         self.barrel_azimuth = 0.0
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_init_trajectory); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_5 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_5 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_shot_info};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
+  __pyx_t_1 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->_init_trajectory(__pyx_v_self, __pyx_v_shot_info); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":179
  * 
  *         self._init_trajectory(shot_info)
  *         self.barrel_azimuth = 0.0             # <<<<<<<<<<<<<<
  *         self.barrel_elevation = atan(height_at_zero / zero_distance)
@@ -7380,24 +7219,24 @@
  * 
  *         # x = horizontal distance down range, y = drop, z = windage
  *         while zero_finding_error > cZeroFindingAccuracy and iterations_count < cMaxIterations:             # <<<<<<<<<<<<<<
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]
  *             height = t.height >> Distance.Foot
  */
   while (1) {
-    __pyx_t_7 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
-    if (__pyx_t_7) {
+    __pyx_t_6 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
+    if (__pyx_t_6) {
     } else {
-      __pyx_t_6 = __pyx_t_7;
+      __pyx_t_5 = __pyx_t_6;
       goto __pyx_L5_bool_binop_done;
     }
-    __pyx_t_7 = (__pyx_v_iterations_count < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations);
-    __pyx_t_6 = __pyx_t_7;
+    __pyx_t_6 = (__pyx_v_iterations_count < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaxIterations);
+    __pyx_t_5 = __pyx_t_6;
     __pyx_L5_bool_binop_done:;
-    if (!__pyx_t_6) break;
+    if (!__pyx_t_5) break;
 
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":186
  *         # x = horizontal distance down range, y = drop, z = windage
  *         while zero_finding_error > cZeroFindingAccuracy and iterations_count < cMaxIterations:
  *             t = self._trajectory(shot_info, maximum_range, zero_distance, CTrajFlag.NONE)[0]             # <<<<<<<<<<<<<<
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
@@ -7450,16 +7289,16 @@
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":189
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance
  *             else:  # last barrel_elevation hit zero!
  */
-    __pyx_t_6 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
-    if (__pyx_t_6) {
+    __pyx_t_5 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
+    if (__pyx_t_5) {
 
       /* "py_ballisticcalc_exts/trajectory_calc.pyx":190
  *             zero_finding_error = fabs(height - height_at_zero)
  *             if zero_finding_error > cZeroFindingAccuracy:
  *                 self.barrel_elevation -= (height - height_at_zero) / zero_distance             # <<<<<<<<<<<<<<
  *             else:  # last barrel_elevation hit zero!
  *                 break
@@ -7469,22 +7308,22 @@
       __pyx_t_1 = PyFloat_FromDouble(__pyx_v_height_at_zero); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_2 = PyNumber_Subtract(__pyx_v_height, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyFloat_FromDouble(__pyx_v_zero_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 190, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_7 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyNumber_InPlaceSubtract(__pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_InPlaceSubtract(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_self->barrel_elevation = __pyx_t_4;
 
       /* "py_ballisticcalc_exts/trajectory_calc.pyx":189
  *             height = t.height >> Distance.Foot
  *             zero_finding_error = fabs(height - height_at_zero)
@@ -7521,57 +7360,57 @@
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":194
  *                 break
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:             # <<<<<<<<<<<<<<
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')
  *         return Angular.Radian(self.barrel_elevation)
  */
-  __pyx_t_6 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
-  if (unlikely(__pyx_t_6)) {
+  __pyx_t_5 = (__pyx_v_zero_finding_error > __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cZeroFindingAccuracy);
+  if (unlikely(__pyx_t_5)) {
 
     /* "py_ballisticcalc_exts/trajectory_calc.pyx":195
  *             iterations_count += 1
  *         if zero_finding_error > cZeroFindingAccuracy:
  *             raise Exception(f'Zero vertical error {zero_finding_error} feet, after {iterations_count} iterations.')             # <<<<<<<<<<<<<<
  *         return Angular.Radian(self.barrel_elevation)
  * 
  */
     __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = 0;
-    __pyx_t_10 = 127;
+    __pyx_t_8 = 0;
+    __pyx_t_9 = 127;
     __Pyx_INCREF(__pyx_kp_u_Zero_vertical_error);
-    __pyx_t_9 += 20;
+    __pyx_t_8 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_Zero_vertical_error);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Zero_vertical_error);
-    __pyx_t_8 = PyFloat_FromDouble(__pyx_v_zero_finding_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 195, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_7 = PyFloat_FromDouble(__pyx_v_zero_finding_error); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_10;
-    __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_9;
+    __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_feet_after);
-    __pyx_t_9 += 13;
+    __pyx_t_8 += 13;
     __Pyx_GIVEREF(__pyx_kp_u_feet_after);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_feet_after);
     __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_iterations_count, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_iterations);
-    __pyx_t_9 += 12;
+    __pyx_t_8 += 12;
     __Pyx_GIVEREF(__pyx_kp_u_iterations);
     PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_iterations);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7592,41 +7431,41 @@
  *         return Angular.Radian(self.barrel_elevation)             # <<<<<<<<<<<<<<
  * 
  *     cdef _trajectory(TrajectoryCalc self, object shot_info,
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Angular); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Radian); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyFloat_FromDouble(__pyx_v_self->barrel_elevation); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
-  __pyx_t_5 = 0;
+  __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
-  if (unlikely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_8);
+  if (unlikely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_7, function);
+      __pyx_t_10 = 1;
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":170
  *         self.stability_coefficient = self.calc_stability_coefficient(shot_info.atmo)
@@ -7637,15 +7476,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc._zero_angle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_XDECREF(__pyx_v_height);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -7665,19 +7504,19 @@
   PyObject *__pyx_v_seen_zero = 0;
   double __pyx_v_density_factor;
   double __pyx_v_mach;
   double __pyx_v_velocity;
   double __pyx_v_delta_time;
   PyObject *__pyx_v_ranges = 0;
   int __pyx_v_ranges_length;
+  int __pyx_v_current_item;
   double __pyx_v_time;
   double __pyx_v_previous_mach;
   double __pyx_v_drag;
   int __pyx_v_len_winds;
-  int __pyx_v_current_item;
   int __pyx_v_current_wind;
   double __pyx_v_next_range_distance;
   double __pyx_v_next_wind_range;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_velocity_vector = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_velocity_adjusted = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_range_vector = 0;
   struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *__pyx_v_delta_range_vector = 0;
@@ -7703,27 +7542,27 @@
   __Pyx_RefNannySetupContext("_trajectory", 1);
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":203
  *             object _flag, seen_zero  # CTrajFlag
  *             double density_factor, mach, velocity, delta_time
  *             list ranges = []             # <<<<<<<<<<<<<<
  *             int ranges_length = int(maximum_range / step) + 1
- *             double time = .0
+ *             int current_item = 0
  */
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":204
  *             double density_factor, mach, velocity, delta_time
  *             list ranges = []
  *             int ranges_length = int(maximum_range / step) + 1             # <<<<<<<<<<<<<<
+ *             int current_item = 0
  *             double time = .0
- *             double previous_mach = .0
  */
   if (unlikely(__pyx_v_step == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
     __PYX_ERR(0, 204, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_PyInt_FromDouble((__pyx_v_maximum_range / __pyx_v_step)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -7733,312 +7572,330 @@
   __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_ranges_length = __pyx_t_3;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":205
  *             list ranges = []
  *             int ranges_length = int(maximum_range / step) + 1
+ *             int current_item = 0             # <<<<<<<<<<<<<<
+ *             double time = .0
+ *             double previous_mach = .0
+ */
+  __pyx_v_current_item = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":206
+ *             int ranges_length = int(maximum_range / step) + 1
+ *             int current_item = 0
  *             double time = .0             # <<<<<<<<<<<<<<
  *             double previous_mach = .0
  *             double drag = .0
  */
   __pyx_v_time = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":206
- *             int ranges_length = int(maximum_range / step) + 1
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":207
+ *             int current_item = 0
  *             double time = .0
  *             double previous_mach = .0             # <<<<<<<<<<<<<<
  *             double drag = .0
  * 
  */
   __pyx_v_previous_mach = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":207
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":208
  *             double time = .0
  *             double previous_mach = .0
  *             double drag = .0             # <<<<<<<<<<<<<<
  * 
  *             int len_winds = len(shot_info.winds)
  */
   __pyx_v_drag = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":209
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":210
  *             double drag = .0
  * 
  *             int len_winds = len(shot_info.winds)             # <<<<<<<<<<<<<<
- *             int current_item, current_wind
+ *             int current_wind = 0
  *             double next_range_distance = .0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_len_winds = __pyx_t_4;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":211
+ * 
  *             int len_winds = len(shot_info.winds)
- *             int current_item, current_wind
+ *             int current_wind = 0             # <<<<<<<<<<<<<<
+ *             double next_range_distance = .0
+ *             double next_wind_range = Wind.MAX_DISTANCE_FEET
+ */
+  __pyx_v_current_wind = 0;
+
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":212
+ *             int len_winds = len(shot_info.winds)
+ *             int current_wind = 0
  *             double next_range_distance = .0             # <<<<<<<<<<<<<<
  *             double next_wind_range = Wind.MAX_DISTANCE_FEET
  * 
  */
   __pyx_v_next_range_distance = .0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":212
- *             int current_item, current_wind
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":213
+ *             int current_wind = 0
  *             double next_range_distance = .0
  *             double next_wind_range = Wind.MAX_DISTANCE_FEET             # <<<<<<<<<<<<<<
  * 
  *             Vector velocity_vector, velocity_adjusted
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Wind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Wind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_next_wind_range = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":217
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
  *             Vector range_vector, delta_range_vector, wind_vector
  * 
  *         if len_winds < 1:             # <<<<<<<<<<<<<<
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  */
   __pyx_t_6 = (__pyx_v_len_winds < 1);
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":219
  * 
  *         if len_winds < 1:
  *             wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":217
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
  *             Vector range_vector, delta_range_vector, wind_vector
  * 
  *         if len_winds < 1:             # <<<<<<<<<<<<<<
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":220
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":221
  *             wind_vector = Vector(.0, .0, .0)
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])             # <<<<<<<<<<<<<<
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_wind_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":221
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":222
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot             # <<<<<<<<<<<<<<
  * 
  *         velocity = self.muzzle_velocity
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_Foot); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_next_wind_range = __pyx_t_5;
   }
   __pyx_L3:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":223
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":224
  *             next_wind_range = shot_info.winds[0].until_distance >> Distance.Foot
  * 
  *         velocity = self.muzzle_velocity             # <<<<<<<<<<<<<<
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  */
   __pyx_t_5 = __pyx_v_self->muzzle_velocity;
   __pyx_v_velocity = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":225
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
  *         velocity = self.muzzle_velocity
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)             # <<<<<<<<<<<<<<
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  */
-  __pyx_t_2 = PyFloat_FromDouble(((-__pyx_v_self->cant_cosine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((-__pyx_v_self->cant_cosine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = PyFloat_FromDouble(((-__pyx_v_self->cant_sine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble(((-__pyx_v_self->cant_sine) * __pyx_v_self->sight_height)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_float__0);
   __Pyx_GIVEREF(__pyx_float__0);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_float__0)) __PYX_ERR(0, 225, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_float__0)) __PYX_ERR(0, 226, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_range_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),             # <<<<<<<<<<<<<<
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  */
-  __pyx_t_7 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * cos(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_7 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * cos(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":228
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),             # <<<<<<<<<<<<<<
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  * 
  */
-  __pyx_t_1 = PyFloat_FromDouble(sin(__pyx_v_self->barrel_elevation)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(sin(__pyx_v_self->barrel_elevation)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":228
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":229
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * sin(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble((cos(__pyx_v_self->barrel_elevation) * sin(__pyx_v_self->barrel_azimuth))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":226
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":227
  *         # x: downrange distance, y: drop, z: windage
  *         range_vector = Vector(.0, -self.cant_cosine*self.sight_height, -self.cant_sine*self.sight_height)
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),             # <<<<<<<<<<<<<<
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity
  */
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7)) __PYX_ERR(0, 226, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7)) __PYX_ERR(0, 227, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error);
   __pyx_t_7 = 0;
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":228
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":229
  *         velocity_vector = Vector(cos(self.barrel_elevation) * cos(self.barrel_azimuth),
  *                                  sin(self.barrel_elevation),
  *                                  cos(self.barrel_elevation) * sin(self.barrel_azimuth)) * velocity             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_8 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_8 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 228, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_v_velocity_vector = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":232
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":233
  * 
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one             # <<<<<<<<<<<<<<
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_seen_zero = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":233
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":234
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  */
   __pyx_t_6 = (__pyx_v_range_vector->y >= 0.0);
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":234
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":235
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down             # <<<<<<<<<<<<<<
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  */
-    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_8 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_8);
     __pyx_t_8 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":233
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":234
  *         # With non-zero look_angle, rounding can suggest multiple adjacent zero-crossings
  *         seen_zero = CTrajFlag.NONE  # Record when we see each zero crossing so we only register one
  *         if range_vector.y >= 0:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  */
     goto __pyx_L4;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":235
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":236
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  * 
  */
   __pyx_t_9 = (__pyx_v_range_vector->y < 0.0);
@@ -8048,208 +7905,208 @@
     goto __pyx_L5_bool_binop_done;
   }
   __pyx_t_9 = (__pyx_v_self->barrel_elevation < __pyx_v_self->look_angle);
   __pyx_t_6 = __pyx_t_9;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":236
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":237
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!             # <<<<<<<<<<<<<<
  * 
  *         #region Trajectory Loop
  */
-    __pyx_t_8 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":235
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":236
  *         if range_vector.y >= 0:
  *             seen_zero |= CTrajFlag.ZERO_UP  # We're starting above zero; we can only go down
  *         elif range_vector.y < 0 and self.barrel_elevation < self.look_angle:             # <<<<<<<<<<<<<<
  *             seen_zero |= CTrajFlag.ZERO_DOWN  # We're below and pointing down from look angle; no zeroes!
  * 
  */
   }
   __pyx_L4:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":239
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":240
  * 
  *         #region Trajectory Loop
  *         while range_vector.x <= maximum_range + self.calc_step:             # <<<<<<<<<<<<<<
  *             _flag = CTrajFlag.NONE
  * 
  */
   while (1) {
     __pyx_t_6 = (__pyx_v_range_vector->x <= (__pyx_v_maximum_range + __pyx_v_self->calc_step));
     if (!__pyx_t_6) break;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":240
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":241
  *         #region Trajectory Loop
  *         while range_vector.x <= maximum_range + self.calc_step:
  *             _flag = CTrajFlag.NONE             # <<<<<<<<<<<<<<
  * 
  *             if range_vector.x >= next_wind_range:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_NONE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v__flag, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":242
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
  *             _flag = CTrajFlag.NONE
  * 
  *             if range_vector.x >= next_wind_range:             # <<<<<<<<<<<<<<
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  */
     __pyx_t_6 = (__pyx_v_range_vector->x >= __pyx_v_next_wind_range);
     if (__pyx_t_6) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":244
  * 
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1             # <<<<<<<<<<<<<<
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)
  */
       __pyx_v_current_wind = (__pyx_v_current_wind + 1);
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":244
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range             # <<<<<<<<<<<<<<
  *                     wind_vector = Vector(.0, .0, .0)
  *                     next_wind_range = Wind.MAX_DISTANCE_FEET
  */
       __pyx_t_6 = (__pyx_v_current_wind >= __pyx_v_len_winds);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":246
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
  *                     next_wind_range = Wind.MAX_DISTANCE_FEET
  *                 else:
  */
-        __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
         __pyx_t_1 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":246
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":247
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  *                     wind_vector = Vector(.0, .0, .0)
  *                     next_wind_range = Wind.MAX_DISTANCE_FEET             # <<<<<<<<<<<<<<
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Wind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Wind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 246, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_MAX_DISTANCE_FEET); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 247, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 246, __pyx_L1_error)
+        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_v_next_wind_range = __pyx_t_5;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":244
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":245
  *             if range_vector.x >= next_wind_range:
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range             # <<<<<<<<<<<<<<
  *                     wind_vector = Vector(.0, .0, .0)
  *                     next_wind_range = Wind.MAX_DISTANCE_FEET
  */
         goto __pyx_L10;
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":248
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":249
  *                     next_wind_range = Wind.MAX_DISTANCE_FEET
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])             # <<<<<<<<<<<<<<
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  */
       /*else*/ {
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
+        __pyx_t_8 = ((PyObject *)__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_wind_to_vector(__pyx_t_1)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF_SET(__pyx_v_wind_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_8));
         __pyx_t_8 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":249
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":250
  *                 else:
  *                     wind_vector = wind_to_vector(shot_info.winds[current_wind])
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot             # <<<<<<<<<<<<<<
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(
  */
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_winds); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_8, __pyx_v_current_wind, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_until_distance); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Foot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = PyNumber_Rshift(__pyx_t_8, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_Rshift(__pyx_t_8, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 249, __pyx_L1_error)
+        __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_v_next_wind_range = __pyx_t_5;
       }
       __pyx_L10:;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":242
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":243
  *             _flag = CTrajFlag.NONE
  * 
  *             if range_vector.x >= next_wind_range:             # <<<<<<<<<<<<<<
  *                 current_wind += 1
  *                 if current_wind >= len_winds:  # No more winds listed after this range
  */
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":251
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":252
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(             # <<<<<<<<<<<<<<
  *                 self.alt0 + range_vector.y)
  * 
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_shot_info, __pyx_n_s_atmo); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_density_factor_and_mach_for); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_density_factor_and_mach_for); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":252
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":253
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(
  *                 self.alt0 + range_vector.y)             # <<<<<<<<<<<<<<
  * 
  *             if filter_flags:
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->alt0 + __pyx_v_range_vector->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_self->alt0 + __pyx_v_range_vector->y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = NULL;
     __pyx_t_3 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_7)) {
@@ -8262,632 +8119,632 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_2};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
       PyObject* sequence = __pyx_t_1;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 251, __pyx_L1_error)
+        __PYX_ERR(0, 252, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_2);
       #else
-      __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
+      __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 251, __pyx_L1_error)
+      __pyx_t_7 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7);
       index = 0; __pyx_t_8 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_8)) goto __pyx_L11_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_8);
       index = 1; __pyx_t_2 = __pyx_t_10(__pyx_t_7); if (unlikely(!__pyx_t_2)) goto __pyx_L11_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_7), 2) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_7), 2) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
       __pyx_t_10 = NULL;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L12_unpacking_done;
       __pyx_L11_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_10 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 251, __pyx_L1_error)
+      __PYX_ERR(0, 252, __pyx_L1_error)
       __pyx_L12_unpacking_done:;
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":251
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":252
  *                     next_wind_range = shot_info.winds[current_wind].until_distance >> Distance.Foot
  * 
  *             density_factor, mach = shot_info.atmo.get_density_factor_and_mach_for_altitude(             # <<<<<<<<<<<<<<
  *                 self.alt0 + range_vector.y)
  * 
  */
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_8); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_11 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_density_factor = __pyx_t_5;
     __pyx_v_mach = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":254
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":255
  *                 self.alt0 + range_vector.y)
  * 
  *             if filter_flags:             # <<<<<<<<<<<<<<
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:
  */
     if (__pyx_v_filter_flags) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":256
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":257
  *             if filter_flags:
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:             # <<<<<<<<<<<<<<
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)
  */
       __pyx_t_6 = (__pyx_v_range_vector->x > 0.0);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":258
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":259
  *                 if range_vector.x > 0:
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)             # <<<<<<<<<<<<<<
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  */
         __pyx_v_reference_height = (__pyx_v_range_vector->x * tan(__pyx_v_self->look_angle));
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":260
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
  *                     reference_height = range_vector.x * tan(self.look_angle)
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:             # <<<<<<<<<<<<<<
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  */
-        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
+        __pyx_t_2 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 261, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 260, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 261, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = (!__pyx_t_6);
         if (__pyx_t_9) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP
  */
           __pyx_t_9 = (__pyx_v_range_vector->y >= __pyx_v_reference_height);
           if (__pyx_t_9) {
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":263
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP             # <<<<<<<<<<<<<<
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  */
-            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 262, __pyx_L1_error)
+            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":263
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":264
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP             # <<<<<<<<<<<<<<
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  */
-            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_UP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
+            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_2);
             __pyx_t_2 = 0;
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":262
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:
  *                         if range_vector.y >= reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_UP
  *                             seen_zero |= CTrajFlag.ZERO_UP
  */
           }
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":260
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":261
  *                     reference_height = range_vector.x * tan(self.look_angle)
  *                     # If we haven't seen ZERO_UP, we look for that first
  *                     if not seen_zero & CTrajFlag.ZERO_UP:             # <<<<<<<<<<<<<<
  *                         if range_vector.y >= reference_height:
  *                             _flag |= CTrajFlag.ZERO_UP
  */
           goto __pyx_L15;
         }
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":265
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:             # <<<<<<<<<<<<<<
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  */
-        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_And(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 265, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 266, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_6 = (!__pyx_t_9);
         if (__pyx_t_6) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  */
           __pyx_t_6 = (__pyx_v_range_vector->y < __pyx_v_reference_height);
           if (__pyx_t_6) {
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":268
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN             # <<<<<<<<<<<<<<
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  * 
  */
-            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+            __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+            __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_2);
             __pyx_t_2 = 0;
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":268
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":269
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN             # <<<<<<<<<<<<<<
  * 
  *                 # Mach crossing check
  */
-            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
+            __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_ZERO_DOWN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
+            __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v_seen_zero, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF_SET(__pyx_v_seen_zero, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
+            /* "py_ballisticcalc_exts/trajectory_calc.pyx":267
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:
  *                         if range_vector.y < reference_height:             # <<<<<<<<<<<<<<
  *                             _flag |= CTrajFlag.ZERO_DOWN
  *                             seen_zero |= CTrajFlag.ZERO_DOWN
  */
           }
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":265
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":266
  *                             seen_zero |= CTrajFlag.ZERO_UP
  *                     # We've crossed above sight line; now look for crossing back through it
  *                     elif not seen_zero & CTrajFlag.ZERO_DOWN:             # <<<<<<<<<<<<<<
  *                         if range_vector.y < reference_height:
  *                             _flag |= CTrajFlag.ZERO_DOWN
  */
         }
         __pyx_L15:;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":256
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":257
  *             if filter_flags:
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:             # <<<<<<<<<<<<<<
  *                     # Zero reference line is the sight line defined by look_angle
  *                     reference_height = range_vector.x * tan(self.look_angle)
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":271
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":272
  * 
  *                 # Mach crossing check
  *                 if (velocity / mach <= 1) and (previous_mach > 1):             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.MACH
  * 
  */
       if (unlikely(__pyx_v_mach == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 271, __pyx_L1_error)
+        __PYX_ERR(0, 272, __pyx_L1_error)
       }
       __pyx_t_9 = ((__pyx_v_velocity / __pyx_v_mach) <= 1.0);
       if (__pyx_t_9) {
       } else {
         __pyx_t_6 = __pyx_t_9;
         goto __pyx_L19_bool_binop_done;
       }
       __pyx_t_9 = (__pyx_v_previous_mach > 1.0);
       __pyx_t_6 = __pyx_t_9;
       __pyx_L19_bool_binop_done:;
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":272
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":273
  *                 # Mach crossing check
  *                 if (velocity / mach <= 1) and (previous_mach > 1):
  *                     _flag |= CTrajFlag.MACH             # <<<<<<<<<<<<<<
  * 
  *                 # Next range check
  */
-        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_MACH); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+        __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":271
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":272
  * 
  *                 # Mach crossing check
  *                 if (velocity / mach <= 1) and (previous_mach > 1):             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.MACH
  * 
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":275
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
  * 
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  */
       __pyx_t_6 = (__pyx_v_range_vector->x >= __pyx_v_next_range_distance);
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":277
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:
  *                     _flag |= CTrajFlag.RANGE             # <<<<<<<<<<<<<<
  *                     next_range_distance += step
  *                     current_item += 1
  */
-        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_e_21py_ballisticcalc_exts_15trajectory_calc_RANGE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_1 = PyNumber_InPlaceOr(__pyx_v__flag, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF_SET(__pyx_v__flag, __pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":277
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":278
  *                 if range_vector.x >= next_range_distance:
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step             # <<<<<<<<<<<<<<
  *                     current_item += 1
  * 
  */
         __pyx_v_next_range_distance = (__pyx_v_next_range_distance + __pyx_v_step);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":278
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":279
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  *                     current_item += 1             # <<<<<<<<<<<<<<
  * 
  *                 # Record TrajectoryData row
  */
         __pyx_v_current_item = (__pyx_v_current_item + 1);
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":275
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":276
  * 
  *                 # Next range check
  *                 if range_vector.x >= next_range_distance:             # <<<<<<<<<<<<<<
  *                     _flag |= CTrajFlag.RANGE
  *                     next_range_distance += step
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":281
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":282
  * 
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:             # <<<<<<<<<<<<<<
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
-      __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag(__pyx_v_filter_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PyNumber_And(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_And(__pyx_v__flag, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_6) {
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":284
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":285
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,             # <<<<<<<<<<<<<<
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  */
-        __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
+        __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":282
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":283
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:
  *                     ranges.append(create_trajectory_row(             # <<<<<<<<<<<<<<
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  */
-        __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
+        __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 283, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":287
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":288
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  *                     if current_item == ranges_length:             # <<<<<<<<<<<<<<
  *                         break
  * 
  */
         __pyx_t_6 = (__pyx_v_current_item == __pyx_v_ranges_length);
         if (__pyx_t_6) {
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":288
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":289
  *                     ))
  *                     if current_item == ranges_length:
  *                         break             # <<<<<<<<<<<<<<
  * 
  *             previous_mach = velocity / mach
  */
           goto __pyx_L8_break;
 
-          /* "py_ballisticcalc_exts/trajectory_calc.pyx":287
+          /* "py_ballisticcalc_exts/trajectory_calc.pyx":288
  *                         density_factor, drag, self.weight, _flag
  *                     ))
  *                     if current_item == ranges_length:             # <<<<<<<<<<<<<<
  *                         break
  * 
  */
         }
 
-        /* "py_ballisticcalc_exts/trajectory_calc.pyx":281
+        /* "py_ballisticcalc_exts/trajectory_calc.pyx":282
  * 
  *                 # Record TrajectoryData row
  *                 if _flag & filter_flags:             # <<<<<<<<<<<<<<
  *                     ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
       }
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":254
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":255
  *                 self.alt0 + range_vector.y)
  * 
  *             if filter_flags:             # <<<<<<<<<<<<<<
  *                 # Zero-crossing checks
  *                 if range_vector.x > 0:
  */
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":290
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":291
  *                         break
  * 
  *             previous_mach = velocity / mach             # <<<<<<<<<<<<<<
  * 
  *             #region Ballistic calculation step
  */
     if (unlikely(__pyx_v_mach == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 290, __pyx_L1_error)
+      __PYX_ERR(0, 291, __pyx_L1_error)
     }
     __pyx_v_previous_mach = (__pyx_v_velocity / __pyx_v_mach);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":293
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":294
  * 
  *             #region Ballistic calculation step
  *             delta_time = self.calc_step / velocity_vector.x             # <<<<<<<<<<<<<<
  *             velocity_adjusted = velocity_vector - wind_vector
  *             velocity = velocity_adjusted.magnitude()
  */
     if (unlikely(__pyx_v_velocity_vector->x == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 293, __pyx_L1_error)
+      __PYX_ERR(0, 294, __pyx_L1_error)
     }
     __pyx_v_delta_time = (__pyx_v_self->calc_step / __pyx_v_velocity_vector->x);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":294
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":295
  *             #region Ballistic calculation step
  *             delta_time = self.calc_step / velocity_vector.x
  *             velocity_adjusted = velocity_vector - wind_vector             # <<<<<<<<<<<<<<
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  */
-    __pyx_t_2 = PyNumber_Subtract(((PyObject *)__pyx_v_velocity_vector), ((PyObject *)__pyx_v_wind_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(((PyObject *)__pyx_v_velocity_vector), ((PyObject *)__pyx_v_wind_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 294, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_velocity_adjusted, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":295
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":296
  *             delta_time = self.calc_step / velocity_vector.x
  *             velocity_adjusted = velocity_vector - wind_vector
  *             velocity = velocity_adjusted.magnitude()             # <<<<<<<<<<<<<<
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_adjusted->__pyx_vtab)->magnitude(__pyx_v_velocity_adjusted); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 295, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_adjusted->__pyx_vtab)->magnitude(__pyx_v_velocity_adjusted); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 296, __pyx_L1_error)
     __pyx_v_velocity = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":296
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":297
  *             velocity_adjusted = velocity_vector - wind_vector
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)             # <<<<<<<<<<<<<<
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,
  */
     if (unlikely(__pyx_v_mach == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 296, __pyx_L1_error)
+      __PYX_ERR(0, 297, __pyx_L1_error)
     }
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->drag_by_mach(__pyx_v_self, (__pyx_v_velocity / __pyx_v_mach)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 296, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->drag_by_mach(__pyx_v_self, (__pyx_v_velocity / __pyx_v_mach)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
     __pyx_v_drag = ((__pyx_v_density_factor * __pyx_v_velocity) * __pyx_t_11);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":297
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":298
  *             velocity = velocity_adjusted.magnitude()
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time             # <<<<<<<<<<<<<<
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,
  */
-    __pyx_t_2 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyNumber_Multiply(((PyObject *)__pyx_v_velocity_adjusted), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(((PyObject *)__pyx_v_velocity_adjusted), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, ((PyObject *)__pyx_v_self->gravity_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, ((PyObject *)__pyx_v_self->gravity_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_8 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_InPlaceSubtract(((PyObject *)__pyx_v_velocity_vector), __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_InPlaceSubtract(((PyObject *)__pyx_v_velocity_vector), __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 297, __pyx_L1_error)
+    if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_velocity_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":298
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  */
-    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->calc_step); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->calc_step); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":300
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector
  */
-    __pyx_t_8 = PyFloat_FromDouble((__pyx_v_velocity_vector->y * __pyx_v_delta_time)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_8 = PyFloat_FromDouble((__pyx_v_velocity_vector->y * __pyx_v_delta_time)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":300
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":301
  *             delta_range_vector = Vector(self.calc_step,
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)             # <<<<<<<<<<<<<<
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_velocity_vector->z * __pyx_v_delta_time)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_velocity_vector->z * __pyx_v_delta_time)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":298
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":299
  *             drag = density_factor * velocity * self.drag_by_mach(velocity / mach)
  *             velocity_vector -= (velocity_adjusted * drag - self.gravity_vector) * delta_time
  *             delta_range_vector = Vector(self.calc_step,             # <<<<<<<<<<<<<<
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  */
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_8);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8)) __PYX_ERR(0, 298, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error);
     __pyx_t_1 = 0;
     __pyx_t_8 = 0;
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v_delta_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":301
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":302
  *                                         velocity_vector.y * delta_time,
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector             # <<<<<<<<<<<<<<
  *             velocity = velocity_vector.magnitude()
  *             time += delta_range_vector.magnitude() / velocity
  */
-    __pyx_t_2 = PyNumber_InPlaceAdd(((PyObject *)__pyx_v_range_vector), ((PyObject *)__pyx_v_delta_range_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceAdd(((PyObject *)__pyx_v_range_vector), ((PyObject *)__pyx_v_delta_range_vector)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 301, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector))))) __PYX_ERR(0, 302, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_range_vector, ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":302
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":303
  *                                         velocity_vector.z * delta_time)
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()             # <<<<<<<<<<<<<<
  *             time += delta_range_vector.magnitude() / velocity
  * 
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_vector->__pyx_vtab)->magnitude(__pyx_v_velocity_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 302, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_velocity_vector->__pyx_vtab)->magnitude(__pyx_v_velocity_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 303, __pyx_L1_error)
     __pyx_v_velocity = __pyx_t_11;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":303
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":304
  *             range_vector += delta_range_vector
  *             velocity = velocity_vector.magnitude()
  *             time += delta_range_vector.magnitude() / velocity             # <<<<<<<<<<<<<<
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_delta_range_vector->__pyx_vtab)->magnitude(__pyx_v_delta_range_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 303, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_v_delta_range_vector->__pyx_vtab)->magnitude(__pyx_v_delta_range_vector); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 304, __pyx_L1_error)
     if (unlikely(__pyx_v_velocity == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 303, __pyx_L1_error)
+      __PYX_ERR(0, 304, __pyx_L1_error)
     }
     __pyx_v_time = (__pyx_v_time + (__pyx_t_11 / __pyx_v_velocity));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":305
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
  *             time += delta_range_vector.magnitude() / velocity
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:             # <<<<<<<<<<<<<<
  *                 break
  *             #endregion
  */
     __pyx_t_9 = (__pyx_v_velocity < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMinimumVelocity);
@@ -8897,84 +8754,84 @@
       goto __pyx_L25_bool_binop_done;
     }
     __pyx_t_9 = (__pyx_v_range_vector->y < __pyx_v_21py_ballisticcalc_exts_15trajectory_calc_cMaximumDrop);
     __pyx_t_6 = __pyx_t_9;
     __pyx_L25_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":307
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:
  *                 break             # <<<<<<<<<<<<<<
  *             #endregion
  *         #endregion
  */
       goto __pyx_L8_break;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":305
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":306
  *             time += delta_range_vector.magnitude() / velocity
  * 
  *             if velocity < cMinimumVelocity or range_vector.y < cMaximumDrop:             # <<<<<<<<<<<<<<
  *                 break
  *             #endregion
  */
     }
   }
   __pyx_L8_break:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":310
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":311
  *         #endregion
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:             # <<<<<<<<<<<<<<
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
   __pyx_t_6 = (!__pyx_v_filter_flags);
   if (__pyx_t_6) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":313
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":314
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,             # <<<<<<<<<<<<<<
  *                         density_factor, drag, self.weight, _flag))
  *         return ranges
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_11 = ((struct __pyx_vtabstruct_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self->__pyx_vtab)->spin_drift(__pyx_v_self, __pyx_v_time); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L1_error)
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":314
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":315
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  *                         density_factor, drag, self.weight, _flag))             # <<<<<<<<<<<<<<
  *         return ranges
  * 
  */
-    if (unlikely(!__pyx_v__flag)) { __Pyx_RaiseUnboundLocalError("_flag"); __PYX_ERR(0, 314, __pyx_L1_error) }
+    if (unlikely(!__pyx_v__flag)) { __Pyx_RaiseUnboundLocalError("_flag"); __PYX_ERR(0, 315, __pyx_L1_error) }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":311
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":312
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:
  *             ranges.append(create_trajectory_row(             # <<<<<<<<<<<<<<
  *                         time, range_vector, velocity_vector,
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  */
-    __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_create_trajectory_row(__pyx_v_time, __pyx_v_range_vector, __pyx_v_velocity_vector, __pyx_v_velocity, __pyx_v_mach, __pyx_t_11, __pyx_v_self->look_angle, __pyx_v_density_factor, __pyx_v_drag, __pyx_v_self->weight, __pyx_v__flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_ranges, __pyx_t_2); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":310
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":311
  *         #endregion
  *         # If filter_flags == 0 then all we want is the ending value
  *         if not filter_flags:             # <<<<<<<<<<<<<<
  *             ranges.append(create_trajectory_row(
  *                         time, range_vector, velocity_vector,
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":315
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":316
  *                         velocity, mach, self.spin_drift(time), self.look_angle,
  *                         density_factor, drag, self.weight, _flag))
  *         return ranges             # <<<<<<<<<<<<<<
  * 
  *     cdef double drag_by_mach(self, double mach):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -9008,15 +8865,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_delta_range_vector);
   __Pyx_XDECREF((PyObject *)__pyx_v_wind_vector);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":317
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":318
  *         return ranges
  * 
  *     cdef double drag_by_mach(self, double mach):             # <<<<<<<<<<<<<<
  *         """ Drag force = V^2 * Cd * AirDensity * S / 2m where:
  *             cStandardDensity of Air = 0.076474 lb/ft^3
  */
 
@@ -9028,46 +8885,46 @@
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("drag_by_mach", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":325
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":326
  *         Thus: The magic constant found here = StandardDensity * pi / (4 * 2 * 144)
  *         """
  *         cdef double cd = calculate_by_curve(self._table_data, self._curve, mach)             # <<<<<<<<<<<<<<
  *         return cd * 2.08551e-04 / self._bc
  * 
  */
   __pyx_t_1 = __pyx_v_self->_table_data;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __pyx_v_self->_curve;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), __pyx_v_mach); if (unlikely(__pyx_t_3 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_by_curve(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), __pyx_v_mach); if (unlikely(__pyx_t_3 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_cd = __pyx_t_3;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":326
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":327
  *         """
  *         cdef double cd = calculate_by_curve(self._table_data, self._curve, mach)
  *         return cd * 2.08551e-04 / self._bc             # <<<<<<<<<<<<<<
  * 
  *     cdef double spin_drift(self, double time):
  */
   __pyx_t_3 = (__pyx_v_cd * 2.08551e-04);
   if (unlikely(__pyx_v_self->_bc == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 326, __pyx_L1_error)
+    __PYX_ERR(0, 327, __pyx_L1_error)
   }
   __pyx_r = (__pyx_t_3 / __pyx_v_self->_bc);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":317
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":318
  *         return ranges
  * 
  *     cdef double drag_by_mach(self, double mach):             # <<<<<<<<<<<<<<
  *         """ Drag force = V^2 * Cd * AirDensity * S / 2m where:
  *             cStandardDensity of Air = 0.076474 lb/ft^3
  */
 
@@ -9078,15 +8935,15 @@
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.drag_by_mach", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":328
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":329
  *         return cd * 2.08551e-04 / self._bc
  * 
  *     cdef double spin_drift(self, double time):             # <<<<<<<<<<<<<<
  *         """Litz spin-drift approximation
  *         :param time: Time of flight
  */
 
@@ -9099,25 +8956,25 @@
   PyObject *__pyx_t_3 = NULL;
   double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spin_drift", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":333
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":334
  *         :return: windage due to spin drift, in feet
  *         """
  *         if self.twist != 0:             # <<<<<<<<<<<<<<
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  */
   __pyx_t_1 = (__pyx_v_self->twist != 0.0);
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":334
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":335
  *         """
  *         if self.twist != 0:
  *             sign = 1 if self.twist > 0 else -1             # <<<<<<<<<<<<<<
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  *         return 0
  */
     __pyx_t_1 = (__pyx_v_self->twist > 0.0);
@@ -9127,54 +8984,54 @@
     } else {
       __Pyx_INCREF(__pyx_int_neg_1);
       __pyx_t_2 = __pyx_int_neg_1;
     }
     __pyx_v_sign = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":335
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":336
  *         if self.twist != 0:
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
-    __pyx_t_2 = PyFloat_FromDouble(((1.25 * (__pyx_v_self->stability_coefficient + 1.2)) * pow(__pyx_v_time, 1.83))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble(((1.25 * (__pyx_v_self->stability_coefficient + 1.2)) * pow(__pyx_v_time, 1.83))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_v_sign, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_v_sign, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_12, 12, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_TrueDivideObjC(__pyx_t_3, __pyx_int_12, 12, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_4;
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":333
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":334
  *         :return: windage due to spin drift, in feet
  *         """
  *         if self.twist != 0:             # <<<<<<<<<<<<<<
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":336
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":337
  *             sign = 1 if self.twist > 0 else -1
  *             return sign * (1.25 * (self.stability_coefficient + 1.2) * pow(time, 1.83) ) / 12
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":328
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":329
  *         return cd * 2.08551e-04 / self._bc
  * 
  *     cdef double spin_drift(self, double time):             # <<<<<<<<<<<<<<
  *         """Litz spin-drift approximation
  *         :param time: Time of flight
  */
 
@@ -9186,15 +9043,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_sign);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":338
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":339
  *         return 0
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):             # <<<<<<<<<<<<<<
  *         """Miller stability coefficient"""
  *         cdef:
  */
 
@@ -9216,15 +9073,15 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calc_stability_coefficient", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":342
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
  *         cdef:
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:             # <<<<<<<<<<<<<<
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  */
   __pyx_t_2 = (__pyx_v_self->twist != 0);
@@ -9240,152 +9097,152 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->diameter != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":344
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:
  *             twist_rate = fabs(self.twist) / self.diameter             # <<<<<<<<<<<<<<
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  */
     __pyx_t_3 = fabs(__pyx_v_self->twist);
     if (unlikely(__pyx_v_self->diameter == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 343, __pyx_L1_error)
+      __PYX_ERR(0, 344, __pyx_L1_error)
     }
     __pyx_v_twist_rate = (__pyx_t_3 / __pyx_v_self->diameter);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":344
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":345
  *         if self.twist and self.length and self.diameter:
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter             # <<<<<<<<<<<<<<
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  */
     if (unlikely(__pyx_v_self->diameter == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 344, __pyx_L1_error)
+      __PYX_ERR(0, 345, __pyx_L1_error)
     }
     __pyx_v_length = (__pyx_v_self->length / __pyx_v_self->diameter);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":345
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":346
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))             # <<<<<<<<<<<<<<
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  */
     __pyx_t_3 = (30.0 * __pyx_v_self->weight);
     __pyx_t_4 = (((pow(__pyx_v_twist_rate, 2.0) * pow(__pyx_v_self->diameter, 3.0)) * __pyx_v_length) * (1.0 + pow(__pyx_v_length, 2.0)));
     if (unlikely(__pyx_t_4 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 345, __pyx_L1_error)
+      __PYX_ERR(0, 346, __pyx_L1_error)
     }
     __pyx_v_sd = (__pyx_t_3 / __pyx_t_4);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":346
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":347
  *             length = self.length / self.diameter
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)             # <<<<<<<<<<<<<<
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg
  */
     __pyx_v_fv = pow((__pyx_v_self->muzzle_velocity / 2800.0), (1.0 / 3.0));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":347
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":348
  *             sd = 30 * self.weight / (pow(twist_rate, 2) * pow(self.diameter, 3) * length * (1 + pow(length, 2)))
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit             # <<<<<<<<<<<<<<
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_temperature); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_temperature); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Temperature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Temperature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Fahrenheit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Fahrenheit); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyNumber_Rshift(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Rshift(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_ft = __pyx_t_4;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":348
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":349
  *             fv = pow(self.muzzle_velocity / 2800, 1.0 / 3.0)
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg             # <<<<<<<<<<<<<<
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_pressure); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_atmo, __pyx_n_s_pressure); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Pressure); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Pressure); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_InHg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_InHg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyNumber_Rshift(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_Rshift(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_7); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_pt = __pyx_t_4;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":349
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":350
  *             ft = atmo.temperature >> Temperature.Fahrenheit
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)             # <<<<<<<<<<<<<<
  *             return sd * fv * ftp
  *         return 0
  */
     if (unlikely(__pyx_v_pt == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 349, __pyx_L1_error)
+      __PYX_ERR(0, 350, __pyx_L1_error)
     }
     __pyx_v_ftp = (((__pyx_v_ft + 460.0) / 519.0) * (29.92 / __pyx_v_pt));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":350
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":351
  *             pt = atmo.pressure >> Pressure.InHg
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     __pyx_r = ((__pyx_v_sd * __pyx_v_fv) * __pyx_v_ftp);
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":342
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":343
  *         cdef:
  *             double twist_rate, length, sd, fv, ft, pt, ftp
  *         if self.twist and self.length and self.diameter:             # <<<<<<<<<<<<<<
  *             twist_rate = fabs(self.twist) / self.diameter
  *             length = self.length / self.diameter
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":351
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":352
  *             ftp = ((ft + 460) / (59 + 460)) * (29.92 / pt)
  *             return sd * fv * ftp
  *         return 0             # <<<<<<<<<<<<<<
  * 
  * cdef Vector wind_to_vector(object wind):
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":338
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":339
  *         return 0
  * 
  *     cdef double calc_stability_coefficient(self, object atmo):             # <<<<<<<<<<<<<<
  *         """Miller stability coefficient"""
  *         cdef:
  */
 
@@ -9404,24 +9261,24 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__, "TrajectoryCalc.__reduce_cython__(self)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__};
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__, "TrajectoryCalc.__reduce_cython__(self)");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -9438,22 +9295,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self));
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self) {
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -9796,24 +9653,24 @@
  *     else:
  *         return __pyx_unpickle_TrajectoryCalc, (type(self), 0x1a1505e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TrajectoryCalc__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__, "TrajectoryCalc.__setstate_cython__(self, __pyx_state)");
-static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__};
-static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__(PyObject *__pyx_v_self, 
+PyDoc_STRVAR(__pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__, "TrajectoryCalc.__setstate_cython__(self, __pyx_state)");
+static PyMethodDef __pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__};
+static PyObject *__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -9879,28 +9736,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("py_ballisticcalc_exts.trajectory_calc.TrajectoryCalc.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__(((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
@@ -9931,15 +9788,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":353
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":354
  *         return 0
  * 
  * cdef Vector wind_to_vector(object wind):             # <<<<<<<<<<<<<<
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  */
 
@@ -9954,127 +9811,127 @@
   PyObject *__pyx_t_4 = NULL;
   double __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wind_to_vector", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":355
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":356
  * cdef Vector wind_to_vector(object wind):
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)             # <<<<<<<<<<<<<<
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)
  *     return Vector(range_component, 0., cross_component)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_FPS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_FPS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Rshift(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Angular); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Radian); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyFloat_FromDouble(cos(__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(cos(__pyx_t_5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_range_component = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":356
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":357
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)             # <<<<<<<<<<<<<<
  *     return Vector(range_component, 0., cross_component)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_velocity); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_FPS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Rshift(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Rshift(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_wind, __pyx_n_s_direction_from); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Angular); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Angular); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_Radian); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Rshift(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyFloat_FromDouble(sin(__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(sin(__pyx_t_5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cross_component = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":357
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":358
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  *         double cross_component = (wind.velocity >> Velocity.FPS) * sin(wind.direction_from >> Angular.Radian)
  *     return Vector(range_component, 0., cross_component)             # <<<<<<<<<<<<<<
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_range_component); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_range_component); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_cross_component); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_cross_component); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error);
   __Pyx_INCREF(__pyx_float_0_);
   __Pyx_GIVEREF(__pyx_float_0_);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_float_0_)) __PYX_ERR(0, 357, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_float_0_)) __PYX_ERR(0, 358, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector), __pyx_t_1, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_Vector *)__pyx_t_4);
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":353
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":354
  *         return 0
  * 
  * cdef Vector wind_to_vector(object wind):             # <<<<<<<<<<<<<<
  *     cdef:
  *         double range_component = (wind.velocity >> Velocity.FPS) * cos(wind.direction_from >> Angular.Radian)
  */
 
@@ -10088,15 +9945,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":359
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":360
  *     return Vector(range_component, 0., cross_component)
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,             # <<<<<<<<<<<<<<
  *                            double velocity, double mach, double spin_drift, double look_angle,
  *                            double density_factor, double drag, double weight, object flag):
  */
 
@@ -10117,94 +9974,94 @@
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_trajectory_row", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":363
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":364
  *                            double density_factor, double drag, double weight, object flag):
  *     cdef:
  *         double windage = range_vector.z + spin_drift             # <<<<<<<<<<<<<<
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  */
   __pyx_v_windage = (__pyx_v_range_vector->z + __pyx_v_spin_drift);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":364
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":365
  *     cdef:
  *         double windage = range_vector.z + spin_drift
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)             # <<<<<<<<<<<<<<
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  */
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_range_vector->y); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_range_vector->y); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L1_error)
   __pyx_v_drop_adjustment = __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":365
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":366
  *         double windage = range_vector.z + spin_drift
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)             # <<<<<<<<<<<<<<
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  */
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_windage); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(__pyx_v_range_vector->x, __pyx_v_windage); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
   __pyx_v_windage_adjustment = __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":366
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":367
  *         double drop_adjustment = get_correction(range_vector.x, range_vector.y)
  *         double windage_adjustment = get_correction(range_vector.x, windage)
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)             # <<<<<<<<<<<<<<
  * 
  *     return TrajectoryData(
  */
   if (unlikely(__pyx_v_velocity_vector->x == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 366, __pyx_L1_error)
+    __PYX_ERR(0, 367, __pyx_L1_error)
   }
   __pyx_v_trajectory_angle = atan((__pyx_v_velocity_vector->y / __pyx_v_velocity_vector->x));
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":368
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  *     return TrajectoryData(             # <<<<<<<<<<<<<<
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TrajectoryData); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":370
  * 
  *     return TrajectoryData(
  *         time=time,             # <<<<<<<<<<<<<<
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_time, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_time, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":370
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":371
  *     return TrajectoryData(
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),             # <<<<<<<<<<<<<<
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10217,34 +10074,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 370, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_distance, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_distance, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":371
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":372
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),             # <<<<<<<<<<<<<<
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FPS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FPS); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_velocity); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10257,50 +10114,50 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_velocity, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_velocity, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":372
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":373
  *         distance=Distance.Foot(range_vector.x),
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,             # <<<<<<<<<<<<<<
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  */
   if (unlikely(__pyx_v_mach == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 372, __pyx_L1_error)
+    __PYX_ERR(0, 373, __pyx_L1_error)
   }
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_velocity / __pyx_v_mach)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_velocity / __pyx_v_mach)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mach, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mach, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":373
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":374
  *         velocity=Velocity.FPS(velocity),
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),             # <<<<<<<<<<<<<<
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Foot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_range_vector->y); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10313,34 +10170,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_height, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_height, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":374
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":375
  *         mach=velocity / mach,
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),             # <<<<<<<<<<<<<<
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(((__pyx_v_range_vector->y - (__pyx_v_range_vector->x * tan(__pyx_v_look_angle))) * cos(__pyx_v_look_angle))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(((__pyx_v_range_vector->y - (__pyx_v_range_vector->x * tan(__pyx_v_look_angle))) * cos(__pyx_v_look_angle))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10353,40 +10210,40 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target_drop, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_target_drop, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":375
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":376
  *         height=Distance.Foot(range_vector.y),
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),             # <<<<<<<<<<<<<<
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_9 = (__pyx_v_range_vector->x != 0);
   if (__pyx_t_9) {
     __pyx_t_1 = __pyx_v_look_angle;
   } else {
     __pyx_t_1 = 0.0;
   }
-  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_drop_adjustment - __pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_drop_adjustment - __pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10399,34 +10256,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drop_adj, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drop_adj, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":376
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":377
  *         target_drop=Distance.Foot((range_vector.y - range_vector.x * tan(look_angle)) * cos(look_angle)),
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),             # <<<<<<<<<<<<<<
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_windage); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_windage); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10439,34 +10296,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":377
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":378
  *         drop_adj=Angular.Radian(drop_adjustment - (look_angle if range_vector.x else 0)),
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),             # <<<<<<<<<<<<<<
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_windage_adjustment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_windage_adjustment); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10479,39 +10336,39 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage_adj, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_windage_adj, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":378
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":379
  *         windage=Distance.Foot(windage),
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),             # <<<<<<<<<<<<<<
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Foot); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_1 = cos(__pyx_v_look_angle);
   if (unlikely(__pyx_t_1 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 378, __pyx_L1_error)
+    __PYX_ERR(0, 379, __pyx_L1_error)
   }
-  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_range_vector->x / __pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_range_vector->x / __pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10524,34 +10381,34 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_look_distance, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_look_distance, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":379
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":380
  *         windage_adj=Angular.Radian(windage_adjustment),
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),             # <<<<<<<<<<<<<<
  *         density_factor = density_factor-1,
  *         drag = drag,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Angular); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Radian); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 380, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_trajectory_angle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_trajectory_angle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10564,59 +10421,59 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 380, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_angle, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_angle, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":380
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":381
  *         look_distance= Distance.Foot(range_vector.x / cos(look_angle)),
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,             # <<<<<<<<<<<<<<
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  */
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_density_factor - 1.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_density_factor - 1.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_density_factor, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_density_factor, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":381
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":382
  *         angle=Angular.Radian(trajectory_angle),
  *         density_factor = density_factor-1,
  *         drag = drag,             # <<<<<<<<<<<<<<
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  */
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_drag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drag, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_drag, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":382
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":383
  *         density_factor = density_factor-1,
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),             # <<<<<<<<<<<<<<
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  *         flag=flag
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Energy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Energy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FootPound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_FootPound); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
@@ -10629,35 +10486,35 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_6};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_energy, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_energy, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":383
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":384
  *         drag = drag,
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),             # <<<<<<<<<<<<<<
  *         flag=flag
  *     )
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Weight); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Weight); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Pound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Pound); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 383, __pyx_L1_error)
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(__pyx_v_weight, __pyx_v_velocity); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
@@ -10670,46 +10527,46 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
     __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ogw, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_ogw, __pyx_t_4) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":384
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":385
  *         energy=Energy.FootPound(calculate_energy(weight, velocity)),
  *         ogw=Weight.Pound(calculate_ogv(weight, velocity)),
  *         flag=flag             # <<<<<<<<<<<<<<
  *     )
  * 
  */
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flag, __pyx_v_flag) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flag, __pyx_v_flag) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":368
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":369
  *         double trajectory_angle = atan(velocity_vector.y / velocity_vector.x)
  * 
  *     return TrajectoryData(             # <<<<<<<<<<<<<<
  *         time=time,
  *         distance=Distance.Foot(range_vector.x),
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":359
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":360
  *     return Vector(range_component, 0., cross_component)
  * 
  * cdef create_trajectory_row(double time, Vector range_vector, Vector velocity_vector,             # <<<<<<<<<<<<<<
  *                            double velocity, double mach, double spin_drift, double look_angle,
  *                            double density_factor, double drag, double weight, object flag):
  */
 
@@ -10725,147 +10582,147 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":388
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":389
  * 
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):             # <<<<<<<<<<<<<<
  *     if distance != 0:
  *         return atan(offset / distance)
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_get_correction(double __pyx_v_distance, double __pyx_v_offset) {
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":389
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:             # <<<<<<<<<<<<<<
  *         return atan(offset / distance)
  *     return 0  # better None
  */
   __pyx_t_1 = (__pyx_v_distance != 0.0);
   if (__pyx_t_1) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":391
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:
  *         return atan(offset / distance)             # <<<<<<<<<<<<<<
  *     return 0  # better None
  * 
  */
     __pyx_r = atan((__pyx_v_offset / __pyx_v_distance));
     goto __pyx_L0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":389
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":390
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):
  *     if distance != 0:             # <<<<<<<<<<<<<<
  *         return atan(offset / distance)
  *     return 0  # better None
  */
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":391
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":392
  *     if distance != 0:
  *         return atan(offset / distance)
  *     return 0  # better None             # <<<<<<<<<<<<<<
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):
  */
   __pyx_r = 0.0;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":388
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":389
  * 
  * @cython.cdivision(True)
  * cdef double get_correction(double distance, double offset):             # <<<<<<<<<<<<<<
  *     if distance != 0:
  *         return atan(offset / distance)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":393
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":394
  *     return 0  # better None
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_energy(double __pyx_v_bullet_weight, double __pyx_v_velocity) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":394
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":395
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):
  *     return bullet_weight * pow(velocity, 2) / 450400             # <<<<<<<<<<<<<<
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):
  */
   __pyx_r = ((__pyx_v_bullet_weight * pow(__pyx_v_velocity, 2.0)) / 450400.0);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":393
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":394
  *     return 0  # better None
  * 
  * cdef double calculate_energy(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":396
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":397
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  */
 
 static double __pyx_f_21py_ballisticcalc_exts_15trajectory_calc_calculate_ogv(double __pyx_v_bullet_weight, double __pyx_v_velocity) {
   double __pyx_r;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":397
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":398
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12             # <<<<<<<<<<<<<<
  * 
  * cdef list calculate_curve(list data_points):
  */
   __pyx_r = ((pow(__pyx_v_bullet_weight, 2.0) * pow(__pyx_v_velocity, 3.0)) * 1.5e-12);
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":396
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":397
  *     return bullet_weight * pow(velocity, 2) / 450400
  * 
  * cdef double calculate_ogv(double bullet_weight, double velocity):             # <<<<<<<<<<<<<<
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":399
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":400
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  * cdef list calculate_curve(list data_points):             # <<<<<<<<<<<<<<
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []
  */
 
@@ -10901,618 +10758,618 @@
   int __pyx_t_11;
   long __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_curve", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":401
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":402
  * cdef list calculate_curve(list data_points):
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []             # <<<<<<<<<<<<<<
  *     cdef CurvePoint curve_point
  *     cdef int num_points, len_data_points, len_data_range
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_curve = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":405
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":406
  *     cdef int num_points, len_data_points, len_data_range
  * 
- *     rate = (data_points[1]['CD'] - data_points[0]['CD']) / (data_points[1]['Mach'] - data_points[0]['Mach'])             # <<<<<<<<<<<<<<
- *     curve = [CurvePoint(0, rate, data_points[0]['CD'] - data_points[0]['Mach'] * rate)]
+ *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)             # <<<<<<<<<<<<<<
+ *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 405, __pyx_L1_error)
+    __PYX_ERR(0, 406, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_CD); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 405, __pyx_L1_error)
+    __PYX_ERR(0, 406, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 405, __pyx_L1_error)
+    __PYX_ERR(0, 406, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 405, __pyx_L1_error)
+    __PYX_ERR(0, 406, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_rate = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":406
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":407
  * 
- *     rate = (data_points[1]['CD'] - data_points[0]['CD']) / (data_points[1]['Mach'] - data_points[0]['Mach'])
- *     curve = [CurvePoint(0, rate, data_points[0]['CD'] - data_points[0]['Mach'] * rate)]             # <<<<<<<<<<<<<<
+ *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)
+ *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]             # <<<<<<<<<<<<<<
  *     len_data_points = int(len(data_points))
  *     len_data_range = len_data_points - 1
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_a, __pyx_float_0_0) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_a, __pyx_float_0_0) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_b, __pyx_t_3) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_b, __pyx_t_3) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 407, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_CD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 407, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data_points, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_c, __pyx_t_3) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_c, __pyx_t_3) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error);
   __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_curve, ((PyObject*)__pyx_t_3));
   __pyx_t_3 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":407
- *     rate = (data_points[1]['CD'] - data_points[0]['CD']) / (data_points[1]['Mach'] - data_points[0]['Mach'])
- *     curve = [CurvePoint(0, rate, data_points[0]['CD'] - data_points[0]['Mach'] * rate)]
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":408
+ *     rate = (data_points[1].CD - data_points[0].CD) / (data_points[1].Mach - data_points[0].Mach)
+ *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))             # <<<<<<<<<<<<<<
  *     len_data_range = len_data_points - 1
  * 
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 408, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_v_data_points); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyList_GET_SIZE(__pyx_v_data_points); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 408, __pyx_L1_error)
   __pyx_v_len_data_points = ((int)__pyx_t_7);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":408
- *     curve = [CurvePoint(0, rate, data_points[0]['CD'] - data_points[0]['Mach'] * rate)]
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":409
+ *     curve = [CurvePoint(0, rate, data_points[0].CD - data_points[0].Mach * rate)]
  *     len_data_points = int(len(data_points))
  *     len_data_range = len_data_points - 1             # <<<<<<<<<<<<<<
  * 
  *     for i in range(1, len_data_range):
  */
   __pyx_v_len_data_range = (__pyx_v_len_data_points - 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":410
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
  *     len_data_range = len_data_points - 1
  * 
  *     for i in range(1, len_data_range):             # <<<<<<<<<<<<<<
- *         x1 = data_points[i - 1]['Mach']
- *         x2 = data_points[i]['Mach']
+ *         x1 = data_points[i - 1].Mach
+ *         x2 = data_points[i].Mach
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_len_data_range); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_len_data_range); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_1)) __PYX_ERR(0, 410, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_1)) __PYX_ERR(0, 411, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4);
     __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 411, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 410, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
           #endif
           if (__pyx_t_7 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 410, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
         #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 410, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
           #endif
           if (__pyx_t_7 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 410, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
         #else
-        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_8(__pyx_t_4);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 410, __pyx_L1_error)
+          else __PYX_ERR(0, 411, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":412
  * 
  *     for i in range(1, len_data_range):
- *         x1 = data_points[i - 1]['Mach']             # <<<<<<<<<<<<<<
- *         x2 = data_points[i]['Mach']
- *         x3 = data_points[i + 1]['Mach']
+ *         x1 = data_points[i - 1].Mach             # <<<<<<<<<<<<<<
+ *         x2 = data_points[i].Mach
+ *         x3 = data_points[i + 1].Mach
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 411, __pyx_L1_error)
+      __PYX_ERR(0, 412, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_x1 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":412
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":413
  *     for i in range(1, len_data_range):
- *         x1 = data_points[i - 1]['Mach']
- *         x2 = data_points[i]['Mach']             # <<<<<<<<<<<<<<
- *         x3 = data_points[i + 1]['Mach']
- *         y1 = data_points[i - 1]['CD']
+ *         x1 = data_points[i - 1].Mach
+ *         x2 = data_points[i].Mach             # <<<<<<<<<<<<<<
+ *         x3 = data_points[i + 1].Mach
+ *         y1 = data_points[i - 1].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 412, __pyx_L1_error)
+      __PYX_ERR(0, 413, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_x2 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":413
- *         x1 = data_points[i - 1]['Mach']
- *         x2 = data_points[i]['Mach']
- *         x3 = data_points[i + 1]['Mach']             # <<<<<<<<<<<<<<
- *         y1 = data_points[i - 1]['CD']
- *         y2 = data_points[i]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":414
+ *         x1 = data_points[i - 1].Mach
+ *         x2 = data_points[i].Mach
+ *         x3 = data_points[i + 1].Mach             # <<<<<<<<<<<<<<
+ *         y1 = data_points[i - 1].CD
+ *         y2 = data_points[i].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 413, __pyx_L1_error)
+      __PYX_ERR(0, 414, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_x3 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":414
- *         x2 = data_points[i]['Mach']
- *         x3 = data_points[i + 1]['Mach']
- *         y1 = data_points[i - 1]['CD']             # <<<<<<<<<<<<<<
- *         y2 = data_points[i]['CD']
- *         y3 = data_points[i + 1]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":415
+ *         x2 = data_points[i].Mach
+ *         x3 = data_points[i + 1].Mach
+ *         y1 = data_points[i - 1].CD             # <<<<<<<<<<<<<<
+ *         y2 = data_points[i].CD
+ *         y3 = data_points[i + 1].CD
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 414, __pyx_L1_error)
+      __PYX_ERR(0, 415, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_v_y1 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":415
- *         x3 = data_points[i + 1]['Mach']
- *         y1 = data_points[i - 1]['CD']
- *         y2 = data_points[i]['CD']             # <<<<<<<<<<<<<<
- *         y3 = data_points[i + 1]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":416
+ *         x3 = data_points[i + 1].Mach
+ *         y1 = data_points[i - 1].CD
+ *         y2 = data_points[i].CD             # <<<<<<<<<<<<<<
+ *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 415, __pyx_L1_error)
+      __PYX_ERR(0, 416, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_v_i); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_y2 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":416
- *         y1 = data_points[i - 1]['CD']
- *         y2 = data_points[i]['CD']
- *         y3 = data_points[i + 1]['CD']             # <<<<<<<<<<<<<<
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":417
+ *         y1 = data_points[i - 1].CD
+ *         y2 = data_points[i].CD
+ *         y3 = data_points[i + 1].CD             # <<<<<<<<<<<<<<
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  */
     if (unlikely(__pyx_v_data_points == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 416, __pyx_L1_error)
+      __PYX_ERR(0, 417, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_data_points, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_y3 = __pyx_t_5;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":417
- *         y2 = data_points[i]['CD']
- *         y3 = data_points[i + 1]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
+ *         y2 = data_points[i].CD
+ *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (             # <<<<<<<<<<<<<<
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  */
     __pyx_t_5 = (((__pyx_v_y3 - __pyx_v_y1) * (__pyx_v_x2 - __pyx_v_x1)) - ((__pyx_v_y2 - __pyx_v_y1) * (__pyx_v_x3 - __pyx_v_x1)));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
- *         y3 = data_points[i + 1]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":419
+ *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))             # <<<<<<<<<<<<<<
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  *         c = y1 - (a * x1 * x1 + b * x1)
  */
     __pyx_t_9 = ((((__pyx_v_x3 * __pyx_v_x3) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x2 - __pyx_v_x1)) - (((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1)) * (__pyx_v_x3 - __pyx_v_x1)));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":417
- *         y2 = data_points[i]['CD']
- *         y3 = data_points[i + 1]['CD']
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":418
+ *         y2 = data_points[i].CD
+ *         y3 = data_points[i + 1].CD
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (             # <<<<<<<<<<<<<<
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  */
     if (unlikely(__pyx_t_9 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 418, __pyx_L1_error)
     }
     __pyx_v_a = (__pyx_t_5 / __pyx_t_9);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":419
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":420
  *         a = ((y3 - y1) * (x2 - x1) - (y2 - y1) * (x3 - x1)) / (
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)             # <<<<<<<<<<<<<<
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)
  */
     __pyx_t_9 = ((__pyx_v_y2 - __pyx_v_y1) - (__pyx_v_a * ((__pyx_v_x2 * __pyx_v_x2) - (__pyx_v_x1 * __pyx_v_x1))));
     __pyx_t_5 = (__pyx_v_x2 - __pyx_v_x1);
     if (unlikely(__pyx_t_5 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 419, __pyx_L1_error)
+      __PYX_ERR(0, 420, __pyx_L1_error)
     }
     __pyx_v_b = (__pyx_t_9 / __pyx_t_5);
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":420
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":421
  *                 (x3 * x3 - x1 * x1) * (x2 - x1) - (x2 * x2 - x1 * x1) * (x3 - x1))
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  *         c = y1 - (a * x1 * x1 + b * x1)             # <<<<<<<<<<<<<<
  *         curve_point = CurvePoint(a, b, c)
  *         curve.append(curve_point)
  */
     __pyx_v_c = (__pyx_v_y1 - (((__pyx_v_a * __pyx_v_x1) * __pyx_v_x1) + (__pyx_v_b * __pyx_v_x1)));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":421
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":422
  *         b = (y2 - y1 - a * (x2 * x2 - x1 * x1)) / (x2 - x1)
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)             # <<<<<<<<<<<<<<
  *         curve.append(curve_point)
  * 
  */
     __pyx_t_10.a = __pyx_v_a;
     __pyx_t_10.b = __pyx_v_b;
     __pyx_t_10.c = __pyx_v_c;
     __pyx_v_curve_point = __pyx_t_10;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":422
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":423
  *         c = y1 - (a * x1 * x1 + b * x1)
  *         curve_point = CurvePoint(a, b, c)
  *         curve.append(curve_point)             # <<<<<<<<<<<<<<
  * 
  *     num_points = len_data_points
  */
-    __pyx_t_3 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_3 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_3); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_3); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":410
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":411
  *     len_data_range = len_data_points - 1
  * 
  *     for i in range(1, len_data_range):             # <<<<<<<<<<<<<<
- *         x1 = data_points[i - 1]['Mach']
- *         x2 = data_points[i]['Mach']
+ *         x1 = data_points[i - 1].Mach
+ *         x2 = data_points[i].Mach
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":424
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":425
  *         curve.append(curve_point)
  * 
  *     num_points = len_data_points             # <<<<<<<<<<<<<<
- *     rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
+ *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
  */
   __pyx_v_num_points = __pyx_v_len_data_points;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":425
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
  * 
  *     num_points = len_data_points
- *     rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \             # <<<<<<<<<<<<<<
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)
+ *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \             # <<<<<<<<<<<<<<
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 425, __pyx_L1_error)
+    __PYX_ERR(0, 426, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 425, __pyx_L1_error)
+    __PYX_ERR(0, 426, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":427
  *     num_points = len_data_points
- *     rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])             # <<<<<<<<<<<<<<
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)
+ *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)             # <<<<<<<<<<<<<<
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)
  */
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 426, __pyx_L1_error)
+    __PYX_ERR(0, 427, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 426, __pyx_L1_error)
+    __PYX_ERR(0, 427, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_Mach); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_Mach); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Subtract(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":425
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":426
  * 
  *     num_points = len_data_points
- *     rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \             # <<<<<<<<<<<<<<
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)
+ *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \             # <<<<<<<<<<<<<<
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  */
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_rate = __pyx_t_5;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":427
- *     rate = (data_points[num_points - 1]['CD'] - data_points[num_points - 2]['CD']) / \
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)             # <<<<<<<<<<<<<<
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":428
+ *     rate = (data_points[num_points - 1].CD - data_points[num_points - 2].CD) / \
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)             # <<<<<<<<<<<<<<
  *     curve.append(curve_point)
  *     return curve
  */
   __pyx_t_10.a = 0.0;
   __pyx_t_10.b = __pyx_v_rate;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 427, __pyx_L1_error)
+    __PYX_ERR(0, 428, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 1);
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_CD); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_v_data_points == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 427, __pyx_L1_error)
+    __PYX_ERR(0, 428, __pyx_L1_error)
   }
   __pyx_t_12 = (__pyx_v_num_points - 2);
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_data_points, __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_10.c = __pyx_t_5;
   __pyx_v_curve_point = __pyx_t_10;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":428
- *            (data_points[num_points - 1]['Mach'] - data_points[num_points - 2]['Mach'])
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":429
+ *            (data_points[num_points - 1].Mach - data_points[num_points - 2].Mach)
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)             # <<<<<<<<<<<<<<
  *     return curve
  * 
  */
-  __pyx_t_1 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_v_curve_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_curve, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":429
- *     curve_point = CurvePoint(0, rate, data_points[num_points - 1]['CD'] - data_points[num_points - 2]['Mach'] * rate)
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":430
+ *     curve_point = CurvePoint(0, rate, data_points[num_points - 1].CD - data_points[num_points - 2].Mach * rate)
  *     curve.append(curve_point)
  *     return curve             # <<<<<<<<<<<<<<
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_curve);
   __pyx_r = __pyx_v_curve;
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":399
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":400
  *     return pow(bullet_weight, 2) * pow(velocity, 3) * 1.5e-12
  * 
  * cdef list calculate_curve(list data_points):             # <<<<<<<<<<<<<<
  *     cdef double rate, x1, x2, x3, y1, y2, y3, a, b, c
  *     cdef list curve = []
  */
 
@@ -11529,15 +11386,15 @@
   __Pyx_XDECREF(__pyx_v_curve);
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "py_ballisticcalc_exts/trajectory_calc.pyx":431
+/* "py_ballisticcalc_exts/trajectory_calc.pyx":432
  *     return curve
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):             # <<<<<<<<<<<<<<
  *     cdef int num_points, mlo, mhi, mid
  *     cdef CurvePoint curve_m
  */
 
@@ -11558,223 +11415,223 @@
   PyObject *__pyx_t_6 = NULL;
   struct __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_by_curve", 1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":435
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":436
  *     cdef CurvePoint curve_m
  * 
  *     num_points = int(len(curve))             # <<<<<<<<<<<<<<
  *     mlo = 0
  *     mhi = num_points - 2
  */
   if (unlikely(__pyx_v_curve == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 435, __pyx_L1_error)
+    __PYX_ERR(0, 436, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 436, __pyx_L1_error)
   __pyx_v_num_points = ((int)__pyx_t_1);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":436
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":437
  * 
  *     num_points = int(len(curve))
  *     mlo = 0             # <<<<<<<<<<<<<<
  *     mhi = num_points - 2
  * 
  */
   __pyx_v_mlo = 0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":437
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":438
  *     num_points = int(len(curve))
  *     mlo = 0
  *     mhi = num_points - 2             # <<<<<<<<<<<<<<
  * 
  *     while mhi - mlo > 1:
  */
   __pyx_v_mhi = (__pyx_v_num_points - 2);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":439
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":440
  *     mhi = num_points - 2
  * 
  *     while mhi - mlo > 1:             # <<<<<<<<<<<<<<
  *         mid = int(floor(mhi + mlo) / 2.0)
- *         if data[mid]['Mach'] < mach:
+ *         if data[mid].Mach < mach:
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_mhi - __pyx_v_mlo) > 1);
     if (!__pyx_t_2) break;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":440
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":441
  * 
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)             # <<<<<<<<<<<<<<
- *         if data[mid]['Mach'] < mach:
+ *         if data[mid].Mach < mach:
  *             mlo = mid
  */
     __pyx_v_mid = ((int)(floor((__pyx_v_mhi + __pyx_v_mlo)) / 2.0));
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":441
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)
- *         if data[mid]['Mach'] < mach:             # <<<<<<<<<<<<<<
+ *         if data[mid].Mach < mach:             # <<<<<<<<<<<<<<
  *             mlo = mid
  *         else:
  */
     if (unlikely(__pyx_v_data == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 441, __pyx_L1_error)
+      __PYX_ERR(0, 442, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mid, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mid, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (__pyx_t_2) {
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":443
  *         mid = int(floor(mhi + mlo) / 2.0)
- *         if data[mid]['Mach'] < mach:
+ *         if data[mid].Mach < mach:
  *             mlo = mid             # <<<<<<<<<<<<<<
  *         else:
  *             mhi = mid
  */
       __pyx_v_mlo = __pyx_v_mid;
 
-      /* "py_ballisticcalc_exts/trajectory_calc.pyx":441
+      /* "py_ballisticcalc_exts/trajectory_calc.pyx":442
  *     while mhi - mlo > 1:
  *         mid = int(floor(mhi + mlo) / 2.0)
- *         if data[mid]['Mach'] < mach:             # <<<<<<<<<<<<<<
+ *         if data[mid].Mach < mach:             # <<<<<<<<<<<<<<
  *             mlo = mid
  *         else:
  */
       goto __pyx_L5;
     }
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":444
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":445
  *             mlo = mid
  *         else:
  *             mhi = mid             # <<<<<<<<<<<<<<
  * 
- *     if data[mhi]['Mach'] - mach > mach - data[mlo]['Mach']:
+ *     if data[mhi].Mach - mach > mach - data[mlo].Mach:
  */
     /*else*/ {
       __pyx_v_mhi = __pyx_v_mid;
     }
     __pyx_L5:;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":446
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
  *             mhi = mid
  * 
- *     if data[mhi]['Mach'] - mach > mach - data[mlo]['Mach']:             # <<<<<<<<<<<<<<
+ *     if data[mhi].Mach - mach > mach - data[mlo].Mach:             # <<<<<<<<<<<<<<
  *         m = mlo
  *     else:
  */
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 446, __pyx_L1_error)
+    __PYX_ERR(0, 447, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mhi, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mhi, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_5, __pyx_n_u_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_Mach); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_mach); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (unlikely(__pyx_v_data == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 446, __pyx_L1_error)
+    __PYX_ERR(0, 447, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mlo, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_data, __pyx_v_mlo, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_Mach); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Subtract(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Subtract(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_6 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (__pyx_t_2) {
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":448
  * 
- *     if data[mhi]['Mach'] - mach > mach - data[mlo]['Mach']:
+ *     if data[mhi].Mach - mach > mach - data[mlo].Mach:
  *         m = mlo             # <<<<<<<<<<<<<<
  *     else:
  *         m = mhi
  */
     __pyx_v_m = __pyx_v_mlo;
 
-    /* "py_ballisticcalc_exts/trajectory_calc.pyx":446
+    /* "py_ballisticcalc_exts/trajectory_calc.pyx":447
  *             mhi = mid
  * 
- *     if data[mhi]['Mach'] - mach > mach - data[mlo]['Mach']:             # <<<<<<<<<<<<<<
+ *     if data[mhi].Mach - mach > mach - data[mlo].Mach:             # <<<<<<<<<<<<<<
  *         m = mlo
  *     else:
  */
     goto __pyx_L6;
   }
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":449
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":450
  *         m = mlo
  *     else:
  *         m = mhi             # <<<<<<<<<<<<<<
  *     curve_m = curve[m]
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)
  */
   /*else*/ {
     __pyx_v_m = __pyx_v_mhi;
   }
   __pyx_L6:;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":450
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":451
  *     else:
  *         m = mhi
  *     curve_m = curve[m]             # <<<<<<<<<<<<<<
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)
  */
   if (unlikely(__pyx_v_curve == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 450, __pyx_L1_error)
+    __PYX_ERR(0, 451, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_curve, __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_curve, __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_7 = __pyx_convert__from_py_struct____pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CurvePoint(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_curve_m = __pyx_t_7;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":451
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":452
  *         m = mhi
  *     curve_m = curve[m]
  *     return curve_m.c + mach * (curve_m.b + curve_m.a * mach)             # <<<<<<<<<<<<<<
  */
   __pyx_r = (__pyx_v_curve_m.c + (__pyx_v_mach * (__pyx_v_curve_m.b + (__pyx_v_curve_m.a * __pyx_v_mach))));
   goto __pyx_L0;
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":431
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":432
  *     return curve
  * 
  * cdef double calculate_by_curve(list data, list curve, double mach):             # <<<<<<<<<<<<<<
  *     cdef int num_points, mlo, mhi, mid
  *     cdef CurvePoint curve_m
  */
 
@@ -12812,17 +12669,16 @@
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyMethodDef __pyx_methods_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc[] = {
   {"zero_angle", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_3zero_angle, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_2zero_angle},
   {"trajectory", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_5trajectory, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_4trajectory},
-  {"_init_trajectory", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6_init_trajectory},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_10__setstate_cython__},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_6__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_8__setstate_cython__},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc},
   {Py_tp_doc, (void *)PyDoc_STR("TrajectoryCalc(ammo: Ammo)")},
   {Py_tp_traverse, (void *)__pyx_tp_traverse_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc},
@@ -13101,58 +12957,57 @@
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_Ammo, __pyx_k_Ammo, sizeof(__pyx_k_Ammo), 0, 0, 1, 1},
     {&__pyx_n_s_Angular, __pyx_k_Angular, sizeof(__pyx_k_Angular), 0, 0, 1, 1},
     {&__pyx_n_s_Atmo, __pyx_k_Atmo, sizeof(__pyx_k_Atmo), 0, 0, 1, 1},
     {&__pyx_n_s_BC, __pyx_k_BC, sizeof(__pyx_k_BC), 0, 0, 1, 1},
-    {&__pyx_n_u_CD, __pyx_k_CD, sizeof(__pyx_k_CD), 0, 1, 0, 1},
+    {&__pyx_n_s_CD, __pyx_k_CD, sizeof(__pyx_k_CD), 0, 0, 1, 1},
     {&__pyx_n_s_Distance, __pyx_k_Distance, sizeof(__pyx_k_Distance), 0, 0, 1, 1},
     {&__pyx_n_s_Energy, __pyx_k_Energy, sizeof(__pyx_k_Energy), 0, 0, 1, 1},
     {&__pyx_n_s_FPS, __pyx_k_FPS, sizeof(__pyx_k_FPS), 0, 0, 1, 1},
     {&__pyx_n_s_Fahrenheit, __pyx_k_Fahrenheit, sizeof(__pyx_k_Fahrenheit), 0, 0, 1, 1},
     {&__pyx_n_s_Foot, __pyx_k_Foot, sizeof(__pyx_k_Foot), 0, 0, 1, 1},
     {&__pyx_n_s_FootPound, __pyx_k_FootPound, sizeof(__pyx_k_FootPound), 0, 0, 1, 1},
     {&__pyx_n_s_Grain, __pyx_k_Grain, sizeof(__pyx_k_Grain), 0, 0, 1, 1},
     {&__pyx_n_s_InHg, __pyx_k_InHg, sizeof(__pyx_k_InHg), 0, 0, 1, 1},
     {&__pyx_n_s_Inch, __pyx_k_Inch, sizeof(__pyx_k_Inch), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
     {&__pyx_n_s_MAX_DISTANCE_FEET, __pyx_k_MAX_DISTANCE_FEET, sizeof(__pyx_k_MAX_DISTANCE_FEET), 0, 0, 1, 1},
-    {&__pyx_n_u_Mach, __pyx_k_Mach, sizeof(__pyx_k_Mach), 0, 1, 0, 1},
+    {&__pyx_n_s_Mach, __pyx_k_Mach, sizeof(__pyx_k_Mach), 0, 0, 1, 1},
     {&__pyx_kp_s_No_value_specified_for_struct_at, __pyx_k_No_value_specified_for_struct_at, sizeof(__pyx_k_No_value_specified_for_struct_at), 0, 0, 1, 0},
     {&__pyx_kp_s_No_value_specified_for_struct_at_2, __pyx_k_No_value_specified_for_struct_at_2, sizeof(__pyx_k_No_value_specified_for_struct_at_2), 0, 0, 1, 0},
     {&__pyx_kp_s_No_value_specified_for_struct_at_3, __pyx_k_No_value_specified_for_struct_at_3, sizeof(__pyx_k_No_value_specified_for_struct_at_3), 0, 0, 1, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_Pound, __pyx_k_Pound, sizeof(__pyx_k_Pound), 0, 0, 1, 1},
+    {&__pyx_n_s_PreferredUnits, __pyx_k_PreferredUnits, sizeof(__pyx_k_PreferredUnits), 0, 0, 1, 1},
     {&__pyx_n_s_Pressure, __pyx_k_Pressure, sizeof(__pyx_k_Pressure), 0, 0, 1, 1},
     {&__pyx_n_s_Radian, __pyx_k_Radian, sizeof(__pyx_k_Radian), 0, 0, 1, 1},
     {&__pyx_n_s_Settings, __pyx_k_Settings, sizeof(__pyx_k_Settings), 0, 0, 1, 1},
     {&__pyx_n_s_Shot, __pyx_k_Shot, sizeof(__pyx_k_Shot), 0, 0, 1, 1},
     {&__pyx_n_s_Temperature, __pyx_k_Temperature, sizeof(__pyx_k_Temperature), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryCalc, __pyx_k_TrajectoryCalc, sizeof(__pyx_k_TrajectoryCalc), 0, 0, 1, 1},
     {&__pyx_n_u_TrajectoryCalc, __pyx_k_TrajectoryCalc, sizeof(__pyx_k_TrajectoryCalc), 0, 1, 0, 1},
     {&__pyx_n_s_TrajectoryCalc___reduce_cython, __pyx_k_TrajectoryCalc___reduce_cython, sizeof(__pyx_k_TrajectoryCalc___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryCalc___setstate_cython, __pyx_k_TrajectoryCalc___setstate_cython, sizeof(__pyx_k_TrajectoryCalc___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_TrajectoryCalc__init_trajectory, __pyx_k_TrajectoryCalc__init_trajectory, sizeof(__pyx_k_TrajectoryCalc__init_trajectory), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryCalc_trajectory, __pyx_k_TrajectoryCalc_trajectory, sizeof(__pyx_k_TrajectoryCalc_trajectory), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryCalc_zero_angle, __pyx_k_TrajectoryCalc_zero_angle, sizeof(__pyx_k_TrajectoryCalc_zero_angle), 0, 0, 1, 1},
     {&__pyx_n_s_TrajectoryData, __pyx_k_TrajectoryData, sizeof(__pyx_k_TrajectoryData), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_USE_POWDER_SENSITIVITY, __pyx_k_USE_POWDER_SENSITIVITY, sizeof(__pyx_k_USE_POWDER_SENSITIVITY), 0, 0, 1, 1},
-    {&__pyx_n_s_Units, __pyx_k_Units, sizeof(__pyx_k_Units), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_Vector, __pyx_k_Vector, sizeof(__pyx_k_Vector), 0, 0, 1, 1},
     {&__pyx_n_s_Vector___reduce_cython, __pyx_k_Vector___reduce_cython, sizeof(__pyx_k_Vector___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Vector___setstate_cython, __pyx_k_Vector___setstate_cython, sizeof(__pyx_k_Vector___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Velocity, __pyx_k_Velocity, sizeof(__pyx_k_Velocity), 0, 0, 1, 1},
     {&__pyx_n_s_Weight, __pyx_k_Weight, sizeof(__pyx_k_Weight), 0, 0, 1, 1},
     {&__pyx_n_s_Wind, __pyx_k_Wind, sizeof(__pyx_k_Wind), 0, 0, 1, 1},
     {&__pyx_kp_u_Zero_vertical_error, __pyx_k_Zero_vertical_error, sizeof(__pyx_k_Zero_vertical_error), 0, 1, 0, 0},
-    {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
+    {&__pyx_n_s__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
     {&__pyx_n_s_altitude, __pyx_k_altitude, sizeof(__pyx_k_altitude), 0, 0, 1, 1},
     {&__pyx_n_s_ammo, __pyx_k_ammo, sizeof(__pyx_k_ammo), 0, 0, 1, 1},
     {&__pyx_n_s_angle, __pyx_k_angle, sizeof(__pyx_k_angle), 0, 0, 1, 1},
@@ -13187,15 +13042,14 @@
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get_density_factor_and_mach_for, __pyx_k_get_density_factor_and_mach_for, sizeof(__pyx_k_get_density_factor_and_mach_for), 0, 0, 1, 1},
     {&__pyx_n_s_get_max_calc_step_size, __pyx_k_get_max_calc_step_size, sizeof(__pyx_k_get_max_calc_step_size), 0, 0, 1, 1},
     {&__pyx_n_s_get_velocity_for_temp, __pyx_k_get_velocity_for_temp, sizeof(__pyx_k_get_velocity_for_temp), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_height, __pyx_k_height, sizeof(__pyx_k_height), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-    {&__pyx_n_s_init_trajectory, __pyx_k_init_trajectory, sizeof(__pyx_k_init_trajectory), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_kp_u_iterations, __pyx_k_iterations, sizeof(__pyx_k_iterations), 0, 1, 0, 0},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
     {&__pyx_n_s_look_angle, __pyx_k_look_angle, sizeof(__pyx_k_look_angle), 0, 0, 1, 1},
     {&__pyx_n_s_look_distance, __pyx_k_look_distance, sizeof(__pyx_k_look_distance), 0, 0, 1, 1},
     {&__pyx_n_s_mach, __pyx_k_mach, sizeof(__pyx_k_mach), 0, 0, 1, 1},
@@ -13257,15 +13111,15 @@
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 411, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 19, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 20, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
@@ -13303,22 +13157,22 @@
  *     result.c = value
  *     return result
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_3); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":218
+  /* "py_ballisticcalc_exts/trajectory_calc.pyx":219
  * 
  *         if len_winds < 1:
  *             wind_vector = Vector(.0, .0, .0)             # <<<<<<<<<<<<<<
  *         else:
  *             wind_vector = wind_to_vector(shot_info.winds[0])
  */
-  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_float__0, __pyx_float__0, __pyx_float__0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_float__0, __pyx_float__0, __pyx_float__0); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x1a1505e, 0xaee47ca, 0x4420ce0):             # <<<<<<<<<<<<<<
@@ -13384,53 +13238,41 @@
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory_2, __pyx_n_s_trajectory, 136, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 136, __pyx_L1_error)
   __pyx_tuple__17 = PyTuple_Pack(1, Py_False); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":151
- *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
- * 
- *     def _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
- *         self.look_angle = shot_info.look_angle >> Angular.Radian
- *         self.twist = shot_info.weapon.twist >> Distance.Inch
- */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_shot_info); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_py_ballisticcalc_exts_trajectory_2, __pyx_n_s_init_trajectory, 151, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 151, __pyx_L1_error)
-
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__20 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_TrajectoryCalc, (type(self), 0x1a1505e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TrajectoryCalc__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TrajectoryCalc, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TrajectoryCalc, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -13531,14 +13373,15 @@
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Vector, (PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_Vector) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   #endif
   __pyx_vtabptr_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = &__pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.get_calc_step = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, struct __pyx_opt_args_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step *__pyx_optional_args))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_get_calc_step;
+  __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._init_trajectory = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__init_trajectory;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._zero_angle = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__zero_angle;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc._trajectory = (PyObject *(*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *, double, double, enum __pyx_t_21py_ballisticcalc_exts_15trajectory_calc_CTrajFlag))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc__trajectory;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.drag_by_mach = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_drag_by_mach;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.spin_drift = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, double))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_spin_drift;
   __pyx_vtable_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc.calc_stability_coefficient = (double (*)(struct __pyx_obj_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc *, PyObject *))__pyx_f_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_calc_stability_coefficient;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc_spec, NULL); if (unlikely(!__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc)) __PYX_ERR(0, 99, __pyx_L1_error)
@@ -14105,74 +13948,56 @@
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__17);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_trajectory, __pyx_t_3) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
 
-  /* "py_ballisticcalc_exts/trajectory_calc.pyx":151
- *         return self._trajectory(shot_info, max_range >> Distance.Foot, dist_step >> Distance.Foot, filter_flags)
- * 
- *     def _init_trajectory(self, shot_info: Shot):             # <<<<<<<<<<<<<<
- *         self.look_angle = shot_info.look_angle >> Angular.Radian
- *         self.twist = shot_info.weapon.twist >> Distance.Inch
- */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shot_info, __pyx_n_s_Shot) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7_init_trajectory, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc__init_trajectory, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_init_trajectory, __pyx_t_2) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
-
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___reduce_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___reduce_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_TrajectoryCalc, (type(self), 0x1a1505e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TrajectoryCalc__set_state(self, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___setstate_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_14TrajectoryCalc_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TrajectoryCalc___setstate_cython, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_21py_ballisticcalc_exts_15trajectory_calc_TrajectoryCalc);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TrajectoryCalc(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc, 0, __pyx_n_s_pyx_unpickle_TrajectoryCalc, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TrajectoryCalc, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_21py_ballisticcalc_exts_15trajectory_calc_1__pyx_unpickle_TrajectoryCalc, 0, __pyx_n_s_pyx_unpickle_TrajectoryCalc, NULL, __pyx_n_s_py_ballisticcalc_exts_trajectory, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TrajectoryCalc, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "py_ballisticcalc_exts/trajectory_calc.pyx":1
  * from libc.math cimport sqrt, fabs, pow, sin, cos, tan, atan, log10, floor             # <<<<<<<<<<<<<<
  * cimport cython
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -19587,15 +19412,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__25);
+        name = __Pyx_NewRef(__pyx_n_s__23);
     }
     return name;
 }
 #endif
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `py_ballisticcalc.exts-2.0.0b2/pyproject.toml` & `py_ballisticcalc.exts-2.0.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 requires = ["setuptools", "wheel", 'cython']
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "py_ballisticcalc.exts"
-version = "2.0.0b2"
+version = "2.0.0b3"
 
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
     { name="dbookstaber", email="bookstaber@gmail.com"}
 ]
 description = "LGPL library for small arms ballistic calculations (Python 3)"
 readme = "README.md"
```

### Comparing `py_ballisticcalc.exts-2.0.0b2/setup.py` & `py_ballisticcalc.exts-2.0.0b3/setup.py`

 * *Files identical despite different names*

