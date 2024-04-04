# Comparing `tmp/machinable-4.9.1.tar.gz` & `tmp/machinable-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinable-4.9.1.tar", max compression
+gzip compressed data, was "machinable-4.9.2.tar", max compression
```

## Comparing `machinable-4.9.1.tar` & `machinable-4.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       85 2024-03-06 02:29:43.695611 machinable-4.9.1/AUTHORS.md
--rw-r--r--   0        0        0     3532 2024-03-06 02:29:43.695611 machinable-4.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2024-03-06 02:29:43.695611 machinable-4.9.1/LICENSE.txt
--rw-r--r--   0        0        0     1135 2024-03-06 02:29:43.695611 machinable-4.9.1/README.md
--rw-r--r--   0        0        0     2159 2024-03-06 02:29:43.699611 machinable-4.9.1/pyproject.toml
--rw-r--r--   0        0        0     1029 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/__init__.py
--rw-r--r--   0        0        0     3627 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/cli.py
--rw-r--r--   0        0        0    37190 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/collection.py
--rw-r--r--   0        0        0     8698 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/component.py
--rw-r--r--   0        0        0     2479 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/config.py
--rw-r--r--   0        0        0    22279 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/element.py
--rw-r--r--   0        0        0      615 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/errors.py
--rw-r--r--   0        0        0    14379 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/execution.py
--rw-r--r--   0        0        0    11511 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/index.py
--rw-r--r--   0        0        0    20388 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/interface.py
--rw-r--r--   0        0        0     2480 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/mixin.py
--rw-r--r--   0        0        0    13264 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/project.py
--rw-r--r--   0        0        0       10 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/py.typed
--rw-r--r--   0        0        0     2558 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/query.py
--rw-r--r--   0        0        0      630 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/schedule.py
--rw-r--r--   0        0        0     1821 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/schema.py
--rw-r--r--   0        0        0      248 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/scope.py
--rw-r--r--   0        0        0     3920 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/storage.py
--rw-r--r--   0        0        0      359 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/types.py
--rw-r--r--   0        0        0    18794 2024-03-06 02:29:43.699611 machinable-4.9.1/src/machinable/utils.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 machinable-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2024-03-18 20:33:42.721075 machinable-4.9.2/AUTHORS.md
+-rw-r--r--   0        0        0     3740 2024-03-18 20:33:42.721075 machinable-4.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2024-03-18 20:33:42.721075 machinable-4.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1135 2024-03-18 20:33:42.721075 machinable-4.9.2/README.md
+-rw-r--r--   0        0        0     2159 2024-03-18 20:33:42.725075 machinable-4.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1029 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/__init__.py
+-rw-r--r--   0        0        0     3640 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/cli.py
+-rw-r--r--   0        0        0    37190 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/collection.py
+-rw-r--r--   0        0        0     8698 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/component.py
+-rw-r--r--   0        0        0     2479 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/config.py
+-rw-r--r--   0        0        0    22279 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/element.py
+-rw-r--r--   0        0        0      615 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/errors.py
+-rw-r--r--   0        0        0    14379 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/execution.py
+-rw-r--r--   0        0        0    11606 2024-03-18 20:33:42.725075 machinable-4.9.2/src/machinable/index.py
+-rw-r--r--   0        0        0    20477 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/interface.py
+-rw-r--r--   0        0        0     2480 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/mixin.py
+-rw-r--r--   0        0        0    13264 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/project.py
+-rw-r--r--   0        0        0       10 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/py.typed
+-rw-r--r--   0        0        0     2558 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/query.py
+-rw-r--r--   0        0        0      630 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/schedule.py
+-rw-r--r--   0        0        0     1821 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/schema.py
+-rw-r--r--   0        0        0      248 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/scope.py
+-rw-r--r--   0        0        0     3920 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/storage.py
+-rw-r--r--   0        0        0      359 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/types.py
+-rw-r--r--   0        0        0    18794 2024-03-18 20:33:42.729075 machinable-4.9.2/src/machinable/utils.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 machinable-4.9.2/PKG-INFO
```

### Comparing `machinable-4.9.1/CHANGELOG.md` & `machinable-4.9.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!-- Please add changes under the Unreleased section that reads 'No current changes' otherwise -->
 
+# Unreleased
+
+No current changes
+
+# v4.9.2
+
+- Always use first CLI argument as target to allow non-component targets
+- Ensure that config field is always reloaded from index to avoid incorrect recomputation
+
 # v4.9.1
 
 - Use text-based link relation by default
 
 # v4.9.0
 
 - Adds `Interface.related_iterator()`
```

### Comparing `machinable-4.9.1/LICENSE.txt` & `machinable-4.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/README.md` & `machinable-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/pyproject.toml` & `machinable-4.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "machinable"
-version = "4.9.1"
+version = "4.9.2"
 description = "A modular configuration system for research projects"
 license = "MIT"
 authors = [
     "Frithjof Gressmann <hello@machinable.org>"
 ]
 maintainers = [
     "Frithjof Gressmann <hello@machinable.org>"
```

### Comparing `machinable-4.9.1/src/machinable/__init__.py` & `machinable-4.9.2/src/machinable/__init__.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/cli.py` & `machinable-4.9.2/src/machinable/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,22 +109,23 @@
         get = machinable.get
         if action != "get":
             get = getattr(get, action.split(".")[-1])
 
         elements, methods = parse(args)
         contexts = []
         component = None
-        for module, *version in elements:
+        for i, (module, *version) in enumerate(elements):
             element = get(module, version)
-            contexts.append(element.__enter__())
-            if isinstance(element, machinable.Component):
+            if i == 0:
                 component = element
+            else:
+                contexts.append(element.__enter__())
 
         if component is None:
-            raise ValueError("You have to provide an component")
+            raise ValueError("You have to provide at least one interface")
 
         for method in methods:
             # check if cli_{method} exists before falling back on {method}
             target = getattr(
                 component, f"cli_{method}", getattr(component, method)
             )
             target()
```

### Comparing `machinable-4.9.1/src/machinable/collection.py` & `machinable-4.9.2/src/machinable/collection.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/component.py` & `machinable-4.9.2/src/machinable/component.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/config.py` & `machinable-4.9.2/src/machinable/config.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/element.py` & `machinable-4.9.2/src/machinable/element.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/errors.py` & `machinable-4.9.2/src/machinable/errors.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/execution.py` & `machinable-4.9.2/src/machinable/execution.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/index.py` & `machinable-4.9.2/src/machinable/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def interface_row_factory(cursor, row) -> schema.Interface:
     model = getattr(schema, row[1], schema.Interface)
     return model(
         uuid=row[0],
         kind=row[1],
         module=row[2],
-        config=None,
+        config=json.loads(row[3]),
         version=json.loads(row[6]),
         predicate=json.loads(row[7]),
         lineage=json.loads(row[8]),
         timestamp=int(row[9]),
         **json.loads(row[10]),
     )
 
@@ -139,18 +139,23 @@
         with db(self.config.database, create=True) as _db:
             cur = _db.cursor()
             if cur.execute(
                 """SELECT uuid FROM 'index' WHERE uuid=?""", (model.uuid,)
             ).fetchone():
                 # already exists
                 return False
-            config = copy.deepcopy(model.config or {})
-            default = config.pop("_default_", {})
-            version = config.pop("_version_", [])
-            update = config.pop("_update_", {})
+            config = copy.deepcopy(model.config)
+            if config:
+                default = config.pop("_default_", {})
+                version = config.pop("_version_", [])
+                update = config.pop("_update_", {})
+            else:
+                default = {}
+                version = []
+                update = {}
 
             cur.execute(
                 """INSERT INTO 'index' (
                     uuid,
                     kind,
                     module,
                     config,
@@ -233,15 +238,14 @@
 
     def find_by_id(self, uuid: str) -> Optional[schema.Interface]:
         with db(self.config.database, create=False) as _db:
             if not _db:
                 return None
             cur = _db.cursor()
             if len(uuid) == 6:  # short id
-                print(f"%{uuid[:2]}-{uuid[2:]}-%")
                 row = cur.execute(
                     """SELECT * FROM 'index' WHERE uuid LIKE ?""",
                     (f"%{uuid[:2]}-{uuid[2:]}-%",),
                 ).fetchone()
             else:
                 row = cur.execute(
                     """SELECT * FROM 'index' WHERE uuid=?""", (uuid,)
@@ -273,15 +277,14 @@
                     [
                         v if isinstance(v, (str, int, float)) else _jn(v)
                         for v in equals
                     ],
                 )
             else:
                 query = cur.execute("""SELECT * FROM 'index'""")
-
             return [interface_row_factory(cur, row) for row in query.fetchall()]
 
     def find_by_hash(self, context_hash: str) -> List[schema.Interface]:
         with db(self.config.database, create=False) as _db:
             if not _db:
                 return []
             cur = _db.cursor()
```

### Comparing `machinable-4.9.1/src/machinable/interface.py` & `machinable-4.9.2/src/machinable/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,17 @@
             module=self.__model__.module,
             config=self.__model__.config,
             version=self.__model__.version,
             lineage=get_lineage(self),
         )
         self.__model__._dump = get_dump(self)
 
+        self._kwargs["uses"] = uses
+        self._kwargs["derived_from"] = derived_from
+
         # initialize relation data
         self.__related__ = {}
         self._relation_cache = {}
         if self.__relations__ is None:
             self.__relations__ = {}
         # relation_names = defaultdict(lambda: 0)
         for name, relation in self.__relations__.items():
```

### Comparing `machinable-4.9.1/src/machinable/mixin.py` & `machinable-4.9.2/src/machinable/mixin.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/project.py` & `machinable-4.9.2/src/machinable/project.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/query.py` & `machinable-4.9.2/src/machinable/query.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/schedule.py` & `machinable-4.9.2/src/machinable/schedule.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/schema.py` & `machinable-4.9.2/src/machinable/schema.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/storage.py` & `machinable-4.9.2/src/machinable/storage.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/src/machinable/utils.py` & `machinable-4.9.2/src/machinable/utils.py`

 * *Files identical despite different names*

### Comparing `machinable-4.9.1/PKG-INFO` & `machinable-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinable
-Version: 4.9.1
+Version: 4.9.2
 Summary: A modular configuration system for research projects
 Home-page: https://machinable.org
 License: MIT
 Keywords: machine-learning,research
 Author: Frithjof Gressmann
 Author-email: hello@machinable.org
 Maintainer: Frithjof Gressmann
```

