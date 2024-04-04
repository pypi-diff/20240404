# Comparing `tmp/hmtaiga-0.1.7.tar.gz` & `tmp/hmtaiga-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.7.tar", last modified: Thu Apr  4 02:47:15 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.8.tar", last modified: Thu Apr  4 03:07:09 2024, max compression
```

## Comparing `hmtaiga-0.1.7.tar` & `hmtaiga-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865828 hmtaiga-0.1.7/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 02:47:15.865640 hmtaiga-0.1.7/PKG-INFO
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.862555 hmtaiga-0.1.7/auth/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.7/auth/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      895 2024-02-12 04:15:32.000000 hmtaiga-0.1.7/auth/authenticate.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865482 hmtaiga-0.1.7/hmtaiga.egg-info/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 shikhaverma   (501) staff       (20)      545 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       44 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/top_level.txt
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.863420 hmtaiga-0.1.7/milestone/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/milestone/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      644 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/milestone/get_milestone.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.863834 hmtaiga-0.1.7/project/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/project/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/project/getProjectBySlug.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-04 02:47:15.865857 hmtaiga-0.1.7/setup.cfg
--rw-r--r--   0 shikhaverma   (501) staff       (20)      183 2024-04-04 02:43:05.000000 hmtaiga-0.1.7/setup.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.864269 hmtaiga-0.1.7/tasks/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.864902 hmtaiga-0.1.7/test/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      939 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_getProjectBySlug.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      527 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_milestone.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865268 hmtaiga-0.1.7/userStory/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/getBusinessValue.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/get_user_story_history.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.766259 hmtaiga-0.1.8/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 03:07:09.766088 hmtaiga-0.1.8/PKG-INFO
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.762482 hmtaiga-0.1.8/auth/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/auth/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      895 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/auth/authenticate.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765921 hmtaiga-0.1.8/hmtaiga.egg-info/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      608 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       51 2024-04-04 03:07:09.000000 hmtaiga-0.1.8/hmtaiga.egg-info/top_level.txt
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763340 hmtaiga-0.1.8/issues/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/issues/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2328 2024-03-25 04:07:28.000000 hmtaiga-0.1.8/issues/get_issues.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763632 hmtaiga-0.1.8/milestone/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/milestone/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      644 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/milestone/get_milestone.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.763915 hmtaiga-0.1.8/project/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/project/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/project/getProjectBySlug.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-04 03:07:09.766297 hmtaiga-0.1.8/setup.cfg
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      183 2024-04-04 03:04:50.000000 hmtaiga-0.1.8/setup.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.764439 hmtaiga-0.1.8/tasks/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/tasks/get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765363 hmtaiga-0.1.8/test/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     8896 2024-04-04 03:04:40.000000 hmtaiga-0.1.8/test/test_getIssues.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      939 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_getProjectBySlug.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      527 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_milestone.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:07:09.765706 hmtaiga-0.1.8/userStory/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/getBusinessValue.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-04 03:02:45.000000 hmtaiga-0.1.8/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.7/auth/authenticate.py` & `hmtaiga-0.1.8/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/milestone/get_milestone.py` & `hmtaiga-0.1.8/milestone/get_milestone.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/project/getProjectBySlug.py` & `hmtaiga-0.1.8/project/getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/tasks/get_task_history.py` & `hmtaiga-0.1.8/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/tasks/get_tasks.py` & `hmtaiga-0.1.8/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/test/test_getProjectBySlug.py` & `hmtaiga-0.1.8/test/test_getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/test/test_get_milestone.py` & `hmtaiga-0.1.8/test/test_get_milestone.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/test/test_get_task_history.py` & `hmtaiga-0.1.8/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/test/test_get_tasks.py` & `hmtaiga-0.1.8/test/test_get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/userStory/getBusinessValue.py` & `hmtaiga-0.1.8/userStory/getBusinessValue.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.7/userStory/get_user_story_history.py` & `hmtaiga-0.1.8/userStory/get_user_story_history.py`

 * *Files identical despite different names*

