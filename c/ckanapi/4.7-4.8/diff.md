# Comparing `tmp/ckanapi-4.7.tar.gz` & `tmp/ckanapi-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ckanapi-4.7.tar", last modified: Wed Apr 20 13:22:44 2022, max compression
+gzip compressed data, was "ckanapi-4.8.tar", last modified: Thu Apr  4 15:45:21 2024, max compression
```

## Comparing `ckanapi-4.7.tar` & `ckanapi-4.8.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/
--rw-rw-r--   0 ian       (1000) ian       (1000)     1083 2022-04-14 18:46:37.000000 ckanapi-4.7/setup.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi/
--rw-r--r--   0 ian       (1000) ian       (1000)     3286 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/localckan.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     9583 2022-03-07 16:28:32.000000 ckanapi-4.7/ckanapi/datapackage.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4423 2021-12-06 16:08:35.000000 ckanapi-4.7/ckanapi/common.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     5026 2021-12-06 16:08:35.000000 ckanapi-4.7/ckanapi/remoteckan.py
--rw-r--r--   0 ian       (1000) ian       (1000)      412 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2365 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/testappckan.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1616 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/errors.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi/cli/
--rw-rw-r--   0 ian       (1000) ian       (1000)     6550 2022-03-12 22:45:17.000000 ckanapi-4.7/ckanapi/cli/batch.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     7741 2022-03-11 19:50:26.000000 ckanapi-4.7/ckanapi/cli/main.py
--rw-rw-r--   0 ian       (1000) ian       (1000)      330 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/cli/ckan_click.py
--rw-r--r--   0 ian       (1000) ian       (1000)      750 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/cli/paster.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2726 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/cli/search.py
--rw-r--r--   0 ian       (1000) ian       (1000)     1385 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/cli/utils.py
--rw-r--r--   0 ian       (1000) ian       (1000)     2548 2022-03-12 22:24:57.000000 ckanapi-4.7/ckanapi/cli/action.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     7686 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/cli/delete.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     7000 2022-03-07 16:28:32.000000 ckanapi-4.7/ckanapi/cli/dump.py
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/cli/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)    11014 2021-09-15 14:55:26.000000 ckanapi-4.7/ckanapi/cli/load.py
--rw-r--r--   0 ian       (1000) ian       (1000)     4053 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/cli/workers.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi/tests/
--rw-r--r--   0 ian       (1000) ian       (1000)    18128 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_cli_load.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi/tests/mock/
--rw-r--r--   0 ian       (1000) ian       (1000)     2184 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/mock/mock_ckan.py
--rw-r--r--   0 ian       (1000) ian       (1000)     2298 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_testapp.py
--rw-r--r--   0 ian       (1000) ian       (1000)     3965 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_remote.py
--rw-r--r--   0 ian       (1000) ian       (1000)    11901 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_cli_dump.py
--rw-r--r--   0 ian       (1000) ian       (1000)        0 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)     5645 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_cli_action.py
--rw-r--r--   0 ian       (1000) ian       (1000)     5715 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_cli_workers.py
--rw-r--r--   0 ian       (1000) ian       (1000)      838 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_call.py
--rw-r--r--   0 ian       (1000) ian       (1000)    11527 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/tests/test_datapackage.py
--rw-r--r--   0 ian       (1000) ian       (1000)       82 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi/version.py
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2022-04-20 13:22:44.000000 ckanapi-4.7/setup.cfg
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)        8 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi.egg-info/not-zip-safe
--rw-r--r--   0 ian       (1000) ian       (1000)      996 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      224 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      276 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       47 2019-12-16 20:32:50.000000 ckanapi-4.7/ckanapi.egg-info/pbr.json
--rw-r--r--   0 ian       (1000) ian       (1000)       72 2022-04-20 13:22:44.000000 ckanapi-4.7/ckanapi.egg-info/requires.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)      276 2022-04-20 13:22:44.000000 ckanapi-4.7/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)    15997 2022-03-25 15:02:14.000000 ckanapi-4.7/README.md
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.622949 ckanapi-4.8/
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1358 2021-04-26 20:58:45.000000 ckanapi-4.8/COPYING
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1463 2021-04-26 20:58:45.000000 ckanapi-4.8/COPYING.fr
+-rw-r--r--   0 ian       (1000) ian       (1000)      610 2024-04-04 15:45:21.622949 ckanapi-4.8/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)    16154 2024-04-04 15:29:24.000000 ckanapi-4.8/README.md
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.614949 ckanapi-4.8/ckanapi/
+-rw-rw-r--   0 ian       (1000) ian       (1000)      412 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/__init__.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.618949 ckanapi-4.8/ckanapi/cli/
+-rw-rw-r--   0 ian       (1000) ian       (1000)        0 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/cli/__init__.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2548 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/cli/action.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     6550 2022-09-21 20:36:18.000000 ckanapi-4.8/ckanapi/cli/batch.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)      371 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/cli/ckan_click.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     7686 2021-04-27 20:51:12.000000 ckanapi-4.8/ckanapi/cli/delete.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     8103 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/cli/dump.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    11169 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/cli/load.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     9389 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/cli/main.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)      750 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/cli/paster.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2787 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/cli/search.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1287 2022-09-21 20:34:37.000000 ckanapi-4.8/ckanapi/cli/utils.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4053 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/cli/workers.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4423 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/common.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     9583 2022-09-21 20:36:18.000000 ckanapi-4.8/ckanapi/datapackage.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1616 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/errors.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3320 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/localckan.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     5026 2022-09-21 20:36:18.000000 ckanapi-4.8/ckanapi/remoteckan.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2365 2021-04-27 20:51:12.000000 ckanapi-4.8/ckanapi/testappckan.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.618949 ckanapi-4.8/ckanapi/tests/
+-rw-rw-r--   0 ian       (1000) ian       (1000)        0 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/tests/__init__.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.618949 ckanapi-4.8/ckanapi/tests/mock/
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2550 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/tests/mock/mock_ckan.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)      838 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/tests/test_call.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     5645 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/tests/test_cli_action.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    15685 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/tests/test_cli_dump.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    18147 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/tests/test_cli_load.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     5715 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/tests/test_cli_workers.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    11561 2022-09-21 20:36:18.000000 ckanapi-4.8/ckanapi/tests/test_datapackage.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3964 2024-04-04 15:29:24.000000 ckanapi-4.8/ckanapi/tests/test_remote.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2298 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/tests/test_testapp.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)       82 2021-04-26 20:58:45.000000 ckanapi-4.8/ckanapi/version.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2024-04-04 15:45:21.618949 ckanapi-4.8/ckanapi.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)      610 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)      989 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)      173 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/entry_points.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2021-04-27 21:04:51.000000 ckanapi-4.8/ckanapi.egg-info/not-zip-safe
+-rw-rw-r--   0 ian       (1000) ian       (1000)      179 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/requires.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        8 2024-04-04 15:45:21.000000 ckanapi-4.8/ckanapi.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2024-04-04 15:45:21.622949 ckanapi-4.8/setup.cfg
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1172 2024-04-04 15:30:19.000000 ckanapi-4.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ckanapi-4.7/ckanapi/localckan.py` & `ckanapi-4.8/ckanapi/localckan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from cgi import FieldStorage
 from tempfile import TemporaryFile
 
 from ckanapi.errors import CKANAPIError
 from ckanapi.common import ActionShortcut
 
 COPY_CHUNK = 1024*1024
 
@@ -60,18 +59,21 @@
                 else:
                     filename = f.name
                 try:
                     f.seek(0)
                 except (AttributeError, IOError):
                     f = _write_temp_file(f)
                     to_close.append(f)
-                field_storage = FieldStorage()
-                field_storage.file = f
-                field_storage.filename = filename
-                data_dict[fieldname] = field_storage
+
+                from werkzeug.datastructures import FileStorage
+
+                file_storage = FileStorage()
+                file_storage.stream = f
+                file_storage.filename = filename
+                data_dict[fieldname] = file_storage
 
             return self._get_action(action)(context, data_dict)
         finally:
             for f in to_close:
                 f.close()
```

### Comparing `ckanapi-4.7/ckanapi/datapackage.py` & `ckanapi-4.8/ckanapi/datapackage.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/common.py` & `ckanapi-4.8/ckanapi/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
     # see http://docs.python-requests.org/en/latest/user/quickstart/#more-complicated-post-requests
     return hasattr(v, 'read') or (
         isinstance(v, tuple) and len(v) >= 2 and hasattr(v[1], 'read'))
 
 
 def prepare_action(action, data_dict=None, apikey=None, files=None,
-                   base_url='action/api/'):
+                   base_url='api/action/'):
     """
     Return action_url, data_json, http_headers
     """
     if not data_dict:
         data_dict = {}
     headers = {}
     if files:
```

### Comparing `ckanapi-4.7/ckanapi/remoteckan.py` & `ckanapi-4.8/ckanapi/remoteckan.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/testappckan.py` & `ckanapi-4.8/ckanapi/testappckan.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/errors.py` & `ckanapi-4.8/ckanapi/errors.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/cli/batch.py` & `ckanapi-4.8/ckanapi/cli/batch.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/cli/main.py` & `ckanapi-4.8/ckanapi/cli/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,23 +10,23 @@
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [--insecure]]
   ckanapi delete (datasets | groups | organizations | users | related)
           (ID_OR_NAME ... | [-I JSONL_INPUT] [-s START] [-m MAX])
           [-p PROCESSES] [-l LOG_FILE] [-qwz]
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [--insecure]]
   ckanapi dump (datasets | groups | organizations | users | related)
           (ID_OR_NAME ... | --all) ([-O JSONL_OUTPUT] | [-D DIRECTORY])
-          [-p PROCESSES] [-dqwz]
+          [-p PROCESSES] [-dqwzRU]
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [-g] [--insecure]]
   ckanapi load datasets
           [--upload-resources] [-I JSONL_INPUT] [-s START] [-m MAX]
           [-p PROCESSES] [-l LOG_FILE] [-n | -o] [-qwz]
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [--insecure]]
   ckanapi load (groups | organizations)
           [--upload-logo] [-I JSONL_INPUT] [-s START] [-m MAX]
-          [-p PROCESSES] [-l LOG_FILE] [-n | -o] [-qwz]
+          [-p PROCESSES] [-l LOG_FILE] [-n | -o] [-qwzU]
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [--insecure]]
   ckanapi load (users | related)
           [-I JSONL_INPUT] [-s START] [-m MAX] [-p PROCESSES] [-l LOG_FILE]
           [-n | -o] [-qwz]
           [[-c CONFIG] [-u USER] | -r SITE_URL [-a APIKEY] [--insecure]]
   ckanapi search datasets
           [(KEY=STRING | KEY:JSON ) ... | -i | -I JSON_INPUT]
@@ -60,18 +60,21 @@
   --insecure                ignore verifying the SSL certificate for sites
                             using https
   -o --update-only          update existing records, don't create new records
   -O --output=JSONL_OUTPUT  output to json lines file instead of stdout
   -p --processes=PROCESSES  set the number of worker processes [default: 1]
   -q --quiet                don't display progress messages
   -r --remote=URL           URL of CKAN server for remote actions
+  -R --resource-views       export resource views information along with
+                            resource metadata as resource_views lists
   -s --start-record=START   start from record number START, where the first
                             record is number 1 [default: 1]
   -u --ckan-user=USER       perform actions as user with this name, uses the
                             site sysadmin user when not specified
+  -U --include-users        include users of a group/organization
   --upload-logo             upload logo image of a group/organization if the
                             image is stored in the original server, otherwise
                             its image url will be used
   --upload-resources        upload resources of a dataset that were uploaded to
                             server. Resources originally linked by external
                             urls will keep the urls,will not be uploaded
   -w --worker               launch worker process - used internally by load,
@@ -79,27 +82,31 @@
   -z --gzip                 read/write gzipped data
 """
 
 import sys
 import os
 from docopt import docopt
 from pkg_resources import load_entry_point
+import subprocess
 
 from ckanapi.version import __version__
 from ckanapi.remoteckan import RemoteCKAN
 from ckanapi.localckan import LocalCKAN
 from ckanapi.errors import CLIError
 from ckanapi.cli.load import load_things
 from ckanapi.cli.dump import dump_things
 from ckanapi.cli.delete import delete_things
 from ckanapi.cli.action import action
 from ckanapi.cli.search import search_datasets
 from ckanapi.cli.batch import batch_actions
 
+from logging import getLogger
 
+# explicit logger namespace for easy logging handlers
+log = getLogger('ckan.ckanapi')
 PYTHON2 = str is bytes
 
 def parse_arguments():
     # docopt is awesome
     return docopt(__doc__, version=__version__)
 
 
@@ -107,27 +114,53 @@
     """
     ckanapi command line entry point
     """
     arguments = parse_arguments()
 
     if not running_with_paster and not arguments['--remote']:
         if PYTHON2:
+            ckan_ini = os.environ.get('CKAN_INI')
+            if ckan_ini and not arguments['--config']:
+                sys.argv[1:1] = ['--config', ckan_ini]
             return _switch_to_paster(arguments)
         return _switch_to_ckan_click(arguments)
 
     if arguments['--remote']:
         ckan = RemoteCKAN(arguments['--remote'],
             apikey=arguments['--apikey'],
             user_agent="ckanapi-cli/{version} (+{url})".format(
                 version=__version__,
                 url='https://github.com/open-data/ckanapi'),
             get_only=arguments['--get-request'],
             )
     else:
         ckan = LocalCKAN(username=arguments['--ckan-user'])
+        # log execution of LocalCKAN commands
+        from ckan.plugins.toolkit import config, asbool
+        if asbool(config.get('ckanapi.log_local')) and len(sys.argv) > 1:
+            cmd = ['who', 'am', 'i']
+            proc = subprocess.Popen(cmd, stdout=subprocess.PIPE,
+                                    stderr=subprocess.PIPE)
+            out, err = proc.communicate()
+            if not out or err:
+                # fallback to whoami if `who am i` is empty or errored
+                cmd = ['whoami']
+                proc = subprocess.Popen(cmd, stdout=subprocess.PIPE,
+                                        stderr=subprocess.PIPE)
+                out, err = proc.communicate()
+            if not out or err:
+                # cannot find user
+                out = '<unknown user>'
+            else:
+                # decode and remove line breaks from whoami's
+                out = out.decode().replace('\n', '').replace('\r', '')
+                # split the `who am i`
+                out = out.split()[0]
+            log.info('OS User %s executed LocalCKAN: ckanapi %s',
+                     out, ' '.join(sys.argv[1:]))
 
     stdout = getattr(sys.stdout, 'buffer', sys.stdout)
     if arguments['action']:
         try:
             for r in action(ckan, arguments):
                 stdout.write(r)
             return
```

### Comparing `ckanapi-4.7/ckanapi/cli/paster.py` & `ckanapi-4.8/ckanapi/cli/paster.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/cli/search.py` & `ckanapi-4.8/ckanapi/cli/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,7 +75,10 @@
         rows = result['results']
         for r in rows:
             jsonl_output.write(compact_json(r, sort_keys=True) + b'\n')
         if not rows or 'rows' in action_args:
             break
 
         start += len(rows)
+
+    if jsonl_output != stdout:
+        jsonl_output.close()
```

### Comparing `ckanapi-4.7/ckanapi/cli/utils.py` & `ckanapi-4.8/ckanapi/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """
 useful bits of code not tied to ckanapi in any way
 """
 
 import time
 
-PYTHON2 = str is bytes
-if PYTHON2:
-    # we need indent= and sort_keys=
-    import simplejson as json
-else:
-    import json
+import simplejson as json
 from contextlib import contextmanager
 
 
 def completion_stats(window=1):
     """
     Generate completions/second reports on each iteration.
```

### Comparing `ckanapi-4.7/ckanapi/cli/action.py` & `ckanapi-4.8/ckanapi/cli/action.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/cli/delete.py` & `ckanapi-4.8/ckanapi/cli/delete.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/cli/dump.py` & `ckanapi-4.8/ckanapi/cli/dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import sys
 import gzip
 import json
 from datetime import datetime
 import os
 
-from ckanapi.errors import (NotFound, NotAuthorized, ValidationError,
+from ckanapi.errors import (CKANAPIError, NotFound, NotAuthorized, ValidationError,
     SearchIndexError)
 from ckanapi.cli import workers
 from ckanapi.cli.utils import completion_stats, compact_json, \
     quiet_int_pipe
 from ckanapi.datapackage import create_datapackage, \
     populate_datastore_res_fields
 
@@ -113,14 +113,16 @@
             while expecting_number in results:
                 record = results.pop(expecting_number)
                 if record:
                     # sort keys so we can diff output
                     jsonl_output.write(compact_json(record,
                         sort_keys=True) + b'\n')
                 expecting_number += 1
+    if jsonl_output != stdout:
+        jsonl_output.close()
     if 'pipe' in errors:
         return 1
     if 'interrupt' in errors:
         return 2
 
 
 def dump_things_worker(ckan, thing, arguments,
@@ -169,26 +171,34 @@
             reply('UnicodeDecodeError')
             continue
 
         try:
             requests_kwargs = None
             if arguments['--insecure']:
                 requests_kwargs = {'verify': False}
+            include_users = False
+            if '--include-users' in arguments \
+            and arguments['--include-users']:
+                include_users = True
             obj = ckan.call_action(thing_show, {'id': name,
                 'include_datasets': False,
                 'include_password_hash': True,
+                'include_users': include_users,
                 }, requests_kwargs=requests_kwargs)
         except NotFound:
             reply('NotFound')
         except NotAuthorized:
             reply('NotAuthorized')
         else:
             if thing == 'datasets' and arguments['--datastore-fields']:
                 for res in obj.get('resources', []):
                     populate_datastore_res_fields(ckan, res)
+            if thing == 'datasets' and arguments['--resource-views']:
+                for res in obj.get('resources', []):
+                    populate_res_views(ckan, res)
             reply(None, obj)
 
 def _worker_command_line(thing, arguments):
     """
     Create a worker command line suitable for Popen with only the
     options the worker process requires
     """
@@ -202,9 +212,30 @@
         ['ckanapi', 'dump', thing, '--worker']
         + a('--config')
         + a('--ckan-user')
         + a('--remote')
         + a('--apikey')
         + b('--get-request')
         + b('--datastore-fields')
+        + b('--resource-views')
+        + b('--include-users')
         + ['value-here-to-make-docopt-happy']
         )
+
+
+def populate_res_views(ckan, res):
+    """
+    update resource dict in-place with resource_view_list values
+    in every resource with views using ckan LocalCKAN/RemoteCKAN instance
+    """
+    try:
+        views = ckan.call_action('resource_view_list', {
+            'id': res['id'],
+            'limit':0})
+    except CKANAPIError:
+        return
+    except NotFound:
+        return  # with localckan we'll get the real CKAN exception not a CKANAPIError subclass
+    if not views:
+        return # return if the resource views list is empty
+    res['resource_views'] = views
+
```

### Comparing `ckanapi-4.7/ckanapi/cli/load.py` & `ckanapi-4.8/ckanapi/cli/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,24 @@
     processes = int(arguments['--processes'])
     if hasattr(ckan, 'parallel_limit'):
         # add your sites to CKANAPI_MY_SITES instead of removing
         processes = min(processes, ckan.parallel_limit)
     stats = completion_stats(processes)
     pool = worker_pool(cmd, processes, line_reader())
 
+    failures = 0
     with quiet_int_pipe() as errors:
         for job_ids, finished, result in pool:
             if not result:
                 # child exited with traceback
                 return 1
             timestamp, action, error, response = json.loads(
                 result.decode('utf-8'))
+            if error:
+                failures += 1
 
             if not arguments['--quiet']:
                 stderr.write(('%s %s %s %s %s %s\n' % (
                     finished,
                     job_ids,
                     next(stats),
                     action,
@@ -106,14 +109,16 @@
                     response,
                     ]) + b'\n')
                 log.flush()
     if 'pipe' in errors:
         return 1
     if 'interrupt' in errors:
         return 2
+    if failures:
+        return 3
 
 
 def load_things_worker(ckan, thing, arguments,
         stdin=None, stdout=None):
     """
     a process that accepts lines of json on stdin which is parsed and
     passed to the {thing}_create/update actions.  it produces lines of json
@@ -176,14 +181,15 @@
                 name = obj.get('id')
                 if name:
                     try:
                         existing = ckan.call_action(thing_show,
                             {'id': name,
                              'include_datasets': False,
                              'include_password_hash': True,
+                             'include_users': True,
                             },
                             requests_kwargs=requests_kwargs)
                     except NotFound:
                         pass
                     except NotAuthorized as e:
                         reply('show', 'NotAuthorized', unicode(e))
                         continue
```

### Comparing `ckanapi-4.7/ckanapi/cli/workers.py` & `ckanapi-4.8/ckanapi/cli/workers.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/tests/test_cli_load.py` & `ckanapi-4.8/ckanapi/tests/test_cli_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.stderr = BytesIO()
 
     def test_create_with_no_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "45","title":"Forty-five"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'create')
@@ -80,15 +80,15 @@
         self.assertEqual(data, 'something-new')
 
     def test_create_with_corrupted_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "45","title":"Forty-five","resources":[{"id":"123"}]}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'create')
@@ -96,15 +96,15 @@
         self.assertEqual(data, 'something-new')
 
     def test_create_with_complete_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(
                  b'{"name": "45","title":"Forty-five",'
                  b'"resources":[{"id":"123","url_type":"","url":"http://example.com"}]}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
@@ -114,15 +114,15 @@
         self.assertEqual(data, 'something-new')
 
     def test_create_only(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': True,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "45","title":"Forty-five"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'create')
@@ -130,45 +130,45 @@
         self.assertEqual(data, 'something-new')
 
     def test_create_empty_dict(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'create')
         self.assertEqual(error, None)
         self.assertEqual(data, 'something-new')
 
     def test_create_bad_option(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': True,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "45","title":"Forty-five"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'show')
         self.assertEqual(error, 'NotFound')
         self.assertEqual(data, [None, '45'])
 
     def test_update_with_no_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "30ish","title":"3.4 times ten"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -176,15 +176,15 @@
         self.assertEqual(data, 'something-updated')
 
     def test_update_with_corrupted_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "30ish","title":"3.4 times ten","resources":[{"id":"123"}]}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -192,15 +192,15 @@
         self.assertEqual(data, 'something-updated')
 
     def test_update_with_complete_resources(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(
                  b'{"name": "30ish","title":"3.4 times ten",'
                  b'"resources":[{"id":"123","url_type":"","url":"http://example.com"}]}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
@@ -210,15 +210,15 @@
         self.assertEqual(data, 'something-updated')
 
     def test_update_only(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': True,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "34","title":"3.4 times ten"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -226,15 +226,15 @@
         self.assertEqual(data, 'something-updated')
 
     def test_update_bad_option(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': True,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "34","title":"3.4 times ten"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'create')
@@ -242,15 +242,15 @@
         self.assertEqual(data, {'name': 'That URL is already in use.'})
 
     def test_update_unauthorized(self):
         load_things_worker(self.ckan, 'datasets', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"name": "seekrit", "title": "Things"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'show')
@@ -258,15 +258,15 @@
         self.assertEqual(data, 'naughty user')
 
     def test_update_group(self):
         load_things_worker(self.ckan, 'groups', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"id": "ab","title":"a balloon"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -274,15 +274,15 @@
         self.assertEqual(data, 'group-updated')
 
     def test_update_organization_two(self):
         load_things_worker(self.ckan, 'organizations', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(
                 b'{"name": "cd", "title": "Go"}\n'
                 b'{"name": "ef", "title": "Play"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response.count(b'\n'), 2, response)
@@ -298,15 +298,15 @@
         self.assertEqual(data, 'org-created')
 
     def test_update_organization_with_users_unchanged(self):
         load_things_worker(self.ckan, 'organizations', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"id": "used", "title": "here"}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -314,15 +314,15 @@
         self.assertEqual(data, 'users-unchanged')
 
     def test_update_organization_with_users_cleared(self):
         load_things_worker(self.ckan, 'organizations', {
                 '--create-only': False,
                 '--update-only': False,
                 '--upload-resources': False,
-                '--insecure': False
+                '--insecure': False,
                 },
             stdin=BytesIO(b'{"id": "unused", "users": []}\n'),
             stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, action, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(action, 'update')
@@ -343,15 +343,15 @@
                 '--input': None,
                 '--create-only': False,
                 '--update-only': False,
                 '--start-record': '1',
                 '--max-records': None,
                 '--upload-resources': False,
                 '--upload-logo': False,
-                '--insecure': False
+                '--insecure': False,
             },
             worker_pool=self._mock_worker_pool,
             stdin=BytesIO(
                 b'{"name": "cd", "title": "Go"}\n'
                 b'{"name": "ef", "title": "Play"}\n'
                 ),
             stdout=self.stdout,
@@ -378,15 +378,15 @@
                 '--input': None,
                 '--create-only': False,
                 '--update-only': False,
                 '--start-record': '2',
                 '--max-records': '2',
                 '--upload-resources': False,
                 '--upload-logo': False,
-                '--insecure': False
+                '--insecure': False,
             },
             worker_pool=self._mock_worker_pool,
             stdin=BytesIO(
                 b'{"name": "cd", "title": "Go"}\n'
                 b'{"name": "ef", "title": "Play"}\n'
                 b'{"name": "gh", "title": "Hotel"}\n'
                 b'{"name": "ij", "title": "Ambient"}\n'
@@ -416,15 +416,15 @@
                 '--input': None,
                 '--create-only': False,
                 '--update-only': False,
                 '--start-record': '1',
                 '--max-records': None,
                 '--upload-resources': False,
                 '--upload-logo': False,
-                '--insecure': False
+                '--insecure': False,
             },
             worker_pool=self._mock_worker_pool,
             stdin=BytesIO(
                 b'{"name": "cd", "title": "Go"}\n'
                 b'{"name": "ef", "title": "Play"}\n'
                 ),
             stdout=self.stdout,
```

### Comparing `ckanapi-4.7/ckanapi/tests/mock/mock_ckan.py` & `ckanapi-4.8/ckanapi/tests/mock/mock_ckan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import json
 import cgi
 import csv
 from wsgiref.util import setup_testing_defaults
 from wsgiref.simple_server import make_server
+try:
+    from cStringIO import StringIO
+except ImportError:
+    from io import StringIO
+
 
 def mock_ckan(environ, start_response):
     status = '200 OK'
     headers = [
         ('Content-type', 'application/json;charset=utf-8'),
         ]
     if environ['PATH_INFO'] == '/api/action/site_read':
@@ -35,15 +40,22 @@
             }).encode('utf-8')]
     if environ['PATH_INFO'] == '/api/action/test_upload':
         fs = cgi.FieldStorage(
             fp=environ['wsgi.input'],
             environ=environ,
             keep_blank_values=True,
             )
-        records = list(csv.reader(fs['upload'].file))
+        upload_data = fs.getvalue('upload').decode('utf-8').splitlines()
+        csv_file = StringIO()
+        writer = csv.writer(csv_file)
+        for line_data in upload_data:
+            row_data = line_data.split(',')
+            writer.writerow(row_data)
+        csv_file.seek(0)
+        records = list(csv.reader(csv_file))
         start_response(status, headers)
         return [json.dumps({
             "help": "none",
             "success": True,
             "result": {
                 'option': fs.getvalue('option'),
                 'last_row': records[-1],
```

### Comparing `ckanapi-4.7/ckanapi/tests/test_testapp.py` & `ckanapi-4.8/ckanapi/tests/test_testapp.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/tests/test_remote.py` & `ckanapi-4.8/ckanapi/tests/test_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 5,sasquach
 """.lstrip()
 
 class TestRemoteAction(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         script = os.path.join(os.path.dirname(__file__), 'mock/mock_ckan.py')
-        _mock_ckan = subprocess.Popen(['python2', script],
+        _mock_ckan = subprocess.Popen(['python', script],
             stdout=DEVNULL, stderr=DEVNULL)
         def kill_child():
             try:
                 _mock_ckan.kill()
                 _mock_ckan.wait()
             except OSError:
                 pass  # alread cleaned up from tearDownClass
```

### Comparing `ckanapi-4.7/ckanapi/tests/test_cli_dump.py` & `ckanapi-4.8/ckanapi/tests/test_cli_dump.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,39 +46,50 @@
                         {'fields': [{
                             'id': 'col1',
                             'type': 'text',
                             'info': {
                                 'label': 'Column One',
                                 'notes': 'Description One',
                             }}]}},
+                'resource_view_list': {
+                    'd902fafc-5717-4dd0-87f2-7a6fc96989b7': [{
+                            'description': 'Test view',
+                            'filterable': True,
+                            'id': 'd902fafc-5717-4dd0-87f2-7a6fc96989d9',
+                            'package_id': 'dp',
+                            'resource_id': 'd902fafc-5717-4dd0-87f2-7a6fc96989b7',
+                            'responsive': True,
+                            'show_fields': ['_id']}]},
             }[name][data_dict.get('id') or data_dict.get('resource_id')]
         except KeyError:
             raise NotFound()
 
 
 class TestCLIDump(unittest.TestCase):
     def setUp(self):
         self.ckan = MockCKAN()
         self.stdout = BytesIO()
         self.stderr = BytesIO()
 
     def test_worker_one(self):
         rval = dump_things_worker(self.ckan, 'datasets',
             {'--datastore-fields': False,
+             '--resource-views': False,
              '--insecure': False},
             stdin=BytesIO(b'"34"\n'), stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response[-1:], b'\n')
         timstamp, error, data = json.loads(response.decode('UTF-8'))
         self.assertEqual(error, None)
         self.assertEqual(data["title"], "Thirty-four")
 
     def test_worker_two(self):
         rval = dump_things_worker(self.ckan, 'datasets',
             {'--datastore-fields': False,
+             '--resource-views': False,
              '--insecure': False},
             stdin=BytesIO(b'"12"\n"34"\n'), stdout=self.stdout)
         response = self.stdout.getvalue()
         self.assertEqual(response.count(b'\n'), 2, response)
         self.assertEqual(response[-1:], b'\n')
         r1, r2 = response.split(b'\n', 1)
         timstamp, error, data = json.loads(r1.decode('UTF-8'))
@@ -130,15 +141,17 @@
                 '--output': None,
                 '--datapackages': None,
                 '--gzip': False,
                 '--all': True,
                 '--processes': '1',
                 '--get-request': False,
                 '--datastore-fields': False,
-                '--insecure': False
+                '--resource-views': False,
+                '--insecure': False,
+                '--include-users': False,
             },
             worker_pool=self._mock_worker_pool,
             stdout=self.stdout,
             stderr=self.stderr)
         self.assertEqual(self.worker_cmd, [
             'ckanapi', 'dump', 'datasets', '--worker',
             'value-here-to-make-docopt-happy'])
@@ -160,15 +173,17 @@
                 '--datapackages': None,
                 '--gzip': False,
                 '--all': False,
                 'ID_OR_NAME': ['12'],
                 '--processes': '5',
                 '--get-request': False,
                 '--datastore-fields': False,
-                '--insecure': False
+                '--resource-views': False,
+                '--insecure': False,
+                '--include-users': False,
             },
             worker_pool=self._mock_worker_pool,
             stdout=self.stdout,
             stderr=self.stderr)
         self.assertEqual(self.worker_cmd, [
             'ckanapi', 'dump', 'datasets', '--worker',
             'value-here-to-make-docopt-happy'])
@@ -187,15 +202,17 @@
                 '--datapackages': None,
                 '--gzip': False,
                 '--all': False,
                 'ID_OR_NAME': ['ab'],
                 '--processes': '1',
                 '--get-request': False,
                 '--datastore-fields': False,
-                '--insecure': False
+                '--resource-views': False,
+                '--insecure': False,
+                '--include-users': False,
             },
 
             worker_pool=self._mock_worker_pool,
             stdout=self.stdout,
             stderr=self.stderr)
         self.assertEqual(self.worker_cmd, [
             'ckanapi', 'dump', 'groups', '--worker',
@@ -216,15 +233,17 @@
                 '--datapackages': None,
                 '--gzip': False,
                 '--all': False,
                 'ID_OR_NAME': ['P', 'Q', 'R', 'S'],
                 '--processes': '1',
                 '--get-request': False,
                 '--datastore-fields': False,
-                '--insecure': False
+                '--resource-views': False,
+                '--insecure': False,
+                '--include-users': False,
             },
             worker_pool=self._mock_worker_pool_reversed,
             stdout=self.stdout,
             stderr=self.stderr)
         self.assertEqual(self.worker_cmd, [
             'ckanapi', 'dump', 'organizations', '--worker',
             'value-here-to-make-docopt-happy'])
@@ -249,15 +268,17 @@
                     '--output': None,
                     '--datapackages': target,
                     '--gzip': False,
                     '--all': True,
                     '--processes': '1',
                     '--get-request': False,
                     '--datastore-fields': False,
-                    '--insecure': False
+                    '--resource-views': False,
+                    '--insecure': False,
+                    '--include-users': False,
                 },
                 worker_pool=self._worker_pool_with_data,
                 stdout=self.stdout,
                 stderr=self.stderr)
             assert exists(target + '/twelve/datapackage.json')
             assert exists(target + '/thirtyfour/datapackage.json')
             assert exists(target + '/dp/datapackage.json')
@@ -282,14 +303,68 @@
                     }
                 }]
             })
         finally:
             shutil.rmtree(target)
 
 
+    def test_resource_views(self):
+        target = tempfile.mkdtemp()
+        try:
+            dump_things(self.ckan, 'datasets', {
+                    'ID_OR_NAME': ['dp'],
+                    '--quiet': False,
+                    '--ckan-user': None,
+                    '--config': None,
+                    '--remote': None,
+                    '--apikey': None,
+                    '--worker': False,
+                    '--log': None,
+                    '--output': target + '/dpf.jsonl',
+                    '--datapackages': None,
+                    '--gzip': False,
+                    '--all': False,
+                    '--processes': '1',
+                    '--get-request': False,
+                    '--datastore-fields': False,
+                    '--resource-views': True,
+                    '--insecure': False,
+                    '--include-users': False,
+                },
+                worker_pool=self._worker_pool_with_resource_views,
+                stdout=self.stdout,
+                stderr=self.stderr)
+            assert exists(target + '/dpf.jsonl')
+            with open(target + '/dpf.jsonl') as dpf:
+                dp = json.load(dpf)
+            self.assertEqual(dp, {
+                'id': 'dp',
+                'name': 'dp',
+                'title': 'Test for datapackage',
+                'resources': [{
+                    'name': 'resource1',
+                    'format': 'csv',
+                    'id': 'd902fafc-5717-4dd0-87f2-7a6fc96989b7',
+                    'url': 'https://google.com',
+                    'datastore_active': True,
+                    'resource_views': [{
+                        'description': 'Test view',
+                        'filterable': True,
+                        'id': 'd902fafc-5717-4dd0-87f2-7a6fc96989d9',
+                        'package_id': 'dp',
+                        'resource_id': 'd902fafc-5717-4dd0-87f2-7a6fc96989b7',
+                        'responsive': True,
+                        'show_fields': ['_id']
+                    }]
+                }]
+            })
+        finally:
+            shutil.rmtree(target)
+
+
     def _mock_worker_pool(self, cmd, processes, job_iter):
         self.worker_cmd = cmd
         self.worker_processes = processes
         self.worker_jobs = list(job_iter)
         for i, j in self.worker_jobs:
             jname = json.loads(j.decode('UTF-8'))
             yield [[], i, json.dumps(['some-date', None, {'id': jname}]
@@ -300,12 +375,28 @@
             self._mock_worker_pool(cmd, processes, job_iter)))
 
     def _worker_pool_with_data(self, cmd, processes, job_iter):
         worker_stdin = BytesIO(b''.join(v for i, v in job_iter))
         worker_stdout = BytesIO()
         dump_things_worker(self.ckan, 'datasets', {
             '--datastore-fields': True,
-            '--insecure': False},
+            '--resource-views': False,
+            '--insecure': False,
+            '--include-users': False,},
+            stdin=worker_stdin,
+            stdout=worker_stdout)
+        for i, v in enumerate(worker_stdout.getvalue().strip().split(b'\n')):
+            yield [[], i, v]
+
+
+    def _worker_pool_with_resource_views(self, cmd, proccesses, job_iter):
+        worker_stdin = BytesIO(b''.join(v for i, v in job_iter))
+        worker_stdout = BytesIO()
+        dump_things_worker(self.ckan, 'datasets', {
+            '--datastore-fields': False,
+            '--resource-views': True,
+            '--insecure': False,
+            '--include-users': False,},
             stdin=worker_stdin,
             stdout=worker_stdout)
         for i, v in enumerate(worker_stdout.getvalue().strip().split(b'\n')):
             yield [[], i, v]
```

### Comparing `ckanapi-4.7/ckanapi/tests/test_cli_action.py` & `ckanapi-4.8/ckanapi/tests/test_cli_action.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/tests/test_cli_workers.py` & `ckanapi-4.8/ckanapi/tests/test_cli_workers.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/tests/test_call.py` & `ckanapi-4.8/ckanapi/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `ckanapi-4.7/ckanapi/tests/test_datapackage.py` & `ckanapi-4.8/ckanapi/tests/test_datapackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,16 @@
         filename = 'image_saved.png'
         os.makedirs('/test/data')
         stderr = BytesIO()
         # TODO mock the HTTP request to example.com
 
         returned_resource = create_resource(
             resource, filename='image_saved.png',
-            datapackage_dir='/test', stderr=stderr)
+            datapackage_dir='/test', stderr=stderr,
+            apikey='')
 
         stderr.seek(0)
         assert not stderr.read()
         assert returned_resource == {
             u'url': u'http://example.com/image.png',
             u'name': u'Image',
             u'format': u'PNG',
@@ -225,15 +226,15 @@
         }
         stderr = BytesIO()
         os.makedirs('/test/data')
         # TODO mock the HTTP request to example.com
 
         datapackage_dir, datapackage, json_path = \
             create_datapackage(record=dataset, base_path='/test/',
-                               stderr=stderr)
+                               stderr=stderr, apikey='')
 
         stderr.seek(0)
         assert not stderr.read()
         assert datapackage_dir == u'/test/test_dataset_00'
         assert datapackage == {
             u'name': u'test_dataset_00',
             u'description': u'Just another test dataset.',
```

### Comparing `ckanapi-4.7/ckanapi.egg-info/SOURCES.txt` & `ckanapi-4.8/ckanapi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+COPYING
+COPYING.fr
 README.md
 setup.py
 ckanapi/__init__.py
 ckanapi/common.py
 ckanapi/datapackage.py
 ckanapi/errors.py
 ckanapi/localckan.py
@@ -9,15 +11,14 @@
 ckanapi/testappckan.py
 ckanapi/version.py
 ckanapi.egg-info/PKG-INFO
 ckanapi.egg-info/SOURCES.txt
 ckanapi.egg-info/dependency_links.txt
 ckanapi.egg-info/entry_points.txt
 ckanapi.egg-info/not-zip-safe
-ckanapi.egg-info/pbr.json
 ckanapi.egg-info/requires.txt
 ckanapi.egg-info/top_level.txt
 ckanapi/cli/__init__.py
 ckanapi/cli/action.py
 ckanapi/cli/batch.py
 ckanapi/cli/ckan_click.py
 ckanapi/cli/delete.py
```

### Comparing `ckanapi-4.7/README.md` & `ckanapi-4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 ## ckanapi
 
 A command line interface and Python module for accessing the
 [CKAN Action API](http://docs.ckan.org/en/latest/api/index.html#action-api-reference)
 
-[![Build Status](https://travis-ci.org/ckan/ckanapi.png?branch=master)](https://travis-ci.org/ckan/ckanapi) tested under Python 2.7, 3.6 and pypy
-
 - [Installation](https://github.com/ckan/ckanapi/blob/master/README.md#installation)
 - [ckanapi CLI](https://github.com/ckan/ckanapi/blob/master/README.md#ckanapi-cli)
   - [Actions](https://github.com/ckan/ckanapi/blob/master/README.md#actions)
   - [Action Arguments](https://github.com/ckan/ckanapi/blob/master/README.md#action-arguments)
   - [Bulk Dumping and Loading](https://github.com/ckan/ckanapi/blob/master/README.md#bulk-dumping-and-loading)
   - [Bulk Delete](https://github.com/ckan/ckanapi/blob/master/README.md#bulk-delete)
   - [Bulk Dataset and Resource Export](https://github.com/ckan/ckanapi/edit/master/README.md#bulk-dataset-and-resource-export---datapackagejson-format)
@@ -160,15 +158,15 @@
 text files and created or updated from JSON lines text files.
 
 `dump` and `load` jobs can be run in parallel with
 multiple worker processes using the `-p` parameter. The jobs in progress,
 the rate of job completion and any individual errors are shown on STDERR
 while the jobs run.
 
-There are no parallel limits when running against a CKAN on localhost.  
+There are no parallel limits when running against a CKAN on localhost.
 When running against a remote site, there's a default limit of 3 worker processes.
 
 The environment variables `CKANAPI_MY_SITES` and`CKANAPI_PARALLEL_LIMIT` can be
 used to adjust these limits.  `CKANAPI_MY_SITES` (comma-delimited list of CKAN urls)
 will not have the `PARALLEL_LIMIT` applied.
 
 `dump` and `load` jobs may be resumed from the last completed
@@ -350,15 +348,15 @@
 ```python
 from ckanapi import RemoteCKAN
 ua = 'ckanapiexample/1.0 (+http://example.com/my/website)'
 
 demo = RemoteCKAN('https://demo.ckan.org', user_agent=ua)
 packages = demo.action.package_search(q='+organization:sample-organization +res_format:GeoJSON +tags:geojson')
 print(packages)
-```  
+```
 
 Many CKAN API functions can only be used by authenticated users. Use the
 `apikey` parameter to supply your CKAN API key to `RemoteCKAN`:
 
     demo = RemoteCKAN('https://demo.ckan.org', apikey='MY-SECRET-API-KEY')
 
 An example of updating a single field in an existing dataset can be seen in the [Examples directory](examples/update_single_field.py)
@@ -461,14 +459,28 @@
 ```python
 from ckanapi import LocalCKAN
 
 anon = LocalCKAN(username='')
 print(anon.action.status_show())
 ```
 
+#### Extra Loggging
+
+To enable extra info logging for the execution of LocalCKAN ckanapi commands, you can enable the config option in your CKAN INI file.
+
+```
+ckanapi.log_local = True
+```
+
+The output of the log will look like:
+
+```
+INFO [ckan.ckanapi] OS User <user> executed LocalCKAN: ckanapi <args>
+```
+
 ### TestAppCKAN
 
 A class is provided for making action requests to a
 [webtest.TestApp](http://webtest.readthedocs.org/en/latest/testapp.html)
 instance for use in CKAN tests:
 
 ```python
```

