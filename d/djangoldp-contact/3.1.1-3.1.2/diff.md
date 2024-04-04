# Comparing `tmp/djangoldp_contact-3.1.1.tar.gz` & `tmp/djangoldp_contact-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_contact-3.1.1.tar", last modified: Wed Jan 24 17:18:53 2024, max compression
+gzip compressed data, was "djangoldp_contact-3.1.2.tar", last modified: Thu Apr  4 12:25:27 2024, max compression
```

## Comparing `djangoldp_contact-3.1.1.tar` & `djangoldp_contact-3.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:53.488389 djangoldp_contact-3.1.1/
--rw-r--r--   0 root         (0) root         (0)      261 2024-01-24 17:18:53.488389 djangoldp_contact-3.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:53.484389 djangoldp_contact-3.1.1/djangoldp_contact/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-01-24 17:18:50.000000 djangoldp_contact-3.1.1/djangoldp_contact/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/check_integrity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:53.488389 djangoldp_contact-3.1.1/djangoldp_contact/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/migrations/0002_auto_20201208_1157.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/migrations/0003_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/migrations/0004_alter_contact_options_alter_contact_urlid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/models.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:53.488389 djangoldp_contact-3.1.1/djangoldp_contact/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     4307 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/djangoldp_contact/tests/tests_permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:53.484389 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/
--rw-r--r--   0 root         (0) root         (0)      261 2024-01-24 17:18:53.000000 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      802 2024-01-24 17:18:53.000000 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 17:18:53.000000 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-01-24 17:18:53.000000 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-01-24 17:18:53.000000 djangoldp_contact-3.1.1/djangoldp_contact.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-01-24 17:18:53.488389 djangoldp_contact-3.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-24 17:18:29.000000 djangoldp_contact-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/djangoldp_contact/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-04 12:25:24.000000 djangoldp_contact-3.1.2/djangoldp_contact/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/check_integrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/djangoldp_contact/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/migrations/0002_auto_20201208_1157.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/migrations/0003_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/migrations/0004_alter_contact_options_alter_contact_urlid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:25:09.000000 djangoldp_contact-3.1.2/djangoldp_contact/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/djangoldp_contact/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 12:25:09.000000 djangoldp_contact-3.1.2/djangoldp_contact/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/djangoldp_contact/tests/tests_permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-04 12:25:27.000000 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      802 2024-04-04 12:25:27.000000 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:25:27.000000 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-04-04 12:25:27.000000 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 12:25:27.000000 djangoldp_contact-3.1.2/djangoldp_contact.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-04-04 12:25:27.464840 djangoldp_contact-3.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-04 12:25:08.000000 djangoldp_contact-3.1.2/setup.py
```

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/admin.py` & `djangoldp_contact-3.1.2/djangoldp_contact/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/check_integrity.py` & `djangoldp_contact-3.1.2/djangoldp_contact/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/migrations/0001_initial.py` & `djangoldp_contact-3.1.2/djangoldp_contact/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/migrations/0002_auto_20201208_1157.py` & `djangoldp_contact-3.1.2/djangoldp_contact/migrations/0002_auto_20201208_1157.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/migrations/0004_alter_contact_options_alter_contact_urlid.py` & `djangoldp_contact-3.1.2/djangoldp_contact/migrations/0004_alter_contact_options_alter_contact_urlid.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/models.py` & `djangoldp_contact-3.1.2/djangoldp_contact/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 from djangoldp.fields import LDPUrlField
 from djangoldp.models import Model
-from djangoldp.permissions import AuthenticatedOnly, OwnerPermissions
+from djangoldp.permissions import AuthenticatedOnly, OwnerPermissions, OwnerCreatePermission
 from djangoldp_notification.models import Notification
 
 
 class Contact(Model):
     user = models.ForeignKey(get_user_model(), on_delete=models.CASCADE, related_name="contacts", null=True, blank=True)
     contact = LDPUrlField(null=True, blank=True)
 
@@ -17,15 +17,15 @@
         return '{} -> {} ({})'.format(self.user.username, self.contact, self.urlid)
 
     class Meta(Model.Meta):
         verbose_name = _('contact')
         verbose_name_plural = _("contacts")
         auto_author = 'user'
         owner_field = 'user'
-        permission_classes = [AuthenticatedOnly, OwnerPermissions]
+        permission_classes = [AuthenticatedOnly, OwnerCreatePermission, OwnerPermissions]
         unique_together = [['user', 'contact']]
         rdf_type = "sib:contact"
 
 @receiver(post_save, sender=Notification)
 def create_contact_on_notification(sender, instance, created, **kwargs):
     if created:
         if instance.type == "Message":
```

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/tests/runner.py` & `djangoldp_contact-3.1.2/djangoldp_contact/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact/tests/tests_permissions.py` & `djangoldp_contact-3.1.2/djangoldp_contact/tests/tests_permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,32 +23,32 @@
     # we write functions like this for convenience - we can reuse between tests
     def _get_random_user(self):
         return LDPUser.objects.create(email='{}@test.co.uk'.format(str(uuid.uuid4())), first_name='Test',
                                       last_name='Test', username=str(uuid.uuid4()))
 
     def _get_context(self):
         return {
-                '@vocab': "http://happy-dev.fr/owl/#",
+                '@vocab': "https://cdn.startinblox.com/owl#",
                 'rdf': "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
                 'rdfs': "http://www.w3.org/2000/01/rdf-schema#",
                 'ldp': "http://www.w3.org/ns/ldp#",
                 'foaf': "http://xmlns.com/foaf/0.1/",
                 'name': "rdfs:label",
                 'acl': "http://www.w3.org/ns/auth/acl#",
                 'permissions': "acl:accessControl",
                 'mode': "acl:mode",
-                'inbox': "http://happy-dev.fr/owl/#inbox",
-                'object': "http://happy-dev.fr/owl/#object",
-                'author': "http://happy-dev.fr/owl/#author",
-                'account': "http://happy-dev.fr/owl/#account",
+                'inbox': "https://cdn.startinblox.com/owl#inbox",
+                'object': "https://cdn.startinblox.com/owl#object",
+                'author': "https://cdn.startinblox.com/owl#author",
+                'account': "https://cdn.startinblox.com/owl#account",
                 'jabberID': "foaf:jabberID",
                 'picture': "foaf:depiction",
-                'firstName': "http://happy-dev.fr/owl/#first_name",
-                'lastName': "http://happy-dev.fr/owl/#last_name",
-                'isAdmin': "http://happy-dev.fr/owl/#is_admin"
+                'firstName': "https://cdn.startinblox.com/owl#first_name",
+                'lastName': "https://cdn.startinblox.com/owl#last_name",
+                'isAdmin': "https://cdn.startinblox.com/owl#is_admin"
             }
 
     def test_post_contact_for_myself(self):
         self.setUpLoggedInUser()
         another_user = self._get_random_user()
 
         body = {
```

### Comparing `djangoldp_contact-3.1.1/djangoldp_contact.egg-info/SOURCES.txt` & `djangoldp_contact-3.1.2/djangoldp_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_contact-3.1.1/setup.cfg` & `djangoldp_contact-3.1.2/setup.cfg`

 * *Files identical despite different names*

