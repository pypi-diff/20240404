# Comparing `tmp/django-auth-ldap-4.7.0.tar.gz` & `tmp/django-auth-ldap-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auth-ldap-4.7.0.tar", last modified: Sat Mar 23 19:47:08 2024, max compression
+gzip compressed data, was "django-auth-ldap-4.8.0.tar", last modified: Thu Apr  4 12:45:46 2024, max compression
```

## Comparing `django-auth-ldap-4.7.0.tar` & `django-auth-ldap-4.8.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.756059 django-auth-ldap-4.7.0/django_auth_ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/django_auth_ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32661 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/django_auth_ldap/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    25017 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/django_auth_ldap/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-23 19:47:08.000000 django-auth-ldap-4.7.0/django_auth_ldap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/custombehavior.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/ext/daldocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/multiconfig.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/docs/users.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 19:47:08.760058 django-auth-ldap-4.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tests/tests.ldif
--rw-r--r--   0 runner    (1001) docker     (127)    62819 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-23 19:46:58.000000 django-auth-ldap-4.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.275133 django-auth-ldap-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-04 12:45:46.275133 django-auth-ldap-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.267133 django-auth-ldap-4.8.0/django_auth_ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/django_auth_ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32739 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/django_auth_ldap/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25017 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/django_auth_ldap/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.275133 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 12:45:46.000000 django-auth-ldap-4.8.0/django_auth_ldap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.271133 django-auth-ldap-4.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/custombehavior.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.271133 django-auth-ldap-4.8.0/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/ext/daldocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/multiconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/docs/users.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 12:45:46.275133 django-auth-ldap-4.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:46.275133 django-auth-ldap-4.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tests/tests.ldif
+-rw-r--r--   0 runner    (1001) docker     (127)    63338 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 12:45:35.000000 django-auth-ldap-4.8.0/tox.ini
```

### Comparing `django-auth-ldap-4.7.0/LICENSE` & `django-auth-ldap-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/PKG-INFO` & `django-auth-ldap-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.7.0
+Version: 4.8.0
 Summary: Django LDAP authentication backend
 Author-email: Peter Sagerson <psagers@ignorare.net>
 Maintainer-email: François Freitag <mail@franek.fr>
 License: BSD
 Project-URL: Homepage, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
```

### Comparing `django-auth-ldap-4.7.0/README.rst` & `django-auth-ldap-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/django_auth_ldap/backend.py` & `django-auth-ldap-4.8.0/django_auth_ldap/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         return get_user_model()
 
     #
     # The Django auth backend API
     #
 
     def authenticate(self, request, username=None, password=None, **kwargs):
+        username = kwargs.get(self.get_user_model().USERNAME_FIELD, username)
         if username is None:
             return None
 
         if password or self.settings.PERMIT_EMPTY_PASSWORD:
             ldap_user = _LDAPUser(self, username=username.strip(), request=request)
             user = self.authenticate_ldap_user(ldap_user, password)
         else:
```

### Comparing `django-auth-ldap-4.7.0/django_auth_ldap/config.py` & `django-auth-ldap-4.8.0/django_auth_ldap/config.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/django_auth_ldap.egg-info/PKG-INFO` & `django-auth-ldap-4.8.0/django_auth_ldap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auth-ldap
-Version: 4.7.0
+Version: 4.8.0
 Summary: Django LDAP authentication backend
 Author-email: Peter Sagerson <psagers@ignorare.net>
 Maintainer-email: François Freitag <mail@franek.fr>
 License: BSD
 Project-URL: Homepage, https://github.com/django-auth-ldap/django-auth-ldap
 Project-URL: Documentation, https://django-auth-ldap.readthedocs.io/
 Project-URL: Source, https://github.com/django-auth-ldap/django-auth-ldap
```

### Comparing `django-auth-ldap-4.7.0/django_auth_ldap.egg-info/SOURCES.txt` & `django-auth-ldap-4.8.0/django_auth_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/Makefile` & `django-auth-ldap-4.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/authentication.rst` & `django-auth-ldap-4.8.0/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/changes.rst` & `django-auth-ldap-4.8.0/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/conf.py` & `django-auth-ldap-4.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/contributing.rst` & `django-auth-ldap-4.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/custombehavior.rst` & `django-auth-ldap-4.8.0/docs/custombehavior.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/example.rst` & `django-auth-ldap-4.8.0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/groups.rst` & `django-auth-ldap-4.8.0/docs/groups.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/index.rst` & `django-auth-ldap-4.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/install.rst` & `django-auth-ldap-4.8.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/logging.rst` & `django-auth-ldap-4.8.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/multiconfig.rst` & `django-auth-ldap-4.8.0/docs/multiconfig.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/performance.rst` & `django-auth-ldap-4.8.0/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/permissions.rst` & `django-auth-ldap-4.8.0/docs/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/reference.rst` & `django-auth-ldap-4.8.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/docs/users.rst` & `django-auth-ldap-4.8.0/docs/users.rst`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/pyproject.toml` & `django-auth-ldap-4.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/tests/models.py` & `django-auth-ldap-4.8.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/tests/tests.ldif` & `django-auth-ldap-4.8.0/tests/tests.ldif`

 * *Files identical despite different names*

### Comparing `django-auth-ldap-4.7.0/tests/tests.py` & `django-auth-ldap-4.8.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,25 @@
     def test_deepcopy(self):
         self._init_settings(USER_DN_TEMPLATE="uid=%(user)s,ou=people,o=test")
 
         user = authenticate(username="Alice", password="password")
         user = deepcopy(user)
 
     @_override_settings(AUTH_USER_MODEL="tests.TestUser")
+    def test_auth_custom_field(self):
+        self._init_settings(
+            USER_DN_TEMPLATE="cn=%(user)s,ou=people,o=test",
+            USER_ATTR_MAP={"identifier": "cn"},
+        )
+        charlie = TestUser.objects.create(identifier="charlie_cooper", uid_number=1004)
+        user = authenticate(identifier="charlie_cooper", password="password")
+        self.assertIsInstance(user, TestUser)
+        self.assertEqual(user.identifier, charlie.identifier)
+
+    @_override_settings(AUTH_USER_MODEL="tests.TestUser")
     def test_auth_custom_user(self):
         self._init_settings(
             USER_DN_TEMPLATE="uid=%(user)s,ou=people,o=test",
             USER_ATTR_MAP={"uid_number": "uidNumber"},
         )
 
         user = authenticate(username="Alice", password="password")
```

### Comparing `django-auth-ldap-4.7.0/tox.ini` & `django-auth-ldap-4.8.0/tox.ini`

 * *Files identical despite different names*

