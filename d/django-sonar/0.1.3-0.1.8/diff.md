# Comparing `tmp/django_sonar-0.1.3.tar.gz` & `tmp/django_sonar-0.1.8.tar.gz`

## Comparing `django_sonar-0.1.3.tar` & `django_sonar-0.1.8.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 django_sonar-0.1.3/manage.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_sonar-0.1.3/requirements.txt
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 django_sonar-0.1.3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/asgi.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/settings.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/urls.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/wsgi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/admin.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/apps.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/mixins.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/tests.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/urls.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/utils.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/middlewares/__init__.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/middlewares/requests.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/migrations/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/sonar_data.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/sonar_request.py
--rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap-icons.min.css
--rw-r--r--   0        0        0   155845 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap.min.css
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/dark-theme.css
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/django-sonar.css
--rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    78743 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0    48036 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/js/htmx.min.js
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/media/logos/favicon.png
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/denied.html
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/login.html
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/dumps/index.html
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/exceptions/index.html
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/home/index.html
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/layouts/auth.html
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/queries/index.html
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail.html
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_dumps.html
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_exception.html
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_headers.html
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_middlewares.html
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_payload.html
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_queries.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_session.html
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/index.html
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/signals/index.html
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 django_sonar-0.1.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sonar-0.1.3/LICENSE
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 django_sonar-0.1.3/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_sonar-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 django_sonar-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 django_sonar-0.1.8/manage.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_sonar-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 django_sonar-0.1.8/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.8/base/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.8/base/asgi.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 django_sonar-0.1.8/base/settings.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 django_sonar-0.1.8/base/urls.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.8/base/wsgi.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/admin.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/apps.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/mixins.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/tests.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/urls.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/utils.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/middlewares/__init__.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/middlewares/requests.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/migrations/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/models/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/models/sonar_data.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/models/sonar_request.py
+-rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/css/bootstrap-icons.min.css
+-rw-r--r--   0        0        0   155845 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/css/bootstrap.min.css
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/css/dark-theme.css
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/css/django-sonar.css
+-rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    78743 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0    48036 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/js/htmx.min.js
+-rw-r--r--   0        0        0   236163 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/js/sql-formatter.min.js
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/static/django_sonar/media/logos/favicon.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/auth/denied.html
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/auth/login.html
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/dumps/index.html
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/exceptions/index.html
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/home/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/layouts/auth.html
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/queries/detail.html
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/queries/index.html
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail.html
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_dumps.html
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_exception.html
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_headers.html
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_middlewares.html
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_payload.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_queries.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_session.html
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/index.html
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 django_sonar-0.1.8/django_sonar/templates/django_sonar/signals/index.html
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 django_sonar-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sonar-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 django_sonar-0.1.8/README.md
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 django_sonar-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 django_sonar-0.1.8/PKG-INFO
```

### Comparing `django_sonar-0.1.3/manage.py` & `django_sonar-0.1.8/manage.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/setup.py` & `django_sonar-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from setuptools import setup, find_packages
 
+import django_sonar
+
 setup(
     name='django_sonar',
-    version='0.1.3',
+    version=django_sonar.VERSION,
     author='Metalogico',
     author_email='michele.brandolin@gmail.com',
     description='The missing debug tool for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/metalogico/django-sonar',
     project_urls={
         "Bug Tracker": "https://github.com/metalogico/django-sonar/issues"
     },
 
     license='MIT',
-    packages=find_packages(),
+    packages=['django_sonar'],
     include_package_data=True,
+    package_data={'django_sonar': ['templates/*']},
     install_requires=[
         'Django>=4.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

### Comparing `django_sonar-0.1.3/base/settings.py` & `django_sonar-0.1.8/base/settings.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/mixins.py` & `django_sonar-0.1.8/django_sonar/mixins.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/urls.py` & `django_sonar-0.1.8/django_sonar/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.urls import path, include
 
 from django_sonar.views import SonarHomeView, SonarLoginView, SonarLogoutView, SonarRequestListView, \
     SonarExceptionsListView, SonarDumpsListView, SonarSignalsListView, SonarQueriesListView, SonarRequestDetailView, \
     SonarRequestClearView, SonarDetailPayloadView, SonarDetailHeadersView, SonarDetailSessionView, \
-    SonarDetailMiddlewaresView, SonarDetailQueriesView, SonarDetailDumpsView, SonarDetailExceptionView, SonarDeniedView
+    SonarDetailMiddlewaresView, SonarDetailQueriesView, SonarDetailDumpsView, SonarDetailExceptionView, SonarDeniedView, \
+    SonarQueriesDetailView
 
 urlpatterns = [
     # general
     path('', SonarHomeView.as_view(), name='sonar_index'),
     path('login/', SonarLoginView.as_view(), name='sonar_login'),
     path('logout/', SonarLogoutView.as_view(), name='sonar_logout'),
     path('denied/', SonarDeniedView.as_view(), name='sonar_denied'),
@@ -16,14 +17,17 @@
     path('requests/', SonarRequestListView.as_view(), name='sonar_requests'),
     path('requests/<uuid:uuid>/', SonarRequestDetailView.as_view(), name='sonar_request_detail'),
     path('exceptions/', SonarExceptionsListView.as_view(), name='sonar_exceptions'),
     path('queries/', SonarQueriesListView.as_view(), name='sonar_queries'),
     path('dumps/', SonarDumpsListView.as_view(), name='sonar_dumps'),
     path('signals/', SonarSignalsListView.as_view(), name='sonar_signals'),
 
+    # queries detail
+    path('queries/<uuid:uuid>/q/<int:index>/', SonarQueriesDetailView.as_view(), name='sonar_queries_detail'),
+
     # request details
     path('requests/<uuid:uuid>/payload/', SonarDetailPayloadView.as_view(), name='sonar_detail_payload'),
     path('requests/<uuid:uuid>/headers/', SonarDetailHeadersView.as_view(), name='sonar_detail_headers'),
     path('requests/<uuid:uuid>/queries/', SonarDetailQueriesView.as_view(), name='sonar_detail_queries'),
     path('requests/<uuid:uuid>/session/', SonarDetailSessionView.as_view(), name='sonar_detail_session'),
     path('requests/<uuid:uuid>/dumps/', SonarDetailDumpsView.as_view(), name='sonar_detail_dumps'),
     path('requests/<uuid:uuid>/middlewares/', SonarDetailMiddlewaresView.as_view(), name='sonar_detail_middlewares'),
```

### Comparing `django_sonar-0.1.3/django_sonar/utils.py` & `django_sonar-0.1.8/django_sonar/utils.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/views.py` & `django_sonar-0.1.8/django_sonar/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,16 +73,18 @@
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         queries = SonarData.objects.filter(category='queries').order_by('-created_at').all()
         # extract queries from SonarData queries
         context['queries'] = []
         for query in queries:
             if 'executed_queries' in query.data:
-                for executed_query in query.data['executed_queries']:
+                for index, executed_query in enumerate(query.data['executed_queries'], start=0):
                     executed_query['created_at'] = query.created_at
+                    executed_query['sonar_request_id'] = query.sonar_request_id
+                    executed_query['index'] = index
                     context['queries'].append(executed_query)
         return context
 
 
 #
 # SONAR Detail Views
 #
@@ -99,14 +101,27 @@
 
         # get details from SonarData
         details = SonarData.objects.filter(sonar_request_id=record.uuid, category='details').first()
         record.details = details.data if details else {}
         return record
 
 
+class SonarQueriesDetailView(SuperuserRequiredMixin, DetailView):
+    context_object_name = 'sonar_query'
+    template_name = 'django_sonar/queries/detail.html'
+
+    def get_object(self):
+        queries = SonarData.objects.filter(category='queries',
+                                           sonar_request_id=self.kwargs.get('uuid')).first()
+        executed_queries = queries.data['executed_queries'] if queries else []
+        single_query = executed_queries[self.kwargs.get('index')] or {}
+        single_query['sonar_request_id'] = self.kwargs.get('uuid')
+        return single_query
+
+
 class SonarDetailPayloadView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_payload.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         payload = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='payload').first()
         context['payload'] = payload.data if payload else {}
@@ -169,8 +184,8 @@
 class SonarDetailExceptionView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_exception.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         exception = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='exception').first()
         context['exception'] = exception.data if exception else {}
-        return context
+        return context
```

### Comparing `django_sonar-0.1.3/django_sonar/middlewares/requests.py` & `django_sonar-0.1.8/django_sonar/middlewares/requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import socket
 import time
 import traceback
 import tracemalloc
 from datetime import datetime
+from urllib.parse import urlencode
 
 from django.conf import settings
 from django.db import connection
 from django.urls import resolve
 from django.utils.timezone import make_aware
-
+from django.contrib.auth import get_user_model
 from django_sonar import utils
 from django_sonar.models import SonarRequest, SonarData
 
-
 class RequestsMiddleware:
     def __init__(self, get_response):
         self.get_response = get_response
         self.sonar_request_uuid = None
         tracemalloc.start()  # Start tracing memory allocation
 
     def __call__(self, request):
@@ -67,36 +67,47 @@
 
         # log all queries
         executed_queries = connection.queries
 
         # Capture request details
         http_verb = request.method
         url_path = request.path
+        query_string = urlencode(get_payload)
         http_status = response.status_code
 
         # logged user
         user_info = None
+        # get user info if user is authenticated
+        User = get_user_model()
         if request.user.is_authenticated:
+            # use get_username() instead of username to support custom user models
+            # use get_email_field_name() instead of email to support custom user models
             user_info = {
-                'user_id': request.user.id,
-                'username': request.user.username,
-                'email': request.user.email
-            }
+                "user_id": request.user.id,
+                "username": request.user.get_username(),
+                "email": getattr(request.user, User.get_email_field_name(), 'No email provided'),
+                }
 
         # Additional details
         is_ajax = self.is_ajax(request)
         timestamp = make_aware(datetime.now())  # Make sure the timestamp is timezone-aware
         hostname = socket.gethostname()
         ip_address = self.get_client_ip(request)
         middlewares_used = settings.MIDDLEWARE
 
+        # if there is a querystring add it to the full url
+        if query_string:
+            full_url = f"{url_path}?{query_string}"
+        else:
+            full_url = url_path
+
         # Create a SonarRequest object
         sonar_request = SonarRequest.objects.create(
             verb=http_verb,
-            path=url_path,
+            path=full_url,
             status=http_status,
             duration=duration,
             ip_address=ip_address,
             hostname=hostname,
             is_ajax=is_ajax,
             created_at=timestamp,
         )
```

### Comparing `django_sonar-0.1.3/django_sonar/migrations/0001_initial.py` & `django_sonar-0.1.8/django_sonar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/models/sonar_data.py` & `django_sonar-0.1.8/django_sonar/models/sonar_data.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/models/sonar_request.py` & `django_sonar-0.1.8/django_sonar/models/sonar_request.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap-icons.min.css` & `django_sonar-0.1.8/django_sonar/static/django_sonar/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap.min.css` & `django_sonar-0.1.8/django_sonar/static/django_sonar/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/css/django-sonar.css` & `django_sonar-0.1.8/django_sonar/static/django_sonar/css/django-sonar.css`

 * *Files 1% similar despite different names*

```diff
@@ -92,8 +92,12 @@
 
 .table thead tr {
     border-bottom: 1px dashed silver !important;
 }
 
 .table>:not(caption)>*>* {
     border-bottom: 0 !important;
+}
+
+pre {
+    font-size: 1rem;
 }
```

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2` & `django_sonar-0.1.8/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js` & `django_sonar-0.1.8/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/js/htmx.min.js` & `django_sonar-0.1.8/django_sonar/static/django_sonar/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/static/django_sonar/media/logos/favicon.png` & `django_sonar-0.1.8/django_sonar/static/django_sonar/media/logos/favicon.png`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/denied.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/auth/denied.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/login.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/auth/login.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/dumps/index.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/dumps/index.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/exceptions/index.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/exceptions/index.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/home/index.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/home/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -123,9 +123,10 @@
                 this.classList.add('active');
             });
         });
 
 
     })
 </script>
+<script src="{% static 'django_sonar/js/sql-formatter.min.js' %}"></script>
 </body>
 </html>
```

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/layouts/auth.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/layouts/auth.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/queries/index.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/queries/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,25 @@
                     <th scope="col">Duration</th>
                     <th scope="col">Happened</th>
                     <th class="w-50px">&nbsp;</th>
                 </tr>
                 </thead>
                 <tbody>
                 {% for query in queries %}
-                <tr>
-                    <td><code>{{ query.sql|truncatechars:90 }}</code></td>
+                <tr {% if query.index == 0 %}class="bg-light"{% endif %}>
+                    <td>
+                        <code>{{ query.sql|truncatechars:90 }}</code></td>
                     <td>{{ query.time }}ms</td>
                     <td>{{ query.created_at|timesince }}</td>
                     <td>
-                        <a class="btn btn-sm btn-icon btn-primary">
+                        <a class="btn btn-sm btn-icon btn-primary"
+                           href="{% url 'sonar_queries_detail' uuid=query.sonar_request_id index=query.index %}"
+                           hx-get="{% url 'sonar_queries_detail' uuid=query.sonar_request_id index=query.index %}"
+                           hx-swap="innerHTML"
+                           hx-target="#main-content">
                             <i class="bi bi-arrow-right"></i>
                         </a>
                     </td>
                 </tr>
                 {% endfor %}
                 </tbody>
             </table>
```

#### html2text {}

```diff
@@ -1,8 +1,6 @@
 **** QQuueerriieess ****
 {% if not queries %}
 No queries found
 {% else %}
-QQuueerryy                       DDuurraattiioonn           HHaappppeenneedd                      ? 
-{{ query.sql|truncatechars: {{ query.time }}ms {{ query.created_at|timesince
-90 }}                                          }}
+QQuueerryy DDuurraattiioonn HHaappppeenneedd ? 
 {% endif %}
```

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_payload.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_payload.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_queries.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_queries.html`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,17 @@
             <div class="text-light-grey">No executed queries</div>
         {% endif %}
     
         {% for query in queries.executed_queries %}
 
             <div class="row">
                 <div class="col border-bottom border-1 border-light pb-3">
-                    <code>{{ query.sql }}</code>
+                    <code id="query_index_{{ forloop.counter0 }}">
+                        {{ query.sql|safe }}
+                    </code>
                     <div>
                         <span class="text-muted text-small fw-lighter">{{ query.time|floatformat:2 }}ms</span>
                     </div>
                 </div>
             </div>
 
         {% endfor %}
```

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_session.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/detail_session.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/index.html` & `django_sonar-0.1.8/django_sonar/templates/django_sonar/requests/index.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/.gitignore` & `django_sonar-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/LICENSE` & `django_sonar-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/README.md` & `django_sonar-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.3/PKG-INFO` & `django_sonar-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,55 @@
 Metadata-Version: 2.3
 Name: django_sonar
-Version: 0.1.3
-Summary: The missing debug tool for Django
+Version: 0.1.8
+Summary: The missing debug tool for Django, inspired by Telescope.
 Project-URL: Homepage, https://github.com/metalogico/django-sonar
 Project-URL: Issues, https://github.com/metalogico/django-sonar/issues
+Project-URL: Download, https://pypi.org/project/django-sonar/
 Author-email: Metalogico <michele.brandolin@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2024 metalogico
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
+Requires-Dist: django>=4.2.9
+Requires-Dist: sqlparse>=0.2
 Description-Content-Type: text/markdown
 
 # DjangoSonar
 
 The missing debug tool for django.
 
 DjangoSonar is a comprehensive debugging and introspection tool for Django applications, inspired by Laravel Telescope.
```

