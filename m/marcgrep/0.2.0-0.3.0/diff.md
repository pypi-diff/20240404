# Comparing `tmp/marcgrep-0.2.0.tar.gz` & `tmp/marcgrep-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marcgrep-0.2.0.tar", max compression
+gzip compressed data, was "marcgrep-0.3.0.tar", max compression
```

## Comparing `marcgrep-0.2.0.tar` & `marcgrep-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1916 2024-03-29 20:22:10.931669 marcgrep-0.2.0/marcgrep/cli.py
--rw-r--r--   0        0        0     3840 2024-03-29 21:57:18.947710 marcgrep-0.2.0/marcgrep/filter.py
--rw-r--r--   0        0        0      114 2024-03-25 02:20:35.944404 marcgrep-0.2.0/marcgrep/utils.py
--rw-r--r--   0        0        0     1036 2024-04-02 18:32:37.692203 marcgrep-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3202 2024-04-02 18:43:00.832625 marcgrep-0.2.0/readme.md
--rw-r--r--   0        0        0     4202 1970-01-01 00:00:00.000000 marcgrep-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1596 2024-04-04 19:20:55.544537 marcgrep-0.3.0/marcgrep/cli.py
+-rw-r--r--   0        0        0     3840 2024-04-04 19:20:55.544537 marcgrep-0.3.0/marcgrep/filter.py
+-rw-r--r--   0        0        0     1036 2024-04-04 19:20:55.544537 marcgrep-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3270 2024-04-04 19:20:55.544537 marcgrep-0.3.0/readme.md
+-rw-r--r--   0        0        0     4270 1970-01-01 00:00:00.000000 marcgrep-0.3.0/PKG-INFO
```

### Comparing `marcgrep-0.2.0/marcgrep/cli.py` & `marcgrep-0.3.0/marcgrep/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,55 @@
-from importlib import metadata
-from typing import BinaryIO
+import math
+from typing import BinaryIO, Literal
 
 import click
 from pymarc import MARCReader
 
 from .filter import Filter
-from .utils import count_records
 
 
 @click.command(help="Find MARC records matching patterns in a file.")
 @click.help_option("-h", "--help")
-# TODO explain pattern syntax in command line help
 @click.argument("file", type=click.File("rb"), default="-")
-@click.option("--version", "-v", help="Show marcgrep version", is_flag=True)
 @click.option("--count", "-c", help="Count matching records", is_flag=True)
 @click.option(
     "--include", "-i", help="Include matching records (repeatable)", multiple=True
 )
 @click.option(
     "--exclude", "-e", help="Exclude matching records (repeatable)", multiple=True
 )
+@click.option("--limit", "-l", help="Limit number of records to process", type=int)
+@click.version_option(package_name="marcgrep", message="%(prog)s %(version)s")
 def main(
     file: BinaryIO,
     count: bool,
-    version: bool,
     include: list[str],
     exclude: list[str],
+    limit: int,
 ):
-    if version:
-        print(metadata.version("marcgrep"))
-        return exit(0)
-
-    num_records = 0
+    counter = 0
+    matched_records = 0
     reader = MARCReader(file)
 
     # build a list of filters, start with exclusive because they rule out records quicker
     filters = [Filter(pattern, inclusive=False) for pattern in exclude]
     filters.extend(Filter(pattern) for pattern in include)
 
-    # if no filters, count or print all records
-    if not len(filters):
-        if count:
-            num_records = count_records(reader)
-            print(num_records)
-            # non-zero exit if no records found
-            return exit(0 if num_records else 1)
-        for record in reader:
-            print(record)
-        return exit(0)
-
     for record in reader:
         if record:
+            counter += 1
             if all(f.match(record) for f in filters):
-                num_records += 1
+                matched_records += 1
                 if not count:
                     print(record)
+            if limit and counter >= limit:
+                break
 
     if count:
-        print(num_records)
+        print(matched_records)
 
     # non-zero exit if no records match
-    return exit(0 if num_records else 1)
+    return exit(0 if matched_records else 1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `marcgrep-0.2.0/marcgrep/filter.py` & `marcgrep-0.3.0/marcgrep/filter.py`

 * *Files identical despite different names*

### Comparing `marcgrep-0.2.0/pyproject.toml` & `marcgrep-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marcgrep"
-version = "0.2.0"
+version = "0.3.0"
 description = "search MARC files for regex matches"
 authors = ["phette23 <phette23@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/phette23/marcgreppy"
 repository = "https://github.com/phette23/marcgreppy"
 keywords = ["marc", "grep", "regex", "libraries", "cli", "metadata", "bibliographic", "cataloging"]
```

### Comparing `marcgrep-0.2.0/readme.md` & `marcgrep-0.3.0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 # full usage information
 $ marcgrep -h
 Usage: marcgrep [OPTIONS] [FILE]
 
   Find MARC records matching patterns in a file.
 
 Options:
-  -h, --help          Show this message and exit.
-  -v, --version       Show marcgrep version
-  -c, --count         Count matching records
-  -i, --include TEXT  Include matching records (repeatable)
-  -e, --exclude TEXT  Exclude matching records (repeatable)
+  -h, --help           Show this message and exit.
+  -c, --count          Count matching records
+  -i, --include TEXT   Include matching records (repeatable)
+  -e, --exclude TEXT   Exclude matching records (repeatable)
+  -l, --limit INTEGER  Limit number of records to process
+  --version            Show the version and exit.
 ```
 
 The `--include` and `--exclude` flags can be used multiple times to specify multiple criteria. They accept a pattern which is a sort of comma-separated filter expression for matching MARC fields. Examples:
 
 ```sh
 # records with a 780 field
 $ marcgrep -i 780 FILE.mrc
@@ -58,15 +59,15 @@
 
 Multiple criteria are combined with logical AND. Multiple `--include` flags is narrower than one, as is an `--include` and an `--exclude`.
 
 ## Development
 
 - [x] -c count
 - [x] -v version
-- [ ] -l limit (number of records to process)
+- [x] -l limit (number of records to process)
 - [x] -i include criteria (multiple)
 - [x] -e exclude criteria (multiple)
 - [ ] -f fields to print
 - [ ] work with MARC leader
 - [ ] regex for all components? e.g. `24.,text in any 240-249 field`
 - [ ] relatedly, specify _not_ to treat value as a regex?
```

### Comparing `marcgrep-0.2.0/PKG-INFO` & `marcgrep-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marcgrep
-Version: 0.2.0
+Version: 0.3.0
 Summary: search MARC files for regex matches
 Home-page: https://github.com/phette23/marcgreppy
 License: MIT
 Keywords: marc,grep,regex,libraries,cli,metadata,bibliographic,cataloging
 Author: phette23
 Author-email: phette23@gmail.com
 Requires-Python: >3.8
@@ -48,19 +48,20 @@
 # full usage information
 $ marcgrep -h
 Usage: marcgrep [OPTIONS] [FILE]
 
   Find MARC records matching patterns in a file.
 
 Options:
-  -h, --help          Show this message and exit.
-  -v, --version       Show marcgrep version
-  -c, --count         Count matching records
-  -i, --include TEXT  Include matching records (repeatable)
-  -e, --exclude TEXT  Exclude matching records (repeatable)
+  -h, --help           Show this message and exit.
+  -c, --count          Count matching records
+  -i, --include TEXT   Include matching records (repeatable)
+  -e, --exclude TEXT   Exclude matching records (repeatable)
+  -l, --limit INTEGER  Limit number of records to process
+  --version            Show the version and exit.
 ```
 
 The `--include` and `--exclude` flags can be used multiple times to specify multiple criteria. They accept a pattern which is a sort of comma-separated filter expression for matching MARC fields. Examples:
 
 ```sh
 # records with a 780 field
 $ marcgrep -i 780 FILE.mrc
@@ -84,15 +85,15 @@
 
 Multiple criteria are combined with logical AND. Multiple `--include` flags is narrower than one, as is an `--include` and an `--exclude`.
 
 ## Development
 
 - [x] -c count
 - [x] -v version
-- [ ] -l limit (number of records to process)
+- [x] -l limit (number of records to process)
 - [x] -i include criteria (multiple)
 - [x] -e exclude criteria (multiple)
 - [ ] -f fields to print
 - [ ] work with MARC leader
 - [ ] regex for all components? e.g. `24.,text in any 240-249 field`
 - [ ] relatedly, specify _not_ to treat value as a regex?
```

