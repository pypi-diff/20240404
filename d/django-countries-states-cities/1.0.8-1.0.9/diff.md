# Comparing `tmp/django-countries-states-cities-1.0.8.tar.gz` & `tmp/django-countries-states-cities-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-countries-states-cities-1.0.8.tar", last modified: Mon Jan 15 07:04:22 2024, max compression
+gzip compressed data, was "dist/django-countries-states-cities-1.0.9.tar", last modified: Mon Jan 15 08:23:38 2024, max compression
```

## Comparing `django-countries-states-cities-1.0.8.tar` & `django-countries-states-cities-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.578356 django-countries-states-cities-1.0.8/
--rw-r--r--   0 idist      (501) staff       (20)    25326 2023-12-11 12:45:52.000000 django-countries-states-cities-1.0.8/LICENSE
--rw-r--r--   0 idist      (501) staff       (20)      197 2024-01-15 06:46:11.000000 django-countries-states-cities-1.0.8/MANIFEST.in
--rw-r--r--   0 idist      (501) staff       (20)     3500 2024-01-15 07:04:22.578502 django-countries-states-cities-1.0.8/PKG-INFO
--rw-r--r--   0 idist      (501) staff       (20)     2671 2024-01-15 06:17:02.000000 django-countries-states-cities-1.0.8/README.md
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.319585 django-countries-states-cities-1.0.8/countries_states_cities/
--rw-r--r--   0 idist      (501) staff       (20)        0 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.8/countries_states_cities/__init__.py
--rw-r--r--   0 idist      (501) staff       (20)     6097 2024-01-13 21:51:39.000000 django-countries-states-cities-1.0.8/countries_states_cities/admin.py
--rw-r--r--   0 idist      (501) staff       (20)      176 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.8/countries_states_cities/apps.py
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.573876 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/
--rw-r--r--   0 idist      (501) staff       (20) 38607167 2024-01-15 05:59:28.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_cities.csv
--rw-r--r--   0 idist      (501) staff       (20)   187815 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_countries.csv
--rw-r--r--   0 idist      (501) staff       (20)     1866 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_regions.csv
--rw-r--r--   0 idist      (501) staff       (20)  2145336 2024-01-15 05:59:10.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_states.csv
--rw-r--r--   0 idist      (501) staff       (20)  5114219 2024-01-15 06:59:06.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_states.json
--rw-r--r--   0 idist      (501) staff       (20)     8135 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_subregions.csv
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.574802 django-countries-states-cities-1.0.8/countries_states_cities/management/
--rw-r--r--   0 idist      (501) staff       (20)     6148 2024-01-15 05:13:25.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/.DS_Store
--rw-r--r--   0 idist      (501) staff       (20)        0 2023-12-28 06:13:08.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/__init__.py
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.575014 django-countries-states-cities-1.0.8/countries_states_cities/management/__pycache__/
--rw-r--r--   0 idist      (501) staff       (20)      201 2024-01-10 15:05:42.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.575922 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/
--rw-r--r--   0 idist      (501) staff       (20)        0 2023-12-28 06:13:08.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/__init__.py
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.576552 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/__pycache__/
--rw-r--r--   0 idist      (501) staff       (20)      210 2024-01-10 15:05:42.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 idist      (501) staff       (20)     3242 2024-01-15 07:02:22.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/__pycache__/csc_loaddata_csv.cpython-38.pyc
--rw-r--r--   0 idist      (501) staff       (20)     3036 2024-01-15 05:59:04.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/csc_dumpdata_csv.py
--rw-r--r--   0 idist      (501) staff       (20)     2897 2024-01-15 06:06:57.000000 django-countries-states-cities-1.0.8/countries_states_cities/management/commands/csc_loaddata_csv.py
--rw-r--r--   0 idist      (501) staff       (20)     7310 2024-01-13 19:08:11.000000 django-countries-states-cities-1.0.8/countries_states_cities/models.py
--rw-r--r--   0 idist      (501) staff       (20)      985 2023-12-30 17:11:49.000000 django-countries-states-cities-1.0.8/countries_states_cities/resource.py
--rw-r--r--   0 idist      (501) staff       (20)     1044 2023-12-07 07:49:07.000000 django-countries-states-cities-1.0.8/countries_states_cities/serializers.py
--rw-r--r--   0 idist      (501) staff       (20)      180 2023-11-01 13:34:47.000000 django-countries-states-cities-1.0.8/countries_states_cities/settings.py
--rw-r--r--   0 idist      (501) staff       (20)       60 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.8/countries_states_cities/tests.py
--rw-r--r--   0 idist      (501) staff       (20)      856 2023-12-30 14:06:29.000000 django-countries-states-cities-1.0.8/countries_states_cities/translation.py
--rw-r--r--   0 idist      (501) staff       (20)      681 2023-11-06 05:21:00.000000 django-countries-states-cities-1.0.8/countries_states_cities/urls.py
--rw-r--r--   0 idist      (501) staff       (20)     2353 2024-01-12 09:14:41.000000 django-countries-states-cities-1.0.8/countries_states_cities/utils.py
--rw-r--r--   0 idist      (501) staff       (20)     6677 2023-12-06 19:04:02.000000 django-countries-states-cities-1.0.8/countries_states_cities/views.py
-drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 07:04:22.578109 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/
--rw-r--r--   0 idist      (501) staff       (20)     3500 2024-01-15 07:04:22.000000 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/PKG-INFO
--rw-r--r--   0 idist      (501) staff       (20)     1560 2024-01-15 07:04:22.000000 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/SOURCES.txt
--rw-r--r--   0 idist      (501) staff       (20)        1 2024-01-15 07:04:22.000000 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/dependency_links.txt
--rw-r--r--   0 idist      (501) staff       (20)       88 2024-01-15 07:04:22.000000 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/requires.txt
--rw-r--r--   0 idist      (501) staff       (20)       24 2024-01-15 07:04:22.000000 django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/top_level.txt
--rw-r--r--   0 idist      (501) staff       (20)       89 2023-11-07 05:59:48.000000 django-countries-states-cities-1.0.8/pyproject.toml
--rw-r--r--   0 idist      (501) staff       (20)      992 2024-01-15 07:04:22.579185 django-countries-states-cities-1.0.8/setup.cfg
--rw-r--r--   0 idist      (501) staff       (20)       37 2023-11-07 05:58:40.000000 django-countries-states-cities-1.0.8/setup.py
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.814576 django-countries-states-cities-1.0.9/
+-rw-r--r--   0 idist      (501) staff       (20)    25326 2023-12-11 12:45:52.000000 django-countries-states-cities-1.0.9/LICENSE
+-rw-r--r--   0 idist      (501) staff       (20)      197 2024-01-15 06:46:11.000000 django-countries-states-cities-1.0.9/MANIFEST.in
+-rw-r--r--   0 idist      (501) staff       (20)     3500 2024-01-15 08:23:38.814718 django-countries-states-cities-1.0.9/PKG-INFO
+-rw-r--r--   0 idist      (501) staff       (20)     2671 2024-01-15 06:17:02.000000 django-countries-states-cities-1.0.9/README.md
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.054927 django-countries-states-cities-1.0.9/countries_states_cities/
+-rw-r--r--   0 idist      (501) staff       (20)        0 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.9/countries_states_cities/__init__.py
+-rw-r--r--   0 idist      (501) staff       (20)     6257 2024-01-15 07:20:05.000000 django-countries-states-cities-1.0.9/countries_states_cities/admin.py
+-rw-r--r--   0 idist      (501) staff       (20)      176 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.9/countries_states_cities/apps.py
+-rw-r--r--   0 idist      (501) staff       (20)     1260 2024-01-15 08:00:09.000000 django-countries-states-cities-1.0.9/countries_states_cities/filters.py
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.809075 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/
+-rw-r--r--   0 idist      (501) staff       (20) 38607167 2024-01-15 05:59:28.000000 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_cities.csv
+-rw-r--r--   0 idist      (501) staff       (20)   187815 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_countries.csv
+-rw-r--r--   0 idist      (501) staff       (20)     1866 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_regions.csv
+-rw-r--r--   0 idist      (501) staff       (20)  2145336 2024-01-15 05:59:10.000000 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_states.csv
+-rw-r--r--   0 idist      (501) staff       (20)     8135 2024-01-15 05:59:09.000000 django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_subregions.csv
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.810456 django-countries-states-cities-1.0.9/countries_states_cities/management/
+-rw-r--r--   0 idist      (501) staff       (20)     6148 2024-01-15 05:13:25.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/.DS_Store
+-rw-r--r--   0 idist      (501) staff       (20)        0 2023-12-28 06:13:08.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/__init__.py
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.810657 django-countries-states-cities-1.0.9/countries_states_cities/management/__pycache__/
+-rw-r--r--   0 idist      (501) staff       (20)      201 2024-01-10 15:05:42.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.811882 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/
+-rw-r--r--   0 idist      (501) staff       (20)        0 2023-12-28 06:13:08.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/__init__.py
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.812869 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/__pycache__/
+-rw-r--r--   0 idist      (501) staff       (20)      210 2024-01-10 15:05:42.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 idist      (501) staff       (20)     3242 2024-01-15 07:02:22.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/__pycache__/csc_loaddata_csv.cpython-38.pyc
+-rw-r--r--   0 idist      (501) staff       (20)     3036 2024-01-15 05:59:04.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/csc_dumpdata_csv.py
+-rw-r--r--   0 idist      (501) staff       (20)     2897 2024-01-15 06:06:57.000000 django-countries-states-cities-1.0.9/countries_states_cities/management/commands/csc_loaddata_csv.py
+-rw-r--r--   0 idist      (501) staff       (20)     7311 2024-01-15 07:50:46.000000 django-countries-states-cities-1.0.9/countries_states_cities/models.py
+-rw-r--r--   0 idist      (501) staff       (20)      985 2023-12-30 17:11:49.000000 django-countries-states-cities-1.0.9/countries_states_cities/resource.py
+-rw-r--r--   0 idist      (501) staff       (20)     1498 2024-01-15 08:19:53.000000 django-countries-states-cities-1.0.9/countries_states_cities/serializers.py
+-rw-r--r--   0 idist      (501) staff       (20)      180 2023-11-01 13:34:47.000000 django-countries-states-cities-1.0.9/countries_states_cities/settings.py
+-rw-r--r--   0 idist      (501) staff       (20)       60 2023-10-17 11:41:39.000000 django-countries-states-cities-1.0.9/countries_states_cities/tests.py
+-rw-r--r--   0 idist      (501) staff       (20)      856 2023-12-30 14:06:29.000000 django-countries-states-cities-1.0.9/countries_states_cities/translation.py
+-rw-r--r--   0 idist      (501) staff       (20)      681 2023-11-06 05:21:00.000000 django-countries-states-cities-1.0.9/countries_states_cities/urls.py
+-rw-r--r--   0 idist      (501) staff       (20)     2353 2024-01-12 09:14:41.000000 django-countries-states-cities-1.0.9/countries_states_cities/utils.py
+-rw-r--r--   0 idist      (501) staff       (20)     6926 2024-01-15 08:00:55.000000 django-countries-states-cities-1.0.9/countries_states_cities/views.py
+drwxr-xr-x   0 idist      (501) staff       (20)        0 2024-01-15 08:23:38.814365 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/
+-rw-r--r--   0 idist      (501) staff       (20)     3500 2024-01-15 08:23:38.000000 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/PKG-INFO
+-rw-r--r--   0 idist      (501) staff       (20)     1546 2024-01-15 08:23:38.000000 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/SOURCES.txt
+-rw-r--r--   0 idist      (501) staff       (20)        1 2024-01-15 08:23:38.000000 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/dependency_links.txt
+-rw-r--r--   0 idist      (501) staff       (20)      122 2024-01-15 08:23:38.000000 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/requires.txt
+-rw-r--r--   0 idist      (501) staff       (20)       24 2024-01-15 08:23:38.000000 django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/top_level.txt
+-rw-r--r--   0 idist      (501) staff       (20)       89 2023-11-07 05:59:48.000000 django-countries-states-cities-1.0.9/pyproject.toml
+-rw-r--r--   0 idist      (501) staff       (20)     1029 2024-01-15 08:23:38.815437 django-countries-states-cities-1.0.9/setup.cfg
+-rw-r--r--   0 idist      (501) staff       (20)       37 2023-11-07 05:58:40.000000 django-countries-states-cities-1.0.9/setup.py
```

### Comparing `django-countries-states-cities-1.0.8/LICENSE` & `django-countries-states-cities-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/PKG-INFO` & `django-countries-states-cities-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-countries-states-cities
-Version: 1.0.8
+Version: 1.0.9
 Summary: Countries States Cities models for Django.
 Home-page: https://github.com/runners-2022/django-countries-states-cities
 Author: Sunwook Kim
 Author-email: sun@runners.im
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-countries-states-cities-1.0.8/README.md` & `django-countries-states-cities-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/admin.py` & `django-countries-states-cities-1.0.9/countries_states_cities/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# vim: set fileencoding=utf-8 :
+# Django
 from django.contrib import admin, messages
 from django.utils.translation import gettext_lazy as _
 from django.utils.html import format_html
-from django.urls import reverse
 
 # 3rd Party
 from import_export.admin import ImportExportModelAdmin
 from modeltranslation.admin import TranslationAdmin
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 # App
@@ -14,24 +13,30 @@
 from countries_states_cities.utils import get_translated_fields
 from countries_states_cities.resource import RegionResource, SubregionResource, CountryResource, StateResource, \
     CityResource
 
 
 # Main Section
 class BaseAreaAdmin(ImportExportModelAdmin, admin.ModelAdmin):
-    name_fields = get_translated_fields(Region, 'name')
     actions = ['mark_duplicates_as_duplicated', 'update_wikidata_id', 'translate_selected']
     list_filter = ('is_duplicated',)
     list_editable = ('wikiDataId',)
-    list_display = ('id',) + name_fields + ('wikidata_link', 'wikiDataId', 'is_duplicated', 'updated_at')
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.name_fields = self.get_translated_fields('name')
+        self.list_display = ('id',) + self.name_fields + ('wikidata_link', 'wikiDataId', 'is_duplicated', 'updated_at')
 
     # Options
     def get_search_fields(self, request):
         return self.name_fields + self.search_fields + ('id', 'wikiDataId')
 
+    def get_translated_fields(self, field_name):
+        return get_translated_fields(self.model, field_name)
+
     # Fields
     def wikidata_link(self, obj):
         if obj.wikiDataId:
             url = f"https://www.wikidata.org/wiki/{obj.wikiDataId}"
             return format_html('<a href="{}" target="_blank">{}</a>', url, obj.wikiDataId)
         return '-'
     wikidata_link.short_description = 'WikiData ID'
```

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_cities.csv` & `django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_cities.csv`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_countries.csv` & `django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_countries.csv`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_regions.csv` & `django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_regions.csv`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_states.csv` & `django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_states.csv`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/fixtures/csc_subregions.csv` & `django-countries-states-cities-1.0.9/countries_states_cities/fixtures/csc_subregions.csv`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/management/.DS_Store` & `django-countries-states-cities-1.0.9/countries_states_cities/management/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/management/commands/__pycache__/csc_loaddata_csv.cpython-38.pyc` & `django-countries-states-cities-1.0.9/countries_states_cities/management/commands/__pycache__/csc_loaddata_csv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/management/commands/csc_dumpdata_csv.py` & `django-countries-states-cities-1.0.9/countries_states_cities/management/commands/csc_dumpdata_csv.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/management/commands/csc_loaddata_csv.py` & `django-countries-states-cities-1.0.9/countries_states_cities/management/commands/csc_loaddata_csv.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/models.py` & `django-countries-states-cities-1.0.9/countries_states_cities/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -196,8 +196,8 @@
     state = models.ForeignKey(State, on_delete=models.SET_NULL, null=True, )
     state_code = models.CharField(max_length=255, blank=True, null=True)
     state_name = models.CharField(max_length=255, blank=True, null=True)
 
     class Meta:
         verbose_name = 'city'
         verbose_name_plural = 'cities'
-        ordering = ['-created_at']
+        ordering = ['-created_at']
```

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/resource.py` & `django-countries-states-cities-1.0.9/countries_states_cities/resource.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/translation.py` & `django-countries-states-cities-1.0.9/countries_states_cities/translation.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/urls.py` & `django-countries-states-cities-1.0.9/countries_states_cities/urls.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/utils.py` & `django-countries-states-cities-1.0.9/countries_states_cities/utils.py`

 * *Files identical despite different names*

### Comparing `django-countries-states-cities-1.0.8/countries_states_cities/views.py` & `django-countries-states-cities-1.0.9/countries_states_cities/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# views.py
+
 # Python
 from decimal import Decimal
 
 # Django
 from django.db.models.expressions import RawSQL
 from django.utils.encoding import force_str
 
@@ -17,20 +19,21 @@
 
 # Django Gis
 # from django.contrib.gis.db.models.functions import Distance
 # from django.contrib.gis.measure import D
 # from django.contrib.gis.geos import Point
 
 # countries_states_cities
+from countries_states_cities.filters import SubregionFilter, RegionFilter, CountryFilter, StateFilter, CityFilter
 from countries_states_cities.models import Region, Subregion, Country, State, City
 from countries_states_cities.serializers import RegionSerializer, SubregionSerializer, CountrySerializer, StateSerializer, CitySerializer
 
 
 # Variable Section
-name_search_fields = ['name', 'name_en', 'name_ja', 'name_ko']
+from countries_states_cities.utils import get_translated_fields
 
 
 # Class Section
 def sort_by_nearest(queryset, latitude: Decimal, longitude: Decimal, max_distance=None):
     """
     Return objects sorted by distance to specified coordinates
     which distance is less than max_distance given in kilometers
@@ -144,53 +147,57 @@
                 'schema': {
                     'type': 'string',
                 },
             },
         ]
 
 
-class IdsFilterSet(django_filters.FilterSet):
-    ids = django_filters.CharFilter(method='filter_id')
-
-    def filter_id(self, queryset, name, value):
-        if value:
-            ids = [int(id) for id in value.replace(' ', '').split(',') if id]
-            print(ids)
-            queryset = queryset.filter(id__in=ids)
 
-        return queryset
 
 
 class ViewSetMixin(mixins.ListModelMixin, mixins.RetrieveModelMixin, GenericViewSet):
-    search_fields = name_search_fields
     filter_backends = [DistanceOrdering, filters.SearchFilter, DjangoFilterBackend]
-    filterset_class = IdsFilterSet
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.search_fields = self.get_search_fields()
+
+    def get_search_fields(self):
+        # get_translated_fields 함수를 사용하여 번역된 필드를 검색 필드에 포함시킵니다.
+        translated_fields = get_translated_fields(self.model, 'name')
+        return ('id', 'wikiDataId') + translated_fields  # 필요한 기본 필드와 결합
 
 
 class RegionViewSet(ViewSetMixin):
+    model = Region
     queryset = Region.objects.all()
     serializer_class = RegionSerializer
     filter_backends = ViewSetMixin.filter_backends
+    filterset_class = RegionFilter
 
 
 class SubregionViewSet(ViewSetMixin):
+    model = Subregion
     queryset = Subregion.objects.all()
     serializer_class = SubregionSerializer
-    filterset_fields = ['ids', 'region']
+    filterset_class = SubregionFilter
 
 
 class CountryViewSet(ViewSetMixin):
+    model = Country
     queryset = Country.objects.all()
     serializer_class = CountrySerializer
-    filterset_fields = ['ids', 'subregion']
+    filterset_class = CountryFilter
 
 
 class StateViewSet(ViewSetMixin):
+    model = State
     queryset = State.objects.all()
     serializer_class = StateSerializer
-    filterset_fields = ['ids', 'country']
+    filterset_class = StateFilter
 
 
 class CityViewSet(ViewSetMixin):
+    model = City
     queryset = City.objects.all()
     serializer_class = CitySerializer
-    filterset_fields = ['ids', 'country', 'state']
+    filterset_class = CityFilter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/PKG-INFO` & `django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-countries-states-cities
-Version: 1.0.8
+Version: 1.0.9
 Summary: Countries States Cities models for Django.
 Home-page: https://github.com/runners-2022/django-countries-states-cities
 Author: Sunwook Kim
 Author-email: sun@runners.im
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-countries-states-cities-1.0.8/django_countries_states_cities.egg-info/SOURCES.txt` & `django-countries-states-cities-1.0.9/django_countries_states_cities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 countries_states_cities/__init__.py
 countries_states_cities/admin.py
 countries_states_cities/apps.py
+countries_states_cities/filters.py
 countries_states_cities/models.py
 countries_states_cities/resource.py
 countries_states_cities/serializers.py
 countries_states_cities/settings.py
 countries_states_cities/tests.py
 countries_states_cities/translation.py
 countries_states_cities/urls.py
 countries_states_cities/utils.py
 countries_states_cities/views.py
 countries_states_cities/fixtures/csc_cities.csv
 countries_states_cities/fixtures/csc_countries.csv
 countries_states_cities/fixtures/csc_regions.csv
 countries_states_cities/fixtures/csc_states.csv
-countries_states_cities/fixtures/csc_states.json
 countries_states_cities/fixtures/csc_subregions.csv
 countries_states_cities/management/.DS_Store
 countries_states_cities/management/__init__.py
 countries_states_cities/management/__pycache__/__init__.cpython-38.pyc
 countries_states_cities/management/commands/__init__.py
 countries_states_cities/management/commands/csc_dumpdata_csv.py
 countries_states_cities/management/commands/csc_loaddata_csv.py
```

### Comparing `django-countries-states-cities-1.0.8/setup.cfg` & `django-countries-states-cities-1.0.9/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-countries-states-cities
-version = 1.0.8
+version = 1.0.9
 description = Countries States Cities models for Django.
 long_description_content_type = text/markdown
 long_description = file:README.md
 url = https://github.com/runners-2022/django-countries-states-cities
 author = Sunwook Kim
 author_email = sun@runners.im
 license = MIT
@@ -21,19 +21,22 @@
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	drf-yasg
-	djangorestframework
-	django-modeltranslation
+	Django
 	django-filter
 	django-import-export
+	django-modeltranslation
+	django-url-filter
+	djangorestframework
+	drf-yasg
+	requests
 
 [options.packages.find]
 exclude = 
 	config*
 	migrations*
 
 [egg_info]
```

