# Comparing `tmp/fab-react-toolkit-0.2.9.tar.gz` & `tmp/fab-react-toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.2.9.tar", last modified: Fri Feb  2 15:46:16 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.3.0.tar", last modified: Thu Apr  4 09:42:32 2024, max compression
```

## Comparing `fab-react-toolkit-0.2.9.tar` & `fab-react-toolkit-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.354754 fab-react-toolkit-0.2.9/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    26896 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-02 15:46:16.000000 fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-02 15:46:02.000000 fab-react-toolkit-0.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-02 15:46:16.358754 fab-react-toolkit-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.191697 fab-react-toolkit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 09:42:32.191697 fab-react-toolkit-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.187697 fab-react-toolkit-0.3.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.187697 fab-react-toolkit-0.3.0/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.187697 fab-react-toolkit-0.3.0/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.191697 fab-react-toolkit-0.3.0/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:32.191697 fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 09:42:32.000000 fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 09:42:32.000000 fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:42:32.000000 fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 09:42:32.000000 fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 09:42:23.000000 fab-react-toolkit-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 09:42:32.191697 fab-react-toolkit-0.3.0/setup.cfg
```

### Comparing `fab-react-toolkit-0.2.9/LICENSE` & `fab-react-toolkit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/PKG-INFO` & `fab-react-toolkit-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.2.9
+Version: 0.3.0
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.2.9/example/app/__init__.py` & `fab-react-toolkit-0.3.0/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/example/app/apis.py` & `fab-react-toolkit-0.3.0/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/example/app/config.py` & `fab-react-toolkit-0.3.0/example/app/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # The SQLAlchemy connection string.
 SQLALCHEMY_DATABASE_URI = "sqlite:///" + os.path.join(basedir, "../app.db")
 # SQLALCHEMY_DATABASE_URI = 'mysql://myapp@localhost/myapp'
 # SQLALCHEMY_DATABASE_URI = 'postgresql://root:password@localhost/myapp'
 
 # Flask-WTF flag for CSRF
 CSRF_ENABLED = True
-FAB_API_SWAGGER_UI = True
 
 # ------------------------------
 # GLOBALS FOR APP Builder
 # ------------------------------
 APP_NAME = "FAB React Toolkit Example"
 WEBAPP = False
 # Uncomment to setup Setup an App icon
```

### Comparing `fab-react-toolkit-0.2.9/example/app/models.py` & `fab-react-toolkit-0.3.0/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/example/run.py` & `fab-react-toolkit-0.3.0/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from flask import render_template_string, send_file
-from flask_appbuilder.api.manager import OpenApi
-from .views import OpenAPIView, IndexView
-from .apis import AuthApi, InfoApi, PermissionViewApi, PermissionsApi, RolesApi, UsersApi, ViewsMenusApi
+from .views import OpenAPIView, IndexView 
+from .apis import AuthApi, InfoApi, PermissionViewApi, PermissionsApi, RolesApi, UsersApi, ViewsMenusApi, OpenApi
 from .api import ModelRestApi
 from .interface import SQLAInterface
 
 import io
 class FABReactToolkit(object):
 
     def __init__(self, appbuilder):
```

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             search_filters[col] = {'label': self.label_columns[col], 'filters': [
                 {"name": as_unicode(flt.name), "operator": flt.arg_name,
                  }
                 for flt in dict_filters[col]
             ]}
             # Add schema info
             search_filters[col]['schema'] = self._get_field_info(self.search_model_schema.fields[col],
-                                                                 self.search_query_rel_fields)
+                                                                 self.search_query_rel_fields.get(col, []))
         response[API_FILTERS_RES_KEY] = search_filters
 
     def merge_filter_options(self, response, **kwargs):
         """
         Overrides parent method to add the schema of a filter to the response. Selection is based on show columns.
         :param response: The response object
         :param kwargs: api endpoint kwargs
```

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import jwt
 import re
 import datetime
-
-from flask import request, redirect, g
+from apispec import APISpec
+from apispec.ext.marshmallow import MarshmallowPlugin
+from apispec.ext.marshmallow.common import resolve_schema_cls
+from flask import request, redirect, g, current_app
 from flask_login import current_user, login_user, logout_user, login_required
 from flask_appbuilder import expose
 from flask_appbuilder.api import BaseApi, Model2SchemaConverter, safe
 from flask_appbuilder.models.sqla.interface import SQLAInterface
 from flask_appbuilder.security.manager import AUTH_DB, AUTH_LDAP, AUTH_REMOTE_USER
 from flask_appbuilder.security.sqla.models import User, Permission, PermissionView, Role, ViewMenu
 from werkzeug.security import generate_password_hash
@@ -708,7 +710,77 @@
 
     # this also effects schema of related models
     page_size = 200
     max_page_size = 200
 
     resource_name = "viewsmenus"
     base_permissions = ['can_get', 'can_info']
+
+
+
+def resolver(schema):
+    schema_cls = resolve_schema_cls(schema)
+    name = schema_cls.__name__
+    if name == "MetaSchema":
+        if hasattr(schema_cls, "Meta"):
+            return (
+                f"{schema_cls.Meta.parent_schema_name}.{schema_cls.Meta.model.__name__}"
+            )
+    if name.endswith("Schema"):
+        return name[:-6] or name
+    return name
+
+
+class OpenApi(BaseApi):
+    route_base = "/api"
+    allow_browser_login = True
+
+    @expose("/<version>/_openapi")
+    @safe
+    def get(self, version):
+        """Endpoint that renders an OpenApi spec for all views that belong
+            to a certain version
+        ---
+        get:
+          description: >-
+            Get the OpenAPI spec for a specific API version
+          parameters:
+          - in: path
+            schema:
+              type: string
+            name: version
+          responses:
+            200:
+              description: The OpenAPI spec
+              content:
+                application/json:
+                  schema:
+                    type: object
+            404:
+              $ref: '#/components/responses/404'
+            500:
+              $ref: '#/components/responses/500'
+        """
+        version_found = False
+        api_spec = self._create_api_spec(version)
+        for base_api in current_app.appbuilder.baseviews:
+            if isinstance(base_api, BaseApi) and base_api.version == version:
+                base_api.add_api_spec(api_spec)
+                version_found = True
+        if version_found:
+            return self.response(200, **api_spec.to_dict())
+        else:
+            return self.response_404()
+
+    @staticmethod
+    def _create_api_spec(version):
+        servers = current_app.config.get(
+            "FAB_OPENAPI_SERVERS", [{"url": request.host_url}]
+        )
+        return APISpec(
+            title=current_app.appbuilder.app_name,
+            version=version,
+            openapi_version="3.0.2",
+            info=dict(description=current_app.appbuilder.app_name),
+            plugins=[MarshmallowPlugin(schema_name_resolver=resolver)],
+            servers=servers,
+        )
```

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit/views.py` & `fab-react-toolkit-0.3.0/fab_react_toolkit/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import os
 
 from flask import url_for
 from flask_appbuilder import BaseView, expose, IndexView as FABIndexView
-from flask_appbuilder.api.manager import OpenApi
-
+from .apis import OpenApi
 
 class OpenAPIView(BaseView):
     route_base = "/openapi"
     default_view = "show"
 
     @expose("/<version>")
     def show(self, version):
```

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.2.9
+Version: 0.3.0
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.2.9/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.3.0/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.2.9/pyproject.toml` & `fab-react-toolkit-0.3.0/pyproject.toml`

 * *Files identical despite different names*

