# Comparing `tmp/django_google_cloud_tasks-2.8.1.tar.gz` & `tmp/django_google_cloud_tasks-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_cloud_tasks-2.8.1.tar", max compression
+gzip compressed data, was "django_google_cloud_tasks-2.8.2.tar", max compression
```

## Comparing `django_google_cloud_tasks-2.8.1.tar` & `django_google_cloud_tasks-2.8.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11358 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/LICENSE.md
--rw-r--r--   0        0        0      153 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/__init__.py
--rw-r--r--   0        0        0     6963 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/apps.py
--rw-r--r--   0        0        0      446 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/context.py
--rw-r--r--   0        0        0      373 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/exceptions.py
--rw-r--r--   0        0        0     1411 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/field.py
--rw-r--r--   0        0        0        0 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/__init__.py
--rw-r--r--   0        0        0      860 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/commands/__init__.py
--rw-r--r--   0        0        0      490 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/commands/initialize_subscribers.py
--rw-r--r--   0        0        0      394 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/commands/initialize_tasks.py
--rw-r--r--   0        0        0      501 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/commands/schedule_tasks.py
--rw-r--r--   0        0        0      252 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/middleware/__init__.py
--rw-r--r--   0        0        0     1179 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/middleware/headers_context_middlware.py
--rw-r--r--   0        0        0     1903 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/middleware/pubsub_headers_middleware.py
--rw-r--r--   0        0        0     3888 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0001_initial.py
--rw-r--r--   0        0        0     1024 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
--rw-r--r--   0        0        0      718 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py
--rw-r--r--   0        0        0        0 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/__init__.py
--rw-r--r--   0        0        0     4660 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/models.py
--rw-r--r--   0        0        0      925 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/serializers.py
--rw-r--r--   0        0        0     2693 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/signals.py
--rw-r--r--   0        0        0      667 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/__init__.py
--rw-r--r--   0        0        0     1118 2023-12-06 15:32:29.448054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/periodic_task.py
--rw-r--r--   0        0        0     4781 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/publisher_task.py
--rw-r--r--   0        0        0     2498 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/routine_task.py
--rw-r--r--   0        0        0     2853 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/subscriber_task.py
--rw-r--r--   0        0        0    11737 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/task.py
--rw-r--r--   0        0        0        0 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tests/__init__.py
--rw-r--r--   0        0        0      795 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tests/factories.py
--rw-r--r--   0        0        0      869 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/tests/tests_base.py
--rw-r--r--   0        0        0      291 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/urls.py
--rw-r--r--   0        0        0     3380 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/django_cloud_tasks/views.py
--rw-r--r--   0        0        0     1143 2023-12-06 15:32:29.452054 django_google_cloud_tasks-2.8.1/pyproject.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/LICENSE.md
+-rw-r--r--   0        0        0      153 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/__init__.py
+-rw-r--r--   0        0        0     6963 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/apps.py
+-rw-r--r--   0        0        0      460 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/context.py
+-rw-r--r--   0        0        0      373 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/exceptions.py
+-rw-r--r--   0        0        0     1411 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/field.py
+-rw-r--r--   0        0        0        0 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/__init__.py
+-rw-r--r--   0        0        0      860 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/commands/__init__.py
+-rw-r--r--   0        0        0      490 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/commands/initialize_subscribers.py
+-rw-r--r--   0        0        0      394 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/commands/initialize_tasks.py
+-rw-r--r--   0        0        0      501 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/commands/schedule_tasks.py
+-rw-r--r--   0        0        0      252 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/middleware/__init__.py
+-rw-r--r--   0        0        0     1179 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/middleware/headers_context_middlware.py
+-rw-r--r--   0        0        0     1903 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/middleware/pubsub_headers_middleware.py
+-rw-r--r--   0        0        0     3888 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1024 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py
+-rw-r--r--   0        0        0      718 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py
+-rw-r--r--   0        0        0        0 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/__init__.py
+-rw-r--r--   0        0        0     4660 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/models.py
+-rw-r--r--   0        0        0      925 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/serializers.py
+-rw-r--r--   0        0        0     2693 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/signals.py
+-rw-r--r--   0        0        0      667 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/__init__.py
+-rw-r--r--   0        0        0     1118 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/periodic_task.py
+-rw-r--r--   0        0        0     4781 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/publisher_task.py
+-rw-r--r--   0        0        0     2498 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/routine_task.py
+-rw-r--r--   0        0        0     2853 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/subscriber_task.py
+-rw-r--r--   0        0        0    11737 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/task.py
+-rw-r--r--   0        0        0        0 2024-01-16 19:00:18.884098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tests/__init__.py
+-rw-r--r--   0        0        0      795 2024-01-16 19:00:18.888098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tests/factories.py
+-rw-r--r--   0        0        0      869 2024-01-16 19:00:18.888098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/tests/tests_base.py
+-rw-r--r--   0        0        0      291 2024-01-16 19:00:18.888098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/urls.py
+-rw-r--r--   0        0        0     3380 2024-01-16 19:00:18.888098 django_google_cloud_tasks-2.8.2/django_cloud_tasks/views.py
+-rw-r--r--   0        0        0     1143 2024-01-16 19:00:18.888098 django_google_cloud_tasks-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 django_google_cloud_tasks-2.8.2/PKG-INFO
```

### Comparing `django_google_cloud_tasks-2.8.1/LICENSE.md` & `django_google_cloud_tasks-2.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/apps.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/apps.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/field.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/field.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/management/commands/__init__.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/middleware/headers_context_middlware.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/middleware/headers_context_middlware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/middleware/pubsub_headers_middleware.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/middleware/pubsub_headers_middleware.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0001_initial.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0002_alter_routine_status_alter_routine_task_name.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/migrations/0003_alter_routine_max_retries_and_more.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/models.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/serializers.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/signals.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/signals.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/__init__.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/periodic_task.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/periodic_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/publisher_task.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/publisher_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/routine_task.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/routine_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/subscriber_task.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/subscriber_task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tasks/task.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tasks/task.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tests/factories.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/tests/tests_base.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/tests/tests_base.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/django_cloud_tasks/views.py` & `django_google_cloud_tasks-2.8.2/django_cloud_tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_google_cloud_tasks-2.8.1/pyproject.toml` & `django_google_cloud_tasks-2.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-google-cloud-tasks"
-version = "2.8.1"
+version = "2.8.2"
 description = "Async Tasks with HTTP endpoints"
 authors = ["Joao Daher <joao@daher.dev>"]
 packages = [
     { include = "django_cloud_tasks" },
 ]
 
 [tool.poetry.dependencies]
```

