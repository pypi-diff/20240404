# Comparing `tmp/heaserver-activity-1.0.3.tar.gz` & `tmp/heaserver-activity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-activity-1.0.3.tar", last modified: Thu Jan  4 20:39:52 2024, max compression
+gzip compressed data, was "heaserver-activity-1.1.0.tar", last modified: Wed Apr  3 23:39:34 2024, max compression
```

## Comparing `heaserver-activity-1.0.3.tar` & `heaserver-activity-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.221254 heaserver-activity-1.0.3/
--rw-rw-rw-   0        0        0    11625 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       39 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4841 2024-01-04 20:39:52.220252 heaserver-activity-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2024-01-04 17:57:20.000000 heaserver-activity-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-01-04 20:39:52.221254 heaserver-activity-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1823 2024-01-04 20:39:15.000000 heaserver-activity-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.130552 heaserver-activity-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.129553 heaserver-activity-1.0.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.153705 heaserver-activity-1.0.3/src/heaserver/activity/
--rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/src/heaserver/activity/__init__.py
--rw-rw-rw-   0        0        0    15062 2023-12-28 18:34:41.000000 heaserver-activity-1.0.3/src/heaserver/activity/service.py
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.154706 heaserver-activity-1.0.3/src/heaserver/activity/wstl/
--rw-rw-rw-   0        0        0     7666 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/src/heaserver/activity/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.219252 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/
--rw-rw-rw-   0        0        0     4841 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      871 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-04 20:39:52.000000 heaserver-activity-1.0.3/src/heaserver_activity.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.131799 heaserver-activity-1.0.3/tests/
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.131799 heaserver-activity-1.0.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.206922 heaserver-activity-1.0.3/tests/heaserver/activitytest/
--rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 20:39:52.217255 heaserver-activity-1.0.3/tests/heaserver/activitytest/__pycache__/
--rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088
--rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284
--rw-rw-rw-   0        0        0     2983 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/permissionstestcase.py
--rw-rw-rw-   0        0        0      249 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/test_all.py
--rw-rw-rw-   0        0        0      338 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     8541 2023-12-18 19:13:06.000000 heaserver-activity-1.0.3/tests/heaserver/activitytest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.818362 heaserver-activity-1.1.0/
+-rw-rw-rw-   0        0        0    11625 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4982 2024-04-03 23:39:34.817003 heaserver-activity-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3663 2024-04-03 21:31:38.000000 heaserver-activity-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 23:39:34.818362 heaserver-activity-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2024-04-03 23:38:58.000000 heaserver-activity-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.708037 heaserver-activity-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.707017 heaserver-activity-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.733002 heaserver-activity-1.1.0/src/heaserver/activity/
+-rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/src/heaserver/activity/__init__.py
+-rw-rw-rw-   0        0        0    15003 2024-04-03 21:16:46.000000 heaserver-activity-1.1.0/src/heaserver/activity/service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.743002 heaserver-activity-1.1.0/src/heaserver/activity/wstl/
+-rw-rw-rw-   0        0        0     7666 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/src/heaserver/activity/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.816002 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/
+-rw-rw-rw-   0        0        0     4982 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      871 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.709008 heaserver-activity-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.709008 heaserver-activity-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.804003 heaserver-activity-1.1.0/tests/heaserver/activitytest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.814005 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284
+-rw-rw-rw-   0        0        0     2983 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     2482 2024-04-03 16:54:29.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/test_all.py
+-rw-rw-rw-   0        0        0      338 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     8546 2024-04-03 17:54:33.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/testcase.py
```

### Comparing `heaserver-activity-1.0.3/LICENSE` & `heaserver-activity-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/PKG-INFO` & `heaserver-activity-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.0.3
+Version: 1.1.0
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.2
+Requires-Dist: heaserver~=1.1.3
 
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.0
+* Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Actually send received desktop objects over any web socket connections.
 * Paginate desktop object actions correctly.
```

### Comparing `heaserver-activity-1.0.3/README.md` & `heaserver-activity-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.0
+* Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Actually send received desktop objects over any web socket connections.
 * Paginate desktop object actions correctly.
```

### Comparing `heaserver-activity-1.0.3/setup.py` & `heaserver-activity-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-activity',
-    version='1.0.3',
+    version='1.1.0',
     description="A service for tracking activity in hea",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.activity'],
     package_data={'heaserver.activity': ['wstl/*.json']},
-    install_requires=['heaserver~=1.0.2'],
+    install_requires=['heaserver~=1.1.3'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-activity-1.0.3/src/heaserver/activity/service.py` & `heaserver-activity-1.1.0/src/heaserver/activity/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from aiohttp import WSMsgType
 from asyncio import gather, TimeoutError as AsyncioTimeoutError
 from datetime import datetime
 import logging
 
 MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION = 'desktopobjectactions'
 
-_wsresponses: dict[web.WebSocketResponse, web.Request] = {}
+_wsresponses: dict[web.WebSocketResponse, tuple[web.Request, list[str]]] = {}
 
 @routes.get('/recentlyaccessedviewsping')
 async def ping(request: web.Request) -> web.Response:
     """
     Checks if this service is running.
 
     :param request: the HTTP request.
@@ -62,15 +62,16 @@
       '404':
         $ref: '#/components/responses/404'
     """
     logger = logging.getLogger(__name__)
     begin = int(request.query.get('begin', 0))
     end_str = request.query.get('end', None)
     end = int(end_str) if end_str else None
-    volume_ids = request.query.getall('volume_id', [])
+    empty_list_of_string: list[str] = []
+    volume_ids = request.query.getall('volume_id', empty_list_of_string)
     sub = request.headers.get(SUB, NONE_USER)
     type_name = request.match_info['type']
     logger.debug('Requested recent accesses')
     if volume_ids:
         volume_id_query = {'$or': [{'new_volume_id': {'$exists': False}}, {'new_volume_id': {'$in': volume_ids + [None]}}]}
     else:
         volume_id_query = {}
@@ -196,44 +197,38 @@
     sort = request.query.get('sort', None)
     if sort is None:
         sort_int = None
     else:
         if sort != 'asc' and sort != 'desc':
             return await response.status_bad_request(f'sort may be asc or desc but was {sort}')
         sort_int = 1 if sort == 'asc' else -1
-
-    return await mongoservicelib.get_all(request, MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION, sort={'status_updated': sort_int} if sort_int is not None else None)
+    exclude_codes = request.query.getall('excludecode', None)
+    return await mongoservicelib.get_all(request, MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION,
+                                         mongoattributes={'code': {'$nin': exclude_codes}} if exclude_codes else None,
+                                         sort={'status_updated': sort_int} if sort_int is not None else None)
 
 
 @routes.get('/desktopobjectactionsupdatelistener')
 async def websocket_handler(request: web.Request) -> web.Response:
     logger = logging.getLogger(__name__)
     count = request.query.get('count', None)
     if count is not None:
         try:
             count_ = int(count)
         except TypeError as e:
             return response.status_bad_request(str(e))
         if count_ < 0:
             return response.status_bad_request(f'count must be non-negative but was {count_}')
-    else:
-        count_ = None
+
+    exclude_codes = request.query.getall('excludecode', [])
 
     wsresponse = web.WebSocketResponse()
     await wsresponse.prepare(request)
     try:
-        # if count_ is None or count_:
-        #     async for index, data in enumerate(mongoservicelib.get_all_gen(request, MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION)):
-        #         logger.debug('Sending %s', data)
-        #         msg, mime_type = await _to_format(request, data)
-        #         logger.debug('Converted to %s: %s', mime_type, msg)
-        #         await wsresponse.send_str(msg)
-        #         if count_ is not None and index >= count_ - 1:
-        #             break
-        _wsresponses[wsresponse] = request
+        _wsresponses[wsresponse] = (request, exclude_codes)
         while True:
             if wsresponse.closed:
                 logger.debug('Web socket response is closed!')
                 break
             try:
                 msg = await wsresponse.receive(timeout=5)
                 if msg.type == WSMsgType.TEXT and msg.data == '__ping__':
@@ -246,15 +241,15 @@
             if not wsresponse.closed:
                 await wsresponse.close()
         finally:
             if wsresponse in _wsresponses:
                 del _wsresponses[wsresponse]
 
 
-async def desktop_object_action_cb(app: web.Application, desktop_object: DesktopObject):
+async def desktop_object_action_cb(app: web.Application, desktop_object: DesktopObjectAction):
     """
     Callback for desktop object actions received from the message broker. Actions may be received by this callback
     repeatedly, possibly with an updated status. This callback cannot assume that it will receive an updated action
     reflecting REQUESTED and IN_PROGRESS status changes, though all status transitions will be reflected in the
     action's attributes. It can assume that it will receive an updated action reflecting the action's final status,
     SUCCEEDED or FAILED.
 
@@ -281,15 +276,17 @@
         desktop_object.id = result
     logger.debug('Desktop object saved: %s', desktop_object)
 
     desktop_object_dict = desktop_object.to_dict()
     if _wsresponses:
         logger.debug('Sending update %s', desktop_object_dict)
         gather_responses = []
-        for wsresponse, request in _wsresponses.items():
+        for wsresponse, (request, excludecodes) in _wsresponses.items():
+            if desktop_object.code in excludecodes:
+                continue
             sub = wsresponse.headers.get(SUB, NONE_USER)
             if desktop_object.has_permissions(sub, RESTPermissionGroup.GETTER_PERMS):
                 logger.debug('Sending update to %s', wsresponse)
                 if not wsresponse.closed:
                     logger.debug('%s is not closed', wsresponse)
                     async def wrapper():
                         try:
```

### Comparing `heaserver-activity-1.0.3/src/heaserver/activity/wstl/all.json` & `heaserver-activity-1.1.0/src/heaserver/activity/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/src/heaserver_activity.egg-info/PKG-INFO` & `heaserver-activity-1.1.0/src/heaserver_activity.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.0.3
+Version: 1.1.0
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.2
+Requires-Dist: heaserver~=1.1.3
 
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.0
+* Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
+
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
 * Actually send received desktop objects over any web socket connections.
 * Paginate desktop object actions correctly.
```

### Comparing `heaserver-activity-1.0.3/src/heaserver_activity.egg-info/SOURCES.txt` & `heaserver-activity-1.1.0/src/heaserver_activity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088` & `heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284` & `heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/tests/heaserver/activitytest/permissionstestcase.py` & `heaserver-activity-1.1.0/tests/heaserver/activitytest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.3/tests/heaserver/activitytest/testcase.py` & `heaserver-activity-1.1.0/tests/heaserver/activitytest/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         'old_object_uri': None,
         'new_object_uri': 'awss3projects/0123456789ab0123456789ab',
         'old_object_type_name': None,
         'new_object_type_name': AWSS3Project.get_type_name(),
         'old_object_id': None,
         'new_object_id': '0123456789ab0123456789ab',
         'application_id': None,
-        'code': None,
+        'code': 'hea-get',
         'duration': None,
         'ended': None,
         'human_readable_duration': None,
         'mime_type': 'application/x.desktopobjectaction',
         'new_volume_id': None,
         'old_volume_id': None,
         'requested': '2022-05-17T00:00:00-06:00',
```

