# Comparing `tmp/sqlx-exec-2.3.2.tar.gz` & `tmp/sqlx-exec-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-exec-2.3.2.tar", last modified: Wed Mar 27 13:49:30 2024, max compression
+gzip compressed data, was "sqlx-exec-2.3.3.tar", last modified: Fri Mar 29 02:19:43 2024, max compression
```

## Comparing `sqlx-exec-2.3.2.tar` & `sqlx-exec-2.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-27 13:49:30.693028 sqlx-exec-2.3.2/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.2/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7236 2024-03-27 13:49:30.692232 sqlx-exec-2.3.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6718 2024-01-23 07:49:56.000000 sqlx-exec-2.3.2/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-03-27 13:49:30.693356 sqlx-exec-2.3.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1298 2024-03-27 13:49:17.000000 sqlx-exec-2.3.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-27 13:49:30.684868 sqlx-exec-2.3.2/sqlexec/
--rw-r--r--   0 summy      (501) staff       (20)     1789 2024-03-27 08:41:08.000000 sqlx-exec-2.3.2/sqlexec/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.2/sqlexec/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     6704 2024-03-27 13:04:34.000000 sqlx-exec-2.3.2/sqlexec/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    13666 2024-03-27 13:46:45.000000 sqlx-exec-2.3.2/sqlexec/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.2/sqlexec/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.2/sqlexec/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.2/sqlexec/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.2/sqlexec/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     2916 2024-03-27 13:46:01.000000 sqlx-exec-2.3.2/sqlexec/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    17485 2024-03-27 08:41:08.000000 sqlx-exec-2.3.2/sqlexec/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-27 13:49:30.690353 sqlx-exec-2.3.2/sqlx_exec.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7236 2024-03-27 13:49:30.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      438 2024-03-27 13:49:30.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 13:49:30.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       21 2024-03-27 13:49:30.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        8 2024-03-27 13:49:30.000000 sqlx-exec-2.3.2/sqlx_exec.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-27 13:49:30.691137 sqlx-exec-2.3.2/test/
--rw-r--r--   0 summy      (501) staff       (20)      444 2024-03-25 01:37:05.000000 sqlx-exec-2.3.2/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.995468 sqlx-exec-2.3.3/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.3/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7492 2024-03-29 02:19:42.994714 sqlx-exec-2.3.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.3/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-03-29 02:19:42.995906 sqlx-exec-2.3.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1298 2024-03-29 02:12:39.000000 sqlx-exec-2.3.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.983882 sqlx-exec-2.3.3/sqlexec/
+-rw-r--r--   0 summy      (501) staff       (20)     1768 2024-03-28 02:42:54.000000 sqlx-exec-2.3.3/sqlexec/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.3/sqlexec/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     6704 2024-03-27 13:04:34.000000 sqlx-exec-2.3.3/sqlexec/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    13843 2024-03-28 01:00:25.000000 sqlx-exec-2.3.3/sqlexec/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1956 2024-03-25 07:14:31.000000 sqlx-exec-2.3.3/sqlexec/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3054 2024-03-28 00:30:18.000000 sqlx-exec-2.3.3/sqlexec/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    17485 2024-03-27 08:41:08.000000 sqlx-exec-2.3.3/sqlexec/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.991541 sqlx-exec-2.3.3/sqlx_exec.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7492 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      438 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       21 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        8 2024-03-29 02:19:42.000000 sqlx-exec-2.3.3/sqlx_exec.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-03-29 02:19:42.992540 sqlx-exec-2.3.3/test/
+-rw-r--r--   0 summy      (501) staff       (20)      444 2024-03-25 01:37:05.000000 sqlx-exec-2.3.3/test/test.py
```

### Comparing `sqlx-exec-2.3.2/LICENSE` & `sqlx-exec-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/PKG-INFO` & `sqlx-exec-2.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.2
+Version: 2.3.3
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
@@ -13,188 +13,188 @@
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   import sqlexec
+       import sqlexec as db
 
-   if __name__ == '__main__':
-       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       if __name__ == '__main__':
+           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+           # or
+           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
+           # or
+           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
 
-       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
-       select_key = "SELECT currval('person_id_seq')"
+           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
+           select_key = "SELECT currval('person_id_seq')"
 
-       id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
+           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
-       count = sqlexec.get('select count(1) from person')
-       # result: 4
+           count = db.get('select count(1) from person')
+           # result: 4
 
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 4
+           count = db.sql('select count(1) from person').get()
+           # result: 4
 
-       persons = sqlexec.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.select('select id, name, age from person')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.sql('select id, name, age from person').select()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.sql('select id, name, age from person').select()
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.table('person').select('id', 'name', 'age')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.table('person').select('id', 'name', 'age')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.select_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').select_one('zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.select('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').select(name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.query('select id, name, age from person')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.query('select id, name, age from person')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.sql('select id, name, age from person').query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.sql('select id, name, age from person').query()
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.query_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').query_one('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').query(name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       effected_rowcount = sqlexec.table('person').where(name='zhangsan').update(name='xxx', age=45)
+           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
 
-       effected_rowcount = sqlexec.table('person').where(id=6).delete()
-       count = sqlexec.table('person').count())
-       # result: 3
+           effected_rowcount = db.table('person').where(id=6).delete()
+           count = db.table('person').count())
+           # result: 3
 
-       effected_rowcount = sqlexec.execute('delete from person where id = :id', id=5)
-       count = sqlexec.get('select count(1) from person')
-       # result: 2
+           effected_rowcount = db.execute('delete from person where id = :id', id=5)
+           count = db.get('select count(1) from person')
+           # result: 2
 
-       effected_rowcount = sqlexec.sql('delete from person where id = ?').execute(4)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 1
+           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
+           count = db.sql('select count(1) from person').get()
+           # result: 1
 
-       effected_rowcount = sqlexec.sql('delete from person where id = :id').execute(id=3)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 0
+           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
+           count = db.sql('select count(1) from person').get()
+           # result: 0
 
-       # select data save as csv
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
+           # select data save as csv
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
 
-       # insert from csv
-       sqlexec.table('person').insert_from_csv('test.csv')
+           # insert from csv
+           db.table('person').insert_from_csv('test.csv')
 
-       # select data transform to DataFrame of pandas
-       df = sqlexec.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
+           # select data transform to DataFrame of pandas
+           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
 
-       df = sqlexec.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
+           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
 
-       # insert from DataFrame of pandas
-       sqlexec.table('person').insert_from_df(dataframe)
+           # insert from DataFrame of pandas
+           db.table('person').insert_from_df(dataframe)
 
-       # select data save as json
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
+           # select data save as json
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
 
-       # insert from json
-       sqlexec.table('person').insert_from_json('test.json')
+           # insert from json
+           db.table('person').insert_from_json('test.json')
 
-       sqlexec.close()
+           db.close()
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlexec import with_transaction, transaction
+       from sqlexec import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
-
-
-   def test_transaction2():
-       with transaction():
+       @with_transaction
+       def test_transaction():
            insert_func(....)
            update_func(....)
 
 
+       def test_transaction2():
+           with transaction():
+               insert_func(....)
+               update_func(....)
+
+
 If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `sqlx-exec-2.3.2/README.rst` & `sqlx-exec-2.3.3/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,184 +1,184 @@
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   import sqlexec
+       import sqlexec as db
 
-   if __name__ == '__main__':
-       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       if __name__ == '__main__':
+           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+           # or
+           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
+           # or
+           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
 
-       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
-       select_key = "SELECT currval('person_id_seq')"
+           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
+           select_key = "SELECT currval('person_id_seq')"
 
-       id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
+           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
-       count = sqlexec.get('select count(1) from person')
-       # result: 4
+           count = db.get('select count(1) from person')
+           # result: 4
 
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 4
+           count = db.sql('select count(1) from person').get()
+           # result: 4
 
-       persons = sqlexec.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.select('select id, name, age from person')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.sql('select id, name, age from person').select()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.sql('select id, name, age from person').select()
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.table('person').select('id', 'name', 'age')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.table('person').select('id', 'name', 'age')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.select_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').select_one('zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.select('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').select(name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.query('select id, name, age from person')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.query('select id, name, age from person')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.sql('select id, name, age from person').query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.sql('select id, name, age from person').query()
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.query_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').query_one('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').query(name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       effected_rowcount = sqlexec.table('person').where(name='zhangsan').update(name='xxx', age=45)
+           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
 
-       effected_rowcount = sqlexec.table('person').where(id=6).delete()
-       count = sqlexec.table('person').count())
-       # result: 3
+           effected_rowcount = db.table('person').where(id=6).delete()
+           count = db.table('person').count())
+           # result: 3
 
-       effected_rowcount = sqlexec.execute('delete from person where id = :id', id=5)
-       count = sqlexec.get('select count(1) from person')
-       # result: 2
+           effected_rowcount = db.execute('delete from person where id = :id', id=5)
+           count = db.get('select count(1) from person')
+           # result: 2
 
-       effected_rowcount = sqlexec.sql('delete from person where id = ?').execute(4)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 1
+           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
+           count = db.sql('select count(1) from person').get()
+           # result: 1
 
-       effected_rowcount = sqlexec.sql('delete from person where id = :id').execute(id=3)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 0
+           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
+           count = db.sql('select count(1) from person').get()
+           # result: 0
 
-       # select data save as csv
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
+           # select data save as csv
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
 
-       # insert from csv
-       sqlexec.table('person').insert_from_csv('test.csv')
+           # insert from csv
+           db.table('person').insert_from_csv('test.csv')
 
-       # select data transform to DataFrame of pandas
-       df = sqlexec.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
+           # select data transform to DataFrame of pandas
+           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
 
-       df = sqlexec.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
+           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
 
-       # insert from DataFrame of pandas
-       sqlexec.table('person').insert_from_df(dataframe)
+           # insert from DataFrame of pandas
+           db.table('person').insert_from_df(dataframe)
 
-       # select data save as json
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
+           # select data save as json
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
 
-       # insert from json
-       sqlexec.table('person').insert_from_json('test.json')
+           # insert from json
+           db.table('person').insert_from_json('test.json')
 
-       sqlexec.close()
+           db.close()
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlexec import with_transaction, transaction
+       from sqlexec import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
-
-
-   def test_transaction2():
-       with transaction():
+       @with_transaction
+       def test_transaction():
            insert_func(....)
            update_func(....)
 
 
+       def test_transaction2():
+           with transaction():
+               insert_func(....)
+               update_func(....)
+
+
 If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `sqlx-exec-2.3.2/setup.py` & `sqlx-exec-2.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.3.2',
+    version='2.3.3',
     install_requires=[
-        'sqlx-executor>=1.1.0',
+        'sqlx-executor>=1.1.1',
     ],
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
```

### Comparing `sqlx-exec-2.3.2/sqlexec/__init__.py` & `sqlx-exec-2.3.3/sqlexec/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     transaction,
     with_connection,
     with_transaction,
     get_connection,
     close,
     Driver,
     Engine,
-    init_db as _init_db
+    init as _init
 )
 from .exec import (
     execute,
     insert,
     save,
     save_sql,
     save_select_key,
@@ -46,29 +46,29 @@
 
 from .sql_exec import sql
 from .page_exec import page
 from .table_exec import table
 from .dialect import Dialect
 
 
-def init_db(*args, **kwargs):
+def init(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
 
     from sqlexec
-    sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+    sqlexec.init('test.db', driver='sqlite3', show_sql=True, debug=True)
     or
-    sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+    sqlexec.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
     or
-    sqlexec.init_db(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
+    sqlexec.init(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
 
     Addition parameters:
     :param driver=None: str|Driver, import driver, 'import pymysql'
     :param pool_size=0: int, default 0, size of connection pool
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
-    engine = _init_db(*args, **kwargs)
+    engine = _init(*args, **kwargs)
     Dialect.init(engine)
```

### Comparing `sqlx-exec-2.3.2/sqlexec/constant.py` & `sqlx-exec-2.3.3/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/dialect.py` & `sqlx-exec-2.3.3/sqlexec/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/exec.py` & `sqlx-exec-2.3.3/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
 
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _get(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
@@ -199,14 +200,15 @@
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _select_one(sql, *args)
 
 
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
@@ -217,14 +219,15 @@
 
 
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _query_one(sql, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
```

### Comparing `sqlx-exec-2.3.2/sqlexec/loader.py` & `sqlx-exec-2.3.3/sqlexec/loader.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/log_support.py` & `sqlx-exec-2.3.3/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/page_exec.py` & `sqlx-exec-2.3.3/sqlexec/page_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/sql_exec.py` & `sqlx-exec-2.3.3/sqlexec/sql_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlexec/sql_support.py` & `sqlx-exec-2.3.3/sqlexec/sql_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import re
 from executor import DBError
 from .dialect import Dialect
 from functools import lru_cache
 from .log_support import sql_log
-from .constant import CACHE_SIZE, NAMED_REGEX
+from executor.sql_support import require_limit
 from typing import Collection, Union, List, Tuple
-from executor.sql_support import require_limit, limit_one_sql_args
+from .constant import CACHE_SIZE, NAMED_REGEX, LIMIT_1
+
+
+def limit_one_sql_args(sql: str, *args):
+    if require_limit(sql):
+        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
+    return sql, args
 
 
 def insert_sql(table: str, cols: Collection[str]):
     cols = cols if isinstance(cols, tuple) else tuple(cols)
     return Dialect.create_insert_sql(table, cols)
```

### Comparing `sqlx-exec-2.3.2/sqlexec/table_exec.py` & `sqlx-exec-2.3.3/sqlexec/table_exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-2.3.2/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-2.3.3/sqlx_exec.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 2.3.2
+Version: 2.3.3
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
@@ -13,188 +13,188 @@
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   import sqlexec
+       import sqlexec as db
 
-   if __name__ == '__main__':
-       sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
+       if __name__ == '__main__':
+           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+           # or
+           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
 
-       # or
-       sqlexec.init_db(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
+           # or
+           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
 
-       effected_rowcount = sqlexec.insert(table='person', name='zhangsan', age=15)
+           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
 
-       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
-       select_key = "SELECT currval('person_id_seq')"
+           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
+           select_key = "SELECT currval('person_id_seq')"
 
-       id = sqlexec.save(select_key=select_key, table='person', name='lisi', age=26)
+           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
 
-       id = sqlexec.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
 
-       count = sqlexec.get('select count(1) from person')
-       # result: 4
+           count = db.get('select count(1) from person')
+           # result: 4
 
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 4
+           count = db.sql('select count(1) from person').get()
+           # result: 4
 
-       persons = sqlexec.select('select id, name, age from person')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.select('select id, name, age from person')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.sql('select id, name, age from person').select()
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.sql('select id, name, age from person').select()
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.table('person').select('id', 'name', 'age')
-       # result:
-       # (3, 'zhangsan', 15)
-       # (4, 'lisi', 26)
-       # (5, 'wangwu', 38)
-       # (6, 'zhaoliu', 45)
+           persons = db.table('person').select('id', 'name', 'age')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
 
-       persons = sqlexec.select_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').select_one('zhangsan')
-       # result:
-       # (3, 'zhangsan', 15)
+           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
 
-       persons = sqlexec.select('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').select(name='zhangsan')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
-       # result:
-       # [(3, 'zhangsan', 15)]
+           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
+           # result:
+           # [(3, 'zhangsan', 15)]
 
-       persons = sqlexec.query('select id, name, age from person')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.query('select id, name, age from person')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.sql('select id, name, age from person').query()
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
-       # {'id': 4, 'name': 'lisi', 'age': 26}
-       # {'id': 5, 'name': 'wangwu', 'age': 38}
-       # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+           persons = db.sql('select id, name, age from person').query()
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
 
-       persons = sqlexec.query_one('select id, name, age from person where name = ?', 'zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.sql('select id, name, age from person where name = ?').query_one('zhangsan')
-       # result:
-       # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
 
-       persons = sqlexec.query('select id, name, age from person where name = :name', name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').query(name='zhangsan')
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       persons = sqlexec.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
-       # result:
-       # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-       effected_rowcount = sqlexec.table('person').where(name='zhangsan').update(name='xxx', age=45)
+           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
 
-       effected_rowcount = sqlexec.table('person').where(id=6).delete()
-       count = sqlexec.table('person').count())
-       # result: 3
+           effected_rowcount = db.table('person').where(id=6).delete()
+           count = db.table('person').count())
+           # result: 3
 
-       effected_rowcount = sqlexec.execute('delete from person where id = :id', id=5)
-       count = sqlexec.get('select count(1) from person')
-       # result: 2
+           effected_rowcount = db.execute('delete from person where id = :id', id=5)
+           count = db.get('select count(1) from person')
+           # result: 2
 
-       effected_rowcount = sqlexec.sql('delete from person where id = ?').execute(4)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 1
+           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
+           count = db.sql('select count(1) from person').get()
+           # result: 1
 
-       effected_rowcount = sqlexec.sql('delete from person where id = :id').execute(id=3)
-       count = sqlexec.sql('select count(1) from person').get()
-       # result: 0
+           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
+           count = db.sql('select count(1) from person').get()
+           # result: 0
 
-       # select data save as csv
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
+           # select data save as csv
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
 
-       # insert from csv
-       sqlexec.table('person').insert_from_csv('test.csv')
+           # insert from csv
+           db.table('person').insert_from_csv('test.csv')
 
-       # select data transform to DataFrame of pandas
-       df = sqlexec.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
+           # select data transform to DataFrame of pandas
+           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
 
-       df = sqlexec.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
+           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
 
-       # insert from DataFrame of pandas
-       sqlexec.table('person').insert_from_df(dataframe)
+           # insert from DataFrame of pandas
+           db.table('person').insert_from_df(dataframe)
 
-       # select data save as json
-       sqlexec.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
+           # select data save as json
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
 
-       sqlexec.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
 
-       # insert from json
-       sqlexec.table('person').insert_from_json('test.json')
+           # insert from json
+           db.table('person').insert_from_json('test.json')
 
-       sqlexec.close()
+           db.close()
 
 Transaction
 '''''''''''
 
 .. code:: python
 
-   from sqlexec import with_transaction, transaction
+       from sqlexec import with_transaction, transaction
 
-   @with_transaction
-   def test_transaction():
-       insert_func(....)
-       update_func(....)
-
-
-   def test_transaction2():
-       with transaction():
+       @with_transaction
+       def test_transaction():
            insert_func(....)
            update_func(....)
 
 
+       def test_transaction2():
+           with transaction():
+               insert_func(....)
+               update_func(....)
+
+
 If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
 
 If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

