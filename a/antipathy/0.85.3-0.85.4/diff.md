# Comparing `tmp/antipathy-0.85.3.tar.gz` & `tmp/antipathy-0.85.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antipathy-0.85.3.tar", last modified: Tue Feb 21 00:53:30 2023, max compression
+gzip compressed data, was "antipathy-0.85.4.tar", last modified: Thu Apr  4 20:19:12 2024, max compression
```

## Comparing `antipathy-0.85.3.tar` & `antipathy-0.85.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2023-02-21 00:53:30.569940 antipathy-0.85.3/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2261 2023-02-21 00:53:30.569940 antipathy-0.85.3/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1271 2023-02-21 00:53:25.000000 antipathy-0.85.3/README
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2023-02-21 00:53:30.569940 antipathy-0.85.3/antipathy/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2600 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/CHANGES
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1359 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/LICENSE
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     1271 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/README
--rw-rw-r--   0 ethan     (1000) ethan     (1000)      206 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/__init__.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)    50460 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/path.py
--rw-rw-r--   0 ethan     (1000) ethan     (1000)    83722 2023-02-21 00:53:25.000000 antipathy-0.85.3/antipathy/test.py
-drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2023-02-21 00:53:30.569940 antipathy-0.85.3/antipathy.egg-info/
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2261 2023-02-21 00:53:30.000000 antipathy-0.85.3/antipathy.egg-info/PKG-INFO
--rw-rw-r--   0 ethan     (1000) ethan     (1000)      258 2023-02-21 00:53:30.000000 antipathy-0.85.3/antipathy.egg-info/SOURCES.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2023-02-21 00:53:30.000000 antipathy-0.85.3/antipathy.egg-info/dependency_links.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       10 2023-02-21 00:53:30.000000 antipathy-0.85.3/antipathy.egg-info/top_level.txt
--rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2023-02-21 00:53:30.569940 antipathy-0.85.3/setup.cfg
--rw-rw-r--   0 ethan     (1000) ethan     (1000)     2700 2023-02-21 00:53:25.000000 antipathy-0.85.3/setup.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-04 20:19:12.882306 antipathy-0.85.4/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2312 2024-04-04 20:19:12.882306 antipathy-0.85.4/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1271 2024-04-04 20:19:06.000000 antipathy-0.85.4/README
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-04 20:19:12.882306 antipathy-0.85.4/antipathy/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2810 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/CHANGES
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1359 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/LICENSE
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     1271 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/README
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)      206 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/__init__.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)    50534 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/path.py
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)    84251 2024-04-04 20:19:06.000000 antipathy-0.85.4/antipathy/test.py
+drwxrwxr-x   0 ethan     (1000) ethan     (1000)        0 2024-04-04 20:19:12.882306 antipathy-0.85.4/antipathy.egg-info/
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2312 2024-04-04 20:19:12.000000 antipathy-0.85.4/antipathy.egg-info/PKG-INFO
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)      258 2024-04-04 20:19:12.000000 antipathy-0.85.4/antipathy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)        1 2024-04-04 20:19:12.000000 antipathy-0.85.4/antipathy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       10 2024-04-04 20:19:12.000000 antipathy-0.85.4/antipathy.egg-info/top_level.txt
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)       38 2024-04-04 20:19:12.882306 antipathy-0.85.4/setup.cfg
+-rw-rw-r--   0 ethan     (1000) ethan     (1000)     2754 2024-04-04 20:19:06.000000 antipathy-0.85.4/setup.py
```

### Comparing `antipathy-0.85.3/PKG-INFO` & `antipathy-0.85.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antipathy
-Version: 0.85.3
+Version: 0.85.4
 Summary: oo view of file paths and names, subclassed from bytes/str/unicode
 Home-page: https://github.com/ethanfurman/antipathy
 Author: Ethan Furman
 Author-email: ethan@stoneleaf.us
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 
 Antipathy -- for those tired of ``os.path``
 ===========================================
 
 Tired of calling a function for every path manipulation you need to do?
 
 Is::
```

### Comparing `antipathy-0.85.3/README` & `antipathy-0.85.4/README`

 * *Files identical despite different names*

### Comparing `antipathy-0.85.3/antipathy/CHANGES` & `antipathy-0.85.4/antipathy/CHANGES`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+0.85.4
+======
+
+strip leading slash after path subtraction, unless subtracting an
+empty string
+
+
+0.85.3
+======
+
+do not start relative paths at root
+
+
+0.85.2
+======
+
+update copytree() for later python versions
+
+
 0.85.0
 ======
 
 stop suppressing trailing slash
 
 BACKWARDS INCOMPATIBLE CHANGE
 -----------------------------
```

### Comparing `antipathy-0.85.3/antipathy/LICENSE` & `antipathy-0.85.4/antipathy/LICENSE`

 * *Files identical despite different names*

### Comparing `antipathy-0.85.3/antipathy/README` & `antipathy-0.85.4/antipathy/README`

 * *Files identical despite different names*

### Comparing `antipathy-0.85.3/antipathy/path.py` & `antipathy-0.85.4/antipathy/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,15 +692,18 @@
             return NotImplemented
         elif isinstance(other, self.data_types):
             other = Path(other)
         s = self._value_
         o = other._value_
         if not s.startswith(o):
             raise ValueError("cannot subtract %r from %r" % (other, self))
-        return Path(s[len(o):])
+        res = Path(s[len(o):])
+        if o:
+            res = res.lstrip(self._SLASH)
+        return res
 
     def access(self, file_name, mode=None):
         if mode is None:
             mode = file_name
             file_name = self
         else:
             file_name = self/file_name
```

### Comparing `antipathy-0.85.3/antipathy/test.py` & `antipathy-0.85.4/antipathy/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         regex = getattr(self, 'assertRaisesRegex', None)
         if regex is None:
             self.assertRaisesRegex = getattr(self, 'assertRaisesRegexp')
         super(TestCase, self).__init__(*args, **kwds)
 
 
 class TestPathBasics(TestCase):
-
+    # expected, vol, dirs, filename, base, ext
     test_paths = (
         ("/temp/place/somefile.abc.xyz",
             '/temp/place/somefile.abc.xyz', '', '/temp/place', 'somefile.abc.xyz', 'somefile.abc', '.xyz'),
         ("/temp/place/somefile.abc.",
             '/temp/place/somefile.abc.', '', '/temp/place', 'somefile.abc.', 'somefile.abc', '.'),
         ("/temp/place/somefile.abc",
             '/temp/place/somefile.abc', '', '/temp/place', 'somefile.abc', 'somefile', '.abc'),
@@ -79,14 +79,15 @@
             '../', '', '..', '', '', ''),
         ("./huh",
             './huh', '', '.', 'huh', 'huh', ''),
         ("../huh",
             '../huh', '', '..', 'huh', 'huh', ''),
         )
 
+    # expected, vol, dirs, filename, base, ext
     test_posix_paths = (
         ("c:\\temp\\place\\somefile.abc.xyz",
             'c:\\temp\\place\\somefile.abc.xyz', '', '', 'c:\\temp\\place\\somefile.abc.xyz', 'c:\\temp\\place\\somefile.abc', '.xyz'),
         ("c:\\temp\\place\\somefile.abc.",
             'c:\\temp\\place\\somefile.abc.', '', '', 'c:\\temp\\place\\somefile.abc.', 'c:\\temp\\place\\somefile.abc', '.'),
         ("c:\\temp\\place\\somefile.abc",
             'c:\\temp\\place\\somefile.abc', '', '', 'c:\\temp\\place\\somefile.abc', 'c:\\temp\\place\\somefile', '.abc'),
@@ -176,14 +177,15 @@
             'c:temp/place/', '', 'c:temp/place', '', '', ''),
         ("c:.xyz",
             'c:.xyz', '', '', 'c:.xyz', 'c:', '.xyz'),
         ("c:temp/.xyz",
             'c:temp/.xyz', '', 'c:temp', '.xyz', '', '.xyz'),
         )
 
+    # expected, vol, dirs, filename, base, ext
     test_win_paths = (
         ("c:\\temp\\place\\somefile.abc.xyz",
             'c:/temp/place/somefile.abc.xyz', 'c:', '/temp/place', 'somefile.abc.xyz', 'somefile.abc', '.xyz'),
         ("c:\\temp\\place\\somefile.abc.",
             'c:/temp/place/somefile.abc.', 'c:', '/temp/place', 'somefile.abc.', 'somefile.abc', '.'),
         ("c:\\temp\\place\\somefile.abc",
             'c:/temp/place/somefile.abc', 'c:', '/temp/place', 'somefile.abc', 'somefile', '.abc'),
@@ -513,34 +515,37 @@
             self.assertEqual(b_huh._ext, b_ext, i)
 
     def test_subtraction(self):
         "check path subtraction"
         self.assertEqual(Path('/temp') - Path('/temp'), Path(''))
         self.assertEqual(Path('/temp/backups') - Path(''), Path('/temp/backups'))
         self.assertEqual(Path('/temp/backups') - Path('/'), Path('temp/backups'))
-        self.assertEqual(Path('/temp/backups') - Path('/temp'), Path('/backups'))
+        self.assertEqual(Path('/temp/backups') - Path('/temp'), Path('backups'))
         self.assertEqual(Path('/temp/backups') - Path('/temp/'), Path('backups'))
         self.assertEqual(Path('/temp/backups') - Path('/temp/backups'), Path(''))
         self.assertEqual(Path('/temp/destination.txt') - Path(''), Path('/temp/destination.txt'))
-        self.assertEqual(Path('/temp/destination.txt') - Path('/temp'), Path('/destination.txt'))
+        self.assertEqual(Path('/temp/destination.txt') - Path('/temp'), Path('destination.txt'))
         self.assertEqual(Path('/temp/destination.txt') - Path('/temp/'), Path('destination.txt'))
         self.assertEqual(Path('/temp/destination.txt') - Path('/temp/destination'), Path('.txt'))
+        self.assertEqual(Path('//machine/share/some/path/and/file.txt') - Path('//machine/share'), Path('some/path/and/file.txt'))
+        self.assertEqual(Path('//machine/share/some/path/and/file.txt') - Path('//machine/share/'), Path('some/path/and/file.txt'))
+        self.assertEqual(Path('//machine/share/some/path/and/file.txt') - Path('//machine/share/some/path'), Path('and/file.txt'))
         self.assertEqual(Path('//machine/share/some/path/and/file.txt') - Path('//machine/share/some/path/'), Path('and/file.txt'))
-        self.assertEqual(Path('/usr/local/bin') - Path(''), Path('/usr/local/bin'))
         self.assertEqual(Path('//machine/share/some/path/and/file.txt') - Path(''), Path('//machine/share/some/path/and/file.txt'))
+        self.assertEqual(Path('/usr/local/bin') - Path(''), Path('/usr/local/bin'))
 
     if os.path.__name__ == 'ntpath':
         def test_win_subtraction(self):
             "check path subtraction"
             self.assertEqual(Path('c:/temp') - Path('c:/temp'), Path(''))
-            self.assertEqual(Path('c:/temp') - Path('c:'), Path('/temp'))
+            self.assertEqual(Path('c:/temp') - Path('c:'), Path('temp'))
             self.assertEqual(Path('c:/temp') - Path('c:/'), Path('temp'))
-            self.assertEqual(Path('c:/temp/backups') - Path('c:'), Path('/temp/backups'))
+            self.assertEqual(Path('c:/temp/backups') - Path('c:'), Path('temp/backups'))
             self.assertEqual(Path('c:/temp/backups') - Path('c:/'), Path('temp/backups'))
-            self.assertEqual(Path('c:/temp/backups') - Path('c:/temp'), Path('/backups'))
+            self.assertEqual(Path('c:/temp/backups') - Path('c:/temp'), Path('backups'))
             self.assertEqual(Path('c:/temp/backups') - Path('c:/temp/'), Path('backups'))
             self.assertEqual(Path('c:/temp/backups') - Path('c:/temp/backups'), Path(''))
             self.assertEqual(Path('c:/temp/destination.txt') - Path(''), Path('c:/temp/destination.txt'))
 
     if py_ver < (3, 0):
         def test_marshall(self):
             from xmlrpclib import dumps, loads
```

### Comparing `antipathy-0.85.3/antipathy.egg-info/PKG-INFO` & `antipathy-0.85.4/antipathy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antipathy
-Version: 0.85.3
+Version: 0.85.4
 Summary: oo view of file paths and names, subclassed from bytes/str/unicode
 Home-page: https://github.com/ethanfurman/antipathy
 Author: Ethan Furman
 Author-email: ethan@stoneleaf.us
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 
 Antipathy -- for those tired of ``os.path``
 ===========================================
 
 Tired of calling a function for every path manipulation you need to do?
 
 Is::
```

### Comparing `antipathy-0.85.3/setup.py` & `antipathy-0.85.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 py2_only = ()
 py3_only = ()
 make = []
 
 data = dict(
        name='antipathy',
-       version='0.85.3',
+       version='0.85.4',
        license='BSD License',
        description='oo view of file paths and names, subclassed from bytes/str/unicode',
        long_description=long_desc,
        url='https://github.com/ethanfurman/antipathy',
        packages=['antipathy'],
        package_data={'antipathy':['LICENSE', 'README', 'CHANGES']},
        author='Ethan Furman',
@@ -71,12 +71,13 @@
             'Programming Language :: Python :: 3.5',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
             ],
             )
 
 if __name__ == '__main__':
     setup(**data)
```

