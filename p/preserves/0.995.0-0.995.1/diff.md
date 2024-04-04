# Comparing `tmp/preserves-0.995.0.tar.gz` & `tmp/preserves-0.995.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preserves-0.995.0.tar", last modified: Fri Mar  8 09:04:15 2024, max compression
+gzip compressed data, was "preserves-0.995.1.tar", last modified: Thu Apr  4 11:29:26 2024, max compression
```

## Comparing `preserves-0.995.0.tar` & `preserves-0.995.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-03-08 09:04:15.916188 preserves-0.995.0/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1969 2024-03-08 09:04:15.916188 preserves-0.995.0/PKG-INFO
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      949 2023-06-27 20:36:11.000000 preserves-0.995.0/README.md
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-03-08 09:04:15.912189 preserves-0.995.0/preserves/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2448 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/__init__.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    14581 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/binary.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     5537 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/compare.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      214 2022-11-23 10:34:15.000000 preserves-0.995.0/preserves/compat.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      642 2023-06-27 20:36:11.000000 preserves-0.995.0/preserves/error.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1079 2024-02-05 21:54:23.000000 preserves-0.995.0/preserves/fold.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2893 2023-12-01 08:01:55.000000 preserves-0.995.0/preserves/merge.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2068 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/path.prb
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    18606 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/path.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2917 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/schema.prb
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    36113 2024-02-02 12:23:35.000000 preserves-0.995.0/preserves/schema.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    20331 2024-03-08 08:47:35.000000 preserves-0.995.0/preserves/text.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    19619 2024-02-05 21:54:23.000000 preserves-0.995.0/preserves/values.py
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-03-08 09:04:15.912189 preserves-0.995.0/preserves.egg-info/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1969 2024-03-08 09:04:15.000000 preserves-0.995.0/preserves.egg-info/PKG-INFO
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      552 2024-03-08 09:04:15.000000 preserves-0.995.0/preserves.egg-info/SOURCES.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)        1 2024-03-08 09:04:15.000000 preserves-0.995.0/preserves.egg-info/dependency_links.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      135 2024-03-08 09:04:15.000000 preserves-0.995.0/preserves.egg-info/requires.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       10 2024-03-08 09:04:15.000000 preserves-0.995.0/preserves.egg-info/top_level.txt
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1040 2024-03-08 08:48:24.000000 preserves-0.995.0/pyproject.toml
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)       38 2024-03-08 09:04:15.916188 preserves-0.995.0/setup.cfg
-drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-03-08 09:04:15.912189 preserves-0.995.0/tests/
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      681 2022-11-23 10:34:15.000000 preserves-0.995.0/tests/test_compare.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)      390 2023-06-27 20:36:11.000000 preserves-0.995.0/tests/test_doctests.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1588 2022-11-23 10:34:15.000000 preserves-0.995.0/tests/test_path.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)    13443 2024-02-02 12:23:35.000000 preserves-0.995.0/tests/test_preserves.py
--rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1284 2022-11-23 10:34:15.000000 preserves-0.995.0/tests/test_schema.py
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-04-04 11:29:26.950671 preserves-0.995.1/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1969 2024-04-04 11:29:26.950671 preserves-0.995.1/PKG-INFO
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      949 2023-10-13 12:04:39.000000 preserves-0.995.1/README.md
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-04-04 11:29:26.946671 preserves-0.995.1/preserves/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2448 2024-01-28 13:36:53.000000 preserves-0.995.1/preserves/__init__.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    14702 2024-03-27 09:57:30.000000 preserves-0.995.1/preserves/binary.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     5537 2024-01-28 13:36:53.000000 preserves-0.995.1/preserves/compare.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      214 2022-01-12 13:12:34.000000 preserves-0.995.1/preserves/compat.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      642 2023-10-13 12:04:39.000000 preserves-0.995.1/preserves/error.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1079 2024-02-05 22:30:57.000000 preserves-0.995.1/preserves/fold.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2893 2024-01-28 13:36:19.000000 preserves-0.995.1/preserves/merge.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2068 2024-03-27 09:46:39.000000 preserves-0.995.1/preserves/path.prb
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    18606 2024-01-28 13:36:53.000000 preserves-0.995.1/preserves/path.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     2917 2024-03-27 09:46:39.000000 preserves-0.995.1/preserves/schema.prb
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    36112 2024-04-04 11:25:20.000000 preserves-0.995.1/preserves/schema.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    20331 2024-03-08 09:19:14.000000 preserves-0.995.1/preserves/text.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    19619 2024-03-27 09:48:37.000000 preserves-0.995.1/preserves/values.py
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-04-04 11:29:26.950671 preserves-0.995.1/preserves.egg-info/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1969 2024-04-04 11:29:26.000000 preserves-0.995.1/preserves.egg-info/PKG-INFO
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      552 2024-04-04 11:29:26.000000 preserves-0.995.1/preserves.egg-info/SOURCES.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)        1 2024-04-04 11:29:26.000000 preserves-0.995.1/preserves.egg-info/dependency_links.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      135 2024-04-04 11:29:26.000000 preserves-0.995.1/preserves.egg-info/requires.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       10 2024-04-04 11:29:26.000000 preserves-0.995.1/preserves.egg-info/top_level.txt
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1040 2024-04-04 11:29:03.000000 preserves-0.995.1/pyproject.toml
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)       38 2024-04-04 11:29:26.950671 preserves-0.995.1/setup.cfg
+drwxr-xr-x   0 tonyg     (1000) tonyg     (1000)        0 2024-04-04 11:29:26.950671 preserves-0.995.1/tests/
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      681 2023-03-15 14:21:09.000000 preserves-0.995.1/tests/test_compare.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)      390 2023-10-13 12:04:39.000000 preserves-0.995.1/tests/test_doctests.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1588 2023-03-15 14:21:09.000000 preserves-0.995.1/tests/test_path.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)    13443 2024-01-28 13:36:53.000000 preserves-0.995.1/tests/test_preserves.py
+-rw-r--r--   0 tonyg     (1000) tonyg     (1000)     1284 2023-03-15 14:21:09.000000 preserves-0.995.1/tests/test_schema.py
```

### Comparing `preserves-0.995.0/PKG-INFO` & `preserves-0.995.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preserves
-Version: 0.995.0
+Version: 0.995.1
 Summary: Data serialization format
 Author-email: Tony Garnock-Jones <tonyg@leastfixedpoint.com>
 License: Apache-2.0
 Project-URL: Homepage, https://preserves.dev/
 Project-URL: Issues, https://gitlab.com/preserves/preserves/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `preserves-0.995.0/README.md` & `preserves-0.995.1/README.md`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/__init__.py` & `preserves-0.995.1/preserves/__init__.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/binary.py` & `preserves-0.995.1/preserves/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,19 @@
         if tag == 0xb2: return self.wrap(self.nextbytes(self.varint()))
         if tag == 0xb3: return self.wrap(Symbol(self.nextbytes(self.varint()).decode('utf-8')))
         if tag == 0xb4:
             vs = self.nextvalues()
             if not vs: raise DecodeError('Too few elements in encoded record')
             return self.wrap(Record(vs[0], vs[1:]))
         if tag == 0xb5: return self.wrap(tuple(self.nextvalues()))
-        if tag == 0xb6: return self.wrap(frozenset(self.nextvalues()))
+        if tag == 0xb6:
+            vs = self.nextvalues()
+            s = frozenset(vs)
+            if len(s) != len(vs): raise DecodeError('Duplicate value')
+            return self.wrap(s)
         if tag == 0xb7: return self.wrap(ImmutableDict.from_kvs(self.nextvalues()))
         raise DecodeError('Invalid tag: ' + hex(tag))
 
     def try_next(self):
         """Like [next][preserves.binary.Decoder.next], but returns `None` instead of raising
         [ShortPacket][preserves.error.ShortPacket]."""
         start = self.index
```

### Comparing `preserves-0.995.0/preserves/compare.py` & `preserves-0.995.1/preserves/compare.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/error.py` & `preserves-0.995.1/preserves/error.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/fold.py` & `preserves-0.995.1/preserves/fold.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/merge.py` & `preserves-0.995.1/preserves/merge.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/path.prb` & `preserves-0.995.1/preserves/path.prb`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/path.py` & `preserves-0.995.1/preserves/path.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/schema.prb` & `preserves-0.995.1/preserves/schema.prb`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/schema.py` & `preserves-0.995.1/preserves/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         if p.key == REC:
             if not isinstance(v, Record): raise SchemaDecodeFailed(cls, p, v)
             cls.parse(p[0], v.key, args)
             cls.parse(p[1], v.fields, args)
             return ()
         if p.key == TUPLE:
             if not sequenceish(v): raise SchemaDecodeFailed(cls, p, v)
-            if len(v) != len(p[0]): raise SchemaDecodeFailed(cls, p, v)
+            if len(v) < len(p[0]): raise SchemaDecodeFailed(cls, p, v)
             i = 0
             for pp in p[0]:
                 cls.parse(pp, v[i], args)
                 i = i + 1
             return ()
         if p.key == TUPLE_PREFIX:
             if not sequenceish(v): raise SchemaDecodeFailed(cls, p, v)
```

### Comparing `preserves-0.995.0/preserves/text.py` & `preserves-0.995.1/preserves/text.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves/values.py` & `preserves-0.995.1/preserves/values.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/preserves.egg-info/PKG-INFO` & `preserves-0.995.1/preserves.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preserves
-Version: 0.995.0
+Version: 0.995.1
 Summary: Data serialization format
 Author-email: Tony Garnock-Jones <tonyg@leastfixedpoint.com>
 License: Apache-2.0
 Project-URL: Homepage, https://preserves.dev/
 Project-URL: Issues, https://gitlab.com/preserves/preserves/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `preserves-0.995.0/preserves.egg-info/SOURCES.txt` & `preserves-0.995.1/preserves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/pyproject.toml` & `preserves-0.995.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "preserves"
-version = "0.995.0"
+version = "0.995.1"
 description = "Data serialization format"
 readme = "README.md"
 requires-python = ">=3.6, <4"
 license = {text = "Apache-2.0"}
 
 authors = [
     {name = "Tony Garnock-Jones", email = "tonyg@leastfixedpoint.com"},
```

### Comparing `preserves-0.995.0/tests/test_compare.py` & `preserves-0.995.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/tests/test_path.py` & `preserves-0.995.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/tests/test_preserves.py` & `preserves-0.995.1/tests/test_preserves.py`

 * *Files identical despite different names*

### Comparing `preserves-0.995.0/tests/test_schema.py` & `preserves-0.995.1/tests/test_schema.py`

 * *Files identical despite different names*

