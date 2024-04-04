# Comparing `tmp/manga_scrape-4.7.1.tar.gz` & `tmp/manga_scrape-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga_scrape-4.7.1.tar", last modified: Fri Jan 19 15:13:01 2024, max compression
+gzip compressed data, was "manga_scrape-4.8.0.tar", last modified: Thu Apr  4 03:21:13 2024, max compression
```

## Comparing `manga_scrape-4.7.1.tar` & `manga_scrape-4.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.963106 manga_scrape-4.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-19 15:13:01.963106 manga_scrape-4.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.959107 manga_scrape-4.7.1/manga/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.959107 manga_scrape-4.7.1/manga/sites/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/sites/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/sites/test.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/sites/unknown_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.959107 manga_scrape-4.7.1/manga/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/guess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/inc_chapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/no_unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/open_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/test_sites.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/unnumbered_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/tools/up_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.959107 manga_scrape-4.7.1/manga/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/utils/extract_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/manga/utils/split_on_num.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 15:13:01.963106 manga_scrape-4.7.1/manga_scrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-19 15:13:01.000000 manga_scrape-4.7.1/manga_scrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-01-19 15:12:54.000000 manga_scrape-4.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 15:13:01.963106 manga_scrape-4.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.820872 manga_scrape-4.8.0/manga/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.820872 manga_scrape-4.8.0/manga/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/sites/unknown_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11821 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/guess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/inc_chapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/no_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/open_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/test_sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/unnumbered_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/tools/up_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/extract_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/manga/utils/split_on_num.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/manga_scrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 03:21:13.000000 manga_scrape-4.8.0/manga_scrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-04 03:21:08.000000 manga_scrape-4.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:21:13.824872 manga_scrape-4.8.0/setup.cfg
```

### Comparing `manga_scrape-4.7.1/LICENSE` & `manga_scrape-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/PKG-INFO` & `manga_scrape-4.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: manga_scrape
-Version: 4.7.1
+Version: 4.8.0
 Summary: A python package used for automating finding manga chapters
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/zwimer/manga
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: osascript
 Requires-Dist: regex
 Requires-Dist: requests
 Requires-Dist: tldextract
 Requires-Dist: tqdm
+Requires-Dist: rich
 
 # Manga
 
 A collection of tools for scraping manga websites.
 These tools are geared towards OSX but can be adapted otherwise.
```

### Comparing `manga_scrape-4.7.1/manga/sites/domains.py` & `manga_scrape-4.8.0/manga/sites/domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 The functions in this file return true if a chapter is found for the specific site
 They take in as input the html of the webpage
 """
+
 from __future__ import annotations
 from collections.abc import Callable
 
 
 #
 # Return true if chapter is found
 #
```

### Comparing `manga_scrape-4.7.1/manga/tools/guess.py` & `manga_scrape-4.8.0/manga/tools/guess.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/tools/inc_chapter.py` & `manga_scrape-4.8.0/manga/tools/inc_chapter.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/tools/no_unicode.py` & `manga_scrape-4.8.0/manga/tools/no_unicode.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/tools/open_new.py` & `manga_scrape-4.8.0/manga/tools/open_new.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/tools/test_sites.py` & `manga_scrape-4.8.0/manga/tools/test_sites.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 from concurrent.futures import Future, thread
-from collections.abc import Callable
+from collections import defaultdict
+from typing import TYPE_CHECKING
 from functools import lru_cache
 from pathlib import Path
-from typing import Any
 import subprocess
 import traceback
 import argparse
 import platform
+import termios
 import time
 import sys
 
+from rich.progress import Progress, BarColumn, TextColumn, TimeRemainingColumn, MofNCompleteColumn, TaskProgressColumn
 from tqdm import tqdm
 import requests
 
 from manga.utils import extract_url, lsf, split_on_num
 from manga import sites
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+    from typing import Any
+
 
 class ThreadHandler(thread.ThreadPoolExecutor):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.futures: list[Future] = []
 
     def add(self, fn: Callable[..., Any], *args: Any, **kwargs: Any) -> None:
@@ -127,15 +133,15 @@
 ######################################################################
 #                           Main Functions                           #
 ######################################################################
 
 
 @lru_cache(maxsize=None)
 def _test_site(url: str):
-    return sites.test(url)
+    return sites.test(url, timeout_retries=5)
 
 
 def _test(left: str, right: str, x: float) -> bool:
     """
     Test if chapter x is found at a URL constructed from left, right, and x
     """
     if int(x) == x:
@@ -143,15 +149,15 @@
     else:
         if _test_site(f"{left}{x}{right}"):
             return True
         return _test_site(f"{left}{str(x).replace('.', '-')}{right}")
 
 
 # pylint: disable=too-many-return-statements,too-many-branches
-def _evaluate(url: str, delay: int) -> Failed | None:
+def _evaluate(url: str) -> Failed | None:
     """
     If url is broken, return a failure class for it
     """
     if "vol" in url.lower():
         return HasVol(url)
     left, n, right = split_on_num(url)
     if n != int(n):
@@ -160,46 +166,54 @@
         return Tiny(url)
     elif "mangabuddy" in left and ("/mbx" in left or any(i.isalpha() for i in right)):
         return Pattern(url)
     test = lambda x: _test(left, right, x)
     try:
         if test(n) and not test(n - 1) and not test(5):
             return Exists(url)
-        time.sleep(0.25)  # No DOS-ing
+        time.sleep(0.05)  # No DOS-ing
         if not test(n):
             for i in (0.1, 1, 1.1, 2, 2.1, 5, 10, 20):
                 if test(n + i):
                     return Missing(url)
-        time.sleep(0.5)  # No DOS-ing
+        time.sleep(0.1)  # No DOS-ing
         if not any(test(i) for i in (n, n - 1, 5, n + 0.1, n + 1, n + 1.1)):
             return Broken(url)
-        time.sleep(0.25)  # No DOS-ing
+        time.sleep(0.05)  # No DOS-ing
         return None
     except sites.UnknownDomain:
         return Unknown(url)
     except requests.exceptions.RequestException as e:
+        print(e)
         return BadRequest(url, e)
-    finally:
-        time.sleep(delay)  # No DOS-ing
 
 
-def evaluate(url: str, delay: int, ret: list, pbar) -> None:
+def evaluate(urls: str, delay: int, ret: list, pbar: Progress) -> None:
     """
     Determine if url is broken
     Store return value in ret because we the return value will be ignored
     """
     try:
-        rv: Failed | None = _evaluate(url, delay)
-        if rv is not None:
-            ret.append(rv)
+        domain = sites.get_domain(urls[0])
+        task = pbar.add_task(f"{domain}:", total=len(urls))
+        update = lambda: pbar.update(task, advance=1)
+        first: bool = False
+        for i in urls:
+            if not first:
+                time.sleep(delay)
+                first = False
+            rv: Failed | None = _evaluate(i)
+            if rv is not None:
+                ret.append(rv)
+            update()
+    except KeyboardInterrupt:
+        raise
     except:
         traceback.print_exc()
         raise
-    finally:
-        pbar.update()
 
 
 def print_each(prefix: str, lst: list[Failed]):
     """
     Print every item in lst
     """
     if lst:
@@ -214,73 +228,84 @@
     if lst:
         print(f"{prefix}\n\t" + "\n\t".join(i.url for i in lst))
         for i in tqdm(lst, dynamic_ncols=True, leave=False):
             subprocess.check_call([opener, i.url], stdout=subprocess.DEVNULL)
         print("")
 
 
-def test_sites(
-    directory: Path, skip: set[str] | list[str], opener: str, prompt: bool, n_workers: int, delay: int
-) -> bool:
+def test_sites(directory: Path, skip: set[str] | list[str], opener: str, no_prompt: bool, delay: int) -> bool:
     """
     Test each file in directory, print the results open them as needed
     """
     if isinstance(skip, list):
-        return test_sites(directory, set(skip), opener, prompt, n_workers, delay)
+        return test_sites(directory, set(skip), opener, no_prompt, delay)
     print("Checking arguments...")
     directory = directory.resolve()
     assert delay >= 0, "Delay may not be negative"
-    assert n_workers > 0, "n_workers must be positive"
     assert directory.exists(), f"{directory} does not exist"
     assert directory.is_dir(), f"{directory} is not a directory"
     # Determine which requests must be made
     print("Scanning files...")
     urls: set[str] = {extract_url(i) for i in lsf(directory)}
+    # Bucket URLs
+    bucketed = defaultdict(list)
+    for i in urls:
+        bucketed[sites.get_domain(i)].append(i)
     # Determine what to open
     tested: list[Failed] = []
-    print(f"Testing {len(urls)} urls using {n_workers} workers...")
-    with tqdm(total=len(urls), dynamic_ncols=True) as pbar:
-        with ThreadHandler(max_workers=n_workers) as executor:  # No DOS-ing
-            for i in urls:
-                if sites.get_domain(i) in skip:
+    print(f"Testing {len(urls)} urls...")
+    with Progress(
+        TextColumn("[progress.description]{task.description}"),
+        TaskProgressColumn(),
+        BarColumn(None),
+        MofNCompleteColumn(),
+        TimeRemainingColumn(compact=True, elapsed_when_finished=True),
+        transient=True,
+        expand=True,
+    ) as pbar:
+        for i in skip:
+            got: list | None = bucketed.pop(i, None)
+            if got is not None:
+                pbar.add_task(i, total=len(got))
+                for i in got:
                     tested.append(Skipped(i))
-                    pbar.update()
-                else:
-                    executor.add(evaluate, i, delay, tested, pbar)
+                pbar.update(i, advance=len(got))
+        with ThreadHandler(max_workers=len(bucketed)) as executor:  # No DOS-ing
+            for k in bucketed.values():
+                executor.add(evaluate, k, delay, tested, pbar)
     # Results
     no_open: list[Failed] = [i for i in tested if isinstance(i, NoOpen)]
     to_open: list[Failed] = [i for i in tested if isinstance(i, ToOpen)]
     # Print no-open failures
     sub_list: Callable[[list[Failed], type], list[Failed]] = lambda lst, t: [i for i in lst if isinstance(i, t)]
     if no_open:
         print(f"{'*'*70}\n*{'Errors'.center(68)}*\n{'*'*70}\n")
         for sub in {i.__class__ for i in no_open}:
             print_each(sub.kind(), sub_list(no_open, sub))
         print(f"\n{'*'*70}\n*{'Done'.center(68)}*\n{'*'*70}\n")
     # Open
-    if prompt:
+    if not no_prompt:
+        termios.tcflush(sys.stdin, termios.TCIFLUSH)
         _ = input("Testing complete. Hit enter to open websites.")
     for sub in {i.__class__ for i in to_open}:
         open_each(opener, sub.kind(), sub_list(to_open, sub))
+    print("Done!")
     return True
 
 
 def main(prog: str, *args: str) -> bool:
     assert "Darwin" == platform.system(), "Not on Mac! Remember to change name and ext!"
     parser = argparse.ArgumentParser(prog=Path(prog).name)
     parser.add_argument("directory", type=Path, help="The directory to test")
     parser.add_argument("--skip", type=str, nargs="+", default=[], help="Domains to skip")
-    parser.add_argument("--n_workers", default=16, type=int, help="The number of sites to test concurrently")
     parser.add_argument("--opener", default="open", help="The default binary to open a URL with")
-    parser.add_argument(
-        "--prompt", action="store_true", help="Do not auto open sites when complete, prompt user instead"
-    )
+    parser.add_argument("--no-prompt", action="store_true", help="Auto open sites when complete, do not prompt user")
     parser.add_argument(
         "--delay",
-        default=1,
+        default=0,
         type=int,
         help="The number of seconds each thread should wait between testing sites (to avoid DOSing)",
     )
     return test_sites(**vars(parser.parse_args(args)))
 
 
 def cli() -> None:
```

### Comparing `manga_scrape-4.7.1/manga/tools/unnumbered_helper.py` & `manga_scrape-4.8.0/manga/tools/unnumbered_helper.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/tools/up_number.py` & `manga_scrape-4.8.0/manga/tools/up_number.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/utils/extract_url.py` & `manga_scrape-4.8.0/manga/utils/extract_url.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/utils/files.py` & `manga_scrape-4.8.0/manga/utils/files.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga/utils/split_on_num.py` & `manga_scrape-4.8.0/manga/utils/split_on_num.py`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/manga_scrape.egg-info/PKG-INFO` & `manga_scrape-4.8.0/manga_scrape.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: manga_scrape
-Version: 4.7.1
+Version: 4.8.0
 Summary: A python package used for automating finding manga chapters
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/zwimer/manga
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: osascript
 Requires-Dist: regex
 Requires-Dist: requests
 Requires-Dist: tldextract
 Requires-Dist: tqdm
+Requires-Dist: rich
 
 # Manga
 
 A collection of tools for scraping manga websites.
 These tools are geared towards OSX but can be adapted otherwise.
```

### Comparing `manga_scrape-4.7.1/manga_scrape.egg-info/SOURCES.txt` & `manga_scrape-4.8.0/manga_scrape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manga_scrape-4.7.1/pyproject.toml` & `manga_scrape-4.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 requires-python = ">=3.10"
 dependencies = [
     "osascript",
     "regex",
     "requests",
     "tldextract",
     "tqdm",
+    "rich",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
@@ -55,7 +56,11 @@
 target-version = ["py310"]
 
 [tool.ruff]
 ignore=["E731"]
 line-length = 120
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
+
+[tool.vulture]
+ignore_names = ["cli"]
+paths = ["manga"]
```

