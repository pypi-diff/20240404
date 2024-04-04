# Comparing `tmp/rewire-sqlmodel-0.0.4.tar.gz` & `tmp/rewire-sqlmodel-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewire-sqlmodel-0.0.4.tar", last modified: Wed Feb 14 09:07:25 2024, max compression
+gzip compressed data, was "rewire-sqlmodel-0.0.5.tar", last modified: Thu Apr  4 20:12:02 2024, max compression
```

## Comparing `rewire-sqlmodel-0.0.4.tar` & `rewire-sqlmodel-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.134908 rewire-sqlmodel-0.0.4/
--rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2131 2024-02-14 09:07:25.133856 rewire-sqlmodel-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.4/README.md
--rw-rw-rw-   0        0        0      812 2024-02-14 09:07:17.000000 rewire-sqlmodel-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.114277 rewire-sqlmodel-0.0.4/rewire_sqlmodel/
--rw-rw-rw-   0        0        0    14961 2024-02-04 09:00:22.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.130856 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/
--rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_merge_dev.py
--rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_migrations.py
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.131856 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_template/
--rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_template/env.py
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.131856 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_template/versions/
--rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
--rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/fastapi.py
--rw-rw-rw-   0        0        0     2485 2024-02-04 08:52:32.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel/tests.py
-drwxrwxrwx   0        0        0        0 2024-02-14 09:07:25.132856 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/
--rw-rw-rw-   0        0        0     2131 2024-02-14 09:07:25.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-02-14 09:07:25.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 09:07:25.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-02-14 09:07:25.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-14 09:07:25.000000 rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-14 09:07:25.134908 rewire-sqlmodel-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2131 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-04 08:31:32.000000 rewire-sqlmodel-0.0.5/README.md
+-rw-rw-rw-   0        0        0      812 2024-04-04 20:11:07.000000 rewire-sqlmodel-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.110632 rewire-sqlmodel-0.0.5/rewire_sqlmodel/
+-rw-rw-rw-   0        0        0    14947 2024-04-04 20:10:45.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.127170 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/
+-rw-rw-rw-   0        0        0     3802 2024-02-12 12:25:01.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_merge_dev.py
+-rw-rw-rw-   0        0        0    22087 2024-02-04 08:49:15.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_migrations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.127170 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/
+-rw-rw-rw-   0        0        0     1990 2024-02-04 08:49:16.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/env.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.128675 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/versions/
+-rw-rw-rw-   0        0        0      446 2024-01-26 19:57:16.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/versions/root_initial.py
+-rw-rw-rw-   0        0        0     1016 2024-02-14 09:07:05.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/fastapi.py
+-rw-rw-rw-   0        0        0     2485 2024-02-04 08:52:32.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:12:02.129682 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/
+-rw-rw-rw-   0        0        0     2131 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 20:12:02.000000 rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 20:12:02.130680 rewire-sqlmodel-0.0.5/setup.cfg
```

### Comparing `rewire-sqlmodel-0.0.4/LICENSE` & `rewire-sqlmodel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/PKG-INFO` & `rewire-sqlmodel-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rewire-sqlmodel-0.0.4/pyproject.toml` & `rewire-sqlmodel-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rewire-sqlmodel"
-version = "0.0.4"
+version = "0.0.5"
 description = "Integration of rewire and sqlmodel"
 readme = "README.md"
 authors = [{ name = "Ivan Vozhakov", email = "gou177@bk.ru" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/__init__.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         def __init__(self, type: Type = None, *args, **kwargs) -> None:
             super().__init__(*args, **kwargs)
             self._type = type
 
         def load_dialect_impl(self, dialect):
             if id(dialect) not in dialect_patched:
-                dialect._json_serializer = BaseModel.__pydantic_serializer__.to_json  # type: ignore
+                dialect._json_serializer = self.type_adapter.dump_json  # type: ignore
                 dialect_patched.add(id(dialect))
             return super().load_dialect_impl(dialect)
 
         def process_bind_param(self, value, dialect):
             if isinstance(value, BaseModel):
                 return dict(value._iter(to_dict=True))
```

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_merge_dev.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_merge_dev.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_migrations.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/alembic_template/env.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/alembic_template/env.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/ext/fastapi.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel/tests.py` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel/tests.py`

 * *Files identical despite different names*

### Comparing `rewire-sqlmodel-0.0.4/rewire_sqlmodel.egg-info/PKG-INFO` & `rewire-sqlmodel-0.0.5/rewire_sqlmodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewire-sqlmodel
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integration of rewire and sqlmodel
 Author-email: Ivan Vozhakov <gou177@bk.ru>
 License: MIT License
         
         Copyright (c) 2024 rewirepy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

