# Comparing `tmp/metro_db-0.3.0.tar.gz` & `tmp/metro_db-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metro_db-0.3.0.tar", last modified: Tue Feb 13 02:10:35 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `metro_db-0.3.0.tar` & `metro_db-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,47 @@
-drwxrwxr-x   0 dlu       (1000) dlu       (1000)        0 2024-02-13 02:10:35.248692 metro_db-0.3.0/
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     1521 2022-10-14 19:30:18.000000 metro_db-0.3.0/LICENSE
--rw-r--r--   0 dlu       (1000) dlu       (1000)      577 2024-02-13 02:10:35.248692 metro_db-0.3.0/PKG-INFO
--rw-rw-r--   0 dlu       (1000) dlu       (1000)      629 2024-02-13 02:07:11.000000 metro_db-0.3.0/README.md
-drwxrwxr-x   0 dlu       (1000) dlu       (1000)        0 2024-02-13 02:10:35.248692 metro_db-0.3.0/metro_db/
--rw-rw-r--   0 dlu       (1000) dlu       (1000)      152 2024-02-13 02:09:49.000000 metro_db-0.3.0/metro_db/__init__.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)    10175 2023-09-22 19:40:08.000000 metro_db-0.3.0/metro_db/_queries.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     2620 2023-09-22 19:40:08.000000 metro_db-0.3.0/metro_db/metro_db.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     1503 2022-10-24 18:49:56.000000 metro_db-0.3.0/metro_db/peek.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)    11759 2023-09-22 19:40:08.000000 metro_db-0.3.0/metro_db/sqlite_db.py
-drwxrwxr-x   0 dlu       (1000) dlu       (1000)        0 2024-02-13 02:10:35.248692 metro_db-0.3.0/metro_db.egg-info/
--rw-r--r--   0 dlu       (1000) dlu       (1000)      577 2024-02-13 02:10:34.000000 metro_db-0.3.0/metro_db.egg-info/PKG-INFO
--rw-rw-r--   0 dlu       (1000) dlu       (1000)      430 2024-02-13 02:10:35.000000 metro_db-0.3.0/metro_db.egg-info/SOURCES.txt
--rw-rw-r--   0 dlu       (1000) dlu       (1000)        1 2024-02-13 02:10:34.000000 metro_db-0.3.0/metro_db.egg-info/dependency_links.txt
--rw-rw-r--   0 dlu       (1000) dlu       (1000)       48 2024-02-13 02:10:34.000000 metro_db-0.3.0/metro_db.egg-info/entry_points.txt
--rw-rw-r--   0 dlu       (1000) dlu       (1000)       47 2024-02-13 02:10:34.000000 metro_db-0.3.0/metro_db.egg-info/requires.txt
--rw-rw-r--   0 dlu       (1000) dlu       (1000)       15 2024-02-13 02:10:34.000000 metro_db-0.3.0/metro_db.egg-info/top_level.txt
--rw-rw-r--   0 dlu       (1000) dlu       (1000)       70 2024-02-13 02:10:35.248692 metro_db-0.3.0/setup.cfg
--rw-rw-r--   0 dlu       (1000) dlu       (1000)      809 2024-02-13 02:09:49.000000 metro_db-0.3.0/setup.py
-drwxrwxr-x   0 dlu       (1000) dlu       (1000)        0 2024-02-13 02:10:35.248692 metro_db-0.3.0/tests/
--rw-rw-r--   0 dlu       (1000) dlu       (1000)        0 2022-10-18 01:28:49.000000 metro_db-0.3.0/tests/__init__.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     9169 2023-09-22 19:40:08.000000 metro_db-0.3.0/tests/test_core.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     1210 2022-12-10 19:13:21.000000 metro_db-0.3.0/tests/test_metro.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     1224 2022-12-10 19:13:21.000000 metro_db-0.3.0/tests/test_peek.py
--rw-rw-r--   0 dlu       (1000) dlu       (1000)     9148 2023-09-22 19:40:08.000000 metro_db-0.3.0/tests/test_queries.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 metro_db-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 metro_db-0.4.0/.git_archival.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 metro_db-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 metro_db-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 metro_db-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 metro_db-0.4.0/.yamllint.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 metro_db-0.4.0/setup.cfg
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 metro_db-0.4.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 metro_db-0.4.0/.github/workflows/publish_pip.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/api.rst
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/db_structure.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/error.rst
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/metro_db.rst
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/overview.md
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/queries.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/sqlite_db.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/tutorials.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/types.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/uri_tricks.md
+-rw-r--r--   0        0        0    47996 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/_static/logo.png
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 metro_db-0.4.0/docs/source/_static/metro.css
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/__init__.py
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/_queries.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/_version.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/metro_db.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/peek.py
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/sqlite_db.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 metro_db-0.4.0/src/metro_db/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/metro.yaml
+-rw-r--r--   0        0        0     9948 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/test_core.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/test_flex_iter.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/test_metro.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/test_peek.py
+-rw-r--r--   0        0        0    11781 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/test_queries.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/out/basic_n1.txt
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 metro_db-0.4.0/tests/out/basic_out.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 metro_db-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metro_db-0.4.0/LICENSE
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 metro_db-0.4.0/README.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 metro_db-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 metro_db-0.4.0/PKG-INFO
```

### Comparing `metro_db-0.3.0/LICENSE` & `metro_db-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metro_db-0.3.0/README.md` & `metro_db-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 
 ## Installation
 [![PyPI version](https://badge.fury.io/py/metro_db.svg)](https://badge.fury.io/py/metro_db)
 
     sudo pip3 install metro_db
 
 ## Documentation
-[![readthedocs badget](https://readthedocs.org/projects/metro_db/badge/?version=latest)](http://metro-db.readthedocs.org/)
+[![readthedocs badge](https://readthedocs.org/projects/metro_db/badge/?version=latest)](http://metro-db.readthedocs.org/)
 
 [`http://metro-db.readthedocs.org/`](http://metro-db.readthedocs.org/)
 
 ## Continuous Integration
 [![Build Status](https://app.travis-ci.com/DLu/metro_db.svg?branch=main)](https://app.travis-ci.com/DLu/metro_db)
```

### Comparing `metro_db-0.3.0/metro_db/_queries.py` & `metro_db-0.4.0/src/metro_db/_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from .types import FlexibleIterator
+
+
 def format_value(self, field, value):
     """If the field's type is text, surround with quotes.
 
     Args:
         field (str): Name of the field
         value: The value to format
 
@@ -65,16 +68,15 @@
 
     Returns:
         iterator: All the values that match the query
     """
     field_s = field if not distinct else f'DISTINCT {field}'
     if not isinstance(clause, str):
         clause = self.generate_clause(clause)
-    for row in self.query(f'SELECT {field_s} FROM {table} {clause}'):
-        yield row[0]
+    return FlexibleIterator(row[0] for row in self.query(f'SELECT {field_s} FROM {table} {clause}'))
 
 
 def lookup(self, field, table, clause=''):
     """Run a SELECT command and return the first (only?) value.
 
     Args:
         field (str): Name of field to return
```

### Comparing `metro_db-0.3.0/metro_db/metro_db.py` & `metro_db-0.4.0/src/metro_db/metro_db.py`

 * *Files identical despite different names*

### Comparing `metro_db-0.3.0/metro_db/peek.py` & `metro_db-0.4.0/src/metro_db/peek.py`

 * *Files identical despite different names*

### Comparing `metro_db-0.3.0/metro_db/sqlite_db.py` & `metro_db-0.4.0/src/metro_db/sqlite_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,16 @@
 import sqlite3
 
-
-class DatabaseError(sqlite3.Error):
-    def __init__(self, error_s, command, parameters=None):
-        s = f'{error_s}\nCommand: {command}'
-        if parameters:
-            s += f'\n\t{parameters}'
-        sqlite3.Error.__init__(self, s)
-        self.command = command
-        self.parameters = parameters
-
-
-class Row(sqlite3.Row):
-    def __repr__(self):
-        return str(dict(self))
-
+from .types import DatabaseError, Row, FlexibleIterator
 
 PYTHON_SQL_TYPE_TRANSLATION = {
     'int': 'INTEGER',
     'float': 'REAL',
     'str': 'TEXT',
+    'datetime': 'TIMESTAMP',
 }
 
 
 class SQLiteDB:
     """Core database structure that handles base sqlite3 interactions"""
 
     def __init__(self, database_path, default_type='str', primary_keys=['id'], uri_query=None):
@@ -107,15 +94,15 @@
             query (str): SQL query to execute
 
         Returns:
             Iterator(Row): The results of the query
         """
         try:
             cursor = self.raw_db.cursor()
-            yield from cursor.execute(query)
+            return FlexibleIterator(cursor.execute(query))
         except (sqlite3.Error, ValueError) as e:
             raise DatabaseError(str(e), query) from None
 
     def execute(self, command, params=()):
         """Execute the given command with the parameters. Returns the cursor
 
         Args:
```

### Comparing `metro_db-0.3.0/tests/test_core.py` & `metro_db-0.4.0/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,44 @@
     row = basic_db.query_one('SELECT * FROM people')
     assert row['name'] == '1'
     assert row['age'] == 1
     assert row['grade'] == 1    # 1 == 1.0
     assert isinstance(row['grade'], float)
     assert row['present'] is True
 
-    # Check string representation of row
+    # Check string representation of Row
     assert str(row) == "{'name': '1', 'age': 1, 'grade': 1.0, 'present': True}"
 
+    # Check iteration
+    assert len(row) == 4
+
+    for k, v in row.items():
+        assert k in ['name', 'age', 'grade', 'present']
+        assert v
+
+    # Check the get method
+    row = basic_db.query_one('SELECT name, grade, present FROM people')
+    assert row.get('name') == '1'
+    assert row.get('age') is None
+    assert row.get('grade') == 1
+    assert row.get('present') is True
+
+    WACKY_VALUE = 'fhqwhgads'
+    assert row.get('name', WACKY_VALUE) == '1'
+    assert row.get('age', WACKY_VALUE) == WACKY_VALUE
+    assert row.get('grade', WACKY_VALUE) == 1
+    assert row.get('present', WACKY_VALUE) is True
+
+    # Check contains method
+    assert 'name' in row
+    assert not ('age' in row)
+    assert 'age' not in row
+    assert 'grade' in row
+    assert 'present' in row
+
     # Check repr
     assert str(basic_db) == 'people(1)\n'
 
 
 def test_insertion_problem(basic_db):
     basic_db.update_database_structure()
     command = 'INSERT INTO people (name, age, grade, present) VALUES(?, ?, ?)'  # Missing ?
@@ -70,15 +97,15 @@
 
     assert 'syntax error' in str(e.value)
     assert command == e.value.command
     assert command in str(e.value)
     assert e.value.parameters is None
 
     with pytest.raises(DatabaseError) as e:
-        list(basic_db.query(command))
+        basic_db.query(command)
 
     assert 'syntax error' in str(e.value)
     assert command == e.value.command
     assert command in str(e.value)
     assert e.value.parameters is None
```

### Comparing `metro_db-0.3.0/tests/test_metro.py` & `metro_db-0.4.0/tests/test_metro.py`

 * *Files identical despite different names*

### Comparing `metro_db-0.3.0/tests/test_peek.py` & `metro_db-0.4.0/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `metro_db-0.3.0/tests/test_queries.py` & `metro_db-0.4.0/tests/test_queries.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,21 +36,67 @@
     ]:
         db.execute('INSERT INTO batters (name, year, hits, position) VALUES(?, ?, ?, ?)', values)
 
     yield db
     db.dispose()
 
 
+def test_query(demo_db):
+    results = demo_db.query('SELECT * FROM batters')
+    c = 0
+    names = set()
+    for row in results:
+        c += 1
+        names.add(row['name'])
+    assert c == 9
+    assert len(names) == 4
+
+
+def test_query_as_list(demo_db):
+    results = demo_db.query('SELECT * FROM batters ORDER BY -hits')
+    assert len(results) == 9
+
+    assert results[0]['name'] == 'Olerud'
+
+
 def test_lookup_all(demo_db):
+    # Explicitly convert results to list
+    # Test from before FlexibleIterator was implemented
+    values = list(demo_db.lookup_all('name', 'batters', {'year': 1998}))
+    assert str(values) == str(['Olerud', 'Piazza', 'Alfonzo'])
+
     values = list(demo_db.lookup_all('name', 'batters', {'year': 1999}))
     assert len(values) == 3
     assert 'Olerud' in values
     assert 'Piazza' in values
     assert 'Alfonzo' in values
 
+    values = list(demo_db.lookup_all('name', 'batters', {'year': 2000}))
+    assert 'Zeile' in values
+    assert 'Piazza' in values
+    assert 'Alfonzo' in values
+    assert len(values) == 3
+
+
+def test_lookup_all_without_cast(demo_db):
+    values = demo_db.lookup_all('name', 'batters', {'year': 1998})
+    assert str(values) == str(['Olerud', 'Piazza', 'Alfonzo'])
+
+    values = demo_db.lookup_all('name', 'batters', {'year': 1999})
+    assert len(values) == 3
+    assert 'Olerud' in values
+    assert 'Piazza' in values
+    assert 'Alfonzo' in values
+
+    values = demo_db.lookup_all('name', 'batters', {'year': 2000})
+    assert 'Zeile' in values
+    assert 'Piazza' in values
+    assert 'Alfonzo' in values
+    assert len(values) == 3
+
 
 def test_lookup(demo_db):
     assert demo_db.lookup('hits', 'batters', {'year': 1999, 'name': 'Alfonzo'}) == 191
 
     # Contrived examples to test quote handling
     assert demo_db.lookup('hits', 'batters', {'year': 1999, 'name': 'O\'Brien'}) is None
     assert demo_db.lookup('hits', 'batters', {'year': 1999, 'name': '"O\'Brien"'}) is None
@@ -210,15 +256,15 @@
     db = SQLiteDB(path)
     db.tables = {
         'great_moments': ['id', 'name', 'date'],
         'better_moments': ['id', 'name', 'datetime'],
     }
     db.field_types['id'] = 'int'
     db.field_types['date'] = 'date'
-    db.field_types['datetime'] = 'timestamp'
+    db.field_types['datetime'] = 'datetime'
     db.update_database_structure()
 
     yield db
     db.dispose()
 
 
 def test_date_handling(date_db):
@@ -258,7 +304,36 @@
 
     # Check clause generation
     event_name = date_db.lookup('name', 'better_moments', {'datetime': datetime.datetime(1986, 10, 25, 20, 30)})
     assert event_name == '1986 Game 6'
 
     count = date_db.count('better_moments', clause='WHERE datetime > "1984-01-01"')
     assert count == 2
+
+
+def test_date_handling_with_old_field_type():
+    # Note: For backwards compatibility, we ensure that declaring the fieldtype "timestamp" still works
+    path = pathlib.Path('old_history.db')
+    date_db = SQLiteDB(path)
+    date_db.tables = {
+        'better_moments': ['id', 'name', 'datetime'],
+    }
+    date_db.field_types['id'] = 'int'
+    date_db.field_types['date'] = 'date'
+    date_db.field_types['datetime'] = 'timestamp'
+    date_db.update_database_structure()
+
+    date_db.insert('better_moments', {'name': '2015 Game 1', 'datetime': datetime.datetime(2015, 10, 27, 20, 7)})
+    date_db.insert('better_moments', {'name': '1986 Game 6', 'datetime': datetime.datetime(1986, 10, 25, 20, 30)})
+    date_db.insert('better_moments', {'name': '1969 Game 5', 'datetime': datetime.datetime(1969, 10, 16)})
+
+    # Check output type
+    assert isinstance(date_db.lookup('datetime', 'better_moments', {'name': '2015 Game 1'}), datetime.datetime)
+
+    # Check clause generation
+    event_name = date_db.lookup('name', 'better_moments', {'datetime': datetime.datetime(1986, 10, 25, 20, 30)})
+    assert event_name == '1986 Game 6'
+
+    count = date_db.count('better_moments', clause='WHERE datetime > "1984-01-01"')
+    assert count == 2
+
+    date_db.dispose()
```

