# Comparing `tmp/fonzie-0.6.0.tar.gz` & `tmp/fonzie-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fonzie-0.6.0.tar", last modified: Wed Mar 13 16:06:10 2024, max compression
+gzip compressed data, was "dist/fonzie-0.7.0.tar", last modified: Thu Apr  4 09:45:20 2024, max compression
```

## Comparing `fonzie-0.6.0.tar` & `fonzie-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie/urls/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      970 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/urls/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/urls/acl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/urls/lms_root.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/urls/status.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      307 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/urls/user.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/views/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1934 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/views/acl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      589 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/views/status.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2884 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/views/user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2024-03-13 16:06:07.000000 fonzie-0.6.0/fonzie/models.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4724 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2024-03-13 16:06:10.000000 fonzie-0.6.0/fonzie.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:10.000000 fonzie-0.6.0/tests/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-03-13 16:06:07.000000 fonzie-0.6.0/tests/views/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6437 2024-03-13 16:06:07.000000 fonzie-0.6.0/tests/views/test_acl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2024-03-13 16:06:07.000000 fonzie-0.6.0/tests/views/test_status.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4985 2024-03-13 16:06:07.000000 fonzie-0.6.0/tests/views/test_user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1494 2024-03-13 16:06:07.000000 fonzie-0.6.0/tests/views/test_versioning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2024-03-13 16:06:07.000000 fonzie-0.6.0/AUTHORS
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35119 2024-03-13 16:06:07.000000 fonzie-0.6.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2024-03-13 16:06:07.000000 fonzie-0.6.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2024-03-13 16:06:07.000000 fonzie-0.6.0/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2106 2024-03-13 16:06:10.000000 fonzie-0.6.0/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       84 2024-03-13 16:06:07.000000 fonzie-0.6.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4724 2024-03-13 16:06:10.000000 fonzie-0.6.0/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie/urls/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      970 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/urls/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      438 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/urls/acl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/urls/lms_root.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/urls/status.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      307 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/urls/user.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/views/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1934 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/views/acl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      589 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/views/status.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3317 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/views/user.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/apps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2024-04-04 09:45:17.000000 fonzie-0.7.0/fonzie/models.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4724 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2024-04-04 09:45:20.000000 fonzie-0.7.0/fonzie.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:20.000000 fonzie-0.7.0/tests/views/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-04-04 09:45:17.000000 fonzie-0.7.0/tests/views/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6437 2024-04-04 09:45:17.000000 fonzie-0.7.0/tests/views/test_acl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2024-04-04 09:45:17.000000 fonzie-0.7.0/tests/views/test_status.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4985 2024-04-04 09:45:17.000000 fonzie-0.7.0/tests/views/test_user.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1494 2024-04-04 09:45:17.000000 fonzie-0.7.0/tests/views/test_versioning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2024-04-04 09:45:17.000000 fonzie-0.7.0/AUTHORS
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35119 2024-04-04 09:45:17.000000 fonzie-0.7.0/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2024-04-04 09:45:17.000000 fonzie-0.7.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2024-04-04 09:45:17.000000 fonzie-0.7.0/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2106 2024-04-04 09:45:20.000000 fonzie-0.7.0/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       84 2024-04-04 09:45:17.000000 fonzie-0.7.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4724 2024-04-04 09:45:20.000000 fonzie-0.7.0/PKG-INFO
```

### Comparing `fonzie-0.6.0/fonzie/urls/__init__.py` & `fonzie-0.7.0/fonzie/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/fonzie/views/acl.py` & `fonzie-0.7.0/fonzie/views/acl.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/fonzie/views/status.py` & `fonzie-0.7.0/fonzie/views/status.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/fonzie/views/user.py` & `fonzie-0.7.0/fonzie/views/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,15 +62,23 @@
                 "language": language,
                 "username": user.username,
                 "is_active": user.is_active,
                 "is_staff": user.is_staff,
                 "is_superuser": user.is_superuser,
             },
         )
-
-        return Response(
+        response = Response(
             {
                 "access_token": str(token),
                 "username": user.username,
                 "full_name": user.profile.name,
             }
         )
+        if "newsletter_subscribed" in request.COOKIES:
+            # delete the cookie, as we only need it once, after registration
+            token.payload["has_subscribed_to_commercial_newsletter"] = (
+                request.COOKIES.get("newsletter_subscribed") == "true"
+            )
+            response.delete_cookie("newsletter_subscribed")
+            response.data["access_token"] = str(token)
+
+        return response
```

### Comparing `fonzie-0.6.0/fonzie/__init__.py` & `fonzie-0.7.0/fonzie/__init__.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/fonzie.egg-info/PKG-INFO` & `fonzie-0.7.0/fonzie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonzie
-Version: 0.6.0
+Version: 0.7.0
 Summary: A FUN API for Open edX
 Home-page: https://github.com/openfun/fonzie
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: AGPL 3.0
 Description: Fonzie, a FUN API for Open edX
         ==============================
```

### Comparing `fonzie-0.6.0/fonzie.egg-info/SOURCES.txt` & `fonzie-0.7.0/fonzie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/tests/views/test_acl.py` & `fonzie-0.7.0/tests/views/test_acl.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/tests/views/test_status.py` & `fonzie-0.7.0/tests/views/test_status.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/tests/views/test_user.py` & `fonzie-0.7.0/tests/views/test_user.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/tests/views/test_versioning.py` & `fonzie-0.7.0/tests/views/test_versioning.py`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/LICENSE.txt` & `fonzie-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/README.rst` & `fonzie-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `fonzie-0.6.0/setup.cfg` & `fonzie-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fonzie
-version = 0.6.0
+version = 0.7.0
 description = A FUN API for Open edX
 long_description = file: README.rst
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://github.com/openfun/fonzie
 license = AGPL 3.0
 keywords = Django, Django Rest Framework, API, Open edX
```

### Comparing `fonzie-0.6.0/PKG-INFO` & `fonzie-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonzie
-Version: 0.6.0
+Version: 0.7.0
 Summary: A FUN API for Open edX
 Home-page: https://github.com/openfun/fonzie
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: AGPL 3.0
 Description: Fonzie, a FUN API for Open edX
         ==============================
```

