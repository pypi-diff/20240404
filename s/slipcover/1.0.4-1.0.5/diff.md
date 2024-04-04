# Comparing `tmp/slipcover-1.0.4.tar.gz` & `tmp/slipcover-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-1.0.4.tar", last modified: Wed Apr  3 23:37:30 2024, max compression
+gzip compressed data, was "slipcover-1.0.5.tar", last modified: Thu Apr  4 17:45:02 2024, max compression
```

## Comparing `slipcover-1.0.4.tar` & `slipcover-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 23:37:30.358822 slipcover-1.0.4/
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-04-03 23:37:07.000000 slipcover-1.0.4/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-03 23:37:07.000000 slipcover-1.0.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-03 23:37:30.358128 slipcover-1.0.4/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     8234 2024-04-03 23:37:07.000000 slipcover-1.0.4/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-03 23:37:30.358926 slipcover-1.0.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     4329 2024-04-03 23:37:07.000000 slipcover-1.0.4/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 23:37:30.341009 slipcover-1.0.4/src/
--rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/probe.cxx
--rw-r--r--   0 runner     (501) staff       (20)      865 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/pyptr.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 23:37:30.344864 slipcover-1.0.4/src/slipcover/
--rw-r--r--   0 runner     (501) staff       (20)      152 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7531 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     6472 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/branch.py
--rw-r--r--   0 runner     (501) staff       (20)    21990 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/fuzz.py
--rw-r--r--   0 runner     (501) staff       (20)     9302 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/importer.py
--rw-r--r--   0 runner     (501) staff       (20)    25106 2024-04-03 23:37:07.000000 slipcover-1.0.4/src/slipcover/slipcover.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 23:37:30.357281 slipcover-1.0.4/src/slipcover.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      669 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-03 23:37:30.000000 slipcover-1.0.4/src/slipcover.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-03 23:37:30.356718 slipcover-1.0.4/tests/
--rw-r--r--   0 runner     (501) staff       (20)    15690 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/test_branch.py
--rw-r--r--   0 runner     (501) staff       (20)    22245 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/test_bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)    25070 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/test_coverage.py
--rw-r--r--   0 runner     (501) staff       (20)     9264 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/test_importer.py
--rw-r--r--   0 runner     (501) staff       (20)    17743 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/test_instrumentation.py
--rw-r--r--   0 runner     (501) staff       (20)     1313 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/testme-class.py
--rw-r--r--   0 runner     (501) staff       (20)     1422 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/testme-inner.py
--rw-r--r--   0 runner     (501) staff       (20)     1279 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/testme-partial.py
--rw-r--r--   0 runner     (501) staff       (20)     1269 2024-04-03 23:37:07.000000 slipcover-1.0.4/tests/testme.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.368946 slipcover-1.0.5/
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-04-04 17:44:35.000000 slipcover-1.0.5/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-04 17:44:35.000000 slipcover-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-04 17:45:02.368286 slipcover-1.0.5/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8234 2024-04-04 17:44:35.000000 slipcover-1.0.5/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-04 17:45:02.369047 slipcover-1.0.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     4329 2024-04-04 17:44:35.000000 slipcover-1.0.5/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.358121 slipcover-1.0.5/src/
+-rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/probe.cxx
+-rw-r--r--   0 runner     (501) staff       (20)      865 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/pyptr.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.361526 slipcover-1.0.5/src/slipcover/
+-rw-r--r--   0 runner     (501) staff       (20)      168 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8340 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6472 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/branch.py
+-rw-r--r--   0 runner     (501) staff       (20)    21990 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/bytecode.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/fuzz.py
+-rw-r--r--   0 runner     (501) staff       (20)     9302 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/importer.py
+-rw-r--r--   0 runner     (501) staff       (20)    24920 2024-04-04 17:44:35.000000 slipcover-1.0.5/src/slipcover/slipcover.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.367767 slipcover-1.0.5/src/slipcover.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     9352 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      669 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-04 17:45:02.000000 slipcover-1.0.5/src/slipcover.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 17:45:02.367355 slipcover-1.0.5/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    15690 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_branch.py
+-rw-r--r--   0 runner     (501) staff       (20)    22245 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_bytecode.py
+-rw-r--r--   0 runner     (501) staff       (20)    26932 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_coverage.py
+-rw-r--r--   0 runner     (501) staff       (20)     9264 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_importer.py
+-rw-r--r--   0 runner     (501) staff       (20)    17743 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/test_instrumentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1313 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-class.py
+-rw-r--r--   0 runner     (501) staff       (20)     1422 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-inner.py
+-rw-r--r--   0 runner     (501) staff       (20)     1279 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme-partial.py
+-rw-r--r--   0 runner     (501) staff       (20)     1269 2024-04-04 17:44:35.000000 slipcover-1.0.5/tests/testme.py
```

### Comparing `slipcover-1.0.4/LICENSE` & `slipcover-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/PKG-INFO` & `slipcover-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.4
+Version: 1.0.5
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.4/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.5/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -57,16 +57,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.4/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.4/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -86,15 +86,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.4/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.5/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.4/README.md` & `slipcover-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/setup.py` & `slipcover-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/probe.cxx` & `slipcover-1.0.5/src/probe.cxx`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/pyptr.h` & `slipcover-1.0.5/src/pyptr.h`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/slipcover/__main__.py` & `slipcover-1.0.5/src/slipcover/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,24 @@
 
     cov = sci.get_coverage()
     if input_tmpfiles:
         for f in input_tmpfiles:
             try:
                 fname = f.name
                 f.seek(0)
-                cov = sc.Slipcover.merge_coverage(cov, json.load(f))
+                sc.merge_coverage(cov, json.load(f))
             except json.JSONDecodeError as e:
                 print(f"Error reading {fname}: {e}")
             finally:
                 f.close()
                 try:
                     os.remove(fname)
                 except FileNotFoundError:
                     pass
 
-        sc.Slipcover.add_summaries(cov)
-
     return cov
 
 
 def exit_shim(args, sci):
     """Shims os._exit(), so a previously forked child process writes its coverage to
        a temporary file read by the parent.
     """
@@ -78,14 +76,41 @@
             output_tmpfile.flush()
 
         original_exit(*pargs, **kwargs)
 
     return wrapper
 
 
+def merge_files(args):
+    """Merges coverage files."""
+    try:
+        with args.merge[0].open() as jf:
+            merged = json.load(jf)
+    except Exception as e:
+        print(f"Error reading in {args.merge[0]}: {e}")
+        return 1
+
+    try:
+        for f in args.merge[1:]:
+            with f.open() as jf:
+                sc.merge_coverage(merged, json.load(jf))
+    except Exception as e:
+        print(f"Error merging in {f}: {e}")
+        return 1
+
+    try:
+        with args.out.open("w", encoding='utf-8') as jf:
+            json.dump(merged, jf)
+    except Exception as e:
+        print(e)
+        return 1
+
+    return 0
+
+
 def main():
     import argparse
 
     #
     # The intended usage is:
     #
     #   slipcover.py [options] (script | -m module [module_args...])
@@ -114,24 +139,31 @@
     ap.add_argument('--debug', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--dont-wrap-pytest', action='store_true', help=argparse.SUPPRESS)
     ap.add_argument('--version', action='version',
                     version=f"%(prog)s v{sc.VERSION} (Python {'.'.join(map(str, sys.version_info[:3]))})")
 
     g = ap.add_mutually_exclusive_group(required=True)
     g.add_argument('-m', dest='module', nargs=1, help="run given module as __main__")
+    g.add_argument('--merge', nargs='+', type=Path, help="merge JSON coverage files, saving to --out")
     g.add_argument('script', nargs='?', type=Path, help="the script to run")
     ap.add_argument('script_or_module_args', nargs=argparse.REMAINDER)
 
     if '-m' in sys.argv: # work around exclusive group not handled properly
         minus_m = sys.argv.index('-m')
         args = ap.parse_args(sys.argv[1:minus_m+2])
         args.script_or_module_args = sys.argv[minus_m+2:]
     else:
         args = ap.parse_args(sys.argv[1:])
 
+
+    if args.merge:
+        if not args.out: ap.error("--out is required with --merge")
+        return merge_files(args)
+
+
     base_path = Path(args.script).resolve().parent if args.script \
                 else Path('.').resolve()
 
 
     file_matcher = sc.FileMatcher()
 
     if args.source:
```

### Comparing `slipcover-1.0.4/src/slipcover/branch.py` & `slipcover-1.0.5/src/slipcover/branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/slipcover/bytecode.py` & `slipcover-1.0.5/src/slipcover/bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/slipcover/importer.py` & `slipcover-1.0.5/src/slipcover/importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/src/slipcover/slipcover.py` & `slipcover-1.0.5/src/slipcover/slipcover.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 if sys.version_info[0:2] < (3,12):
     from . import probe
     from . import bytecode as bc
 
 from pathlib import Path
 from . import branch as br
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 # FIXME provide __all__
 
 # Counter.total() is new in 3.10
 if sys.version_info[0:2] < (3,10):
     def counter_total(self: Counter) -> int:
         return sum([self[n] for n in self])
     setattr(Counter, 'total', counter_total)
 
 
 if sys.version_info[0:2] >= (3,12):
     _op_RESUME = dis.opmap["RESUME"]
 
 
+class SlipcoverError(Exception):
+    pass
+
+
 class PathSimplifier:
     def __init__(self):
         self.cwd = Path.cwd()
 
     def simplify(self, path : str) -> str:
         f = Path(path)
         try:
@@ -125,14 +129,95 @@
     headers = ["File", "#lines", "#l.miss",
                *(["#br.", "#br.miss", "brCov%", "totCov%"] if branch_coverage else ["Cover%"]),
                "Missing"]
     maxcolwidths = [None] * (len(headers)-1) + [missing_width]
     print(tabulate(table(), headers=headers, maxcolwidths=maxcolwidths), file=outfile)
 
 
+def add_summaries(cov: dict) -> None:
+    """Adds (or updates) 'summary' entries in coverage information."""
+    # global summary
+    g_summary = defaultdict(int)
+    g_nom = g_den = 0
+
+    if 'files' in cov:
+        for f_cov in cov['files'].values():
+            summary = { # per-file summary
+                'covered_lines': len(f_cov['executed_lines']),
+                'missing_lines': len(f_cov['missing_lines']),
+            }
+
+            nom = summary['covered_lines']
+            den = nom + summary['missing_lines']
+
+            if 'executed_branches' in f_cov:
+                summary.update({
+                    'covered_branches': len(f_cov['executed_branches']),
+                    'missing_branches': len(f_cov['missing_branches'])
+                })
+
+                nom += summary['covered_branches']
+                den += summary['covered_branches'] + summary['missing_branches']
+
+            summary['percent_covered'] = 100.0 if den == 0 else 100*nom/den
+            f_cov['summary'] = summary
+
+            for k in summary:
+                g_summary[k] += summary[k]
+            g_nom += nom
+            g_den += den
+
+    g_summary['percent_covered'] = 100.0 if g_den == 0 else 100*g_nom/g_den
+    cov['summary'] = g_summary
+
+
+def merge_coverage(a: dict, b: dict) -> dict:
+    """Merges coverage result 'b' into 'a'."""
+
+    if a.get('meta', {}).get('software', None) != 'slipcover':
+        raise SlipcoverError('Cannot merge coverage: only SlipCover format supported.')
+
+    if a.get('meta', {}).get('show_contexts', False) or \
+       b.get('meta', {}).get('show_contexts', False):
+        raise SlipcoverError('Merging coverage with show_contexts=True unsupported')
+
+    branch_coverage = a.get('meta', {}).get('branch_coverage', False)
+    if branch_coverage and not b.get('meta', {}).get('branch_coverage', False):
+        raise SlipcoverError('Cannot merge coverage: branch coverage missing')
+
+    a_files = a['files']
+    b_files = b['files']
+
+    def both(f, field):
+        return (a_files[f][field] if f in a_files else []) + b_files[f][field]
+
+    for f in b_files:
+        executed_lines = set(both(f, 'executed_lines'))
+        missing_lines = set(both(f, 'missing_lines'))
+        missing_lines -= executed_lines
+        update = {
+            'executed_lines': sorted(executed_lines),
+            'missing_lines': sorted(missing_lines)
+        }
+
+        if branch_coverage:
+            executed_branches = set(tuple(br) for br in both(f, 'executed_branches'))
+            missing_branches = set(tuple(br) for br in both(f, 'missing_branches'))
+            missing_branches -= executed_branches
+            update.update({
+                'executed_branches': sorted(list(br) for br in executed_branches),
+                'missing_branches': sorted(list(br) for br in missing_branches)
+            })
+
+        a_files[f] = update
+
+    add_summaries(a)
+    return a
+
+
 class Slipcover:
     def __init__(self, immediate: bool = False,
                  d_miss_threshold: int = 50, branch: bool = False,
                  disassemble: bool = False, source: List[str] = None):
         self.immediate = immediate
         self.d_miss_threshold = d_miss_threshold
         self.branch = branch
@@ -438,95 +523,14 @@
             'version': VERSION,
             'timestamp': datetime.datetime.now().isoformat(),
             'branch_coverage': branch_coverage,
             'show_contexts': False
         }
 
 
-    @staticmethod
-    def merge_coverage(a: dict, b: dict) -> dict:
-        """Merges two coverage results dictionaries.
-           The merged coverage does NOT contain summaries: call add_summaries if you need them.
-        """
-        assert not a.get('meta', {}).get('show_contexts', False)
-        assert not b.get('meta', {}).get('show_contexts', False)
-
-        branch_coverage = a.get('meta', {}).get('branch_coverage', False) and \
-                          b.get('meta', {}).get('branch_coverage', False)
-
-        a_files = a['files']
-        b_files = b['files']
-
-        def both(f, field):
-            return (a_files[f][field] if f in a_files else []) +\
-                   (b_files[f][field] if f in b_files else [])
-
-        merge_files = {}
-        for f in (a_files.keys() | b_files.keys()):
-            executed_lines = set(both(f, 'executed_lines'))
-            missing_lines = set(both(f, 'missing_lines'))
-            missing_lines -= executed_lines
-            merge_files[f] = {
-                'executed_lines': sorted(executed_lines),
-                'missing_lines': sorted(missing_lines)
-            }
-
-            if branch_coverage:
-                executed_branches = set(tuple(br) for br in both(f, 'executed_branches'))
-                missing_branches = set(tuple(br) for br in both(f, 'missing_branches'))
-                missing_branches -= executed_branches
-                merge_files[f].update({
-                    'executed_branches': sorted(list(br) for br in executed_branches),
-                    'missing_branches': sorted(list(br) for br in missing_branches)
-                })
-
-        return {
-            'meta': Slipcover._make_meta(branch_coverage),
-            'files': merge_files
-        }
-
-
-    @staticmethod
-    def add_summaries(cov: dict) -> None:
-        """Adds (or updates) 'summary' entries in coverage information."""
-        # global summary
-        g_summary = defaultdict(int)
-        g_nom = g_den = 0
-
-        if 'files' in cov:
-            for f_cov in cov['files'].values():
-                summary = { # per-file summary
-                    'covered_lines': len(f_cov['executed_lines']),
-                    'missing_lines': len(f_cov['missing_lines']),
-                }
-
-                nom = summary['covered_lines']
-                den = nom + summary['missing_lines']
-
-                if 'executed_branches' in f_cov:
-                    summary.update({
-                        'covered_branches': len(f_cov['executed_branches']),
-                        'missing_branches': len(f_cov['missing_branches'])
-                    })
-
-                    nom += summary['covered_branches']
-                    den += summary['covered_branches'] + summary['missing_branches']
-
-                summary['percent_covered'] = 100.0 if den == 0 else 100*nom/den
-                f_cov['summary'] = summary
-
-                for k in summary:
-                    g_summary[k] += summary[k]
-                g_nom += nom
-                g_den += den
-
-        g_summary['percent_covered'] = 100.0 if g_den == 0 else 100*g_nom/g_den
-        cov['summary'] = g_summary
-
-
     def get_coverage(self):
         """Returns coverage information collected."""
 
         with self.lock:
             # FIXME calling _get_newly_seen will prevent de-instrumentation if still running!
             newly_seen = self._get_newly_seen()
 
@@ -558,15 +562,15 @@
                 files[simp.simplify(f)] = f_files
 
             cov = {
                 'meta': Slipcover._make_meta(self.branch),
                 'files': files
             }
 
-            Slipcover.add_summaries(cov)
+            add_summaries(cov)
             return cov
 
 
     # @deprecated
     def print_coverage(self, outfile=sys.stdout, *, missing_width=None) -> None:
         """Prints the coveage collected by this Slipcover."""
         print_coverage(self.get_coverage(), outfile=outfile, missing_width=missing_width)
```

### Comparing `slipcover-1.0.4/src/slipcover.egg-info/PKG-INFO` & `slipcover-1.0.5/src/slipcover.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.4
+Version: 1.0.5
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.4/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.5/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -57,16 +57,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.4/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.4/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.5/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -86,15 +86,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.4/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.5/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.4/src/slipcover.egg-info/SOURCES.txt` & `slipcover-1.0.5/src/slipcover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/test_branch.py` & `slipcover-1.0.5/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/test_bytecode.py` & `slipcover-1.0.5/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/test_coverage.py` & `slipcover-1.0.5/tests/test_coverage.py`

 * *Files 7% similar despite different names*

```diff
@@ -695,14 +695,27 @@
     assert baz_file in cov['files']
     assert [] == cov['files'][baz_file]['executed_lines']
     assert [1] == cov['files'][baz_file]['missing_lines']
     assert [] == cov['files'][baz_file]['executed_branches']
     assert [] == cov['files'][baz_file]['missing_branches']
 
 
+def check_summaries(cov):
+    import copy
+
+    check = copy.deepcopy(cov)
+    sc.add_summaries(check)
+
+    for f in cov['files']:
+        assert 'summary' in cov['files'][f]
+        assert check['files'][f]['summary'] == cov['files'][f]['summary']
+
+    assert check['summary'] == cov['summary']
+
+
 @pytest.mark.parametrize("do_branch", [True, False, None])
 def test_merge_coverage(tmp_path, monkeypatch, do_branch):
     monkeypatch.chdir(tmp_path)
 
     (tmp_path / "t.py").write_text("""\
 import sys
 
@@ -732,49 +745,51 @@
 
     with (tmp_path / "a.json").open() as f:
         a = json.load(f)
     with (tmp_path / "b.json").open() as f:
         b = json.load(f)
 
     if do_branch is None:
-        del a['meta']
         del b['meta']['branch_coverage']
 
     assert 't2.py' not in a['files']
     assert 't2.py' in b['files']
     assert a['files']['t.py']['executed_lines'] != b['files']['t.py']['executed_lines']
 
-    cov = sc.Slipcover.merge_coverage(a, b)
+    sc.merge_coverage(a, b)
 
-    assert 't.py' in cov['files']
-    assert [1, 3, 4, 7, 8, 10, 13] == cov['files']['t.py']['executed_lines']
-    assert [11] == cov['files']['t.py']['missing_lines']
+    assert 't.py' in a['files']
+    assert [1, 3, 4, 7, 8, 10, 13] == a['files']['t.py']['executed_lines']
+    assert [11] == a['files']['t.py']['missing_lines']
 
     if do_branch:
-        assert [[3, 4], [3, 7], [10, 13]] == cov['files']['t.py']['executed_branches']
-        assert [[10, 11]] == cov['files']['t.py']['missing_branches']
+        assert [[3, 4], [3, 7], [10, 13]] == a['files']['t.py']['executed_branches']
+        assert [[10, 11]] == a['files']['t.py']['missing_branches']
     else:
-        assert 'executed_branches' not in cov['files']['t.py']
-        assert 'missing_branches' not in cov['files']['t.py']
+        assert 'executed_branches' not in a['files']['t.py']
+        assert 'missing_branches' not in a['files']['t.py']
 
-    assert 't2.py' in cov['files']
-    assert [1] == cov['files']['t2.py']['executed_lines']
-    assert [] == cov['files']['t2.py']['missing_lines']
+    assert 't2.py' in a['files']
+    assert [1] == a['files']['t2.py']['executed_lines']
+    assert [] == a['files']['t2.py']['missing_lines']
 
     if do_branch:
-        assert [] == cov['files']['t2.py']['executed_branches']
-        assert [] == cov['files']['t2.py']['missing_branches']
+        assert [] == a['files']['t2.py']['executed_branches']
+        assert [] == a['files']['t2.py']['missing_branches']
     else:
-        assert 'executed_branches' not in cov['files']['t2.py']
-        assert 'missing_branches' not in cov['files']['t2.py']
+        assert 'executed_branches' not in a['files']['t2.py']
+        assert 'missing_branches' not in a['files']['t2.py']
+
+    assert bool(do_branch) == a['meta']['branch_coverage']
 
-    assert bool(do_branch) == cov['meta']['branch_coverage']
+    check_summaries(a)
 
 
-def test_merge_coverage_branch_coverage_disagree(tmp_path, monkeypatch):
+@pytest.fixture
+def cov_merge_fixture(tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
 
     (tmp_path / "t.py").write_text("""\
 import sys
 
 if len(sys.argv) < 2:   # 3
     print("A branch")
@@ -783,47 +798,92 @@
 
 if not sys.argv:        # 8
     print("I'm unreachable!")
 
 print("all done!")      # 11
 """)
 
-    subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
-                    '--json', '--out', tmp_path / "a.json", "t.py"], check=True)
-    subprocess.run([sys.executable, '-m', 'slipcover',
-                    '--json', '--out', tmp_path / "b.json", "t.py", "X"], check=True)
+    yield tmp_path
 
-    with (tmp_path / "a.json").open() as f:
+
+
+@pytest.mark.parametrize("branch_in", ['a', 'b'])
+def test_merge_coverage_branch_coverage_disagree(cov_merge_fixture, branch_in):
+    subprocess.run([sys.executable, '-m', 'slipcover'] +\
+                   (['--branch'] if branch_in == 'a' else []) +\
+                    ['--json', '--out', "a.json", "t.py"], check=True)
+    subprocess.run([sys.executable, '-m', 'slipcover'] +\
+                   (['--branch'] if branch_in == 'b' else []) +\
+                    ['--json', '--out', "b.json", "t.py", "X"], check=True)
+
+    with Path("a.json").open() as f:
         a = json.load(f)
-    with (tmp_path / "b.json").open() as f:
+    with Path("b.json").open() as f:
         b = json.load(f)
 
     assert [1, 3, 4, 8, 11] == a['files']['t.py']['executed_lines']
     assert [1, 3, 6, 8, 11] == b['files']['t.py']['executed_lines']
 
-    cov = sc.Slipcover.merge_coverage(a, b)
+    if branch_in == 'a':
+        with pytest.raises(sc.SlipcoverError):
+            sc.merge_coverage(a, b)
+
+    else:
+        sc.merge_coverage(a, b)
+        assert False == a['meta']['branch_coverage']
 
-    assert False == cov['meta']['branch_coverage']
+        assert [1, 3, 4, 6, 8, 11] == a['files']['t.py']['executed_lines']
+        assert [9] == a['files']['t.py']['missing_lines']
 
-    assert [1, 3, 4, 6, 8, 11] == cov['files']['t.py']['executed_lines']
-    assert [9] == cov['files']['t.py']['missing_lines']
+        assert 'executed_branches' not in a['files']['t.py']
+        assert 'missing_branches' not in a['files']['t.py']
 
-    assert 'executed_branches' not in cov['files']['t.py']
-    assert 'missing_branches' not in cov['files']['t.py']
+        check_summaries(a)
 
 
 @pytest.mark.skipif(sys.platform == 'win32', reason='pytest-forked is Unix-specific')
 def test_pytest_forked(tmp_path):
     out = tmp_path / "out.json"
     test_file = str(Path('tests') / 'pyt.py')
 
     subprocess.run([sys.executable, '-m', 'slipcover', '--json', '--out', str(out),
                                     '-m', 'pytest', '--forked', test_file], check=True)
 
     with out.open() as f:
         cov = json.load(f)
 
+    check_summaries(cov)
+
     assert test_file in cov['files']
     assert {test_file} == set(cov['files'].keys())
     cov = cov['files'][test_file]
     assert [1, 2, 3, 4, 5, 6, 8, 9, 10, 11, 13, 14] == cov['executed_lines']
     assert [] == cov['missing_lines']
+
+
+def test_merge_flag(cov_merge_fixture):
+    subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
+                    '--json', '--out', "a.json", "t.py"], check=True)
+    subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
+                    '--json', '--out', "b.json", "t.py", "X"], check=True)
+
+    subprocess.run([sys.executable, '-m', 'slipcover', '--merge',
+                    'a.json', 'b.json', '--out', 'c.json'], check=True)
+
+    with Path("c.json").open() as f:
+        c = json.load(f)
+
+    assert [1, 3, 4, 6, 8, 11] == c['files']['t.py']['executed_lines']
+    assert [9] == c['files']['t.py']['missing_lines']
+    assert True == c['meta']['branch_coverage']
+
+    check_summaries(c)
+
+
+def test_merge_flag_no_out(cov_merge_fixture):
+    subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
+                    '--json', '--out', "a.json", "t.py"], check=True)
+    subprocess.run([sys.executable, '-m', 'slipcover', '--branch',
+                    '--json', '--out', "b.json", "t.py", "X"], check=True)
+
+    with pytest.raises(subprocess.CalledProcessError):
+        subprocess.run([sys.executable, '-m', 'slipcover', '--merge', 'a.json', 'b.json'], check=True)
```

### Comparing `slipcover-1.0.4/tests/test_importer.py` & `slipcover-1.0.5/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/test_instrumentation.py` & `slipcover-1.0.5/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/testme-class.py` & `slipcover-1.0.5/tests/testme-class.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/testme-inner.py` & `slipcover-1.0.5/tests/testme-inner.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/testme-partial.py` & `slipcover-1.0.5/tests/testme-partial.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.4/tests/testme.py` & `slipcover-1.0.5/tests/testme.py`

 * *Files identical despite different names*

