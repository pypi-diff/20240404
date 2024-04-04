# Comparing `tmp/mo-sqlite-2.579.24081.tar.gz` & `tmp/mo-sqlite-2.582.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-sqlite-2.579.24081.tar", last modified: Thu Mar 21 02:50:33 2024, max compression
+gzip compressed data, was "mo-sqlite-2.582.24095.tar", last modified: Thu Apr  4 04:18:29 2024, max compression
```

## Comparing `mo-sqlite-2.579.24081.tar` & `mo-sqlite-2.582.24095.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 02:50:33.377534 mo-sqlite-2.579.24081/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo-sqlite-2.579.24081/LICENSE
--rw-rw-rw-   0        0        0     3462 2024-03-21 02:50:33.375918 mo-sqlite-2.579.24081/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2024-03-10 19:35:09.000000 mo-sqlite-2.579.24081/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 02:50:33.328162 mo-sqlite-2.579.24081/mo_sqlite/
--rw-rw-rw-   0        0        0      507 2024-02-27 03:34:35.000000 mo-sqlite-2.579.24081/mo_sqlite/__init__.py
--rw-rw-rw-   0        0        0    19263 2024-02-27 03:34:35.000000 mo-sqlite-2.579.24081/mo_sqlite/database.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:50:33.371640 mo-sqlite-2.579.24081/mo_sqlite/expressions/
--rw-rw-rw-   0        0        0     1580 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/_utils.py
--rw-rw-rw-   0        0        0      585 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_add_op.py
--rw-rw-rw-   0        0        0      691 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_alias_op.py
--rw-rw-rw-   0        0        0     2991 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_and_op.py
--rw-rw-rw-   0        0        0     3244 2024-03-21 02:50:25.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_case_op.py
--rw-rw-rw-   0        0        0      672 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_cast_op.py
--rw-rw-rw-   0        0        0     1034 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_coalesce_op.py
--rw-rw-rw-   0        0        0      575 2024-03-10 19:35:09.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_concat_op.py
--rw-rw-rw-   0        0        0      497 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_eq_op.py
--rw-rw-rw-   0        0        0      446 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0      497 2024-02-15 03:48:30.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_gt_op.py
--rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_gte_op.py
--rw-rw-rw-   0        0        0      502 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_in_op.py
--rw-rw-rw-   0        0        0      681 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_inner_join_op.py
--rw-rw-rw-   0        0        0     1183 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_instr_op.py
--rw-rw-rw-   0        0        0      552 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_is_null_op.py
--rw-rw-rw-   0        0        0      378 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_limit_op.py
--rw-rw-rw-   0        0        0      725 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_literal.py
--rw-rw-rw-   0        0        0      617 2024-02-15 03:48:30.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_lt_op.py
--rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_lte_op.py
--rw-rw-rw-   0        0        0      570 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_not_op.py
--rw-rw-rw-   0        0        0     1713 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_or_op.py
--rw-rw-rw-   0        0        0      991 2024-03-10 20:49:59.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_order_by_op.py
--rw-rw-rw-   0        0        0     4839 2024-03-21 02:50:25.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_script.py
--rw-rw-rw-   0        0        0     2585 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0     1160 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_substr_op.py
--rw-rw-rw-   0        0        0      769 2024-03-11 06:29:29.000000 mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_variable.py
--rw-rw-rw-   0        0        0     6684 2024-02-15 03:48:30.000000 mo-sqlite-2.579.24081/mo_sqlite/sql_script.py
--rw-rw-rw-   0        0        0     6210 2024-03-18 02:53:29.000000 mo-sqlite-2.579.24081/mo_sqlite/transacfion.py
--rw-rw-rw-   0        0        0     1543 2024-01-28 17:16:21.000000 mo-sqlite-2.579.24081/mo_sqlite/types.py
--rw-rw-rw-   0        0        0     5687 2024-03-20 02:25:01.000000 mo-sqlite-2.579.24081/mo_sqlite/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:50:33.374574 mo-sqlite-2.579.24081/mo_sqlite.egg-info/
--rw-rw-rw-   0        0        0     3462 2024-03-21 02:50:33.000000 mo-sqlite-2.579.24081/mo_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1364 2024-03-21 02:50:33.000000 mo-sqlite-2.579.24081/mo_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 02:50:33.000000 mo-sqlite-2.579.24081/mo_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      341 2024-03-21 02:50:33.000000 mo-sqlite-2.579.24081/mo_sqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 02:50:33.000000 mo-sqlite-2.579.24081/mo_sqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 02:50:33.377534 mo-sqlite-2.579.24081/setup.cfg
--rw-rw-rw-   0        0        0     3333 2024-03-21 02:50:28.000000 mo-sqlite-2.579.24081/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:18:29.845609 mo-sqlite-2.582.24095/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo-sqlite-2.582.24095/LICENSE
+-rw-rw-rw-   0        0        0     3462 2024-04-04 04:18:29.845609 mo-sqlite-2.582.24095/PKG-INFO
+-rw-rw-rw-   0        0        0     1913 2024-03-10 19:35:09.000000 mo-sqlite-2.582.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 04:18:29.792431 mo-sqlite-2.582.24095/mo_sqlite/
+-rw-rw-rw-   0        0        0      507 2024-02-27 03:34:35.000000 mo-sqlite-2.582.24095/mo_sqlite/__init__.py
+-rw-rw-rw-   0        0        0    16964 2024-04-04 04:18:21.000000 mo-sqlite-2.582.24095/mo_sqlite/database.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:18:29.842099 mo-sqlite-2.582.24095/mo_sqlite/expressions/
+-rw-rw-rw-   0        0        0     1580 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/_utils.py
+-rw-rw-rw-   0        0        0      585 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_add_op.py
+-rw-rw-rw-   0        0        0      691 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_alias_op.py
+-rw-rw-rw-   0        0        0     2991 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_and_op.py
+-rw-rw-rw-   0        0        0     3244 2024-03-21 02:50:25.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_case_op.py
+-rw-rw-rw-   0        0        0      672 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_cast_op.py
+-rw-rw-rw-   0        0        0     1034 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_coalesce_op.py
+-rw-rw-rw-   0        0        0      575 2024-03-10 19:35:09.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_concat_op.py
+-rw-rw-rw-   0        0        0      497 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_eq_op.py
+-rw-rw-rw-   0        0        0      446 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0      497 2024-02-15 03:48:30.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_gt_op.py
+-rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_gte_op.py
+-rw-rw-rw-   0        0        0      502 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_in_op.py
+-rw-rw-rw-   0        0        0      681 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_inner_join_op.py
+-rw-rw-rw-   0        0        0     1183 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_instr_op.py
+-rw-rw-rw-   0        0        0      552 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_is_null_op.py
+-rw-rw-rw-   0        0        0      378 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_limit_op.py
+-rw-rw-rw-   0        0        0      725 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_literal.py
+-rw-rw-rw-   0        0        0      617 2024-02-15 03:48:30.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_lt_op.py
+-rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_lte_op.py
+-rw-rw-rw-   0        0        0      570 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_not_op.py
+-rw-rw-rw-   0        0        0     1713 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_or_op.py
+-rw-rw-rw-   0        0        0      991 2024-03-10 20:49:59.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_order_by_op.py
+-rw-rw-rw-   0        0        0     4839 2024-03-21 02:50:25.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_script.py
+-rw-rw-rw-   0        0        0     2585 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0     1160 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_substr_op.py
+-rw-rw-rw-   0        0        0      769 2024-03-11 06:29:29.000000 mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_variable.py
+-rw-rw-rw-   0        0        0     6684 2024-02-15 03:48:30.000000 mo-sqlite-2.582.24095/mo_sqlite/sql_script.py
+-rw-rw-rw-   0        0        0     6210 2024-03-18 02:53:29.000000 mo-sqlite-2.582.24095/mo_sqlite/transacfion.py
+-rw-rw-rw-   0        0        0     1543 2024-01-28 17:16:21.000000 mo-sqlite-2.582.24095/mo_sqlite/types.py
+-rw-rw-rw-   0        0        0     5687 2024-03-20 02:25:01.000000 mo-sqlite-2.582.24095/mo_sqlite/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:18:29.842099 mo-sqlite-2.582.24095/mo_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     3462 2024-04-04 04:18:29.000000 mo-sqlite-2.582.24095/mo_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1364 2024-04-04 04:18:29.000000 mo-sqlite-2.582.24095/mo_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 04:18:29.000000 mo-sqlite-2.582.24095/mo_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      341 2024-04-04 04:18:29.000000 mo-sqlite-2.582.24095/mo_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 04:18:29.000000 mo-sqlite-2.582.24095/mo_sqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 04:18:29.845609 mo-sqlite-2.582.24095/setup.cfg
+-rw-rw-rw-   0        0        0     3333 2024-04-04 04:18:24.000000 mo-sqlite-2.582.24095/setup.py
```

### Comparing `mo-sqlite-2.579.24081/LICENSE` & `mo-sqlite-2.582.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/PKG-INFO` & `mo-sqlite-2.582.24095/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sqlite
-Version: 2.579.24081
+Version: 2.582.24095
 Summary: Multithreading for Sqlite, plus expression composition
 Home-page: https://github.com/klahnakoski/mo-sqlite
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jx-python==4.579.24081
-Requires-Dist: mo-dots==9.578.24081
-Requires-Dist: mo-files==6.579.24081
+Requires-Dist: jx-python==4.582.24095
+Requires-Dist: mo-dots==9.582.24095
+Requires-Dist: mo-files==6.582.24095
 Requires-Dist: mo-future==7.546.24057
 Requires-Dist: mo-imports==7.546.24057
-Requires-Dist: mo-json==6.579.24081
-Requires-Dist: mo-kwargs==7.578.24081
-Requires-Dist: mo-logs==8.579.24081
-Requires-Dist: mo-math==7.579.24081
-Requires-Dist: mo-sql==4.579.24081
-Requires-Dist: mo-sql==4.579.24081
-Requires-Dist: mo-threads==6.579.24081
-Requires-Dist: mo-times==5.579.24081
+Requires-Dist: mo-json==6.582.24095
+Requires-Dist: mo-kwargs==7.582.24095
+Requires-Dist: mo-logs==8.582.24095
+Requires-Dist: mo-math==7.582.24095
+Requires-Dist: mo-sql==4.582.24095
+Requires-Dist: mo-sql==4.582.24095
+Requires-Dist: mo-threads==6.582.24095
+Requires-Dist: mo-times==5.582.24095
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More SQLite!
 
 Multithreading for Sqlite, plus expression composition
```

### Comparing `mo-sqlite-2.579.24081/README.md` & `mo-sqlite-2.582.24095/README.md`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/database.py` & `mo-sqlite-2.582.24095/mo_sqlite/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,78 +3,65 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-import os
 import re
-import sys
+import sqlite3
+from collections import namedtuple
+from typing import List
 
 from mo_dots import Data, coalesce, list_to_data, from_data
 from mo_files import File
-from mo_future import allocate_lock as _allocate_lock, text, zip_longest
+from mo_future import allocate_lock as _allocate_lock
 from mo_imports import delay_import
 from mo_kwargs import override
 from mo_logs import ERROR, logger, Except, get_stacktrace, format_trace
 from mo_math.stats import percentile
 from mo_sql import *
+from mo_sqlite.transacfion import Transaction
+from mo_sqlite.utils import quote_column, sql_query, CommandItem, COMMIT, BEGIN, ROLLBACK, FORMAT_COMMAND
 from mo_threads import Lock, Queue, Thread, Till
 from mo_times import Timer
 
-from mo_sqlite.transacfion import Transaction
-from mo_sqlite.utils import quote_column, sql_query, CommandItem, COMMIT, quote_value, BEGIN, ROLLBACK, FORMAT_COMMAND
-
 jx_expression = delay_import("jx_base.jx_expression")
 table2csv = delay_import("jx_python.convert.table2csv")
 Relation = delay_import("jx_sqlite.models.relation.Relation")
 
-
 DEBUG = False
 TRACE = True
 
 DOUBLE_TRANSACTION_ERROR = "You can not query outside a transaction you have open already"
 TOO_LONG_TO_HOLD_TRANSACTION = 10
 
-_sqlite3 = None
-_load_extension_warning_sent = False
-_upgraded = False
 known_databases = {}
 
+SqliteColumn = namedtuple("SqliteColumn", ["cid", "name", "dtype", "notnull", "dflt_value", "pk"])
+
 
 class Sqlite(DB):
     """
     Allows multi-threaded access
     Loads extension functions (like SQRT)
     """
 
     @override
     def __init__(
-        self, filename=None, db=None, trace=None, upgrade=False, load_functions=False, debug=False, kwargs=None,
+        self, filename=None, db=None, trace=None, load_functions=False, debug=False, kwargs=None,
     ):
         """
         :param filename:  FILE TO USE FOR DATABASE
         :param db: AN EXISTING sqlite3 DB YOU WOULD LIKE TO USE (INSTEAD OF USING filename)
         :param trace: GET THE STACK TRACE AND THREAD FOR EVERY DB COMMAND (GOOD FOR DEBUGGING)
-        :param upgrade: REPLACE PYTHON sqlite3 DLL WITH MORE RECENT ONE, WITH MORE FUNCTIONS (NOT WORKING)
         :param load_functions: LOAD EXTENDED MATH FUNCTIONS (MAY REQUIRE upgrade)
         :param kwargs:
         """
-        global _upgraded
-        global _sqlite3
-
         self.settings = kwargs
-        if not _upgraded:
-            if upgrade:
-                _upgrade()
-            _upgraded = True
-            import sqlite3 as _sqlite3
-
-            _ = _sqlite3
 
         if filename is None:
             self.filename = None
         else:
             file = File(filename)
             file.parent.create()
             self.filename = file.abs_path
@@ -84,26 +71,24 @@
                 )
             else:
                 known_databases[self.filename] = self
         self.debug = debug | DEBUG
         self.trace = coalesce(trace, TRACE) or self.debug
 
         # SETUP DATABASE
-        self.debug and logger.note("Sqlite version {{version}}", version=_sqlite3.sqlite_version)
+        self.debug and logger.note("Sqlite version {{version}}", version=sqlite3.sqlite_version)
         try:
-            if not isinstance(db, _sqlite3.Connection):
-                self.db = _sqlite3.connect(
+            if not isinstance(db, sqlite3.Connection):
+                self.db = sqlite3.connect(
                     database=coalesce(self.filename, ":memory:"), check_same_thread=False, isolation_level=None,
                 )
             else:
                 self.db = db
         except Exception as e:
             logger.error("could not open file {{filename}}", filename=self.filename, cause=e)
-        self.upgrade = upgrade
-        load_functions and self._load_functions()
 
         self.locker = Lock()
         self.available_transactions = []  # LIST OF ALL THE TRANSACTIONS BEING MANAGED
         self.queue = Queue("sql commands")  # HOLD (command, result, signal, stacktrace) TUPLES
 
         self.closed = False
 
@@ -173,22 +158,22 @@
                 if t.thread is thread:
                     parent = t
 
         output = Transaction(self, parent=parent, thread=thread)
         self.available_transactions.append(output)
         return output
 
-    def about(self, table_name):
+    def about(self, table_name) -> List[SqliteColumn]:
         """
         :param table_name: TABLE OF INTEREST
         :return: SOME INFORMATION ABOUT THE TABLE
             (cid, name, dtype, notnull, dfft_value, pk) tuples
         """
         details = self.query("PRAGMA table_info" + sql_iso(quote_column(table_name)))
-        return details.data
+        return [SqliteColumn(*row) for row in details.data]
 
     def get_tables(self):
         result = self.query(sql_query({
             "from": "sqlite_master",
             "where": {"eq": {"type": "table"}},
             "orderby": "name",
         }))
@@ -267,36 +252,14 @@
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
-    def _load_functions(self):
-        global _load_extension_warning_sent
-        library_loc = File.new_instance(sys.modules[__name__].__file__, "../../..")
-        full_path = File.new_instance(library_loc, "vendor/sqlite/libsqlitefunctions.so").abs_path
-        try:
-            trace = get_stacktrace(0)[0]
-            if self.upgrade:
-                if os.name == "nt":
-                    file = File.new_instance(trace["file"], "../../vendor/sqlite/libsqlitefunctions.so")
-                else:
-                    file = File.new_instance(trace["file"], "../../vendor/sqlite/libsqlitefunctions")
-
-                full_path = file.abs_path
-                self.db.enable_load_extension(True)
-                self.db.execute(str(SQL_SELECT + "load_extension" + sql_iso(quote_value(full_path))))
-        except Exception as e:
-            if not _load_extension_warning_sent:
-                _load_extension_warning_sent = True
-                logger.warning(
-                    "Could not load {{file}}, doing without. (no SQRT for you!)", file=full_path, cause=e,
-                )
-
     def create_new_functions(self):
         def regexp(pattern, item):
             return re.search(pattern, item) is not None
 
         self.db.create_function("REGEXP", 2, regexp)
 
     def show_transactions_blocked_warning(self):
@@ -470,36 +433,7 @@
                     cause=cause,
                 )
                 result.exception = err
                 if transaction:
                     transaction.exception = err
             finally:
                 signal.release()
-
-
-def _upgrade():
-    global _upgraded
-    global _sqlite3
-
-    try:
-        import sys
-        import platform
-
-        if "windows" in platform.system().lower():
-            original_dll = File.new_instance(sys.exec_prefix, "dlls/sqlite3.dll")
-            if platform.architecture()[0] == "32bit":
-                source_dll = File("vendor/jx-sqlite/vendor/sqlite/sqlite3_32.dll")
-            else:
-                source_dll = File("vendor/jx-sqlite/vendor/sqlite/sqlite3_64.dll")
-
-            if not all(a == b for a, b in zip_longest(source_dll.read_bytes(), original_dll.read_bytes())):
-                original_dll.backup()
-                File.copy(source_dll, original_dll)
-        else:
-            pass
-    except Exception as e:
-        logger.warning("could not upgrade python's sqlite", cause=e)
-
-    import sqlite3 as _sqlite3
-
-    _ = _sqlite3
-    _upgraded = True
```

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/__init__.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/_utils.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_add_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_add_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_alias_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_alias_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_and_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_and_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_case_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_case_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_cast_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_cast_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_coalesce_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_coalesce_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_concat_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_concat_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_inner_join_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_inner_join_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_instr_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_instr_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_is_null_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_is_null_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_literal.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_literal.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_lt_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_lt_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_not_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_not_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_or_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_or_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_order_by_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_order_by_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_script.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_script.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_select_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_substr_op.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_substr_op.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/expressions/sql_variable.py` & `mo-sqlite-2.582.24095/mo_sqlite/expressions/sql_variable.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/sql_script.py` & `mo-sqlite-2.582.24095/mo_sqlite/sql_script.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/transacfion.py` & `mo-sqlite-2.582.24095/mo_sqlite/transacfion.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/types.py` & `mo-sqlite-2.582.24095/mo_sqlite/types.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite/utils.py` & `mo-sqlite-2.582.24095/mo_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/mo_sqlite.egg-info/PKG-INFO` & `mo-sqlite-2.582.24095/mo_sqlite.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sqlite
-Version: 2.579.24081
+Version: 2.582.24095
 Summary: Multithreading for Sqlite, plus expression composition
 Home-page: https://github.com/klahnakoski/mo-sqlite
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jx-python==4.579.24081
-Requires-Dist: mo-dots==9.578.24081
-Requires-Dist: mo-files==6.579.24081
+Requires-Dist: jx-python==4.582.24095
+Requires-Dist: mo-dots==9.582.24095
+Requires-Dist: mo-files==6.582.24095
 Requires-Dist: mo-future==7.546.24057
 Requires-Dist: mo-imports==7.546.24057
-Requires-Dist: mo-json==6.579.24081
-Requires-Dist: mo-kwargs==7.578.24081
-Requires-Dist: mo-logs==8.579.24081
-Requires-Dist: mo-math==7.579.24081
-Requires-Dist: mo-sql==4.579.24081
-Requires-Dist: mo-sql==4.579.24081
-Requires-Dist: mo-threads==6.579.24081
-Requires-Dist: mo-times==5.579.24081
+Requires-Dist: mo-json==6.582.24095
+Requires-Dist: mo-kwargs==7.582.24095
+Requires-Dist: mo-logs==8.582.24095
+Requires-Dist: mo-math==7.582.24095
+Requires-Dist: mo-sql==4.582.24095
+Requires-Dist: mo-sql==4.582.24095
+Requires-Dist: mo-threads==6.582.24095
+Requires-Dist: mo-times==5.582.24095
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More SQLite!
 
 Multithreading for Sqlite, plus expression composition
```

### Comparing `mo-sqlite-2.579.24081/mo_sqlite.egg-info/SOURCES.txt` & `mo-sqlite-2.582.24095/mo_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo-sqlite-2.579.24081/setup.py` & `mo-sqlite-2.582.24095/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='Multithreading for Sqlite, plus expression composition',
     extras_require={"tests":["mo-testing>=7.562.24075","beautifulsoup4>=4.12.3"]},
     include_package_data=True,
-    install_requires=["jx-python==4.579.24081","mo-dots==9.578.24081","mo-files==6.579.24081","mo-future==7.546.24057","mo-imports==7.546.24057","mo-json==6.579.24081","mo-kwargs==7.578.24081","mo-logs==8.579.24081","mo-math==7.579.24081","mo-sql==4.579.24081","mo-sql==4.579.24081","mo-threads==6.579.24081","mo-times==5.579.24081"],
+    install_requires=["jx-python==4.582.24095","mo-dots==9.582.24095","mo-files==6.582.24095","mo-future==7.546.24057","mo-imports==7.546.24057","mo-json==6.582.24095","mo-kwargs==7.582.24095","mo-logs==8.582.24095","mo-math==7.582.24095","mo-sql==4.582.24095","mo-sql==4.582.24095","mo-threads==6.582.24095","mo-times==5.582.24095"],
     license='MPL 2.0',
     long_description='# More SQLite!\n\nMultithreading for Sqlite, plus expression composition\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-sqlite.svg)](https://pypi.org/project/mo-sqlite/)\n[![Build Status](https://github.com/klahnakoski/mo-sqlite/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-sqlite/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-sqlite/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-sqlite?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-sqlite/month)](https://pepy.tech/project/mo-sqlite)\n\n\n## Multi-threaded Sqlite\n\nThis module wraps the `sqlite3.connection` with thread-safe traffic manager.  Here is typical usage: \n\n    from mo_sqlite import Sqlite\n    db = Sqlite("mydb.sqlite")\n    with db.transaction() as t:\n        t.command("insert into mytable values (1, 2, 3)")\n\nWhile you may have each thread own a `sqlite3.connection` to the same file, you will still get exceptions when another thread has the file locked.\n\n## Pull JSON out of database\n\nThis module includes a minimum experimental structure that can describe pulling deeply nested JSON documents out of a normalized database.  The tactic is to shape a single query who\'s resultset can be easily converted to the desired JSON by Python. Read more on [pulling json from a database](docs/JSON%20in%20Database.md)\n\nThere are multiple normal forms, including domain key normal form, and columnar form;  these have a multitude one-to-one relations, all represent the same logical schema, but differ in their access patterns to optimize for particular use cases.  This module intends to hide the particular database schema from the caller; exposing just the logical schema. \n\n\n\nThis experiment compliments the [mo-columns](https://github.com/klahnakoski/mo-columns) experiment, which is about pushing JSON into a database. \n   ',
     long_description_content_type='text/markdown',
     name='mo-sqlite',
     packages=["mo_sqlite","mo_sqlite.expressions"],
     url='https://github.com/klahnakoski/mo-sqlite',
-    version='2.579.24081'
+    version='2.582.24095'
 )
```

