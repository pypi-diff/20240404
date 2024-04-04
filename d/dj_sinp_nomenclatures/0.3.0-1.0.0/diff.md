# Comparing `tmp/dj_sinp_nomenclatures-0.3.0.tar.gz` & `tmp/dj_sinp_nomenclatures-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_nomenclatures-0.3.0.tar", max compression
+gzip compressed data, was "dj_sinp_nomenclatures-1.0.0.tar", max compression
```

## Comparing `dj_sinp_nomenclatures-0.3.0.tar` & `dj_sinp_nomenclatures-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    34523 2024-03-26 09:06:26.628947 dj_sinp_nomenclatures-0.3.0/LICENSE
--rw-r--r--   0        0        0      125 2024-03-26 09:06:26.628947 dj_sinp_nomenclatures-0.3.0/README.rst
--rw-r--r--   0        0        0     1979 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/__init__.py
--rw-r--r--   0        0        0      401 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/admin.py
--rw-r--r--   0        0        0      259 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/apps.py
--rw-r--r--   0        0        0        0 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/fixtures/.gitkeep
--rw-r--r--   0        0        0    53118 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/fixtures/sinp_nomenclatures.json
--rw-r--r--   0        0        0     2433 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      467 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/manager.py
--rw-r--r--   0        0        0     8571 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0001_initial.py
--rw-r--r--   0        0        0      353 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
--rw-r--r--   0        0        0      454 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
--rw-r--r--   0        0        0     3314 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py
--rw-r--r--   0        0        0     1340 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py
--rw-r--r--   0        0        0        0 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/__init__.py
--rw-r--r--   0        0        0     3741 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/models.py
--rw-r--r--   0        0        0        0 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/permissions.py
--rw-r--r--   0        0        0     1007 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/serializers.py
--rw-r--r--   0        0        0     3075 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/tests.py
--rw-r--r--   0        0        0      499 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/urls.py
--rw-r--r--   0        0        0     1791 2024-03-26 09:06:26.632947 dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-04 07:51:10.248191 dj_sinp_nomenclatures-1.0.0/LICENSE
+-rw-r--r--   0        0        0      125 2024-04-04 07:51:10.248191 dj_sinp_nomenclatures-1.0.0/README.rst
+-rw-r--r--   0        0        0     1997 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/admin.py
+-rw-r--r--   0        0        0      259 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/apps.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/.gitkeep
+-rw-r--r--   0        0        0    53118 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json
+-rw-r--r--   0        0        0   138267 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/sinp_dict_data_v1.0.json
+-rw-r--r--   0        0        0     2592 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      696 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/manager.py
+-rw-r--r--   0        0        0     8571 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
+-rw-r--r--   0        0        0      454 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
+-rw-r--r--   0        0        0     3314 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py
+-rw-r--r--   0        0        0     1340 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py
+-rw-r--r--   0        0        0      727 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0006_alter_source_options_source_url.py
+-rw-r--r--   0        0        0      360 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0007_remove_nomenclature_mnemonic.py
+-rw-r--r--   0        0        0      708 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0008_alter_nomenclature_active_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/__init__.py
+-rw-r--r--   0        0        0     3727 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/models.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/permissions.py
+-rw-r--r--   0        0        0      981 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/serializers.py
+-rw-r--r--   0        0        0     3075 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/tests.py
+-rw-r--r--   0        0        0      499 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/urls.py
+-rw-r--r--   0        0        0     1755 2024-04-04 07:51:10.252191 dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/views.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-1.0.0/PKG-INFO
```

### Comparing `dj_sinp_nomenclatures-0.3.0/LICENSE` & `dj_sinp_nomenclatures-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/pyproject.toml` & `dj_sinp_nomenclatures-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj_sinp_nomenclatures"
-version = "0.3.0"
+version = "1.0.0"
 description = "Django app to manage french SINP nomenclatures standards"
 authors = ["dbChiro project <project@dbchiro.org>"]
 license = "AGPLv3"
 keywords = ["SINP", "Nomenclatures", "Django", "France", "dbChiroWeb"]
 readme = "README.rst"
 homepage = "https://github.com/dbchiro/DjangoSinpNomenclature"
 repository = "https://github.com/dbchiro/DjangoSinpNomenclature"
@@ -29,14 +29,15 @@
 django-fixture-magic = "^0.1.5"
 pygraphviz = "^1.11"
 django-extensions = "^3.2.1"
 flake8-pyproject = "^1.2.3"
 pylint = "^3.0.3"
 pylint-django = "^2.5.5"
 dj-database-url = "^2.1.0"
+bpython = "^0.24"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6"
 sphinx-rtd-theme = "^2.0.0"
 rstcheck = "^6.2.0"
 myst-parser = "^2.0.0"
```

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/fixtures/sinp_nomenclatures.json` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/fixtures/old_sinp_nomenclatures.json`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/locale/fr/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,98 +4,108 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-02-26 20:32+0000\n"
+"POT-Creation-Date: 2024-04-04 07:36+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: sinp_nomenclatures/models.py:12
+#: sinp_nomenclatures/admin.py:8
+msgid "Mark selected items as active"
+msgstr "Activer les objects sélectionnés"
+
+#: sinp_nomenclatures/admin.py:14
+msgid "Mark selected items as inactive"
+msgstr "Désactiver les objects sélectionnés"
+
+#: sinp_nomenclatures/models.py:16
 msgid "Valid"
 msgstr "Valide"
 
-#: sinp_nomenclatures/models.py:13
+#: sinp_nomenclatures/models.py:17
 msgid "Frozen"
 msgstr "Gelée"
 
-#: sinp_nomenclatures/models.py:57
+#: sinp_nomenclatures/models.py:44
 msgid "Name"
 msgstr "Nom"
 
-#: sinp_nomenclatures/models.py:58
+#: sinp_nomenclatures/models.py:45
 msgid "Version"
 msgstr "Version"
 
-#: sinp_nomenclatures/models.py:60 sinp_nomenclatures/models.py:87
+#: sinp_nomenclatures/models.py:46
+msgid "URL"
+msgstr ""
+
+#: sinp_nomenclatures/models.py:48 sinp_nomenclatures/models.py:81
 msgid "Official creation date"
 msgstr "Date de création officielle"
 
-#: sinp_nomenclatures/models.py:63 sinp_nomenclatures/models.py:90
+#: sinp_nomenclatures/models.py:51 sinp_nomenclatures/models.py:84
 msgid "Official modification date"
 msgstr "Date de modification officielle"
 
-#: sinp_nomenclatures/models.py:69
-msgid "Nomenclature source"
-msgstr "Source des nomenclatures"
+#: sinp_nomenclatures/models.py:57
+msgid "source"
+msgstr "Source"
 
-#: sinp_nomenclatures/models.py:70
-#, fuzzy
-#| msgid "Nomenclature source"
-msgid "Nomenclature sources"
-msgstr "Source des nomenclatures"
+#: sinp_nomenclatures/models.py:58
+msgid "sources"
+msgstr "Source"
 
-#: sinp_nomenclatures/models.py:79 sinp_nomenclatures/models.py:119
+#: sinp_nomenclatures/models.py:73 sinp_nomenclatures/models.py:117
 msgid "Code"
 msgstr "Code"
 
-#: sinp_nomenclatures/models.py:81 sinp_nomenclatures/models.py:121
+#: sinp_nomenclatures/models.py:75
 msgid "Mnemonic"
 msgstr "Mnémonique"
 
-#: sinp_nomenclatures/models.py:82 sinp_nomenclatures/models.py:122
+#: sinp_nomenclatures/models.py:76 sinp_nomenclatures/models.py:119
 msgid "Label"
 msgstr "Libellé"
 
-#: sinp_nomenclatures/models.py:84
+#: sinp_nomenclatures/models.py:78
 msgid "Status"
 msgstr "Statut"
 
-#: sinp_nomenclatures/models.py:96
+#: sinp_nomenclatures/models.py:90
 msgid "Source"
 msgstr "Source"
 
-#: sinp_nomenclatures/models.py:104
+#: sinp_nomenclatures/models.py:98
 msgid "Type of nomenclature"
 msgstr "Type de nomenclature"
 
-#: sinp_nomenclatures/models.py:105
+#: sinp_nomenclatures/models.py:99
 msgid "Type of nomenclatures"
 msgstr "Type de nomenclatures"
 
-#: sinp_nomenclatures/models.py:114
+#: sinp_nomenclatures/models.py:112
 msgid "Type"
 msgstr "Type"
 
-#: sinp_nomenclatures/models.py:123
+#: sinp_nomenclatures/models.py:120
 msgid "Description"
 msgstr "Description"
 
-#: sinp_nomenclatures/models.py:124
-msgid "Is used"
-msgstr "Est utilisé"
+#: sinp_nomenclatures/models.py:121
+msgid "Is active"
+msgstr "Est actif"
 
-#: sinp_nomenclatures/models.py:127
+#: sinp_nomenclatures/models.py:124
 msgid "Parent nomenclature"
 msgstr "Nomenclature parent"
 
-#: sinp_nomenclatures/models.py:135
+#: sinp_nomenclatures/models.py:132
 msgid "nomenclatures"
 msgstr "nomenclatures"
```

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0001_initial.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0004_alter_source_options_alter_type_options_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/migrations/0005_remove_nomenclature_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/models.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,26 +39,27 @@
     Returns:
         [type]: [description]
     """
 
     objects = SourceManager()
     name = models.CharField(_("Name"), max_length=50)
     version = models.CharField(_("Version"), max_length=50)
+    url = models.URLField(_("URL"), max_length=250, blank=True)
     create_date = models.DateField(
         _("Official creation date"), auto_now=False, auto_now_add=False
     )
     update_date = models.DateField(
         _("Official modification date"),
         auto_now=False,
         auto_now_add=False,
     )
 
     class Meta:
-        verbose_name = _("Nomenclature source")
-        verbose_name_plural = _("Nomenclature sources")
+        verbose_name = _("source")
+        verbose_name_plural = _("sources")
         unique_together = ["name", "version"]
 
     def __str__(self):
         return f"{self.name} ({self.version})"
 
     def natural_key(self):
         return (self.name, self.version)
@@ -97,32 +98,31 @@
         verbose_name = _("Type of nomenclature")
         verbose_name_plural = _("Type of nomenclatures")
 
     def __str__(self):
         return f"{self.code} - {self.mnemonic}"
 
     def natural_key(self):
-        return self.code
+        return (self.code,)
 
 
 class Nomenclature(BaseModel):
     objects = NomenclatureManager()
     type = models.ForeignKey(
         "Type",
         verbose_name=_("Type"),
         on_delete=models.CASCADE,
         related_name="nomenclatures",
     )
     code = models.CharField(
         max_length=255, db_index=True, verbose_name=_("Code")
     )
-    mnemonic = models.CharField(_("Mnemonic"), max_length=50)
     label = models.CharField(max_length=255, verbose_name=_("Label"))
     description = models.TextField(_("Description"), blank=True)
-    active = models.BooleanField(default=True, verbose_name=_("Is used"))
+    active = models.BooleanField(default=True, verbose_name=_("Is active"))
     parent = models.ForeignKey(
         "Nomenclature",
         verbose_name=_("Parent nomenclature"),
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name="child_nomenclature",
@@ -132,8 +132,8 @@
         verbose_name_plural = _("nomenclatures")
         unique_together = ("type", "code")
 
     def __str__(self):
         return f"{self.label}"
 
     def natural_key(self):
-        return (self.type, self.code)
+        return (self.type.code, self.code)
```

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/serializers.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Django SINP Nomenclatures API serializers"""
 
 from rest_framework.serializers import ModelSerializer
 
 from .models import Nomenclature, Source, Type
 
 
 class NomenclatureSerializer(ModelSerializer):
     """Nomenclature item serializer"""
 
     class Meta:
         model = Nomenclature
-        fields = ["id", "code", "mnemonic", "label", "type"]
+        fields = ["id", "code", "label", "type", "parent"]
 
 
 class TypeSerializer(ModelSerializer):
     """Nomenclature type serializer"""
 
     class Meta:  # noqa
         model = Type
```

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/tests.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/tests.py`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.3.0/sinp_nomenclatures/views.py` & `dj_sinp_nomenclatures-1.0.0/sinp_nomenclatures/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Django SINP Nomenclatures API Views"""
 
 
 import logging
 
 from django_filters.rest_framework import DjangoFilterBackend
 
@@ -25,15 +24,15 @@
 class NomenclatureViewset(ReadOnlyModelViewSet):
     """Nomenclature item viewset (ReadOnly)"""
 
     serializer_class = NomenclatureSerializer
     permission_classes = [IsAuthenticated]
     queryset = Nomenclature.objects.filter(active=True).all()
     filter_backends = [DjangoFilterBackend]
-    filterset_fields = ["type", "code", "mnemonic"]
+    filterset_fields = ["type", "code"]
 
 
 class TypeViewset(ReadOnlyModelViewSet):
     """Nomenclature type viewset (ReadOnly)"""
 
     serializer_class = TypeSerializer
     permission_classes = [IsAuthenticated]
```

### Comparing `dj_sinp_nomenclatures-0.3.0/PKG-INFO` & `dj_sinp_nomenclatures-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_sinp_nomenclatures
-Version: 0.3.0
+Version: 1.0.0
 Summary: Django app to manage french SINP nomenclatures standards
 Home-page: https://github.com/dbchiro/DjangoSinpNomenclature
 License: AGPLv3
 Keywords: SINP,Nomenclatures,Django,France,dbChiroWeb
 Author: dbChiro project
 Author-email: project@dbchiro.org
 Requires-Python: >=3.8.1,<4.0
```

