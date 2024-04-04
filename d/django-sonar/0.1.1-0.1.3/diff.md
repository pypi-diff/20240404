# Comparing `tmp/django_sonar-0.1.1.tar.gz` & `tmp/django_sonar-0.1.3.tar.gz`

## Comparing `django_sonar-0.1.1.tar` & `django_sonar-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 django_sonar-0.1.1/manage.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_sonar-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 django_sonar-0.1.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.1/base/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.1/base/asgi.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 django_sonar-0.1.1/base/settings.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 django_sonar-0.1.1/base/urls.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.1/base/wsgi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/admin.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/apps.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/tests.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/urls.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/utils.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/middlewares/__init__.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/middlewares/requests.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/migrations/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/models/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/models/sonar_data.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/models/sonar_request.py
--rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/bootstrap-icons.min.css
--rw-r--r--   0        0        0   155845 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/bootstrap.min.css
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/dark-theme.css
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/django-sonar.css
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/solid.min.css
--rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    78743 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0    48036 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/js/htmx.min.js
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/static/django_sonar/media/logos/favicon.png
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/auth/login.html
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/dumps/index.html
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/exceptions/index.html
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/home/index.html
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/layouts/auth.html
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/queries/index.html
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail.html
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_dumps.html
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_exception.html
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_headers.html
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_middlewares.html
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_payload.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_queries.html
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_session.html
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/index.html
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_sonar-0.1.1/django_sonar/templates/django_sonar/signals/index.html
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 django_sonar-0.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sonar-0.1.1/LICENSE
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 django_sonar-0.1.1/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_sonar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 django_sonar-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 django_sonar-0.1.3/manage.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_sonar-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 django_sonar-0.1.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/asgi.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/settings.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/urls.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 django_sonar-0.1.3/base/wsgi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/admin.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/apps.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/mixins.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/tests.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/urls.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/utils.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/middlewares/__init__.py
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/middlewares/requests.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/migrations/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/sonar_data.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/models/sonar_request.py
+-rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap-icons.min.css
+-rw-r--r--   0        0        0   155845 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap.min.css
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/dark-theme.css
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/django-sonar.css
+-rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    78743 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0    48036 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/js/htmx.min.js
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/static/django_sonar/media/logos/favicon.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/denied.html
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/login.html
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/dumps/index.html
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/exceptions/index.html
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/home/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/layouts/auth.html
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/queries/index.html
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail.html
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_dumps.html
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_exception.html
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_headers.html
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_middlewares.html
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_payload.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_queries.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_session.html
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/index.html
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 django_sonar-0.1.3/django_sonar/templates/django_sonar/signals/index.html
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 django_sonar-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_sonar-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 django_sonar-0.1.3/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_sonar-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 django_sonar-0.1.3/PKG-INFO
```

### Comparing `django_sonar-0.1.1/manage.py` & `django_sonar-0.1.3/manage.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/setup.py` & `django_sonar-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django_sonar',
-    version='0.1.1',
+    version='0.1.3',
     author='Metalogico',
-    author_email='michele.brandolin@gmail.com',  # Replace with your email
+    author_email='michele.brandolin@gmail.com',
     description='The missing debug tool for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/metalogico/django-sonar',
     project_urls={
         "Bug Tracker": "https://github.com/metalogico/django-sonar/issues"
     },
+
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Django>=4.0',
     ],
     classifiers=[
```

### Comparing `django_sonar-0.1.1/base/settings.py` & `django_sonar-0.1.3/base/settings.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/urls.py` & `django_sonar-0.1.3/django_sonar/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.urls import path, include
 
 from django_sonar.views import SonarHomeView, SonarLoginView, SonarLogoutView, SonarRequestListView, \
     SonarExceptionsListView, SonarDumpsListView, SonarSignalsListView, SonarQueriesListView, SonarRequestDetailView, \
     SonarRequestClearView, SonarDetailPayloadView, SonarDetailHeadersView, SonarDetailSessionView, \
-    SonarDetailMiddlewaresView, SonarDetailQueriesView, SonarDetailDumpsView, SonarDetailExceptionView
+    SonarDetailMiddlewaresView, SonarDetailQueriesView, SonarDetailDumpsView, SonarDetailExceptionView, SonarDeniedView
 
 urlpatterns = [
     # general
     path('', SonarHomeView.as_view(), name='sonar_index'),
     path('login/', SonarLoginView.as_view(), name='sonar_login'),
     path('logout/', SonarLogoutView.as_view(), name='sonar_logout'),
+    path('denied/', SonarDeniedView.as_view(), name='sonar_denied'),
 
     # navigations
     path('requests/', SonarRequestListView.as_view(), name='sonar_requests'),
     path('requests/<uuid:uuid>/', SonarRequestDetailView.as_view(), name='sonar_request_detail'),
     path('exceptions/', SonarExceptionsListView.as_view(), name='sonar_exceptions'),
     path('queries/', SonarQueriesListView.as_view(), name='sonar_queries'),
     path('dumps/', SonarDumpsListView.as_view(), name='sonar_dumps'),
```

### Comparing `django_sonar-0.1.1/django_sonar/utils.py` & `django_sonar-0.1.3/django_sonar/utils.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/views.py` & `django_sonar-0.1.3/django_sonar/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,77 @@
-import json
-
-import uuid
-
 from django.contrib.auth.views import LoginView, LogoutView
 from django.urls import reverse_lazy
-from django.views.generic import TemplateView, DetailView, ListView, RedirectView
+from django.views.generic import TemplateView, DetailView, RedirectView
 
+from django_sonar.mixins import SuperuserRequiredMixin
 from django_sonar.models import SonarRequest, SonarData
 
 
 class SonarLoginView(LoginView):
     template_name = 'django_sonar/auth/login.html'
     redirect_authenticated_user = True
     next_page = reverse_lazy('sonar_index')
 
 
 class SonarLogoutView(LogoutView):
     next_page = reverse_lazy('sonar_login')
 
 
-class SonarHomeView(TemplateView):
+class SonarDeniedView(TemplateView):
+    template_name = 'django_sonar/auth/denied.html'
+
+
+class SonarHomeView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/home/index.html'
 
 
-class SonarRequestClearView(RedirectView):
+class SonarRequestClearView(SuperuserRequiredMixin, RedirectView):
     url = reverse_lazy('sonar_index')
 
     def get(self, request, *args, **kwargs):
         SonarRequest.objects.all().delete()
         return super().get(request, *args, **kwargs)
 
 
 #
 # SONAR LIST VIEWS
 #
 
-class SonarRequestListView(TemplateView):
+class SonarRequestListView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/index.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['sonar_requests'] = SonarRequest.objects.order_by('-created_at').all()
         return context
 
 
-class SonarExceptionsListView(TemplateView):
+class SonarExceptionsListView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/exceptions/index.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['exceptions'] = SonarData.objects.filter(category='exception').order_by('-created_at').all()
         return context
 
 
-class SonarDumpsListView(TemplateView):
+class SonarDumpsListView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/dumps/index.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['dumps'] = SonarData.objects.filter(category='dumps').order_by('-created_at').all()
         return context
 
 
-class SonarSignalsListView(TemplateView):
+class SonarSignalsListView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/signals/index.html'
 
 
-class SonarQueriesListView(TemplateView):
+class SonarQueriesListView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/queries/index.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         queries = SonarData.objects.filter(category='queries').order_by('-created_at').all()
         # extract queries from SonarData queries
         context['queries'] = []
@@ -83,93 +84,93 @@
 
 
 #
 # SONAR Detail Views
 #
 
 
-class SonarRequestDetailView(DetailView):
+class SonarRequestDetailView(SuperuserRequiredMixin, DetailView):
     context_object_name = 'sonar_request'
     template_name = 'django_sonar/requests/detail.html'
 
     def get_object(self):
         record = SonarRequest.objects.get(uuid=self.kwargs.get('uuid'))
         record.is_read = True
         record.save()
 
         # get details from SonarData
         details = SonarData.objects.filter(sonar_request_id=record.uuid, category='details').first()
         record.details = details.data if details else {}
         return record
 
 
-class SonarDetailPayloadView(TemplateView):
+class SonarDetailPayloadView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_payload.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         payload = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='payload').first()
         context['payload'] = payload.data if payload else {}
         return context
 
 
-class SonarDetailHeadersView(TemplateView):
+class SonarDetailHeadersView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_headers.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         headers = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='headers').first()
         context['headers'] = headers.data if headers else {}
         return context
 
 
-class SonarDetailQueriesView(TemplateView):
+class SonarDetailQueriesView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_queries.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         queries = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='queries').first()
         context['queries'] = queries.data if queries else {}
         return context
 
 
-class SonarDetailSessionView(TemplateView):
+class SonarDetailSessionView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_session.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         session = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='session').first()
         context['session'] = session.data if session else {}
         return context
 
 
-class SonarDetailMiddlewaresView(TemplateView):
+class SonarDetailMiddlewaresView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_middlewares.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         middlewares = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='details').first()
         context['middlewares'] = middlewares.data if middlewares else {}
         return context
 
 
-class SonarDetailDumpsView(TemplateView):
+class SonarDetailDumpsView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_dumps.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context['dumps'] = []
         dumps = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='dumps').all()
         for dump in dumps:
             context['dumps'] += [dump.data]
 
         return context
 
 
-class SonarDetailExceptionView(TemplateView):
+class SonarDetailExceptionView(SuperuserRequiredMixin, TemplateView):
     template_name = 'django_sonar/requests/detail_exception.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         exception = SonarData.objects.filter(sonar_request_id=self.kwargs.get('uuid'), category='exception').first()
         context['exception'] = exception.data if exception else {}
         return context
```

### Comparing `django_sonar-0.1.1/django_sonar/middlewares/requests.py` & `django_sonar-0.1.3/django_sonar/middlewares/requests.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/migrations/0001_initial.py` & `django_sonar-0.1.3/django_sonar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/models/sonar_data.py` & `django_sonar-0.1.3/django_sonar/models/sonar_data.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/models/sonar_request.py` & `django_sonar-0.1.3/django_sonar/models/sonar_request.py`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/css/bootstrap-icons.min.css` & `django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/css/bootstrap.min.css` & `django_sonar-0.1.3/django_sonar/static/django_sonar/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/css/django-sonar.css` & `django_sonar-0.1.3/django_sonar/static/django_sonar/css/django-sonar.css`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     max-width: 50px !important;
 }
 
 .fw-small {
     font-size: 10px !important;
 }
 
+.text-light-grey {
+    color: #bec6cc !important;
+}
+
 .card-header {
     padding-top: 20px !important;
     padding-bottom: 20px !important;
     vertical-align: middle !important;
     background-color: #ffffff !important;
 }
```

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2` & `django_sonar-0.1.3/django_sonar/static/django_sonar/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js` & `django_sonar-0.1.3/django_sonar/static/django_sonar/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/js/htmx.min.js` & `django_sonar-0.1.3/django_sonar/static/django_sonar/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/static/django_sonar/media/logos/favicon.png` & `django_sonar-0.1.3/django_sonar/static/django_sonar/media/logos/favicon.png`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/auth/login.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/auth/login.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends "django_sonar/layouts/auth.html" %}
 
 {% block content %}
 <div class="container">
     <div class="row justify-content-center">
-        <div class="col-md-6">
+        <div class="col-md-4">
             <h1 class="text-center mt-5">
                 <i class="bi bi-broadcast me-1"></i>Django Sonar
             </h1>
             <div class="card shadow-sm  mt-5">
                 <div class="card-body">
                     <h5 class="card-title text-center">Login</h5>
                     <form method="post">
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/exceptions/index.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/exceptions/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 <div class="card shadow-sm  border-light" hx-get="{% url 'sonar_exceptions' %}" hx-trigger="every 5s" hx-swap="outerHTML">
     <div class="card-header">
         <h5 class="card-title">Queries</h5>
     </div>
     <div class="card-body">
 
-        <table class="table table-dashed table-hover">
-            <thead>
-            <tr>
-                <th scope="col">Type</th>
-                <th scope="col">File/Line</th>
-                <th scope="col">Function</th>
-                <th scope="col">Happened</th>
-                <th class="w-50px">&nbsp;</th>
-            </tr>
-            </thead>
-            <tbody>
-            {% for exception in exceptions %}
-            <tr>
-                <td>{{ exception.data.exception_message }}</td>
-                <td><code>{{ exception.data.file_name }}:{{ exception.data.line_number }}</code></td>
-                <td>{{ exception.created_at|timesince }}</td>
-                <td>
-                    <a class="btn btn-sm btn-icon btn-primary">
-                        <i class="bi bi-arrow-right"></i>
-                    </a>
-                </td>
-            </tr>
-            {% endfor %}
-            </tbody>
-        </table>
+
+        {% if not exceptions %}
+            <div class="text-light-grey">No exceptions found</div>
+        {% else %}
+            <table class="table table-dashed table-hover">
+                <thead>
+                <tr>
+                    <th scope="col">Type</th>
+                    <th scope="col">File/Line</th>
+                    <th scope="col">Function</th>
+                    <th scope="col">Happened</th>
+                    <th class="w-50px">&nbsp;</th>
+                </tr>
+                </thead>
+                <tbody>
+                {% for exception in exceptions %}
+                <tr>
+                    <td>{{ exception.data.exception_message }}</td>
+                    <td><code>{{ exception.data.file_name }}:{{ exception.data.line_number }}</code></td>
+                    <td>{{ exception.created_at|timesince }}</td>
+                    <td>
+                        <a class="btn btn-sm btn-icon btn-primary">
+                            <i class="bi bi-arrow-right"></i>
+                        </a>
+                    </td>
+                </tr>
+                {% endfor %}
+                </tbody>
+            </table>
+        {% endif %}
 
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
 **** QQuueerriieess ****
+{% if not exceptions %}
+No exceptions found
+{% else %}
 TTyyppee                             FFiillee//LLiinnee                  FFuunnccttiioonn                       HHaappppeenneedd ? 
                                  {
 {                                { exception.data.file_name {
 {                                }}:{                       {
 exception.data.exception_message {                          exception.created_at|timesince
 }}                               exception.data.line_number }}
                                  }}
+{% endif %}
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/home/index.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/home/index.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/layouts/auth.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/layouts/auth.html`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     <meta charset="UTF-8">
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <title>Django Sonar</title>
     <link rel="shortcut icon" href="{% static 'django_sonar/media/logos/favicon.png' %}">
     <link rel="stylesheet" href="{% static 'django_sonar/css/bootstrap.min.css' %}">
+    <link rel="stylesheet" href="{% static 'django_sonar/css/django-sonar.css' %}">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
 </head>
 <body class="">
 
     {% block content %}{% endblock %}
 
 </body>
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/queries/index.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/queries/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 <div class="card shadow-sm  border-light" hx-get="{% url 'sonar_queries' %}" hx-trigger="every 5s" hx-swap="outerHTML">
     <div class="card-header">
         <h5 class="card-title">Queries</h5>
     </div>
     <div class="card-body">
 
-        <table class="table table-dashed table-hover">
-            <thead>
-            <tr>
-                <th scope="col">Query</th>
-                <th scope="col">Duration</th>
-                <th scope="col">Happened</th>
-                <th class="w-50px">&nbsp;</th>
-            </tr>
-            </thead>
-            <tbody>
-            {% for query in queries %}
-            <tr>
-                <td><code>{{ query.sql|truncatechars:90 }}</code></td>
-                <td>{{ query.time }}ms</td>
-                <td>{{ query.created_at|timesince }}</td>
-                <td>
-                    <a class="btn btn-sm btn-icon btn-primary">
-                        <i class="bi bi-arrow-right"></i>
-                    </a>
-                </td>
-            </tr>
-            {% endfor %}
-            </tbody>
-        </table>
+
+        {% if not queries %}
+            <div class="text-light-grey">No queries found</div>
+        {% else %}
+            <table class="table table-dashed table-hover">
+                <thead>
+                <tr>
+                    <th scope="col">Query</th>
+                    <th scope="col">Duration</th>
+                    <th scope="col">Happened</th>
+                    <th class="w-50px">&nbsp;</th>
+                </tr>
+                </thead>
+                <tbody>
+                {% for query in queries %}
+                <tr>
+                    <td><code>{{ query.sql|truncatechars:90 }}</code></td>
+                    <td>{{ query.time }}ms</td>
+                    <td>{{ query.created_at|timesince }}</td>
+                    <td>
+                        <a class="btn btn-sm btn-icon btn-primary">
+                            <i class="bi bi-arrow-right"></i>
+                        </a>
+                    </td>
+                </tr>
+                {% endfor %}
+                </tbody>
+            </table>
+        {% endif %}
 
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,8 @@
 **** QQuueerriieess ****
+{% if not queries %}
+No queries found
+{% else %}
 QQuueerryy                       DDuurraattiioonn           HHaappppeenneedd                      ? 
 {{ query.sql|truncatechars: {{ query.time }}ms {{ query.created_at|timesince
 90 }}                                          }}
+{% endif %}
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail.html`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_payload.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_payload.html`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,16 @@
                     <div class="col border-bottom border-1 border-light pb-3">
                         <strong>{{ name }}:</strong>
                         <code>{{ value }}</code>
                     </div>
                 </div>
             {% endfor %}
 
+        {% else %}
+            <div class="text-light-grey">No GET Payload</div>
         {% endif %}
 
 
         {% if payload.post_payload %}
 
             <h6>GET</h6>
 
@@ -28,13 +30,15 @@
                 <div class="row">
                     <div class="col border-bottom border-1 border-light pb-3">
                         <code>{{ name }}: {{ value }}</code>
                     </div>
                 </div>
             {% endfor %}
 
+        {% else %}
+            <div class="text-light-grey">No POST Payload</div>
         {% endif %}
 
 
     </div>
 
 </div>
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/detail_queries.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/detail_queries.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 <div class="card shadow-sm  border-light mt-3">
 
     <div class="card-body">
 
+        {% if not queries.executed_queries %}
+            <div class="text-light-grey">No executed queries</div>
+        {% endif %}
+    
         {% for query in queries.executed_queries %}
 
             <div class="row">
                 <div class="col border-bottom border-1 border-light pb-3">
                     <code>{{ query.sql }}</code>
                     <div>
                         <span class="text-muted text-small fw-lighter">{{ query.time|floatformat:2 }}ms</span>
```

### Comparing `django_sonar-0.1.1/django_sonar/templates/django_sonar/requests/index.html` & `django_sonar-0.1.3/django_sonar/templates/django_sonar/requests/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 <div class="card shadow-sm  border-light" hx-get="{% url 'sonar_requests' %}" hx-trigger="every 5s" hx-swap="outerHTML">
     <div class="card-header">
         <h5 class="card-title">Requests</h5>
     </div>
     <div class="card-body">
+
+        {% if not sonar_requests %}
+            <div class="text-light-grey">No requests found</div>
+        {% else %}
+
         <table class="table table-dashed table-row-dashed table-hover">
             <thead>
             <tr class="">
                 <th scope="col">Verb</th>
                 <th scope="col">Path</th>
                 <th scope="col">Status</th>
                 <th scope="col">Duration</th>
@@ -42,9 +47,11 @@
                         </a>
                     </td>
                 </tr>
             {% endfor %}
             </tbody>
         </table>
 
+        {% endif %}
+
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
 **** RReeqquueessttss ****
+{% if not sonar_requests %}
+No requests found
+{% else %}
 VVeerrbb               PPaatthh               SSttaattuuss               DDuurraattiioonn               HHaappppeenneedd                           ? 
                                       {% if
                                       sonar_request.status
                                       < '400' %} {
                                       {
                                       sonar_request.status
                                       }} {% elif
@@ -12,7 +15,8 @@
 }}                 }}                 < '500' %} {         }}ms                   }} ago
                                       {
                                       sonar_request.status
                                       }} {% else %} {
                                       {
                                       sonar_request.status
                                       }} {% endif %}
+{% endif %}
```

### Comparing `django_sonar-0.1.1/.gitignore` & `django_sonar-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/LICENSE` & `django_sonar-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sonar-0.1.1/README.md` & `django_sonar-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # DjangoSonar
 
 The missing debug tool for django.
 
 DjangoSonar is a comprehensive debugging and introspection tool for Django applications, inspired by Laravel Telescope.
 
 
-![cover-image](https://github.com/metalogico/django-sonar/assets/7287030/32183dcb-5cf5-4878-b27c-3a34a6aa4ba1)
+![image](https://github.com/metalogico/django-sonar/assets/7287030/fa6a49b2-afdc-44ad-81af-c84dd713776a)
 
 
 
 ## 🥳 Motivation
 
 Having spent years developing with Laravel before switching to Django, the first thing I missed from this change was the amazing [Laravel Telescope](https://github.com/laravel/telescope). So, I decided to create it myself.
 
@@ -105,14 +105,16 @@
 
 To access the dashboard you will point your browser to the /sonar/ url (but you can change it as described before). The interface is very simple and self explanatory.
 
 You could use DjangoSonar in production too, since it gives you an historical overview of all the requests, but be sure to clear the data and disable it when you have debugged the problem.
 
 🔔 If you forget to disable/clear DjangoSonar you could end up with several gigabytes of data collected. So please use it with caution when in production 🔔 
 
+**Only authenticated superusers can access sonar.** If you are trying to access the dashboard with a wrong type of user, you will see an error page, otherwise you should see the DjangoSonar login page.    
+
 ### sonar() - the dump helper
 
 You can dump values to DjangoSonar using the **sonar()** helper function:
 
 ```python
 
 from django_sonar.utils import sonar
```

### Comparing `django_sonar-0.1.1/pyproject.toml` & `django_sonar-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django_sonar"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
     { name = "Metalogico", email = "michele.brandolin@gmail.com" },
 ]
 description = "The missing debug tool for Django"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django_sonar-0.1.1/PKG-INFO` & `django_sonar-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django_sonar
-Version: 0.1.1
+Version: 0.1.3
 Summary: The missing debug tool for Django
 Project-URL: Homepage, https://github.com/metalogico/django-sonar
 Project-URL: Issues, https://github.com/metalogico/django-sonar/issues
 Author-email: Metalogico <michele.brandolin@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
@@ -26,15 +26,15 @@
 # DjangoSonar
 
 The missing debug tool for django.
 
 DjangoSonar is a comprehensive debugging and introspection tool for Django applications, inspired by Laravel Telescope.
 
 
-![cover-image](https://github.com/metalogico/django-sonar/assets/7287030/32183dcb-5cf5-4878-b27c-3a34a6aa4ba1)
+![image](https://github.com/metalogico/django-sonar/assets/7287030/fa6a49b2-afdc-44ad-81af-c84dd713776a)
 
 
 
 ## 🥳 Motivation
 
 Having spent years developing with Laravel before switching to Django, the first thing I missed from this change was the amazing [Laravel Telescope](https://github.com/laravel/telescope). So, I decided to create it myself.
 
@@ -130,14 +130,16 @@
 
 To access the dashboard you will point your browser to the /sonar/ url (but you can change it as described before). The interface is very simple and self explanatory.
 
 You could use DjangoSonar in production too, since it gives you an historical overview of all the requests, but be sure to clear the data and disable it when you have debugged the problem.
 
 🔔 If you forget to disable/clear DjangoSonar you could end up with several gigabytes of data collected. So please use it with caution when in production 🔔 
 
+**Only authenticated superusers can access sonar.** If you are trying to access the dashboard with a wrong type of user, you will see an error page, otherwise you should see the DjangoSonar login page.    
+
 ### sonar() - the dump helper
 
 You can dump values to DjangoSonar using the **sonar()** helper function:
 
 ```python
 
 from django_sonar.utils import sonar
```

