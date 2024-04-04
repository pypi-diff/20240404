# Comparing `tmp/aleksis_app_cursus-0.1.0.dev1.tar.gz` & `tmp/aleksis_app_cursus-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_cursus-0.1.0.dev1.tar", max compression
+gzip compressed data, was "aleksis_app_cursus-0.1.dev0.tar", max compression
```

## Comparing `aleksis_app_cursus-0.1.0.dev1.tar` & `aleksis_app_cursus-0.1.dev0.tar`

### file list

```diff
@@ -1,50 +1,32 @@
--rw-r--r--   0        0        0      438 2023-01-30 16:17:42.914040 aleksis_app_cursus-0.1.0.dev1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-01-30 16:17:42.926040 aleksis_app_cursus-0.1.0.dev1/LICENCE.rst
--rw-r--r--   0        0        0     1090 2023-01-30 16:17:42.930040 aleksis_app_cursus-0.1.0.dev1/README.rst
--rw-r--r--   0        0        0      152 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/__init__.py
--rw-r--r--   0        0        0      717 2024-03-22 11:29:24.833011 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/apps.py
--rw-r--r--   0        0        0     6222 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/Course.vue
--rw-r--r--   0        0        0     5240 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/CreateCourse.vue
--rw-r--r--   0        0        0     3929 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/CreateSubject.vue
--rw-r--r--   0        0        0     7544 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/SchoolStructure.vue
--rw-r--r--   0        0        0     6807 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/Subject.vue
--rw-r--r--   0        0        0      616 2024-04-04 09:25:21.762119 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/SubjectChip.vue
--rw-r--r--   0        0        0     2861 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/SubjectField.vue
--rw-r--r--   0        0        0     1110 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/course.graphql
--rw-r--r--   0        0        0      123 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/helper.graphql
--rw-r--r--   0        0        0      691 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/schoolStructure.graphql
--rw-r--r--   0        0        0     1066 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/subject.graphql
--rw-r--r--   0        0        0     1305 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/index.js
--rw-r--r--   0        0        0     1347 2023-10-26 12:43:15.848664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/messages/de.json
--rw-r--r--   0        0        0     1344 2023-10-26 12:43:15.856664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/.keepdir
--rw-r--r--   0        0        0      463 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1782 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1947 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1695 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1650 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1650 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1840 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1650 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2024-04-04 12:53:51.407392 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1927 2024-04-04 12:52:24.817652 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5812 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0001_initial.py
--rw-r--r--   0        0        0      733 2023-10-26 12:43:15.884664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0002_cursusglobalpermissions.py
--rw-r--r--   0        0        0      817 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0003_drop_site.py
--rw-r--r--   0        0        0        0 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/__init__.py
--rw-r--r--   0        0        0     2817 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/models.py
--rw-r--r--   0        0        0     2501 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/rules.py
--rw-r--r--   0        0        0     9593 2024-03-22 11:29:24.833011 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/schema.py
--rw-r--r--   0        0        0       92 2024-03-22 11:29:24.833011 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/settings.py
--rw-r--r--   0        0        0       17 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/urls.py
--rw-r--r--   0        0        0      559 2024-03-22 11:29:24.837012 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/util/group_types.py
--rw-r--r--   0        0        0      283 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/util/predicates.py
--rw-r--r--   0        0        0     2457 2024-04-04 09:25:43.866248 aleksis_app_cursus-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-02-17 14:23:58.206985 aleksis_app_cursus-0.1.0.dev1/tox.ini
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 aleksis_app_cursus-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      438 2023-01-30 16:17:42.914040 aleksis_app_cursus-0.1.dev0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-01-30 16:17:42.926040 aleksis_app_cursus-0.1.dev0/LICENCE.rst
+-rw-r--r--   0        0        0     1090 2023-01-30 16:17:42.930040 aleksis_app_cursus-0.1.dev0/README.rst
+-rw-r--r--   0        0        0      152 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/__init__.py
+-rw-r--r--   0        0        0      395 2023-07-06 18:06:24.616006 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/apps.py
+-rw-r--r--   0        0        0     6222 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/Course.vue
+-rw-r--r--   0        0        0     5240 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/CreateCourse.vue
+-rw-r--r--   0        0        0     3929 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/CreateSubject.vue
+-rw-r--r--   0        0        0     7544 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/SchoolStructure.vue
+-rw-r--r--   0        0        0     6807 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/Subject.vue
+-rw-r--r--   0        0        0      542 2024-02-17 14:23:58.206985 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/SubjectChip.vue
+-rw-r--r--   0        0        0     2861 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/SubjectField.vue
+-rw-r--r--   0        0        0     1110 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/course.graphql
+-rw-r--r--   0        0        0      123 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/helper.graphql
+-rw-r--r--   0        0        0      691 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/schoolStructure.graphql
+-rw-r--r--   0        0        0     1066 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/subject.graphql
+-rw-r--r--   0        0        0     1305 2023-10-26 12:43:15.840664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/index.js
+-rw-r--r--   0        0        0     1347 2023-10-26 12:43:15.848664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/messages/de.json
+-rw-r--r--   0        0        0     1344 2023-10-26 12:43:15.856664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/locale/.keepdir
+-rw-r--r--   0        0        0     5812 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0001_initial.py
+-rw-r--r--   0        0        0      733 2023-10-26 12:43:15.884664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0002_cursusglobalpermissions.py
+-rw-r--r--   0        0        0      817 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0003_drop_site.py
+-rw-r--r--   0        0        0        0 2023-01-30 16:17:42.942040 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/__init__.py
+-rw-r--r--   0        0        0     2817 2024-02-16 20:04:28.180906 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/models.py
+-rw-r--r--   0        0        0     2501 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/rules.py
+-rw-r--r--   0        0        0     9821 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/schema.py
+-rw-r--r--   0        0        0       17 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/urls.py
+-rw-r--r--   0        0        0      283 2023-10-26 12:43:15.892664 aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/util/predicates.py
+-rw-r--r--   0        0        0     2455 2024-02-24 10:55:08.644996 aleksis_app_cursus-0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-02-17 14:23:58.206985 aleksis_app_cursus-0.1.dev0/tox.ini
+-rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 aleksis_app_cursus-0.1.dev0/PKG-INFO
```

### Comparing `aleksis_app_cursus-0.1.0.dev1/LICENCE.rst` & `aleksis_app_cursus-0.1.dev0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/README.rst` & `aleksis_app_cursus-0.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/Course.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/Course.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/CreateCourse.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/CreateCourse.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/CreateSubject.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/CreateSubject.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/SchoolStructure.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/SchoolStructure.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/Subject.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/Subject.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/SubjectField.vue` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/SubjectField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/course.graphql` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/course.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/schoolStructure.graphql` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/schoolStructure.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/components/subject.graphql` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/components/subject.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/index.js` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/messages/de.json` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/frontend/messages/en.json` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0001_initial.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0002_cursusglobalpermissions.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0002_cursusglobalpermissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/migrations/0003_drop_site.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/migrations/0003_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/models.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/rules.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/aleksis/apps/cursus/schema.py` & `aleksis_app_cursus-0.1.dev0/aleksis/apps/cursus/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
+from django.apps import apps
 from django.core.exceptions import PermissionDenied
 from django.db.models import Q
 
 import graphene
 from graphene_django.types import DjangoObjectType
 from graphene_django_cud.mutations import (
     DjangoBatchCreateMutation,
     DjangoBatchDeleteMutation,
     DjangoBatchPatchMutation,
 )
 from guardian.shortcuts import get_objects_for_user
 
-from aleksis.apps.cursus.settings import SCHOOL_CLASS_GROUP_TYPE_NAME, SCHOOL_GRADE_GROUP_TYPE_NAME
-from aleksis.apps.cursus.util.group_types import (
-    get_school_class_group_type,
-    get_school_grade_group_type,
-)
-from aleksis.core.models import Group, Person
+from aleksis.core.models import Group, GroupType, Person
 from aleksis.core.schema.base import (
     DjangoFilterMixin,
     FilterOrderList,
     PermissionBatchDeleteMixin,
     PermissionBatchPatchMixin,
     PermissionsTypeMixin,
 )
 from aleksis.core.schema.group import GroupType as GraphQLGroupType
 from aleksis.core.schema.person import PersonType as GraphQLPersonType
 from aleksis.core.util.core_helpers import has_person
 
 from .models import Course, Subject
 
+SCHOOL_GRADE_GROUP_TYPE_NAME = "School grade"
+
 
 class SubjectType(PermissionsTypeMixin, DjangoFilterMixin, DjangoObjectType):
     class Meta:
         model = Subject
         fields = (
             "id",
             "short_name",
@@ -183,29 +181,35 @@
     class Meta:
         model = Group
         permissions = ("core.add_group",)
         only_fields = ("name", "short_name", "school_term", "parent_groups")
 
     @classmethod
     def before_mutate(cls, root, info, input):  # noqa
-        group_type = get_school_class_group_type()
+        app_label = apps.get_containing_app_config(cls.__module__).label
+        group_type, __ = GroupType.objects.managed_by_app(app_label).get_or_create(
+            name="School class", managed_by_app_label=app_label
+        )
         for school_class in input:
             school_class["group_type"] = group_type.pk
         return input
 
 
 class CreateSchoolGradeMutation(DjangoBatchCreateMutation):
     class Meta:
         model = Group
         permissions = ("core.add_group",)
         only_fields = ("name", "short_name", "school_term", "parent_groups")
 
     @classmethod
     def before_mutate(cls, root, info, input):  # noqa
-        group_type = get_school_grade_group_type()
+        app_label = apps.get_containing_app_config(cls.__module__).label
+        group_type, __ = GroupType.objects.managed_by_app(app_label).get_or_create(
+            name=SCHOOL_GRADE_GROUP_TYPE_NAME, managed_by_app_label=app_label
+        )
         for school_grade in input:
             school_grade["group_type"] = group_type.pk
         return input
 
 
 class Query(graphene.ObjectType):
     subjects = FilterOrderList(SubjectType)
@@ -227,15 +231,15 @@
         return course
 
     @staticmethod
     def resolve_school_classes(root, info, **kwargs):
         return get_objects_for_user(
             info.context.user,
             "core.view_group",
-            Group.objects.filter(group_type__name=SCHOOL_CLASS_GROUP_TYPE_NAME),
+            Group.objects.filter(group_type__name="School class"),
         )
 
     @staticmethod
     def resolve_school_grades(root, info, **kwargs):
         return get_objects_for_user(
             info.context.user,
             "core.view_group",
```

### Comparing `aleksis_app_cursus-0.1.0.dev1/pyproject.toml` & `aleksis_app_cursus-0.1.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Cursus"
-version = "0.1.0.dev1"
+version = "0.1.dev0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -31,15 +31,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aleksis-core = "^4.0.0.dev6"
+aleksis-core = "^4.0.0.dev4"
 
 [tool.poetry.plugins."aleksis.app"]
 cursus = "aleksis.apps.cursus.apps:DefaultConfig"
 
 
 [tool.poetry.group.dev.dependencies]
 django-stubs = "^4.2"
```

### Comparing `aleksis_app_cursus-0.1.0.dev1/tox.ini` & `aleksis_app_cursus-0.1.dev0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_cursus-0.1.0.dev1/PKG-INFO` & `aleksis_app_cursus-0.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: AlekSIS-App-Cursus
-Version: 0.1.0.dev1
+Version: 0.1.dev0
 Summary: AlekSIS (School Information System) — App Cursus (Manage subjects and courses)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=4.0.0.dev6,<5.0.0)
+Requires-Dist: aleksis-core (>=4.0.0.dev4,<5.0.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Cursus
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Cursus (Manage subjects and courses)
 ==================================================================================================
```

