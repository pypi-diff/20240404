# Comparing `tmp/django_cotton-0.0.7.tar.gz` & `tmp/django_cotton-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cotton-0.0.7.tar", max compression
+gzip compressed data, was "django_cotton-0.0.8.tar", max compression
```

## Comparing `django_cotton-0.0.7.tar` & `django_cotton-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1064 2024-02-24 22:29:48.371683 django_cotton-0.0.7/LICENSE
--rw-r--r--   0        0        0      194 2024-02-24 22:29:48.371683 django_cotton-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/__init__.py
--rwxr-xr-x   0        0        0     8759 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/cotton_loader.py
--rw-r--r--   0        0        0        0 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/templatetags/__init__.py
--rw-r--r--   0        0        0     3008 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/templatetags/_component.py
--rw-r--r--   0        0        0     1249 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/templatetags/_slot.py
--rw-r--r--   0        0        0     1324 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/templatetags/_var.py
--rw-r--r--   0        0        0      862 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/templatetags/cotton.py
--rw-r--r--   0        0        0     1490 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/urls.py
--rw-r--r--   0        0        0      786 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/views.py
--rw-r--r--   0        0        0      405 2024-02-24 22:29:48.375684 django_cotton-0.0.7/django_cotton/wsgi.py
--rw-r--r--   0        0        0     1233 2024-02-24 22:29:50.591717 django_cotton-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 django_cotton-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-04 12:43:29.400761 django_cotton-0.0.8/LICENSE
+-rw-r--r--   0        0        0      194 2024-04-04 12:43:29.400761 django_cotton-0.0.8/README.md
+-rw-r--r--   0        0        0       40 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/__init__.py
+-rw-r--r--   0        0        0     2356 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/apps.py
+-rwxr-xr-x   0        0        0    12697 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/cotton_loader.py
+-rw-r--r--   0        0        0        0 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/__init__.py
+-rw-r--r--   0        0        0     1924 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_component.py
+-rw-r--r--   0        0        0     1362 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_props.py
+-rw-r--r--   0        0        0     2525 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_props_frame.py
+-rw-r--r--   0        0        0     1686 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_slot.py
+-rw-r--r--   0        0        0      996 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/cotton.py
+-rw-r--r--   0        0        0     1701 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/urls.py
+-rw-r--r--   0        0        0      786 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/views.py
+-rw-r--r--   0        0        0      405 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/wsgi.py
+-rw-r--r--   0        0        0     1233 2024-04-04 12:43:33.184802 django_cotton-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 django_cotton-0.0.8/PKG-INFO
```

### Comparing `django_cotton-0.0.7/LICENSE` & `django_cotton-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.7/django_cotton/templatetags/_var.py` & `django_cotton-0.0.8/django_cotton/templatetags/_props.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from django import template
 
 register = template.Library()
 
 
-def cotton_var(parser, token):
+def cotton_props(parser, token):
     # Split the token to get variable assignments
     parts = token.split_contents()
-    cotton_vars = {}
+    cotton_props = {}
     for part in parts[1:]:
-        key, value = part.split('=')
-        cotton_vars[key] = value
+        key, value = part.split("=")
+        cotton_props[key] = value
 
-    return CottonVarNode(cotton_vars)
+    return CottonPropNode(cotton_props)
 
 
-register.tag("cotton_var", cotton_var)
-
-
-class CottonVarNode(template.Node):
-    def __init__(self, cotton_vars):
-        self.cotton_vars = cotton_vars
+class CottonPropNode(template.Node):
+    def __init__(self, cotton_props):
+        self.cotton_props = cotton_props
 
     def render(self, context):
-        resolved_vars = {}
+        resolved_props = {}
 
         # if the same var is already set in context, it's being passed explicitly to override the cotton_var
         # if not, then we resolve it from the context
-        for key, value in self.cotton_vars.items():
+        for key, value in self.cotton_props.items():
             # if key in context:
-            #     resolved_vars[key] = context[key]
+            #     resolved_props[key] = context[key]
             #     continue
             try:
-                resolved_vars[key] = template.Variable(value).resolve(context)
+                resolved_props[key] = template.Variable(value).resolve(context)
             except (TypeError, template.VariableDoesNotExist):
-                resolved_vars[key] = value
+                resolved_props[key] = value
 
-        cotton_vars = {'cotton_vars': resolved_vars}
+        cotton_props = {"cotton_props": resolved_props}
 
         # Update the global context directly
-        context.update(resolved_vars)
-        context.update(cotton_vars)
-        context['cotton_vars'].update(resolved_vars)
+        context.update(resolved_props)
+        context.update(cotton_props)
+        context.update({"cotton_props": resolved_props})
+        context["cotton_props"].update(resolved_props)
 
-        return ''
+        return ""
```

### Comparing `django_cotton-0.0.7/django_cotton/templatetags/cotton.py` & `django_cotton-0.0.8/django_cotton/templatetags/cotton.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from django import template
 from django.utils.html import format_html_join
 
 from django_cotton.templatetags._component import cotton_component
 from django_cotton.templatetags._slot import cotton_slot
-from django_cotton.templatetags._var import cotton_var
+from django_cotton.templatetags._props import cotton_props
+from django_cotton.templatetags._props_frame import cotton_props_frame
 
 register = template.Library()
 register.tag("cotton_component", cotton_component)
 register.tag("cotton_slot", cotton_slot)
-register.tag("cotton_var", cotton_var)
+register.tag("cotton_props", cotton_props)
+register.tag("cotton_props_frame", cotton_props_frame)
 
 
 @register.filter
 def merge(attrs, args):
     # attrs is expected to be a dictionary of existing attributes
     # args is a string of additional attributes to merge, e.g., "class:extra-class"
     for arg in args.split(","):
```

### Comparing `django_cotton-0.0.7/django_cotton/urls.py` & `django_cotton-0.0.8/django_cotton/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,13 @@
     path("test/compiled-cotton", views.compiled_cotton_test_view),
     path("test/cotton", views.cotton_test_view),
     path("test/native-extends", views.native_extends_test_view),
     path("test/native-include", views.native_include_test_view),
     path("attribute-merging", views.attribute_merging_test_view),
     path("attribute-passing", views.attribute_passing_test_view),
     path("django-syntax-decoding", views.django_syntax_decoding_test_view),
+    path(
+        "string-with-spaces",
+        TemplateView.as_view(template_name="string_with_spaces.cotton.html"),
+    ),
+    path("props-test", TemplateView.as_view(template_name="props_test.cotton.html")),
 ]
```

### Comparing `django_cotton-0.0.7/django_cotton/views.py` & `django_cotton-0.0.8/django_cotton/views.py`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.7/pyproject.toml` & `django_cotton-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-cotton"
-version = "0.0.7"
+version = "0.0.8"
 description = "Bringing component based design to Django templates."
 authors = [ "Will Abbott <wabbott@dyvenia.com>",]
 license = "MIT"
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Programming Language :: Python :: 3.10", "Framework :: Django",]
 keywords = [ "django", "cotton", "reusable", "app",]
 exclude = [ "dev", "docs", "django_cotton/tests", "django_cotton/templates",]
```

### Comparing `django_cotton-0.0.7/PKG-INFO` & `django_cotton-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cotton
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bringing component based design to Django templates.
 License: MIT
 Keywords: django,cotton,reusable,app
 Author: Will Abbott
 Author-email: wabbott@dyvenia.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha
```

