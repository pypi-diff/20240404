# Comparing `tmp/Pegamoid-2.8.4.tar.gz` & `tmp/Pegamoid-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pegamoid-2.8.4.tar", last modified: Fri Oct 13 11:28:20 2023, max compression
+gzip compressed data, was "Pegamoid-2.9.tar", last modified: Fri Nov 24 08:29:53 2023, max compression
```

## Comparing `Pegamoid-2.8.4.tar` & `Pegamoid-2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-10-13 11:28:20.676066 Pegamoid-2.8.4/
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)    35059 2019-10-28 09:04:52.000000 Pegamoid-2.8.4/LICENSE
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8549 2023-10-13 11:28:20.676066 Pegamoid-2.8.4/PKG-INFO
-drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-10-13 11:28:20.676066 Pegamoid-2.8.4/Pegamoid.egg-info/
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8549 2023-10-13 11:28:20.000000 Pegamoid-2.8.4/Pegamoid.egg-info/PKG-INFO
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)      197 2023-10-13 11:28:20.000000 Pegamoid-2.8.4/Pegamoid.egg-info/SOURCES.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-10-13 11:28:20.000000 Pegamoid-2.8.4/Pegamoid.egg-info/dependency_links.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       76 2023-10-13 11:28:20.000000 Pegamoid-2.8.4/Pegamoid.egg-info/requires.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-10-13 11:28:20.000000 Pegamoid-2.8.4/Pegamoid.egg-info/top_level.txt
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8423 2020-09-15 10:56:55.000000 Pegamoid-2.8.4/README.md
--rwxrwxr-x   0 ignacio   (1001) ignacio   (1001)   300858 2023-10-13 11:25:06.000000 Pegamoid-2.8.4/pegamoid.py
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       38 2023-10-13 11:28:20.676066 Pegamoid-2.8.4/setup.cfg
--rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     1095 2023-10-13 11:28:05.000000 Pegamoid-2.8.4/setup.py
+drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-11-24 08:29:53.058321 Pegamoid-2.9/
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)    35059 2019-10-28 09:04:52.000000 Pegamoid-2.9/LICENSE
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-11-24 08:29:53.058321 Pegamoid-2.9/PKG-INFO
+drwxrwxr-x   0 ignacio   (1001) ignacio   (1001)        0 2023-11-24 08:29:53.058321 Pegamoid-2.9/Pegamoid.egg-info/
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8547 2023-11-24 08:29:52.000000 Pegamoid-2.9/Pegamoid.egg-info/PKG-INFO
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)      197 2023-11-24 08:29:52.000000 Pegamoid-2.9/Pegamoid.egg-info/SOURCES.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-11-24 08:29:52.000000 Pegamoid-2.9/Pegamoid.egg-info/dependency_links.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       76 2023-11-24 08:29:52.000000 Pegamoid-2.9/Pegamoid.egg-info/requires.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)        1 2023-11-24 08:29:52.000000 Pegamoid-2.9/Pegamoid.egg-info/top_level.txt
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     8423 2020-09-15 10:56:55.000000 Pegamoid-2.9/README.md
+-rwxrwxr-x   0 ignacio   (1001) ignacio   (1001)   301100 2023-11-20 13:44:33.000000 Pegamoid-2.9/pegamoid.py
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)       38 2023-11-24 08:29:53.058321 Pegamoid-2.9/setup.cfg
+-rw-rw-r--   0 ignacio   (1001) ignacio   (1001)     1093 2023-11-20 13:44:20.000000 Pegamoid-2.9/setup.py
```

### Comparing `Pegamoid-2.8.4/LICENSE` & `Pegamoid-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Pegamoid-2.8.4/PKG-INFO` & `Pegamoid-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pegamoid
-Version: 2.8.4
+Version: 2.9
 Summary: Orbital viewer for OpenMolcas
 Home-page: https://gitlab.com/Jellby/Pegamoid
 Author: Ignacio Fdez. Galván
 Author-email: jellby@yahoo.com
 License: GPL v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Pegamoid-2.8.4/Pegamoid.egg-info/PKG-INFO` & `Pegamoid-2.9/Pegamoid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pegamoid
-Version: 2.8.4
+Version: 2.9
 Summary: Orbital viewer for OpenMolcas
 Home-page: https://gitlab.com/Jellby/Pegamoid
 Author: Ignacio Fdez. Galván
 Author-email: jellby@yahoo.com
 License: GPL v3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Pegamoid-2.8.4/README.md` & `Pegamoid-2.9/README.md`

 * *Files identical despite different names*

### Comparing `Pegamoid-2.8.4/pegamoid.py` & `Pegamoid-2.9/pegamoid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import division, absolute_import, print_function
 from builtins import bytes, dict, int, range, super
 
 __name__ = 'Pegamoid'
 __author__ = u'Ignacio Fdez. Galván'
 __copyright__ = u'Copyright © 2018–2020,2022–2023'
 __license__ = 'GPL v3.0'
-__version__ = '2.8.4'
+__version__ = '2.9'
 
 import sys
 try:
   from qtpy.QtCore import Qt, QObject, QThread, QEvent, QSettings
   from qtpy.QtWidgets import *
   from qtpy.QtGui import QPixmap, QIcon, QKeySequence, QColor, QPalette, QScreen, QCursor
   import qtpy
@@ -2317,14 +2317,21 @@
 # Pad a list with additional item up to a minimum length
 def list_pad(a, n, item=None):
   if (len(a) < n):
     a.extend([item] * (n-len(a)))
 
 #===============================================================================
 
+# Snap occupation numbers close to an integer (for sorting purposes)
+def snap(x):
+  f, _ = np.modf(x)
+  return x if np.abs(f) > 1e-6 else np.rint(x)
+
+#===============================================================================
+
 # Convert a Fortran-formatted number to float
 # replace d/D with e, add e if missing
 fortfixexp = re.compile(r'([\d.])[dD]?(((?<=[dD])[+-]?|[+-])\d)')
 def fortran_float(num):
   try:
     num = str(num.decode('ascii'))
   except AttributeError:
@@ -2539,15 +2546,15 @@
                    <p><b>{3}</b>: Show this window</p>
                    <p><b>Ctrl+_</b>: Collapse/expand options panel</p>
                    <p><b>PgUp</b>/<b>PgDown</b>: Switch to previous/next orbital</p>
                    <p><b>Alt+PgUp</b>/<b>Alt+PgDown</b>: Switch to previous/next density type</p>
                    <p><b>Shift+PgUp</b>/<b>Shift+PgDown</b>: Switch to previous/next root</p>
                    <p><b>Ctrl+PgUp</b>/<b>Ctrl+PgDown</b>: Switch to previous/next irrep</p>
                    <p><b>A</b>/<b>B</b>/<b>E</b>: Switch to alpha/hole, beta/particle or natural orbitals, respectively</p>
-                   <p><b>Shift+S</b>: Toggle sorting of orbital list by energy &amp; occupation</p>
+                   <p><b>Shift+S</b>: Toggle sorting of orbital list by occupation &amp; energy</p>
                    <p><b>Ctrl+L</b>: Show/hide full list of orbitals</p>
                    <p><b>F</b>: Change orbital type to frozen</p>
                    <p><b>I</b>: Change orbital type to inactive</p>
                    <p><b>1</b>: Change orbital type to RAS1 (active)</p>
                    <p><b>2</b>: Change orbital type to RAS2 (active)</p>
                    <p><b>3</b>: Change orbital type to RAS3 (active)</p>
                    <p><b>S</b>: Change orbital type to secondary</p>
@@ -3242,16 +3249,16 @@
     self.rootButton.setWhatsThis('Select a root to compute the natural active orbitals for, if the file contains root-specific density matrices.<br>Keys: <b>Shift+PgUp</b>, <b>Shift+PgDown</b>')
     self.irrepButton.setToolTip('Select irrep for the orbital list')
     self.irrepButton.setWhatsThis('This list shows the irreps available in the file, by name or number. Selecting one irrep restricts the orbitals available in the button on the right to the selected irrep. Select "All" for no restriction.<br>Keys: <b>Ctrl+PgUp</b>, <b>Ctrl+PgDown</b>')
     self.orbitalButton.setToolTip('Select orbital to display')
     self.orbitalButton.setWhatsThis('This shows all the orbitals available in the file, belonging to the selected irrep and spin if applicable. If no irrep is selected ("All") and if the file is not a precomputed grid, the electron density, the spin density and the Laplacian of the electron density may also be available. Selecting an orbital displays it in the 3D view above.<br>Keys: <b>PgUp</b>, <b>PgDown</b>')
     self.spinButton.setToolTip('Select spin for the orbital list')
     self.spinButton.setWhatsThis('Select alpha or beta orbitals. This list is only visible if the file contains spin-orbitals.<br>Keys: <b>A</b>, <b>B</b>')
-    self.sortedBox.setToolTip('Sort orbitals by energy & occupation')
-    self.sortedBox.setWhatsThis('Sort the list of orbitals according to the energy and occupation values. The index still refers to the original order.<br>Key: <b>Shift+S</b>')
+    self.sortedBox.setToolTip('Sort orbitals by occupation & energy')
+    self.sortedBox.setWhatsThis('Sort the list of orbitals according to the occupation and energy values. The index still refers to the original order.<br>Key: <b>Shift+S</b>')
     self.listButton.setToolTip('Show/hide full list of orbitals')
     self.listButton.setWhatsThis('Open or close a window showing the list of all orbitals (no restrictions), where custom notes can be added.<br>Key: <b>Shift+L</b>')
     activeFrame.setWhatsThis('RAS1, RAS2 and RAS3 orbitals count as "active"')
     self.frozenButton.setToolTip('Set orbital as frozen')
     self.frozenButton.setWhatsThis('Set the type of the current orbital to "Frozen". This type will be saved in HDF5 or InpOrb files.<br>Key: <b>F</b>')
     self.inactiveButton.setToolTip('Set orbital as inactive')
     self.inactiveButton.setWhatsThis('Set the type of the current orbital to "Inactive". This type will be saved in HDF5 or InpOrb files.<br>Key: <b>I</b>')
@@ -4691,15 +4698,15 @@
     prev = self.orbital
     self.orbitalButton.blockSignals(True)
     self.orbitalButton.clear()
     if (self.MO is None):
       return
     if (self.irrep == 'All'):
       orblist = {i+1:self.orb_to_list(i+1, o) for i,o in enumerate(self.MO) if (not o.get('hide'))}
-      orbidx = {i+1:[-np.inf if np.isnan(o['ene']) else o['ene'], np.copysign(1, o['occup']), -o['occup']]
+      orbidx = {i+1:[-snap(o['occup']), -np.inf if np.isnan(o['ene']) else o['ene'], np.copysign(1, o['occup'])]
                      for i,o in enumerate(self.MO) if (not o.get('hide'))}
       if ((not self.isGrid) and any([(o['occup'] != 0.0) for o in self.MO])):
         is_it_spin = (self.dens == 'State') and any([(o['occup'] < -1e-4) for o in self.MO])
         if (self.dens == 'State'):
           if (not is_it_spin):
             orblist[0] = 'Density'
             orblist[-2] = 'Laplacian (numerical)'
@@ -4718,15 +4725,15 @@
           elif (self.spin == 'particle'):
             orblist[-4] = 'Particle density'
           orblist[-6] = 'Transition density'
         elif ((self.dens == 'WFA') and ('_NO' in self.rootButton.currentText())):
           orblist[0] = 'Density'
     else:
       orblist = {i+1:self.orb_to_list(i+1, o) for i,o in enumerate(self.MO) if ((o['sym'] == self.irrep) and not o.get('hide'))}
-      orbidx = {i+1:[-np.inf if np.isnan(o['ene']) else o['ene'], np.copysign(1, o['occup']), -o['occup'], o['sym']]
+      orbidx = {i+1:[-snap(o['occup']), -np.inf if np.isnan(o['ene']) else o['ene'], np.copysign(1, o['occup']), o['sym']]
                      for i,o in enumerate(self.MO) if ((o['sym'] == self.irrep) and not o.get('hide'))}
     if (self.sortedBox.isChecked()):
       for k in orblist.keys():
         if (not k in orbidx):
           orbidx[k] = [-np.inf, k]
       orbsort = sorted(orbidx.keys(), key=lambda k: orbidx[k])
     else:
```

### Comparing `Pegamoid-2.8.4/setup.py` & `Pegamoid-2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 
 with open("README.md", "r") as f:
     # Remove screenshots
     long_description = re.sub('Screenshots\n-*\n*(<.*> *\n*)*', '', f.read())
 
 setup(name='Pegamoid',
-      version='2.8.4',
+      version='2.9',
       description='Orbital viewer for OpenMolcas',
       author=u'Ignacio Fdez. Galván',
       author_email='jellby@yahoo.com',
       url='https://gitlab.com/Jellby/Pegamoid',
       license='GPL v3.0',
       scripts=['pegamoid.py'],
       install_requires=['numpy (>=1.9.0)', 'h5py', 'VTK (>=8.1.0)', 'qtpy', 'future (>=0.15.2);python_version<"3.0"' ],
```

