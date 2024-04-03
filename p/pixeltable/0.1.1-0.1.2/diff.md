# Comparing `tmp/pixeltable-0.1.1.tar.gz` & `tmp/pixeltable-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.1.1.tar", max compression
+gzip compressed data, was "pixeltable-0.1.2.tar", max compression
```

## Comparing `pixeltable-0.1.1.tar` & `pixeltable-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      102 2023-01-30 01:56:55.531210 pixeltable-0.1.1/README.md
--rw-r--r--   0        0        0      281 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/__init__.py
--rw-r--r--   0        0        0    65851 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/catalog.py
--rw-r--r--   0        0        0     1091 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/client.py
--rw-r--r--   0        0        0    20828 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/dataframe.py
--rw-r--r--   0        0        0     2809 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/env.py
--rw-r--r--   0        0        0      312 2023-01-30 00:30:47.877364 pixeltable-0.1.1/pixeltable/exceptions.py
--rw-r--r--   0        0        0    68598 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/exprs.py
--rw-r--r--   0        0        0    12275 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/function.py
--rw-r--r--   0        0        0     4733 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0      436 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/functions/clip.py
--rw-r--r--   0        0        0      763 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/functions/pil/__init__.py
--rw-r--r--   0        0        0      475 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      830 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/functions/tf.py
--rw-r--r--   0        0        0     2009 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/index.py
--rw-r--r--   0        0        0     7966 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/store.py
--rw-r--r--   0        0        0     4010 2023-01-30 00:30:47.881364 pixeltable-0.1.1/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0      552 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0     1213 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_dict.py
--rw-r--r--   0        0        0     3184 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0    13866 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0     3369 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0      302 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_functions.py
--rw-r--r--   0        0        0    13794 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     2503 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_tf.py
--rw-r--r--   0        0        0     1162 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     1603 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0     4690 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     1289 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/tf.py
--rw-r--r--   0        0        0    17376 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/type_system.py
--rw-r--r--   0        0        0     1763 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0      628 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     1143 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/utils/tf.py
--rw-r--r--   0        0        0     1007 2023-01-30 00:30:48.181368 pixeltable-0.1.1/pixeltable/utils/video.py
--rw-r--r--   0        0        0     1125 2023-01-31 17:25:41.962852 pixeltable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 pixeltable-0.1.1/setup.py
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 pixeltable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-31 18:04:23.296982 pixeltable-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1529 2023-01-31 21:53:42.576973 pixeltable-0.1.2/README.md
+-rw-r--r--   0        0        0      555 2023-01-31 19:38:54.974389 pixeltable-0.1.2/pixeltable/__init__.py
+-rw-r--r--   0        0        0    65851 2023-01-29 20:49:01.408709 pixeltable-0.1.2/pixeltable/catalog.py
+-rw-r--r--   0        0        0     1167 2023-01-31 19:38:54.986389 pixeltable-0.1.2/pixeltable/client.py
+-rw-r--r--   0        0        0    20828 2023-01-26 21:23:21.696325 pixeltable-0.1.2/pixeltable/dataframe.py
+-rw-r--r--   0        0        0     3039 2023-01-31 19:38:54.986389 pixeltable-0.1.2/pixeltable/env.py
+-rw-r--r--   0        0        0      312 2022-12-31 02:20:14.015054 pixeltable-0.1.2/pixeltable/exceptions.py
+-rw-r--r--   0        0        0    68598 2023-01-26 21:16:49.234285 pixeltable-0.1.2/pixeltable/exprs.py
+-rw-r--r--   0        0        0    12275 2023-01-26 21:03:45.349972 pixeltable-0.1.2/pixeltable/function.py
+-rw-r--r--   0        0        0     4733 2023-01-28 01:06:30.148294 pixeltable-0.1.2/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0      436 2023-01-14 00:29:18.887129 pixeltable-0.1.2/pixeltable/functions/clip.py
+-rw-r--r--   0        0        0      763 2023-01-14 00:28:50.938053 pixeltable-0.1.2/pixeltable/functions/pil/__init__.py
+-rw-r--r--   0        0        0      475 2023-01-14 00:29:09.757602 pixeltable-0.1.2/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      830 2023-01-02 01:50:47.080216 pixeltable-0.1.2/pixeltable/functions/tf.py
+-rw-r--r--   0        0        0     2009 2023-01-26 19:07:22.458943 pixeltable-0.1.2/pixeltable/index.py
+-rw-r--r--   0        0        0     7966 2023-01-28 00:29:53.745375 pixeltable-0.1.2/pixeltable/store.py
+-rw-r--r--   0        0        0     4021 2023-01-31 19:38:54.986389 pixeltable-0.1.2/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0      552 2022-12-04 22:00:46.869734 pixeltable-0.1.2/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0     1213 2023-01-26 19:09:43.641122 pixeltable-0.1.2/pixeltable/tests/test_dict.py
+-rw-r--r--   0        0        0     3184 2022-12-04 22:00:46.869734 pixeltable-0.1.2/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0    13866 2023-01-24 22:36:40.612975 pixeltable-0.1.2/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0     3369 2023-01-24 22:17:41.023939 pixeltable-0.1.2/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0      302 2022-12-29 19:46:11.560655 pixeltable-0.1.2/pixeltable/tests/test_functions.py
+-rw-r--r--   0        0        0    13567 2023-01-31 19:38:54.974389 pixeltable-0.1.2/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     2503 2022-12-14 18:40:00.725704 pixeltable-0.1.2/pixeltable/tests/test_tf.py
+-rw-r--r--   0        0        0     1162 2022-12-23 19:46:35.048506 pixeltable-0.1.2/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     1608 2023-01-31 19:38:54.986389 pixeltable-0.1.2/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0     4700 2023-01-31 19:38:54.986389 pixeltable-0.1.2/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     1289 2022-12-12 18:43:56.266606 pixeltable-0.1.2/pixeltable/tf.py
+-rw-r--r--   0        0        0    17651 2023-01-31 19:38:54.962389 pixeltable-0.1.2/pixeltable/type_system.py
+-rw-r--r--   0        0        0     1763 2023-01-26 20:33:01.322762 pixeltable-0.1.2/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0      628 2022-11-17 22:30:23.820246 pixeltable-0.1.2/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     1143 2022-12-14 19:15:53.412903 pixeltable-0.1.2/pixeltable/utils/tf.py
+-rw-r--r--   0        0        0     1007 2023-01-26 19:56:43.298564 pixeltable-0.1.2/pixeltable/utils/video.py
+-rw-r--r--   0        0        0     1187 2023-01-31 22:29:24.196884 pixeltable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 pixeltable-0.1.2/setup.py
+-rw-r--r--   0        0        0     2595 1970-01-01 00:00:00.000000 pixeltable-0.1.2/PKG-INFO
```

### Comparing `pixeltable-0.1.1/pixeltable/catalog.py` & `pixeltable-0.1.2/pixeltable/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/client.py` & `pixeltable-0.1.2/pixeltable/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Dict
+import os
 
 import sqlalchemy.orm as orm
 
 from pixeltable import catalog, store
 from pixeltable.env import Env
 
 __all__ = [
@@ -12,15 +13,15 @@
 
 class Client:
     """Missing docstring.
     """
 
     def __init__(self) -> None:
         self.db_cache: Dict[str, catalog.Db] = {}
-        Env.get().set_up()
+        Env.get().set_up(os.environ.get('PIXELTABLE_HOME'), os.environ.get('PIXELTABLE_DB'))
 
     def create_db(self, name: str) -> catalog.Db:
         db = catalog.Db.create(name)
         self.db_cache[name] = db
         return db
 
     def drop_db(self, name: str, force: bool = False) -> None:
```

### Comparing `pixeltable-0.1.1/pixeltable/dataframe.py` & `pixeltable-0.1.2/pixeltable/dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/env.py` & `pixeltable-0.1.2/pixeltable/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,37 +21,40 @@
         self._db_path: Optional[Path] = None
         self._img_dir: Optional[Path] = None
         self._nnidx_dir: Optional[Path] = None
         self._tmp_video_dir: Optional[Path] = None
         self._sa_engine: Optional[sql.engine.base.Engine] = None
         self._db_name: Optional[str] = None
 
-    def set_up(
-        self, home_parent: Optional[Path] = Path.home(), db_name: str = 'pixeltable', echo: bool = False
-    ) -> None:
-        self.set_home(home_parent / '.pixeltable')
+    def set_up(self, home_str: Optional[str], db_name: Optional[str], echo: bool = False) -> None:
+        home = Path.home() / '.pixeltable' if home_str is None else Path(home_str)
+        if db_name is None:
+            db_name = 'pixeltable'
+        self.set_home(home)
         if self._home.exists() and not self._home.is_dir():
             raise RuntimeError(f'{self._home} is not a directory')
 
         self._db_name = db_name
         db_url = f'postgresql:///{self._db_name}'
 
         if not self._home.exists():
-            print(f'creating {self._home}')
+            print(f'setting up Pixeltable at {self._home}, db at {db_url}')
             self._home.mkdir()
             self._img_dir.mkdir()
             self._nnidx_dir.mkdir()
             self._tmp_video_dir.mkdir()
             self.tear_down()
             if not database_exists(db_url):
                 create_database(db_url)
             self._sa_engine = sql.create_engine(db_url, echo=echo, future=True)
             from pixeltable import store
             store.Base.metadata.create_all(self._sa_engine)
         else:
+            if not database_exists(db_url):
+                raise RuntimeError(f'Database not found: {db_url}')
             if self._sa_engine is None:
                 self._sa_engine = sql.create_engine(db_url, echo=echo, future=True)
 
     def tear_down(self) -> None:
         db_url = f'postgresql:///{self._db_name}'
         if database_exists(db_url):
             drop_database(db_url)
```

### Comparing `pixeltable-0.1.1/pixeltable/exprs.py` & `pixeltable-0.1.2/pixeltable/exprs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/function.py` & `pixeltable-0.1.2/pixeltable/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/functions/__init__.py` & `pixeltable-0.1.2/pixeltable/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/functions/pil/__init__.py` & `pixeltable-0.1.2/pixeltable/functions/pil/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/functions/tf.py` & `pixeltable-0.1.2/pixeltable/functions/tf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/index.py` & `pixeltable-0.1.2/pixeltable/index.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/store.py` & `pixeltable-0.1.2/pixeltable/store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/conftest.py` & `pixeltable-0.1.2/pixeltable/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 from pixeltable.tests.utils import read_data_file, make_tbl, create_table_data
 
 
 @pytest.fixture(scope='session')
 def init_db(tmp_path_factory) -> None:
     from pixeltable.env import Env
     # this also runs create_all()
-    db_name = 'test'
-    Env.get().set_up(tmp_path_factory.mktemp('base'), db_name=db_name, echo=True)
+    Env.get().set_up(str(tmp_path_factory.mktemp('base') / '.pixeltable'), 'test', echo=True)
     yield
     # leave db in place for debugging purposes
 
 
 @pytest.fixture(scope='function')
-def test_db(init_db: None) -> pt.Db:
+def test_db(init_db: None) -> catalog.Db:
     cl = pt.Client()
     db = cl.create_db(f'test')
     yield db
     cl.drop_db(db.name, force=True)
 
 
 @pytest.fixture(scope='function')
-def test_tbl(test_db: pt.Db) -> catalog.Table:
+def test_tbl(test_db: catalog.Db) -> catalog.Table:
     cols = [
         catalog.Column('c1', StringType(), nullable=False),
         catalog.Column('c2', IntType(), nullable=False),
         catalog.Column('c3', FloatType(), nullable=False),
         catalog.Column('c4', BoolType(), nullable=False),
         catalog.Column('c5', TimestampType(), nullable=False),
         catalog.Column('c6', JsonType(), nullable=False),
@@ -80,15 +79,15 @@
     data = {'c1': c1_data, 'c2': c2_data, 'c3': c3_data, 'c4': c4_data, 'c5': c5_data, 'c6': c6_data, 'c7': c7_data}
     pd_df = pd.DataFrame(data=data)
     t.insert_pandas(pd_df)
     return t
 
 
 @pytest.fixture(scope='function')
-def img_tbl(test_db: pt.Db) -> catalog.Table:
+def img_tbl(test_db: catalog.Db) -> catalog.Table:
     cols = [
         catalog.Column('img', ImageType(), nullable=False, indexed=False),
         catalog.Column('category', StringType(), nullable=False),
         catalog.Column('split', StringType(), nullable=False),
     ]
     # this table is not indexed in order to avoid the cost of computing embeddings
     tbl = test_db.create_table('test_img_tbl', cols)
@@ -99,15 +98,15 @@
 
 # TODO: why does this not work with a session scope? (some user tables don't get created with create_all())
 #@pytest.fixture(scope='session')
 #def indexed_img_tbl(init_db: None) -> catalog.Table:
 #    cl = pt.Client()
 #    db = cl.create_db('test_indexed')
 @pytest.fixture(scope='function')
-def indexed_img_tbl(test_db: pt.Db) -> catalog.Table:
+def indexed_img_tbl(test_db: catalog.Db) -> catalog.Table:
     db = test_db
     cols = [
         catalog.Column('img', ImageType(), nullable=False, indexed=True),
         catalog.Column('category', StringType(), nullable=False),
         catalog.Column('split', StringType(), nullable=False),
     ]
     tbl = db.create_table('test_indexed_img_tbl', cols)
```

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_client.py` & `pixeltable-0.1.2/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_dict.py` & `pixeltable-0.1.2/pixeltable/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_dirs.py` & `pixeltable-0.1.2/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_exprs.py` & `pixeltable-0.1.2/pixeltable/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_function.py` & `pixeltable-0.1.2/pixeltable/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_table.py` & `pixeltable-0.1.2/pixeltable/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pandas as pd
 import pytest
 import math
 
 import pixeltable as pt
 from pixeltable import exceptions as exc
 from pixeltable import catalog
 from pixeltable.type_system import \
@@ -141,29 +140,27 @@
                 extracted_frame_idx_col='frame_idx', extracted_fps=0)
         with pytest.raises(exc.BadFormatError):
             # unknown column
             _ = db.create_table(
                 'exc', cols, extract_frames_from='video', extracted_frame_col='frame',
                 extracted_frame_idx_col='breaks', extracted_fps=0)
 
-    @pytest.mark.dependency(name='test_insert')
     def test_insert(self, test_db: catalog.Db) -> None:
         db = test_db
         t1 = make_tbl(db, 'test1', ['c1', 'c2'])
         data1 = create_table_data(t1)
         t1.insert_pandas(data1)
         assert t1.count() == len(data1)
 
         # incompatible schema
         t2 = make_tbl(db, 'test2', ['c2', 'c1'])
         t2_data = create_table_data(t2)
         with pytest.raises(exc.InsertError):
             t1.insert_pandas(t2_data)
 
-    @pytest.mark.dependency(depends=['test_insert'])
     def test_query(self, test_db: catalog.Db) -> None:
         db = test_db
         t = make_tbl(db, 'test', ['c1', 'c2', 'c3', 'c4', 'c5'])
         t_data = create_table_data(t)
         t.insert_pandas(t_data)
         _ = t.show(n=0)
 
@@ -281,30 +278,28 @@
         new_t.add_column(catalog.Column(
             'c6', computed_with=sum_uda(new_t.c5).window(partition_by=new_t.c4, order_by=new_t.c3)))
         data_df = t[t.c2, t.c4, t.c3].show(0).to_pandas()
         new_t.insert_pandas(data_df)
         _ = new_t.show(0)
         print(_)
 
-    @pytest.mark.dependency(depends=['test_insert'])
     def test_revert(self, test_db: catalog.Db) -> None:
         db = test_db
         t1 = make_tbl(db, 'test1', ['c1', 'c2'])
         data1 = create_table_data(t1)
         t1.insert_pandas(data1)
         assert t1.count() == len(data1)
         data2 = create_table_data(t1)
         t1.insert_pandas(data2)
         assert t1.count() == len(data1) + len(data2)
         t1.revert()
         assert t1.count() == len(data1)
         t1.insert_pandas(data2)
         assert t1.count() == len(data1) + len(data2)
 
-    @pytest.mark.dependency(depends=['test_insert'])
     def test_snapshot(self, test_db: catalog.Db) -> None:
         db = test_db
         db.create_dir('main')
         tbl = make_tbl(db, 'main.test1', ['c1', 'c2'])
         data1 = create_table_data(tbl)
         tbl.insert_pandas(data1)
         assert tbl.count() == len(data1)
```

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_tf.py` & `pixeltable-0.1.2/pixeltable/tests/test_tf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_types.py` & `pixeltable-0.1.2/pixeltable/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/tests/test_video.py` & `pixeltable-0.1.2/pixeltable/tests/test_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pixeltable.tests.utils import get_video_files
 from pixeltable import catalog
 from pixeltable import utils
 from pixeltable import exceptions as exc
 
 
 class TestVideo:
-    def test_basic(self, test_db: pt.Db) -> None:
+    def test_basic(self, test_db: catalog.Db) -> None:
         video_filepaths = get_video_files()
         db = test_db
         cols = [
             catalog.Column('video', VideoType(), nullable=False),
             catalog.Column('frame', ImageType(), nullable=False),
             catalog.Column('frame_idx', IntType(), nullable=False),
         ]
```

### Comparing `pixeltable-0.1.1/pixeltable/tests/utils.py` & `pixeltable-0.1.2/pixeltable/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         return FloatType()
     if t == ColumnType.Type.BOOL:
         return BoolType()
     if t == ColumnType.Type.TIMESTAMP:
         return TimestampType()
     assert False
 
-def make_tbl(db: pt.Db, name: str = 'test', col_names: List[str] = ['c1']) -> pt.MutableTable:
+def make_tbl(db: catalog.Db, name: str = 'test', col_names: List[str] = ['c1']) -> catalog.MutableTable:
     schema: List[catalog.Column] = []
     for i, col_name in enumerate(col_names):
         schema.append(catalog.Column(f'{col_name}', make_default_type(ColumnType.Type(i % 5))))
     return db.create_table(name, schema)
 
 def create_table_data(t: catalog.Table, col_names: List[str] = [], num_rows: int = 10) -> pd.DataFrame:
     data: Dict[str, Any] = {}
```

### Comparing `pixeltable-0.1.1/pixeltable/tf.py` & `pixeltable-0.1.2/pixeltable/tf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/type_system.py` & `pixeltable-0.1.2/pixeltable/type_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional, Tuple, Dict, Callable, List, Union
 import enum
 import datetime
 import json
 
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
-import tensorflow as tf
+#import tensorflow as tf
 import PIL.Image
 import sqlalchemy as sql
 
 
 
 class ColumnType:
     @enum.unique
@@ -24,15 +24,16 @@
         ARRAY = 6
         IMAGE = 7
         VIDEO = 8
 
         # exprs that don't evaluate to a computable value in Pixeltable, such as an Image member function
         INVALID = 9
 
-        def to_tf(self) -> tf.dtypes.DType:
+        def to_tf(self) -> 'tf.dtypes.DType':
+            import tensorflow as tf
             if self == self.STRING:
                 return tf.string
             if self == self.INT:
                 return tf.int64
             if self == self.FLOAT:
                 return tf.float32
             if self == self.BOOL:
@@ -285,29 +286,29 @@
         """
         Return Callable that converts a column value of type self to a value of type 'target'.
         Returns None if conversion isn't possible.
         """
         return None
 
     @abc.abstractmethod
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         pass
 
 
 class InvalidType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.INVALID)
 
     def to_sql(self) -> str:
         assert False
 
     def to_sa_type(self) -> Any:
         assert False
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         raise TypeError(f'Invalid type cannot be converted to Tensorflow')
 
 
 class StringType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.STRING)
 
@@ -324,74 +325,78 @@
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
+        import tensorflow as tf
         return tf.TensorSpec(shape=(), dtype=tf.string)
 
 
 class IntType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.INT)
 
     def to_sql(self) -> str:
         return 'INTEGER'
 
     def to_sa_type(self) -> str:
         return sql.Integer
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         # TODO: how to specify the correct int subtype?
+        import tensorflow as tf
         return tf.TensorSpec(shape=(), dtype=tf.int64)
 
 
 class FloatType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.FLOAT)
 
     def to_sql(self) -> str:
         return 'FLOAT'
 
     def to_sa_type(self) -> str:
         return sql.Float
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
+        import tensorflow as tf
         # TODO: how to specify the correct float subtype?
         return tf.TensorSpec(shape=(), dtype=tf.float32)
 
 
 class BoolType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.BOOL)
 
     def to_sql(self) -> str:
         return 'BOOLEAN'
 
     def to_sa_type(self) -> str:
         return sql.Boolean
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
+        import tensorflow as tf
         # TODO: how to specify the correct int subtype?
         return tf.TensorSpec(shape=(), dtype=tf.bool)
 
 
 class TimestampType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.TIMESTAMP)
 
     def to_sql(self) -> str:
         return 'INTEGER'
 
     def to_sa_type(self) -> str:
         return sql.TIMESTAMP
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         raise TypeError(f'Timestamp type cannot be converted to Tensorflow')
 
 
 class JsonType(ColumnType):
     # TODO: type_spec also needs to be able to express lists
     def __init__(self, type_spec: Optional[Dict[str, ColumnType]] = None):
         super().__init__(self.Type.JSON)
@@ -415,15 +420,15 @@
 
     def to_sql(self) -> str:
         return 'JSONB'
 
     def to_sa_type(self) -> str:
         return sql.dialects.postgresql.JSONB
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         if self.type_spec is None:
             raise TypeError(f'Cannot convert {self.__class__.__name__} with missing type spec to TensorFlow')
         return {k: v.to_tf() for k, v in self.type_spec.items()}
 
 
 class ArrayType(ColumnType):
     def __init__(
@@ -459,15 +464,16 @@
 
     def to_sql(self) -> str:
         return 'BYTEA'
 
     def to_sa_type(self) -> str:
         return sql.VARBINARY
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
+        import tensorflow as tf
         return tf.TensorSpec(shape=self.shape, dtype=self.dtype.to_tf())
 
 
 class ImageType(ColumnType):
     @enum.unique
     class Mode(enum.Enum):
         L = 0,
@@ -543,15 +549,16 @@
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
+        import tensorflow as tf
         return tf.TensorSpec(shape=(self.height, self.width, self.num_channels), dtype=tf.uint8)
 
 
 class VideoType(ColumnType):
     def __init__(self):
         super().__init__(self.Type.VIDEO)
 
@@ -566,9 +573,9 @@
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
 
-    def to_tf(self) -> Union[tf.TypeSpec, Dict[str, tf.TypeSpec]]:
+    def to_tf(self) -> Union['tf.TypeSpec', Dict[str, 'tf.TypeSpec']]:
         assert False
```

### Comparing `pixeltable-0.1.1/pixeltable/utils/__init__.py` & `pixeltable-0.1.2/pixeltable/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/utils/clip.py` & `pixeltable-0.1.2/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/utils/tf.py` & `pixeltable-0.1.2/pixeltable/utils/tf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pixeltable/utils/video.py` & `pixeltable-0.1.2/pixeltable/utils/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.1.1/pyproject.toml` & `pixeltable-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pixeltable"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "Pixeltable: a dataframe-like interface to image and video data"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
     "pixeltable/tests/data"
```

