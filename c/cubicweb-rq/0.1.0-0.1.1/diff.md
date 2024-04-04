# Comparing `tmp/cubicweb-rq-0.1.0.tar.gz` & `tmp/cubicweb-rq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-rq-0.1.0.tar", last modified: Mon Jan  8 22:04:25 2024, max compression
+gzip compressed data, was "cubicweb-rq-0.1.1.tar", last modified: Thu Apr  4 08:40:28 2024, max compression
```

## Comparing `cubicweb-rq-0.1.0.tar` & `cubicweb-rq-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.957057 cubicweb-rq-0.1.0/
--rw-r--r--   0 murloc    (1000) murloc    (1000)      327 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/MANIFEST.in
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2793 2024-01-08 22:04:25.957057 cubicweb-rq-0.1.0/PKG-INFO
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2081 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/README.rst
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.949057 cubicweb-rq-0.1.0/cubicweb_rq/
--rw-r--r--   0 murloc    (1000) murloc    (1000)      751 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/__init__.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)      702 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/__pkginfo__.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1794 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/ccplugin.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     5366 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/entities.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)      861 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/hooks.py
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.953057 cubicweb-rq-0.1.0/cubicweb_rq/i18n/
--rw-r--r--   0 murloc    (1000) murloc    (1000)      248 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/i18n/en.po
--rw-r--r--   0 murloc    (1000) murloc    (1000)      248 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/i18n/es.po
--rw-r--r--   0 murloc    (1000) murloc    (1000)      248 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/i18n/fr.po
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.953057 cubicweb-rq-0.1.0/cubicweb_rq/migration/
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1083 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/migration/postcreate.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     4141 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/rq.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1176 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/schema.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)      873 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/cubicweb_rq/views.py
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.953057 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2793 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/PKG-INFO
--rw-r--r--   0 murloc    (1000) murloc    (1000)      613 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/SOURCES.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/dependency_links.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)       34 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/entry_points.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2024-01-08 20:10:13.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/not-zip-safe
--rw-r--r--   0 murloc    (1000) murloc    (1000)      100 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/requires.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)       12 2024-01-08 22:04:25.000000 cubicweb-rq-0.1.0/cubicweb_rq.egg-info/top_level.txt
--rw-r--r--   0 murloc    (1000) murloc    (1000)       38 2024-01-08 22:04:25.957057 cubicweb-rq-0.1.0/setup.cfg
--rw-r--r--   0 murloc    (1000) murloc    (1000)     2717 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/setup.py
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.953057 cubicweb-rq-0.1.0/test/
-drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2024-01-08 22:04:25.953057 cubicweb-rq-0.1.0/test/data/
--rw-r--r--   0 murloc    (1000) murloc    (1000)        3 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/test/data/bootstrap_cubes
--rw-r--r--   0 murloc    (1000) murloc    (1000)     4100 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/test/test_rq.py
--rw-r--r--   0 murloc    (1000) murloc    (1000)     1322 2024-01-08 10:39:20.000000 cubicweb-rq-0.1.0/tox.ini
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.670300 cubicweb-rq-0.1.1/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      327 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/MANIFEST.in
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     2793 2024-04-04 08:40:28.670300 cubicweb-rq-0.1.1/PKG-INFO
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     2081 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/README.rst
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.666967 cubicweb-rq-0.1.1/cubicweb_rq/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      752 2024-04-03 09:29:40.000000 cubicweb-rq-0.1.1/cubicweb_rq/__init__.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      701 2024-04-03 12:25:11.000000 cubicweb-rq-0.1.1/cubicweb_rq/__pkginfo__.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     1794 2024-04-03 08:17:49.000000 cubicweb-rq-0.1.1/cubicweb_rq/ccplugin.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     5535 2024-04-03 08:39:20.000000 cubicweb-rq-0.1.1/cubicweb_rq/entities.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      861 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/hooks.py
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.666967 cubicweb-rq-0.1.1/cubicweb_rq/i18n/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      248 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/i18n/en.po
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      248 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/i18n/es.po
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      248 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/i18n/fr.po
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.666967 cubicweb-rq-0.1.1/cubicweb_rq/migration/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     1083 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/migration/postcreate.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     4141 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/rq.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     1176 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/schema.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      873 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/cubicweb_rq/views.py
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.670300 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     2793 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/PKG-INFO
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      613 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/SOURCES.txt
+-rw-r--r--   0 alubert   (1000) alubert   (1000)        1 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/dependency_links.txt
+-rw-r--r--   0 alubert   (1000) alubert   (1000)       34 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/entry_points.txt
+-rw-r--r--   0 alubert   (1000) alubert   (1000)        1 2024-04-03 07:11:45.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/not-zip-safe
+-rw-r--r--   0 alubert   (1000) alubert   (1000)      100 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/requires.txt
+-rw-r--r--   0 alubert   (1000) alubert   (1000)       12 2024-04-04 08:40:28.000000 cubicweb-rq-0.1.1/cubicweb_rq.egg-info/top_level.txt
+-rw-r--r--   0 alubert   (1000) alubert   (1000)       38 2024-04-04 08:40:28.670300 cubicweb-rq-0.1.1/setup.cfg
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     2717 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/setup.py
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.666967 cubicweb-rq-0.1.1/test/
+drwxr-xr-x   0 alubert   (1000) alubert   (1000)        0 2024-04-04 08:40:28.666967 cubicweb-rq-0.1.1/test/data/
+-rw-r--r--   0 alubert   (1000) alubert   (1000)        3 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/test/data/bootstrap_cubes
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     4100 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/test/test_rq.py
+-rw-r--r--   0 alubert   (1000) alubert   (1000)     1322 2024-04-02 15:43:18.000000 cubicweb-rq-0.1.1/tox.ini
```

### Comparing `cubicweb-rq-0.1.0/PKG-INFO` & `cubicweb-rq-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-rq
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cube for starting RqJobs on a Rq worker
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/rq
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-rq-0.1.0/README.rst` & `cubicweb-rq-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/__init__.py` & `cubicweb-rq-0.1.1/cubicweb_rq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """cubicweb-rq application package
 
 Cube for starting RqJobs on a Rq worker
 """
+
 from sched import scheduler
 
 from cubicweb import repoapi
 from cubicweb.cwconfig import CubicWebConfiguration
 from cubicweb.cwctl import init_cmdline_log_threshold
 from cubicweb.server.repository import Repository
```

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/__pkginfo__.py` & `cubicweb-rq-0.1.1/cubicweb_rq/__pkginfo__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """cubicweb-rq application packaging information"""
 
-
 modname = "cubicweb_rq"
 distname = "cubicweb-rq"
 
-numversion = (0, 1, 0)
+numversion = (0, 1, 1)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Cube for starting RqJobs on a Rq worker"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/rq"
```

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/ccplugin.py` & `cubicweb-rq-0.1.1/cubicweb_rq/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/entities.py` & `cubicweb-rq-0.1.1/cubicweb_rq/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,43 +14,47 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """cubicweb-rq entity's classes"""
 
 import rq
-import redis
 
 from datetime import datetime
 
 from cubicweb import Binary
 
 from cubicweb.predicates import is_instance
 
 from cubicweb.server.hook import DataOperationMixIn, Operation
 
 from cubicweb.entity import EntityAdapter
 from cubicweb.entities import AnyEntity
 
+from cubicweb_rq.ccplugin import get_rq_redis_connection
+
 
 class RqTask(AnyEntity):
     __regid__ = "RqTask"
 
     def dc_title(self):
         return "{} ({})".format(self.title, self.name)
 
 
 class StartRqTaskOp(DataOperationMixIn, Operation):
     def postcommit_event(self):
         # use connection if it exists (e.g. one created by FakeRedis), else create new connection
         # the demo does not seem to connect automatically to the redis instance, so we need
         # to manually create it
-        queue = rq.Queue(
-            connection=rq.connections.get_current_connection() or redis.Redis()
-        )
+        connection = rq.connections.get_current_connection()
+        if not connection:
+            appid = self.cnx.repo.config.appid
+            connection = get_rq_redis_connection(appid)
+
+        queue = rq.Queue(connection=connection)
         for args, kwargs in self.cnx.transaction_data.get("rq_tasks", []):
             kwargs.setdefault("job_timeout", "12h")
             queue.enqueue(*args, **kwargs)
 
 
 class IRqJob(EntityAdapter):
     """provide a proxy from an entity to rq Job"""
```

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/hooks.py` & `cubicweb-rq-0.1.1/cubicweb_rq/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/migration/postcreate.py` & `cubicweb-rq-0.1.1/cubicweb_rq/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/rq.py` & `cubicweb-rq-0.1.1/cubicweb_rq/rq.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/schema.py` & `cubicweb-rq-0.1.1/cubicweb_rq/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq/views.py` & `cubicweb-rq-0.1.1/cubicweb_rq/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq.egg-info/PKG-INFO` & `cubicweb-rq-0.1.1/cubicweb_rq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-rq
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cube for starting RqJobs on a Rq worker
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/rq
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-rq-0.1.0/cubicweb_rq.egg-info/SOURCES.txt` & `cubicweb-rq-0.1.1/cubicweb_rq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/setup.py` & `cubicweb-rq-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/test/test_rq.py` & `cubicweb-rq-0.1.1/test/test_rq.py`

 * *Files identical despite different names*

### Comparing `cubicweb-rq-0.1.0/tox.ini` & `cubicweb-rq-0.1.1/tox.ini`

 * *Files identical despite different names*

