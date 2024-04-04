# Comparing `tmp/path-16.8.0.tar.gz` & `tmp/path-16.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "path-16.8.0.tar", last modified: Mon Dec  4 20:03:36 2023, max compression
+gzip compressed data, was "path-16.9.0.tar", last modified: Mon Dec  4 20:29:35 2023, max compression
```

## Comparing `path-16.8.0.tar` & `path-16.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.100106 path-16.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-04 20:03:13.000000 path-16.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-04 20:03:13.000000 path-16.8.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-04 20:03:13.000000 path-16.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.092106 path-16.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-04 20:03:13.000000 path-16.8.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-04 20:03:13.000000 path-16.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.092106 path-16.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-04 20:03:13.000000 path-16.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-04 20:03:13.000000 path-16.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-04 20:03:13.000000 path-16.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-04 20:03:13.000000 path-16.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-04 20:03:13.000000 path-16.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-04 20:03:13.000000 path-16.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-04 20:03:13.000000 path-16.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2023-12-04 20:03:13.000000 path-16.8.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2023-12-04 20:03:36.100106 path-16.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-04 20:03:13.000000 path-16.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-04 20:03:13.000000 path-16.8.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.092106 path-16.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2023-12-04 20:03:13.000000 path-16.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-04 20:03:13.000000 path-16.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-04 20:03:13.000000 path-16.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-04 20:03:13.000000 path-16.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-04 20:03:13.000000 path-16.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-04 20:03:13.000000 path-16.8.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.096106 path-16.8.0/path/
--rw-r--r--   0 runner    (1001) docker     (127)    50416 2023-12-04 20:03:13.000000 path-16.8.0/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15303 2023-12-04 20:03:13.000000 path-16.8.0/path/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-04 20:03:13.000000 path-16.8.0/path/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-04 20:03:13.000000 path-16.8.0/path/classes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2023-12-04 20:03:13.000000 path-16.8.0/path/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-04 20:03:13.000000 path-16.8.0/path/masks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-04 20:03:13.000000 path-16.8.0/path/matchers.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-04 20:03:13.000000 path-16.8.0/path/matchers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:13.000000 path-16.8.0/path/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:03:36.096106 path-16.8.0/path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2023-12-04 20:03:36.000000 path-16.8.0/path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-04 20:03:36.000000 path-16.8.0/path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 20:03:36.000000 path-16.8.0/path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-04 20:03:36.000000 path-16.8.0/path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-04 20:03:36.000000 path-16.8.0/path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-04 20:03:13.000000 path-16.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-04 20:03:13.000000 path-16.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-12-04 20:03:36.100106 path-16.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    45266 2023-12-04 20:03:13.000000 path-16.8.0/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-04 20:03:13.000000 path-16.8.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-04 20:03:13.000000 path-16.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.268139 path-16.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-04 20:29:16.000000 path-16.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-04 20:29:16.000000 path-16.9.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-04 20:29:16.000000 path-16.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.260139 path-16.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-04 20:29:16.000000 path-16.9.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-04 20:29:16.000000 path-16.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.260139 path-16.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-04 20:29:16.000000 path-16.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-04 20:29:16.000000 path-16.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-04 20:29:16.000000 path-16.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-04 20:29:16.000000 path-16.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-04 20:29:16.000000 path-16.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-04 20:29:16.000000 path-16.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-04 20:29:16.000000 path-16.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15260 2023-12-04 20:29:16.000000 path-16.9.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-12-04 20:29:35.268139 path-16.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-04 20:29:16.000000 path-16.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-04 20:29:16.000000 path-16.9.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.260139 path-16.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2023-12-04 20:29:16.000000 path-16.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-04 20:29:16.000000 path-16.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-04 20:29:16.000000 path-16.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-04 20:29:16.000000 path-16.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-04 20:29:16.000000 path-16.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-04 20:29:16.000000 path-16.9.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.264139 path-16.9.0/path/
+-rw-r--r--   0 runner    (1001) docker     (127)    50640 2023-12-04 20:29:16.000000 path-16.9.0/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15303 2023-12-04 20:29:16.000000 path-16.9.0/path/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-04 20:29:16.000000 path-16.9.0/path/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-04 20:29:16.000000 path-16.9.0/path/classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2023-12-04 20:29:16.000000 path-16.9.0/path/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-04 20:29:16.000000 path-16.9.0/path/masks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-04 20:29:16.000000 path-16.9.0/path/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-04 20:29:16.000000 path-16.9.0/path/matchers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:16.000000 path-16.9.0/path/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 20:29:35.264139 path-16.9.0/path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-12-04 20:29:35.000000 path-16.9.0/path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-04 20:29:35.000000 path-16.9.0/path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 20:29:35.000000 path-16.9.0/path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-04 20:29:35.000000 path-16.9.0/path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-04 20:29:35.000000 path-16.9.0/path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-04 20:29:16.000000 path-16.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-04 20:29:16.000000 path-16.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-04 20:29:35.268139 path-16.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    45463 2023-12-04 20:29:16.000000 path-16.9.0/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-04 20:29:16.000000 path-16.9.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-04 20:29:16.000000 path-16.9.0/tox.ini
```

### Comparing `path-16.8.0/.github/workflows/main.yml` & `path-16.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `path-16.8.0/LICENSE` & `path-16.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `path-16.8.0/NEWS.rst` & `path-16.9.0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v16.9.0
+=======
+
+Features
+--------
+
+- Added Path.iterdir() and deprecated Path.listdir(). Ref #214. (#214)
+
+
 v16.8.0
 =======
 
 Features
 --------
 
 - Use '.' as the default path. (#216)
```

### Comparing `path-16.8.0/PKG-INFO` & `path-16.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: path
-Version: 16.8.0
+Version: 16.9.0
 Summary: A module wrapper for os.path
 Home-page: https://github.com/jaraco/path
 Author: Jason Orendorff
 Author-email: jason.orendorff@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff; extra == "testing"
 Requires-Dist: appdirs; extra == "testing"
 Requires-Dist: packaging; extra == "testing"
 Requires-Dist: pywin32; (platform_system == "Windows" and python_version < "3.12") and extra == "testing"
+Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: pygments; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
```

### Comparing `path-16.8.0/README.rst` & `path-16.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `path-16.8.0/docs/Makefile` & `path-16.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `path-16.8.0/docs/conf.py` & `path-16.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `path-16.8.0/path/__init__.py` & `path-16.9.0/path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,51 +471,59 @@
             relpath = os.curdir
         else:
             relpath = self.module.join(*segments)
         return self._next_class(relpath)
 
     # --- Listing, searching, walking, and matching
 
-    def listdir(self, match=None):
-        """List of items in this directory.
+    def iterdir(self, match=None):
+        """Yields items in this directory.
 
         Use :meth:`files` or :meth:`dirs` instead if you want a listing
         of just files or just subdirectories.
 
         The elements of the list are Path objects.
 
         With the optional `match` argument, a callable,
         only return items whose names match the given pattern.
 
         .. seealso:: :meth:`files`, :meth:`dirs`
         """
         match = matchers.load(match)
-        return list(filter(match, (self / child for child in os.listdir(self))))
+        return filter(match, (self / child for child in os.listdir(self)))
+
+    def listdir(self, match=None):
+        warnings.warn(
+            ".listdir is deprecated; use iterdir",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return list(self.iterdir(match=match))
 
     def dirs(self, *args, **kwargs):
         """List of this directory's subdirectories.
 
         The elements of the list are Path objects.
         This does not walk recursively into subdirectories
         (but see :meth:`walkdirs`).
 
-        Accepts parameters to :meth:`listdir`.
+        Accepts parameters to :meth:`iterdir`.
         """
-        return [p for p in self.listdir(*args, **kwargs) if p.isdir()]
+        return [p for p in self.iterdir(*args, **kwargs) if p.isdir()]
 
     def files(self, *args, **kwargs):
         """List of the files in self.
 
         The elements of the list are Path objects.
         This does not walk into subdirectories (see :meth:`walkfiles`).
 
-        Accepts parameters to :meth:`listdir`.
+        Accepts parameters to :meth:`iterdir`.
         """
 
-        return [p for p in self.listdir(*args, **kwargs) if p.isfile()]
+        return [p for p in self.iterdir(*args, **kwargs) if p.isfile()]
 
     def walk(self, match=None, errors='strict'):
         """Iterator over files and subdirs, recursively.
 
         The iterator yields Path objects naming each child item of
         this directory and its descendants.  This requires that
         ``D.isdir()``.
@@ -530,15 +538,15 @@
         `errors` may also be an arbitrary callable taking a msg parameter.
         """
 
         errors = Handlers._resolve(errors)
         match = matchers.load(match)
 
         try:
-            childList = self.listdir()
+            childList = self.iterdir()
         except Exception as exc:
             errors(f"Unable to list directory '{self}': {exc}")
             return
 
         for child in childList:
             traverse = None
             if match(child):
@@ -1332,15 +1340,15 @@
         wrapped in ``only_newer``. For example::
 
             src.merge_tree(dst, copy_function=only_newer(shutil.copy2))
         """
         dst = self._next_class(dst)
         dst.makedirs_p()
 
-        sources = self.listdir()
+        sources = list(self.iterdir())
         _ignored = ignore(self, [item.name for item in sources])
 
         def ignored(item):
             return item.name in _ignored
 
         for source in itertools.filterfalse(ignored, sources):
             dest = dst / source.name
```

### Comparing `path-16.8.0/path/__init__.pyi` & `path-16.9.0/path/__init__.pyi`

 * *Files identical despite different names*

### Comparing `path-16.8.0/path/classes.py` & `path-16.9.0/path/classes.py`

 * *Files identical despite different names*

### Comparing `path-16.8.0/path/masks.py` & `path-16.9.0/path/masks.py`

 * *Files identical despite different names*

### Comparing `path-16.8.0/path/matchers.py` & `path-16.9.0/path/matchers.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         pattern = self.get_pattern(normcase)
         return fnmatch.fnmatchcase(normcase(path.name), pattern)
 
 
 class CaseInsensitive(Pattern):
     """
     A Pattern with a ``'normcase'`` property, suitable for passing to
-    :meth:`listdir`, :meth:`dirs`, :meth:`files`, :meth:`walk`,
+    :meth:`iterdir`, :meth:`dirs`, :meth:`files`, :meth:`walk`,
     :meth:`walkdirs`, or :meth:`walkfiles` to match case-insensitive.
 
     For example, to get all files ending in .py, .Py, .pY, or .PY in the
     current directory::
 
         from path import Path, matchers
         Path('.').files(matchers.CaseInsensitive('*.py'))
```

### Comparing `path-16.8.0/path/matchers.pyi` & `path-16.9.0/path/matchers.pyi`

 * *Files identical despite different names*

### Comparing `path-16.8.0/path.egg-info/PKG-INFO` & `path-16.9.0/path.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: path
-Version: 16.8.0
+Version: 16.9.0
 Summary: A module wrapper for os.path
 Home-page: https://github.com/jaraco/path
 Author: Jason Orendorff
 Author-email: jason.orendorff@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff; extra == "testing"
 Requires-Dist: appdirs; extra == "testing"
 Requires-Dist: packaging; extra == "testing"
 Requires-Dist: pywin32; (platform_system == "Windows" and python_version < "3.12") and extra == "testing"
+Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: pygments; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
```

### Comparing `path-16.8.0/path.egg-info/SOURCES.txt` & `path-16.9.0/path.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `path-16.8.0/pytest.ini` & `path-16.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `path-16.8.0/setup.cfg` & `path-16.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 	python_implementation != "PyPy"
 	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	appdirs
 	packaging
 	pywin32; platform_system == "Windows" and python_version < "3.12"
+	more_itertools
 	
 	pygments
 docs = 
 	sphinx >= 3.5
 	sphinx < 7.2.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
```

### Comparing `path-16.8.0/test_path.py` & `path-16.9.0/test_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import datetime
 import subprocess
 import re
 import contextlib
 import stat
 
 import pytest
+from more_itertools import ilen
 
 import path
 from path import Path
 from path import TempDir
 from path import matchers
 from path import SpecialResolver
 from path import Multi
@@ -508,24 +509,24 @@
                     or
                     # ctime is approximately the mtime
                     ct2 == pytest.approx(f.mtime, 0.001)
                 )
 
     def test_listing(self, tmpdir):
         d = Path(tmpdir)
-        assert d.listdir() == []
+        assert list(d.iterdir()) == []
 
         f = 'testfile.txt'
         af = d / f
         assert af == os.path.join(d, f)
         af.touch()
         try:
             assert af.exists()
 
-            assert d.listdir() == [af]
+            assert list(d.iterdir()) == [af]
 
             # .glob()
             assert d.glob('testfile.txt') == [af]
             assert d.glob('test*.txt') == [af]
             assert d.glob('*.txt') == [af]
             assert d.glob('*txt') == [af]
             assert d.glob('*') == [af]
@@ -541,15 +542,15 @@
 
         # Try a test with 20 files
         files = [d / ('%d.txt' % i) for i in range(20)]
         for f in files:
             with open(f, 'w', encoding='utf-8') as fobj:
                 fobj.write('some text\n')
         try:
-            files2 = d.listdir()
+            files2 = list(d.iterdir())
             files.sort()
             files2.sort()
             assert files == files2
         finally:
             for f in files:
                 with contextlib.suppress(Exception):
                     f.remove()
@@ -561,25 +562,25 @@
         try:
             with open(os.path.join(base, name), 'wb'):
                 pass
         except Exception as exc:
             raise pytest.skip(f"Invalid encodings disallowed {exc}")
         return name
 
-    def test_listdir_other_encoding(self, tmpdir, bytes_filename):  # pragma: nocover
+    def test_iterdir_other_encoding(self, tmpdir, bytes_filename):  # pragma: nocover
         """
         Some filesystems allow non-character sequences in path names.
-        ``.listdir`` should still function in this case.
+        ``.iterdir`` should still function in this case.
         See issue #61 for details.
         """
         # first demonstrate that os.listdir works
         assert os.listdir(str(tmpdir).encode('ascii'))
 
         # now try with path
-        results = Path(tmpdir).listdir()
+        results = Path(tmpdir).iterdir()
         (res,) = results
         assert isinstance(res, Path)
         assert len(res.basename()) == len(bytes_filename)
 
     def test_makedirs(self, tmpdir):
         d = Path(tmpdir)
 
@@ -659,38 +660,38 @@
         # Make a link for the next test to use.
         testFile.symlink(testLink)
 
         # Test copying directory tree.
         testA.copytree(testC)
         assert testC.isdir()
         self.assertSetsEqual(
-            testC.listdir(),
+            testC.iterdir(),
             [testC / testCopy.name, testC / testFile.name, testCopyOfLink],
         )
         assert not testCopyOfLink.islink()
 
         # Clean up for another try.
         testC.rmtree()
         assert not testC.exists()
 
         # Copy again, preserving symlinks.
         testA.copytree(testC, True)
         assert testC.isdir()
         self.assertSetsEqual(
-            testC.listdir(),
+            testC.iterdir(),
             [testC / testCopy.name, testC / testFile.name, testCopyOfLink],
         )
         if hasattr(os, 'symlink'):
             assert testCopyOfLink.islink()
             assert testCopyOfLink.realpath() == testFile
 
         # Clean up.
         testDir.rmtree()
         assert not testDir.exists()
-        self.assertList(d.listdir(), [])
+        self.assertList(d.iterdir(), [])
 
     def assertList(self, listing, expected):
         assert sorted(listing) == sorted(expected)
 
     def test_patterns(self, tmpdir):
         d = Path(tmpdir)
         names = ['x.tmp', 'x.xtmp', 'x2g', 'x22', 'x.txt']
@@ -698,15 +699,15 @@
 
         for e in dirs:
             if not e.isdir():
                 e.makedirs()
 
             for name in names:
                 (e / name).touch()
-        self.assertList(d.listdir('*.tmp'), [d / 'x.tmp', d / 'xdir.tmp'])
+        self.assertList(d.iterdir('*.tmp'), [d / 'x.tmp', d / 'xdir.tmp'])
         self.assertList(d.files('*.tmp'), [d / 'x.tmp'])
         self.assertList(d.dirs('*.tmp'), [d / 'xdir.tmp'])
         self.assertList(
             d.walk(), [e for e in dirs if e != d] + [e / n for e in dirs for n in names]
         )
         self.assertList(d.walk('*.tmp'), [e / 'x.tmp' for e in dirs] + [d / 'xdir.tmp'])
         self.assertList(d.walkfiles('*.tmp'), [e / 'x.tmp' for e in dirs])
@@ -918,25 +919,25 @@
     def test_with_nonexisting_dst_kwargs(self):
         self.subdir_a.merge_tree(self.subdir_b, symlinks=True)
         assert self.subdir_b.isdir()
         expected = {
             self.subdir_b / self.test_file.name,
             self.subdir_b / self.test_link.name,
         }
-        assert set(self.subdir_b.listdir()) == expected
+        assert set(self.subdir_b.iterdir()) == expected
         self.check_link()
 
     def test_with_nonexisting_dst_args(self):
         self.subdir_a.merge_tree(self.subdir_b, True)
         assert self.subdir_b.isdir()
         expected = {
             self.subdir_b / self.test_file.name,
             self.subdir_b / self.test_link.name,
         }
-        assert set(self.subdir_b.listdir()) == expected
+        assert set(self.subdir_b.iterdir()) == expected
         self.check_link()
 
     def test_with_existing_dst(self):
         self.subdir_b.rmtree()
         self.subdir_a.copytree(self.subdir_b, True)
 
         self.test_link.remove()
@@ -949,27 +950,27 @@
 
         assert self.subdir_b.isdir()
         expected = {
             self.subdir_b / self.test_file.name,
             self.subdir_b / self.test_link.name,
             self.subdir_b / test_new.name,
         }
-        assert set(self.subdir_b.listdir()) == expected
+        assert set(self.subdir_b.iterdir()) == expected
         self.check_link()
         assert len(Path(self.subdir_b / self.test_file.name).bytes()) == 5000
 
     def test_copytree_parameters(self):
         """
         merge_tree should accept parameters to copytree, such as 'ignore'
         """
         ignore = shutil.ignore_patterns('testlink*')
         self.subdir_a.merge_tree(self.subdir_b, ignore=ignore)
 
         assert self.subdir_b.isdir()
-        assert self.subdir_b.listdir() == [self.subdir_b / self.test_file.name]
+        assert list(self.subdir_b.iterdir()) == [self.subdir_b / self.test_file.name]
 
     def test_only_newer(self):
         """
         merge_tree should accept a copy_function in which only
         newer files are copied and older files do not overwrite
         newer copies in the dest.
         """
@@ -981,14 +982,18 @@
         assert target.read_text(encoding='utf-8') == 'this is newer'
 
     def test_nested(self):
         self.subdir_a.joinpath('subsub').mkdir()
         self.subdir_a.merge_tree(self.subdir_b)
         assert self.subdir_b.joinpath('subsub').isdir()
 
+    def test_listdir(self):
+        with pytest.deprecated_call():
+            Path().listdir()
+
 
 class TestChdir:
     def test_chdir_or_cd(self, tmpdir):
         """tests the chdir or cd method"""
         d = Path(str(tmpdir))
         cwd = d.getcwd()
 
@@ -1107,55 +1112,55 @@
         def normcase(path):
             return path.upper()
 
         p = Path('FooBar')
         assert p.fnmatch('foobar', normcase=normcase)
         assert p.fnmatch('FOO[ABC]AR', normcase=normcase)
 
-    def test_listdir_simple(self):
+    def test_iterdir_simple(self):
         p = Path('.')
-        assert len(p.listdir()) == len(os.listdir('.'))
+        assert ilen(p.iterdir()) == len(os.listdir('.'))
 
-    def test_listdir_empty_pattern(self):
+    def test_iterdir_empty_pattern(self):
         p = Path('.')
-        assert p.listdir('') == []
+        assert list(p.iterdir('')) == []
 
-    def test_listdir_patterns(self, tmpdir):
+    def test_iterdir_patterns(self, tmpdir):
         p = Path(tmpdir)
         (p / 'sub').mkdir()
         (p / 'File').touch()
-        assert p.listdir('s*') == [p / 'sub']
-        assert len(p.listdir('*')) == 2
+        assert list(p.iterdir('s*')) == [p / 'sub']
+        assert ilen(p.iterdir('*')) == 2
 
-    def test_listdir_custom_module(self, tmpdir):
+    def test_iterdir_custom_module(self, tmpdir):
         """
         Listdir patterns should honor the case sensitivity of the path module
         used by that Path class.
         """
         always_unix = Path.using_module(posixpath)
         p = always_unix(tmpdir)
         (p / 'sub').mkdir()
         (p / 'File').touch()
-        assert p.listdir('S*') == []
+        assert list(p.iterdir('S*')) == []
 
         always_win = Path.using_module(ntpath)
         p = always_win(tmpdir)
-        assert p.listdir('S*') == [p / 'sub']
-        assert p.listdir('f*') == [p / 'File']
+        assert list(p.iterdir('S*')) == [p / 'sub']
+        assert list(p.iterdir('f*')) == [p / 'File']
 
-    def test_listdir_case_insensitive(self, tmpdir):
+    def test_iterdir_case_insensitive(self, tmpdir):
         """
         Listdir patterns should honor the case sensitivity of the path module
         used by that Path class.
         """
         p = Path(tmpdir)
         (p / 'sub').mkdir()
         (p / 'File').touch()
-        assert p.listdir(matchers.CaseInsensitive('S*')) == [p / 'sub']
-        assert p.listdir(matchers.CaseInsensitive('f*')) == [p / 'File']
+        assert list(p.iterdir(matchers.CaseInsensitive('S*'))) == [p / 'sub']
+        assert list(p.iterdir(matchers.CaseInsensitive('f*'))) == [p / 'File']
         assert p.files(matchers.CaseInsensitive('S*')) == []
         assert p.dirs(matchers.CaseInsensitive('f*')) == []
 
     def test_walk_case_insensitive(self, tmpdir):
         p = Path(tmpdir)
         (p / 'sub1' / 'foo').makedirs_p()
         (p / 'sub2' / 'foo').makedirs_p()
```

### Comparing `path-16.8.0/tox.ini` & `path-16.9.0/tox.ini`

 * *Files identical despite different names*

