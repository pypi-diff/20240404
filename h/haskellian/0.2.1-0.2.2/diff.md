# Comparing `tmp/haskellian-0.2.1.tar.gz` & `tmp/haskellian-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-0.2.1.tar", last modified: Tue Apr  2 05:10:02 2024, max compression
+gzip compressed data, was "haskellian-0.2.2.tar", last modified: Thu Apr  4 09:00:04 2024, max compression
```

## Comparing `haskellian-0.2.1.tar` & `haskellian-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:10:02.351956 haskellian-0.2.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-02 05:10:02.351956 haskellian-0.2.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-04-02 04:47:51.000000 haskellian-0.2.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-02 05:09:53.000000 haskellian-0.2.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-02 05:10:02.351956 haskellian-0.2.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:10:02.351956 haskellian-0.2.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:10:02.351956 haskellian-0.2.1/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:10:02.351956 haskellian-0.2.1/src/haskellian/core/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-02 05:09:49.000000 haskellian-0.2.1/src/haskellian/core/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1039 2024-04-02 05:02:46.000000 haskellian-0.2.1/src/haskellian/core/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      412 2024-04-02 05:09:41.000000 haskellian-0.2.1/src/haskellian/core/lazy.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 05:10:02.351956 haskellian-0.2.1/src/haskellian.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-02 05:10:02.000000 haskellian-0.2.1/src/haskellian.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      265 2024-04-02 05:10:02.000000 haskellian-0.2.1/src/haskellian.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-02 05:10:02.000000 haskellian-0.2.1/src/haskellian.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-02 05:10:02.000000 haskellian-0.2.1/src/haskellian.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.599822 haskellian-0.2.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-04 09:00:04.599822 haskellian-0.2.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-04-02 04:47:51.000000 haskellian-0.2.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-04 08:58:13.000000 haskellian-0.2.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 09:00:04.599822 haskellian-0.2.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian/core/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-02 05:09:49.000000 haskellian-0.2.2/src/haskellian/core/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1111 2024-04-04 08:59:29.000000 haskellian-0.2.2/src/haskellian/core/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      412 2024-04-02 05:09:41.000000 haskellian-0.2.2/src/haskellian/core/lazy.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:00:04.589822 haskellian-0.2.2/src/haskellian.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      232 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      265 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 09:00:04.000000 haskellian-0.2.2/src/haskellian.egg-info/top_level.txt
```

### Comparing `haskellian-0.2.1/src/haskellian/core/funcs.py` & `haskellian-0.2.2/src/haskellian/core/funcs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import TypeVar, Callable, Iterable
+from typing import TypeVar, Callable, Iterable, TypeVarTuple
 from functools import reduce, wraps
 
 A = TypeVar('A')
 B = TypeVar('B')
+As = TypeVarTuple('As')
 
 
 def pipe(x: A, *funcs: Callable[[A], B]) -> B:
   """Apply to `x` a left-to-right composition of `funcs`
   >>> pipe('  hello ', str.strip, str.title) # 'Hello'
   """
-  return reduce(lambda x, f: f(x), funcs, x)
+  return reduce(lambda x, f: f(x), funcs, x) # type: ignore
 
 def flow(*funcs: Callable[[A], B]) -> Callable[[A], B]:
   """Left-to-right composition of `funcs`
   >>> func = flow(str.strip, str.title) # same as: func = lambda s: s.strip().title()
   """
   return lambda x: pipe(x, *funcs)
 
@@ -21,23 +22,23 @@
 def safe(f: Callable[[], A]) -> A | None:
   """Tries to return `f()`, otherwise `None`"""
   try:
     return f()
   except:
     ...
 
-def listify(func: Callable[[A], Iterable[B]]) -> Callable[[A], list[B]]:
+def listify(func: Callable[[*As], Iterable[B]]) -> Callable[[*As], list[B]]:
     """Make a generator return a list
     
     ```
     @listify
     def mygenerator():
       for x in range(3):
         yield x
 
     mygenerator() # [0, 1, 2]
     ```
     """
     @wraps(func)
     def _f(*args, **kwargs):
-        return list(func(*args, **kwargs))
+        return list(func(*args, **kwargs)) # type: ignore
     return _f
```

