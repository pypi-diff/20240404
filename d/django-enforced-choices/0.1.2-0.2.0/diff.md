# Comparing `tmp/django-enforced-choices-0.1.2.tar.gz` & `tmp/django-enforced-choices-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-enforced-choices-0.1.2.tar", last modified: Mon Sep 18 10:33:53 2023, max compression
+gzip compressed data, was "django-enforced-choices-0.2.0.tar", last modified: Thu Apr  4 19:03:32 2024, max compression
```

## Comparing `django-enforced-choices-0.1.2.tar` & `django-enforced-choices-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.778274 django-enforced-choices-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.778274 django-enforced-choices-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/.github/workflows/django-enforced-choices-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/django_enforced_choices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/django_enforced_choices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/django_enforced_choices/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/django_enforced_choices/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/django_enforced_choices/fields/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/django_enforced_choices/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-09-18 10:33:53.000000 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-09-18 10:33:53.000000 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 10:33:53.000000 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-18 10:33:53.000000 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-18 10:33:53.000000 django-enforced-choices-0.1.2/django_enforced_choices.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/api_fields_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/api_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/docs/source/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-09-18 10:33:53.782274 django-enforced-choices-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 10:33:49.000000 django-enforced-choices-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/.github/workflows/django-enforced-choices-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/django_enforced_choices/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/django_enforced_choices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/django_enforced_choices/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/django_enforced_choices/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/django_enforced_choices/fields/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/django_enforced_choices/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-04 19:03:32.000000 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-04 19:03:32.000000 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:03:32.000000 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 19:03:32.000000 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 19:03:32.000000 django-enforced-choices-0.2.0/django_enforced_choices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/api_fields_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/api_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/docs/source/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 19:03:32.455948 django-enforced-choices-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:03:28.000000 django-enforced-choices-0.2.0/setup.py
```

### Comparing `django-enforced-choices-0.1.2/.github/workflows/django-enforced-choices-ci.yml` & `django-enforced-choices-0.2.0/.github/workflows/django-enforced-choices-ci.yml`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/LICENSE` & `django-enforced-choices-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/PKG-INFO` & `django-enforced-choices-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: django-enforced-choices
-Version: 0.1.2
-Summary: A Django package to enforce choices as database constraints.
-Home-page: https://github.com/hapytex/django-enforced-choices/
-Author: Willem Van Onsem
-Author-email: yourfriends@hapytex.eu
-License: BSD-3-Clause
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django-enforced-choices
 
 [![PyPi version](https://badgen.net/pypi/v/django-enforced-choices/)](https://pypi.python.org/pypi/django-enforced-choices/)
 [![Documentation Status](https://readthedocs.org/projects/django-enforced-choices/badge/?version=latest)](http://django-enforced-choices.readthedocs.io/?badge=latest)
 [![PyPi license](https://badgen.net/pypi/license/django-enforced-choices/)](https://pypi.python.org/pypi/django-enforced-choices/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -55,29 +26,39 @@
 
 we can then fill the table with a data migration for example. This also makes some sense: a quote I once heared is that there should only be three constants in programming: zero, one and infinity, meaning that typically one should not restrict the number of genres.
 
 But regardless, people often use the former model. This is good if we work with `Form`s, or `Serializer`s, but models don't (eagerly) validate data, and even if they did, the database does not know about the choices, and thus will happily accept `'s'` as value (for example for science fiction).
 
 ## What does this package provide?
 
-This package provides a `ChoicesConstraintModelMixin` mixin to mix into models. This will look for the model fields, and if there are choices it will add `CheckConstraint`s for these fields. One can exclude certain fields that have choices by adding the corresponding names in a class attribute named `exclude_choice_check_fields`, which is by default empty.
+This package provides two mixins:
+
+ - `ChoicesConstraintModelMixin` which checks on the `choices=` parameter of the fields of that model, and based on that, creates a constraint to enforce the choices at the datbase side; and
+ - `RangeConstraintModelMixin`, which checks the `validators=` parameter of the fields of that model, and based on that, creates a constraint to enforce that at the database side.
+
+You can combine the mixins that are defined with `FullChoicesConstraintModelMixin`, it is probably advisable to use `FullChoicesConstraintModelMixin` over the mixins defined above, since as more validators are enforced ,
+it will automatically add more constraints for these models, whereas `ChoicesConstraintModelMixin` for example, will only limit itself to choices.
+
+One can exclude certain fields with the `exclude_choice_check_fields` and `exclude_range_check_fields` attributes that you can alter in the model. These need to provide a collection of strings that contain the *name* of the field.
 
 Another option is to import the correspond field from the `django_enforced_choices.fields` module, or `django_enforced_choices.fields.postgres` for PostgreSQL-specific fields. This will, by default, also check if the fields have choices, but we do *not* recommend to use these, since this means the field has for example as type `ChoiceCharField`, and certain Django functionalities (and packages) sometimes check full type equality to determine a widget, not through an `instanceof`. This thus means that certain functionalities might no longer work as intended.
 
 ### Usage
 
 One can import the `ChoicesConstraintModelMixin` and mix it into a model, like:
 
 ```
-from django_enforced_choices.models import ChoicesConstraintModelMixin
+from django.core.validators import MaxValuevalidator, MinValueValidator 
+from django_enforced_choices.models import FullChoicesConstraintModelMixin
 
-class Movie(ChoicesConstraintModelMixin, models.Model):
+class Movie(FullChoicesConstraintModelMixin, models.Model):
     genre = models.CharField(max_length=1, choices=[('d', 'drama'), ('h', 'horror')])
+    year = models.IntegerField(validators=[MinValueValidator(1888)])
 ```
 
-this will then add `CheckConstraint`s to the model to enforce that `genre` only can contain `'d'` and `'h'` at the database side.
+this will then add `CheckConstraint`s to the model to enforce that `genre` only can contain `'d'` and `'h'` at the database side, and that the `year` is greater than or equal to [1888](https://en.wikipedia.org/wiki/Roundhay_Garden_Scene).
 
 ## How does the package work?
 
-For the fields defined, it will check if the `choices` are defined. If that is the case, it will create a `CheckConstraint` with `fieldname__in` with the keys in the choices. If the field is NULLable, it will also allow `NULL`/`None` to be used.
-
+For the fields defined, it will check if the `choices` and `validators` are defined.  If that is the case, it will create a `CheckConstraint` with `fieldname__in` with the keys in the choices for choices, and `__range`, `__lte` or `__gte` for ranges depending on what values are picked.
 
+If the field is NULLable, it will also allow `NULL`/`None` to be used.
```

### Comparing `django-enforced-choices-0.1.2/django_enforced_choices/fields/postgres.py` & `django-enforced-choices-0.2.0/django_enforced_choices/fields/postgres.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     DateRangeField,
     DateTimeRangeField,
     DecimalRangeField,
     HStoreField,
     IntegerRangeField,
     RangeField,
 )
-from django_enforce_choices.fields import ChoicesConstraintMixin
+from django_enforce_choices.fields import ChoicesConstraintMixin, RangeConstraintMixin
 
 
 class ChoiceArrayField(ChoicesConstraintMixin, ArrayField):
     pass
 
 
 class ChoiceBigIntegerRangeField(ChoicesConstraintMixin, BigIntegerRangeField):
@@ -52,7 +52,51 @@
 
 class ChoiceIntegerRangeField(ChoicesConstraintMixin, IntegerRangeField):
     pass
 
 
 class ChoiceRangeField(ChoicesConstraintMixin, RangeField):
     pass
+
+
+class RangeArrayField(RangeConstraintMixin, ArrayField):
+    pass
+
+
+class RangeBigIntegerRangeField(RangeConstraintMixin, BigIntegerRangeField):
+    pass
+
+
+class RangeCICharField(RangeConstraintMixin, CICharField):
+    pass
+
+
+class RangeCIEmailField(RangeConstraintMixin, CIEmailField):
+    pass
+
+
+class RangeCITextField(RangeConstraintMixin, CITextField):
+    pass
+
+
+class RangeDateRangeField(RangeConstraintMixin, DateRangeField):
+    pass
+
+
+class RangeDateTimeRangeField(RangeConstraintMixin, DateTimeRangeField):
+    pass
+
+
+class RangeDecimalRangeField(RangeConstraintMixin, DecimalRangeField):
+    pass
+
+
+class RangeHStoreField(RangeConstraintMixin, HStoreField):
+    pass
+
+
+class RangeIntegerRangeField(RangeConstraintMixin, IntegerRangeField):
+    pass
+
+
+class RangeRangeField(RangeConstraintMixin, RangeField):
+    pass
```

### Comparing `django-enforced-choices-0.1.2/django_enforced_choices/models.py` & `django-enforced-choices-0.2.0/django_enforced_choices/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,90 @@
 from django.db import models
 from django.db.models.base import ModelBase
 
 # Create your models here.
 
-from .fields import add_choice_constraint
+from .fields import add_choice_constraint, add_range_constraint
 
 
-class ChoicesConstraintModelMetaMixin(ModelBase):
+class ConstraintMetaMixin:
+    def check_fields(cls, exclude_attribute_name, add_check):
+        to_exclude = set(getattr(cls, exclude_attribute_name, ()) or ())
+        for field in cls._meta.fields:
+            if field.name not in to_exclude:
+                add_check(field, cls, field.name)
+
+
+class ChoicesConstraintModelMetaMixin(ConstraintMetaMixin, ModelBase):
     """
     A meta-class with the logic in the _prepare method to inspect the fields, and
     add CheckConstraints for the fields that have choices.
     """
 
     def _prepare(cls, *args, **kwargs):
         """
         Override the _prepare method to also add CheckConstraints for the corresponding
         fields.
         """
-        to_exclude = getattr(cls, "exclude_choice_check_fields", ()) or ()
         super()._prepare(*args, **kwargs)
-        for field in cls._meta.fields:
-            if field.name not in to_exclude:
-                add_choice_constraint(field, cls, field.name)
+        cls.check_fields("exclude_choice_check_fields", add_choice_constraint)
 
 
-class ChoicesConstraintModelMixin(metaclass=ChoicesConstraintModelMetaMixin):
+class RangeConstraintModelMetaMixin(ConstraintMetaMixin, ModelBase):
+    """
+    A meta-class with the logic in the _prepare method to inspect the fields, and
+    add CheckConstraints for the fields that have choices.
+    """
+
+    def _prepare(cls, *args, **kwargs):
+        """
+        Override the _prepare method to also add CheckConstraints for the corresponding
+        fields.
+        """
+        super()._prepare(*args, **kwargs)
+        cls.check_fields("exclude_range_check_fields", add_range_constraint)
+
+
+class FullConstraintModelMetaMixin(
+    ChoicesConstraintModelMetaMixin, RangeConstraintModelMetaMixin, ModelBase
+):
+    pass
+
+
+class ChoicesConstraintModelMixin(
+    models.Model, metaclass=ChoicesConstraintModelMetaMixin
+):
     """
     A model mixin, essentially what it does is ensuring that the model inherits
     from the ChoicesConstraintsModelMetaMixin, a subclass of ModelBase, which
     has some extra _prepare logic.
     """
 
     exclude_choice_check_fields = ()
+
+    class Meta:
+        abstract = True
+
+
+class RangeConstraintModelMixin(
+    models.Model, metaclass=ChoicesConstraintModelMetaMixin
+):
+    """
+    A model mixin, essentially what it does is ensuring that the model inherits
+    from the ChoicesConstraintsModelMetaMixin, a subclass of ModelBase, which
+    has some extra _prepare logic.
+    """
+
+    exclude_range_check_fields = ()
+
+    class Meta:
+        abstract = True
+
+
+class FullChoicesConstraintModelMixin(
+    ChoicesConstraintModelMixin,
+    RangeConstraintModelMixin,
+    models.Model,
+    metaclass=FullConstraintModelMetaMixin,
+):
+    class Meta:
+        abstract = True
```

### Comparing `django-enforced-choices-0.1.2/django_enforced_choices.egg-info/PKG-INFO` & `django-enforced-choices-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-enforced-choices
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Django package to enforce choices as database constraints.
 Home-page: https://github.com/hapytex/django-enforced-choices/
 Author: Willem Van Onsem
 Author-email: yourfriends@hapytex.eu
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -55,29 +55,41 @@
 
 we can then fill the table with a data migration for example. This also makes some sense: a quote I once heared is that there should only be three constants in programming: zero, one and infinity, meaning that typically one should not restrict the number of genres.
 
 But regardless, people often use the former model. This is good if we work with `Form`s, or `Serializer`s, but models don't (eagerly) validate data, and even if they did, the database does not know about the choices, and thus will happily accept `'s'` as value (for example for science fiction).
 
 ## What does this package provide?
 
-This package provides a `ChoicesConstraintModelMixin` mixin to mix into models. This will look for the model fields, and if there are choices it will add `CheckConstraint`s for these fields. One can exclude certain fields that have choices by adding the corresponding names in a class attribute named `exclude_choice_check_fields`, which is by default empty.
+This package provides two mixins:
+
+ - `ChoicesConstraintModelMixin` which checks on the `choices=` parameter of the fields of that model, and based on that, creates a constraint to enforce the choices at the datbase side; and
+ - `RangeConstraintModelMixin`, which checks the `validators=` parameter of the fields of that model, and based on that, creates a constraint to enforce that at the database side.
+
+You can combine the mixins that are defined with `FullChoicesConstraintModelMixin`, it is probably advisable to use `FullChoicesConstraintModelMixin` over the mixins defined above, since as more validators are enforced ,
+it will automatically add more constraints for these models, whereas `ChoicesConstraintModelMixin` for example, will only limit itself to choices.
+
+One can exclude certain fields with the `exclude_choice_check_fields` and `exclude_range_check_fields` attributes that you can alter in the model. These need to provide a collection of strings that contain the *name* of the field.
 
 Another option is to import the correspond field from the `django_enforced_choices.fields` module, or `django_enforced_choices.fields.postgres` for PostgreSQL-specific fields. This will, by default, also check if the fields have choices, but we do *not* recommend to use these, since this means the field has for example as type `ChoiceCharField`, and certain Django functionalities (and packages) sometimes check full type equality to determine a widget, not through an `instanceof`. This thus means that certain functionalities might no longer work as intended.
 
 ### Usage
 
 One can import the `ChoicesConstraintModelMixin` and mix it into a model, like:
 
 ```
-from django_enforced_choices.models import ChoicesConstraintModelMixin
+from django.core.validators import MaxValuevalidator, MinValueValidator 
+from django_enforced_choices.models import FullChoicesConstraintModelMixin
 
-class Movie(ChoicesConstraintModelMixin, models.Model):
+class Movie(FullChoicesConstraintModelMixin, models.Model):
     genre = models.CharField(max_length=1, choices=[('d', 'drama'), ('h', 'horror')])
+    year = models.IntegerField(validators=[MinValueValidator(1888)])
 ```
 
-this will then add `CheckConstraint`s to the model to enforce that `genre` only can contain `'d'` and `'h'` at the database side.
+this will then add `CheckConstraint`s to the model to enforce that `genre` only can contain `'d'` and `'h'` at the database side, and that the `year` is greater than or equal to [1888](https://en.wikipedia.org/wiki/Roundhay_Garden_Scene).
 
 ## How does the package work?
 
-For the fields defined, it will check if the `choices` are defined. If that is the case, it will create a `CheckConstraint` with `fieldname__in` with the keys in the choices. If the field is NULLable, it will also allow `NULL`/`None` to be used.
+For the fields defined, it will check if the `choices` and `validators` are defined.  If that is the case, it will create a `CheckConstraint` with `fieldname__in` with the keys in the choices for choices, and `__range`, `__lte` or `__gte` for ranges depending on what values are picked.
+
+If the field is NULLable, it will also allow `NULL`/`None` to be used.
```

### Comparing `django-enforced-choices-0.1.2/django_enforced_choices.egg-info/SOURCES.txt` & `django-enforced-choices-0.2.0/django_enforced_choices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/docs/Makefile` & `django-enforced-choices-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/docs/make.bat` & `django-enforced-choices-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/docs/source/conf.py` & `django-enforced-choices-0.2.0/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Configuration file for the Sphinx documentation builder.
 
 # -- Project information
 
 project = "django-enforced-choices"
-copyright = "2023, Willem Van Onsem"
+copyright = "2023-2024, Willem Van Onsem"
 author = "Willem Van Onsem"
 
-release = "0.1.2"
-version = "0.1.2"
+release = "0.2.0"
+version = "0.2.0"
 
 from os import environ
 from os.path import dirname
 from sys import path
 
 path.insert(0, dirname(dirname(dirname(__file__))))
 environ.setdefault("DJANGO_SETTINGS_MODULE", "docs.source.settings")
```

### Comparing `django-enforced-choices-0.1.2/docs/source/getting_started.rst` & `django-enforced-choices-0.2.0/docs/source/getting_started.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 ===============
 Getting started
 ===============
 
-Once the package is installed, you can use the `ChoicesConstraintModelMetaMixin` mixin in the models, for example:
+Once the package is installed, you can use the `FullChoicesConstraintModelMixin` mixin in the models, for example:
 
   .. code-block:: python3
-   
+
+   from django.core.validators import MinValueValidator
    from django.db import models
-   from django_enforced_choices import ChoicesConstraintModelMetaMixin
+   from django_enforced_choices import FullChoicesConstraintModelMixin
 
    
-   class Movie(ChoicesConstraintModelMetaMixin, models.Model):
+   class Movie(FullChoicesConstraintModelMixin, models.Model):
        genre = models.CharField(max_length=1, choices=[('d', 'drama'), ('h', 'horror')])
+       year = models.IntegerField(validators=[MinValueValidator(1888)])
 
-When we then run `makemigrations` it will create a model with the `genre` field, and include a `CheckConstraint` to restrict the values to `'d'` and `'h'`.
+When we then run `makemigrations` it will create a model with the `genre` field, and include a `CheckConstraint` to restrict the values to `'d'` and `'h'`; and the `year` field with a `CheckConstraint` that ensures the value is greater than or equal to 1888.
```

### Comparing `django-enforced-choices-0.1.2/docs/source/index.rst` & `django-enforced-choices-0.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/docs/source/settings.py` & `django-enforced-choices-0.2.0/docs/source/settings.py`

 * *Files identical despite different names*

### Comparing `django-enforced-choices-0.1.2/setup.cfg` & `django-enforced-choices-0.2.0/setup.cfg`

 * *Files identical despite different names*

