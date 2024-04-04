# Comparing `tmp/arrangio-0.4.0.tar.gz` & `tmp/arrangio-0.5.0.tar.gz`

## Comparing `arrangio-0.4.0.tar` & `arrangio-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/__init__.pyi
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/__main__.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/_parser_.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/_parser_.pyi
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/_utils_.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/_utils_.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arrangio-0.4.0/src/arrangio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arrangio-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 arrangio-0.4.0/tests/test___main__.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 arrangio-0.4.0/tests/test__parser_.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 arrangio-0.4.0/tests/test__utils_.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 arrangio-0.4.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 arrangio-0.4.0/LICENSE
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 arrangio-0.4.0/README.md
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 arrangio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 arrangio-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/__init__.pyi
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/__main__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/_parser_.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/_parser_.pyi
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/_utils_.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/_utils_.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arrangio-0.5.0/src/arrangio/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arrangio-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 arrangio-0.5.0/tests/test___main__.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 arrangio-0.5.0/tests/test__parser_.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 arrangio-0.5.0/tests/test__utils_.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 arrangio-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 arrangio-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 arrangio-0.5.0/README.md
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 arrangio-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 arrangio-0.5.0/PKG-INFO
```

### Comparing `arrangio-0.4.0/src/arrangio/__init__.py` & `arrangio-0.5.0/src/arrangio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 
 __all__: Final[tuple] = ()
 
 __author__: Final[str] = 'Electric Mass Records'
 __license__: Final[str] = 'MIT'
 __project__: Final[str] = __package__
-__version__: Final[str] = '0.4.0'
+__version__: Final[str] = '0.5.0'
```

### Comparing `arrangio-0.4.0/src/arrangio/__main__.py` & `arrangio-0.5.0/src/arrangio/__main__.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.4.0/src/arrangio/_parser_.py` & `arrangio-0.5.0/src/arrangio/_parser_.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.4.0/src/arrangio/_utils_.py` & `arrangio-0.5.0/src/arrangio/_utils_.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 | get_subsets  | `list(tuple(int, list))`  | gets the subsets of songs |
 | show_results | `None`                    | shows the results         |
 
 All other resources in this module are considered implementation
 details.
 """
 
+from collections import defaultdict, deque
 from datetime import timedelta as _timedelta
 from functools import lru_cache as cache
 from json import dumps as _dumps
 from re import compile as _compile
 from typing import Final
 
 
+__all__: Final[tuple] = ('get_songs', 'get_subsets', 'to_json', 'to_text')
+
+
 REGXPR: Final[str] = (
     r'^(?P<label>\w+):'
     r'((?P<hours>\d+)h)?((?P<minutes>\d+)m)?(?P<seconds>\d+)s$')
 TIMEFMT: Final[str] = '%H:%M:%S'
 
 
 def _to_seconds(
@@ -113,20 +117,20 @@
     if songs_length == 0:
         _min, _ = min(subsets)
         _max, _ = max(subsets)
         return (_max - _min, subsets)
     _songs = songs[1:]
     _song = songs[0]
     _songs_length = songs_length - 1
-    _possible_subsets = ()
+    _possible_subsets = set()
     for index, element in enumerate(subsets):
         _subset = (_song, *element[1])
-        _element = (element[0] + _song[0], _subset)
+        _element = (element[0] + _song, _subset)
         _subsets = (_element, *subsets[:index], *subsets[index + 1:])
-        _possible_subsets = (_subsets, *_possible_subsets)
+        _possible_subsets.update(set((_subsets,)))
     return min(
         __get_subsets(_songs, _songs_length, sub)
         for sub
         in _possible_subsets)
 
 
 def get_subsets(songs: tuple, num: int) -> tuple:
@@ -139,20 +143,26 @@
     Args:
         songs (tuple): The list of songs (from `get_songs`).
         num (int): The number of subsets to divide the set into.
 
     Returns:
         tuple(tuple(int, tuple(tuple(int, str)))): The list of subsets).
     """
-    songs_length = len(songs)
-    subsets = ((0, ()),) * num
-    return __get_subsets(
-        songs,
-        songs_length,
-        subsets)
+    song_lenghts = tuple(sorted(song[0] for song in songs))
+    songs_ref = defaultdict(deque)
+    for lenght, name in songs:
+        songs_ref[lenght].append(name)
+    subsets = __get_subsets(
+        song_lenghts,
+        len(song_lenghts),
+        ((0, ()),) * num)
+    return (
+        subsets[0],
+        tuple((sub[0], tuple((lenght, songs_ref.get(lenght).popleft())
+                             for lenght in sub[1])) for sub in subsets[1]))
 
 
 def to_json(result: tuple) -> str:
     """Convert the `result` to JSON.
 
     Convert the content of the `result` variable to a JSON string. The
     `result` should be the output of the `get_subsets` function.
```

### Comparing `arrangio-0.4.0/tests/test___main__.py` & `arrangio-0.5.0/tests/test___main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 @mark.parametrize('args,output,exception,exit_code', [
     ([__project__, '--dummy'], None, SystemExit, 2),
     ([__project__, '--quiet'], None, SystemExit, 2),
     ([__project__, '-s', '0:00:01'], None, SystemExit, 9),
     ([__project__, '--version'], f"{__version__}\n", SystemExit, 0),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s'],
-        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:49 ['song01 (0:00:55)', 'song02 (0:03:41)', 'song07 (0:03:45)', 'song04 (0:04:51)', 'song03 (0:05:37)']\n  [2] 0:18:41 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song06 (0:05:16)', 'song05 (0:05:54)']\n",
+        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:41 ['song05 (0:05:54)', 'song06 (0:05:16)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [2] 0:18:49 ['song03 (0:05:37)', 'song04 (0:04:51)', 'song07 (0:03:45)', 'song02 (0:03:41)', 'song01 (0:00:55)']\n",
         None,
         0
     ),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '2'],
-        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:49 ['song01 (0:00:55)', 'song02 (0:03:41)', 'song07 (0:03:45)', 'song04 (0:04:51)', 'song03 (0:05:37)']\n  [2] 0:18:41 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song06 (0:05:16)', 'song05 (0:05:54)']\n",
+        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:41 ['song05 (0:05:54)', 'song06 (0:05:16)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [2] 0:18:49 ['song03 (0:05:37)', 'song04 (0:04:51)', 'song07 (0:03:45)', 'song02 (0:03:41)', 'song01 (0:00:55)']\n",
         None,
         0
     ),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '3'],
-        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 20\nGroups:\n  [1] 0:12:26 ['song01 (0:00:55)', 'song03 (0:05:37)', 'song05 (0:05:54)']\n  [2] 0:12:22 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song04 (0:04:51)']\n  [3] 0:12:42 ['song02 (0:03:41)', 'song07 (0:03:45)', 'song06 (0:05:16)']\n",
+        f"{__project__} version {__version__}\nby Electric Mass Records under MIT license\nDifference (in seconds): 20\nGroups:\n  [1] 0:12:26 ['song05 (0:05:54)', 'song03 (0:05:37)', 'song01 (0:00:55)']\n  [2] 0:12:42 ['song06 (0:05:16)', 'song07 (0:03:45)', 'song02 (0:03:41)']\n  [3] 0:12:22 ['song04 (0:04:51)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n",
         None,
         0
     ),
     (
         [__project__, '--quiet', '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '2'],
-        '{"difference": 8, "groups": [{"id": 0, "lenght": 1129, "songs": [{"name": "song01", "lenght": 55}, {"name": "song02", "lenght": 221}, {"name": "song07", "lenght": 225}, {"name": "song04", "lenght": 291}, {"name": "song03", "lenght": 337}]}, {"id": 1, "lenght": 1121, "songs": [{"name": "song09", "lenght": 170}, {"name": "song08", "lenght": 281}, {"name": "song06", "lenght": 316}, {"name": "song05", "lenght": 354}]}]}\n',
-        #"(8, ((1129, ((55, 'song01'), (221, 'song02'), (225, 'song07'), (291, 'song04'), (337, 'song03'))), (1121, ((170, 'song09'), (281, 'song08'), (316, 'song06'), (354, 'song05')))))\n",
+        '{"difference": 8, "groups": [{"id": 0, "lenght": 1121, "songs": [{"name": "song05", "lenght": 354}, {"name": "song06", "lenght": 316}, {"name": "song08", "lenght": 281}, {"name": "song09", "lenght": 170}]}, {"id": 1, "lenght": 1129, "songs": [{"name": "song03", "lenght": 337}, {"name": "song04", "lenght": 291}, {"name": "song07", "lenght": 225}, {"name": "song02", "lenght": 221}, {"name": "song01", "lenght": 55}]}]}\n',
         None,
         0
     ),
 ])
 def test___main__(capsys, mocker, args, output, exception, exit_code):
     """test___main__."""
     mocker.patch.object(sys, 'argv', args)
```

### Comparing `arrangio-0.4.0/tests/test__parser_.py` & `arrangio-0.5.0/tests/test__parser_.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.4.0/tests/test__utils_.py` & `arrangio-0.5.0/tests/test__utils_.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,30 +69,30 @@
             _ = utils.get_songs(args)
     else:
         assert result == utils.get_songs(args)
 
 
 @mark.parametrize('args,result', [
     ([(), 0, ((0, ()),)], (0, ((0, ()),))),
-    ([((2, 'song_01'),), 1, ((0, ()),)], (0, ((2, ((2, 'song_01'),)),))),
+    ([(2,), 1, ((0, ()),)], (0, ((2, (2,)),))),
 ])
 def test__utils____get_subsets(args, result):
     """test__utils____get_subsets."""
     assert result == utils.__get_subsets(*args)
 
 
 @mark.parametrize('args,result', [
     ([(), 1], (0, ((0, ()),))),
     (
         [((354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')), 2],
-        (8, ((1129, ((55, 'song01'), (221, 'song02'), (225, 'song07'), (291, 'song04'), (337, 'song03'))), (1121, ((170, 'song09'), (281, 'song08'), (316, 'song06'), (354, 'song05')))))
+        (8, ((1121, ((354, 'song05'), (316, 'song06'), (281, 'song08'), (170, 'song09'))), (1129, ((337, 'song03'), (291, 'song04'), (225, 'song07'), (221, 'song02'), (55, 'song01')))))
     ),
     (
         [((354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')), 3],
-        (20, ((746, ((55, 'song01'), (337, 'song03'), (354, 'song05'))), (742, ((170, 'song09'), (281, 'song08'), (291, 'song04'))), (762, ((221, 'song02'), (225, 'song07'), (316, 'song06')))))
+        (20, ((746, ((354, 'song05'), (337, 'song03'), (55, 'song01'))), (762, ((316, 'song06'), (225, 'song07'), (221, 'song02'))), (742, ((291, 'song04'), (281, 'song08'), (170, 'song09')))))
     ),
 ])
 def test__utils__get_subsets(args, result):
     """test__utils__get_subsets."""
     assert result == utils.get_subsets(*args)
```

### Comparing `arrangio-0.4.0/LICENSE` & `arrangio-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrangio-0.4.0/README.md` & `arrangio-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `arrangio-0.4.0/pyproject.toml` & `arrangio-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Utilities',
     'Typing :: Typed',
 ]
 dependencies = []
 description = 'Arranges a set of songs in groups with similar total play time.'
 dynamic = [
     'version',
@@ -322,39 +323,41 @@
 default-docstring-type = 'google'
 
 # ruff
 [tool.ruff]
 extend-exclude = ['*.pyi']
 # ignore = ['DTZ']
 line-length = 79
-select = ['ALL']
 src = ['src']
-tab-size = 4
+indent-width = 4
 target-version = 'py38'
 
-[tool.ruff.isort]
+[tool.ruff.lint]
+select = ['ALL']
+
+[tool.ruff.lint.isort]
 combine-as-imports = true
 lines-after-imports = 2
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = 'double'
 inline-quotes = 'single'
 multiline-quotes = 'double'
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 5
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 #'__init__.pyi' = ['D100']
 '__main__.py' = ['T201']
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 72
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = 'google'
 
-[tool.ruff.pylint]
+[tool.ruff.lint.pylint]
 max-args = 5
 max-branches = 12
 max-returns = 6
 max-statements = 50
```

### Comparing `arrangio-0.4.0/PKG-INFO` & `arrangio-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: arrangio
-Version: 0.4.0
+Version: 0.5.0
 Summary: Arranges a set of songs in groups with similar total play time.
 Project-URL: Documentation, http://electric-mass.github.io/arrangio
 Project-URL: Homepage, https://github.com/electric-mass/arrangio
 Project-URL: Source, https://github.com/electric-mass/arrangio
 Author: Frederico Martins
 License: MIT
 License-File: LICENSE
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.8
 Provides-Extra: dev
 Requires-Dist: autopep8>=1.6.0; extra == 'dev'
 Requires-Dist: build>=0.8.0; extra == 'dev'
 Requires-Dist: coverage[toml]>=6.4.1; extra == 'dev'
```

