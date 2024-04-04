# Comparing `tmp/hmtaiga-0.1.6.tar.gz` & `tmp/hmtaiga-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.6.tar", last modified: Wed Apr  3 03:47:56 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.7.tar", last modified: Thu Apr  4 02:47:15 2024, max compression
```

## Comparing `hmtaiga-0.1.6.tar` & `hmtaiga-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.432887 hmtaiga-0.1.6/
--rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-03 03:47:56.432541 hmtaiga-0.1.6/PKG-INFO
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.432008 hmtaiga-0.1.6/hmtaiga.egg-info/
--rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-03 03:47:56.000000 hmtaiga-0.1.6/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 hasanshahid   (501) staff       (20)      480 2024-04-03 03:47:56.000000 hmtaiga-0.1.6/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 hasanshahid   (501) staff       (20)        1 2024-04-03 03:47:56.000000 hmtaiga-0.1.6/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 hasanshahid   (501) staff       (20)       39 2024-04-03 03:47:56.000000 hmtaiga-0.1.6/hmtaiga.egg-info/top_level.txt
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.426405 hmtaiga-0.1.6/milestone/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:11.000000 hmtaiga-0.1.6/milestone/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)      644 2024-04-03 03:28:25.000000 hmtaiga-0.1.6/milestone/get_milestone.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.427968 hmtaiga-0.1.6/project/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:03.000000 hmtaiga-0.1.6/project/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     1213 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/project/getProjectBySlug.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)       38 2024-04-03 03:47:56.433122 hmtaiga-0.1.6/setup.cfg
--rw-r--r--   0 hasanshahid   (501) staff       (20)      182 2024-04-03 03:47:47.000000 hmtaiga-0.1.6/setup.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.429947 hmtaiga-0.1.6/tasks/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/tasks/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     5914 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/tasks/get_task_history.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     2446 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/tasks/get_tasks.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.430935 hmtaiga-0.1.6/test/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/test/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)      939 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/test/test_getProjectBySlug.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     4839 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/test/test_get_task_history.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     4571 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/test/test_get_tasks.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:47:56.431542 hmtaiga-0.1.6/userStory/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:46:48.000000 hmtaiga-0.1.6/userStory/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)      855 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/userStory/getBusinessValue.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     2298 2024-04-03 03:23:28.000000 hmtaiga-0.1.6/userStory/get_user_story_history.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865828 hmtaiga-0.1.7/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 02:47:15.865640 hmtaiga-0.1.7/PKG-INFO
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.862555 hmtaiga-0.1.7/auth/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.7/auth/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      895 2024-02-12 04:15:32.000000 hmtaiga-0.1.7/auth/authenticate.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865482 hmtaiga-0.1.7/hmtaiga.egg-info/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      545 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       44 2024-04-04 02:47:15.000000 hmtaiga-0.1.7/hmtaiga.egg-info/top_level.txt
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.863420 hmtaiga-0.1.7/milestone/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/milestone/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      644 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/milestone/get_milestone.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.863834 hmtaiga-0.1.7/project/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/project/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/project/getProjectBySlug.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-04 02:47:15.865857 hmtaiga-0.1.7/setup.cfg
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      183 2024-04-04 02:43:05.000000 hmtaiga-0.1.7/setup.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.864269 hmtaiga-0.1.7/tasks/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/tasks/get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.864902 hmtaiga-0.1.7/test/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      939 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_getProjectBySlug.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      527 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_milestone.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:47:15.865268 hmtaiga-0.1.7/userStory/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/getBusinessValue.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-04 02:41:58.000000 hmtaiga-0.1.7/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.6/milestone/get_milestone.py` & `hmtaiga-0.1.7/milestone/get_milestone.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/project/getProjectBySlug.py` & `hmtaiga-0.1.7/project/getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/tasks/get_task_history.py` & `hmtaiga-0.1.7/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/tasks/get_tasks.py` & `hmtaiga-0.1.7/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/test/test_getProjectBySlug.py` & `hmtaiga-0.1.7/test/test_getProjectBySlug.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/test/test_get_task_history.py` & `hmtaiga-0.1.7/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/test/test_get_tasks.py` & `hmtaiga-0.1.7/test/test_get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/userStory/getBusinessValue.py` & `hmtaiga-0.1.7/userStory/getBusinessValue.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.6/userStory/get_user_story_history.py` & `hmtaiga-0.1.7/userStory/get_user_story_history.py`

 * *Files identical despite different names*

