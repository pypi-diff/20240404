# Comparing `tmp/jobbergate_agent-5.0.0a0.tar.gz` & `tmp/jobbergate_agent-5.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_agent-5.0.0a0.tar", max compression
+gzip compressed data, was "jobbergate_agent-5.0.0a1.tar", max compression
```

## Comparing `jobbergate_agent-5.0.0a0.tar` & `jobbergate_agent-5.0.0a1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1077 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/LICENSE
--rw-r--r--   0        0        0     1346 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/README.md
--rw-r--r--   0        0        0        0 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/clients/__init__.py
--rw-r--r--   0        0        0     3597 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/clients/cluster_api.py
--rw-r--r--   0        0        0        0 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/__init__.py
--rw-r--r--   0        0        0      150 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/constants.py
--rw-r--r--   0        0        0     2805 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/schemas.py
--rw-r--r--   0        0        0    10780 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/submit.py
--rw-r--r--   0        0        0     3676 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/update.py
--rw-r--r--   0        0        0      491 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/main.py
--rw-r--r--   0        0        0     2674 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/settings.py
--rw-r--r--   0        0        0     2201 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/tasks.py
--rw-r--r--   0        0        0        0 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/__init__.py
--rw-r--r--   0        0        0     4663 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/exception.py
--rw-r--r--   0        0        0     1440 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/logging.py
--rw-r--r--   0        0        0     1414 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/plugin.py
--rw-r--r--   0        0        0     2155 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/scheduler.py
--rw-r--r--   0        0        0      730 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/sentry.py
--rw-r--r--   0        0        0     2500 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/jobbergate_agent/utils/user_mapper.py
--rw-r--r--   0        0        0     3179 2024-03-26 18:59:26.819343 jobbergate_agent-5.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/clients/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/clients/cluster_api.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/internals/__init__.py
+-rw-r--r--   0        0        0     2737 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/internals/update.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/constants.py
+-rw-r--r--   0        0        0     2805 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/schemas.py
+-rw-r--r--   0        0        0    10780 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/submit.py
+-rw-r--r--   0        0        0     3676 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/update.py
+-rw-r--r--   0        0        0      491 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/main.py
+-rw-r--r--   0        0        0     2759 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/settings.py
+-rw-r--r--   0        0        0     2627 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/__init__.py
+-rw-r--r--   0        0        0     4663 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/exception.py
+-rw-r--r--   0        0        0     1440 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/logging.py
+-rw-r--r--   0        0        0     1414 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/plugin.py
+-rw-r--r--   0        0        0     2153 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/scheduler.py
+-rw-r--r--   0        0        0      730 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/sentry.py
+-rw-r--r--   0        0        0     2500 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/jobbergate_agent/utils/user_mapper.py
+-rw-r--r--   0        0        0     3235 2024-04-04 21:27:34.688349 jobbergate_agent-5.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.0.0a1/PKG-INFO
```

### Comparing `jobbergate_agent-5.0.0a0/LICENSE` & `jobbergate_agent-5.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/README.md` & `jobbergate_agent-5.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/clients/cluster_api.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/clients/cluster_api.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/schemas.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/submit.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/submit.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/jobbergate/update.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/jobbergate/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/settings.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     # Single user submitter settings
     SINGLE_USER_SUBMITTER: Optional[str]
 
     # Task settings
     TASK_JOBS_INTERVAL_SECONDS: int = Field(60, ge=10, le=3600)  # seconds
     TASK_GARBAGE_COLLECTION_HOUR: Optional[int] = Field(None, ge=0, le=23)  # hour of day
+    TASK_SELF_UPDATE_INTERVAL_SECONDS: Optional[int] = Field(None, ge=10)  # seconds
 
     # Job submission settings
     WRITE_SUBMISSION_FILES: bool = True
 
     @root_validator
     def compute_extra_settings(cls, values):
         """
```

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/tasks.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 import asyncio
 from typing import Union
 
 from buzz import handle_errors
 from loguru import logger
 
 from jobbergate_agent.clients.cluster_api import backend_client
+from jobbergate_agent.internals.update import self_update_agent
 from jobbergate_agent.jobbergate.submit import submit_pending_jobs
 from jobbergate_agent.jobbergate.update import update_active_jobs
 from jobbergate_agent.settings import SETTINGS
 from jobbergate_agent.utils.logging import log_error, logger_wraps
 from jobbergate_agent.utils.scheduler import BaseScheduler, Job
 
 
+def self_update_task(scheduler: BaseScheduler) -> Job:
+    """
+    Schedule a task to self update the agent every ``TASK_SELF_UPDATE_INTERVAL_SECONDS`` seconds.
+    """
+    if SETTINGS.TASK_SELF_UPDATE_INTERVAL_SECONDS is None:
+        return None
+    return scheduler.add_job(self_update_agent, "interval", seconds=SETTINGS.TASK_SELF_UPDATE_INTERVAL_SECONDS)
+
+
 def active_submissions_task(scheduler: BaseScheduler) -> Job:
     """
     Schedule a task to handle active jobs every ``TASK_JOBS_INTERVAL_SECONDS`` seconds.
     """
     return scheduler.add_job(update_active_jobs, "interval", seconds=SETTINGS.TASK_JOBS_INTERVAL_SECONDS)
```

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/exception.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/logging.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/plugin.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/scheduler.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from apscheduler.schedulers.base import BaseScheduler
 from buzz import handle_errors
 
 from jobbergate_agent.utils.logging import logger, logger_wraps
 from jobbergate_agent.utils.plugin import load_plugins
 
 
+scheduler = AsyncIOScheduler()
+
+
 class JobbergateTask(Protocol):
     """Protocol to be implemented by any task that is expected to run on the scheduler."""
 
     def __call__(self, scheduler: BaseScheduler) -> Union[Job, None]:
         """
         Specify a callable used to schedule a task and return the resulting job.
 
@@ -49,15 +52,14 @@
         if job is not None:
             job.name = name
 
 
 @logger_wraps()
 def init_scheduler() -> BaseScheduler:
     """Initialize the scheduler and schedule all tasks."""
-    scheduler = AsyncIOScheduler()
     scheduler.start()
     schedule_tasks(scheduler)
     return scheduler
 
 
 @logger_wraps()
 def shut_down_scheduler(scheduler: BaseScheduler, wait: bool = True) -> None:
```

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/sentry.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/jobbergate_agent/utils/user_mapper.py` & `jobbergate_agent-5.0.0a1/jobbergate_agent/utils/user_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a0/pyproject.toml` & `jobbergate_agent-5.0.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-agent"
-version = "5.0.0a0"
+version = "5.0.0a1"
 description = "Jobbergate Agent"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -45,14 +45,15 @@
 [tool.poetry.scripts]
 jg-run = "jobbergate_agent.main:main"
 
 [tool.poetry.plugins.'jobbergate_agent.tasks']
 active-jobs = 'jobbergate_agent.tasks:active_submissions_task'
 pending-jobs = 'jobbergate_agent.tasks:pending_submissions_task'
 garbage-collection = 'jobbergate_agent.tasks:garbage_collection_task'
+self-update = 'jobbergate_agent.tasks:self_update_task'
 
 [tool.poetry.plugins.'jobbergate_agent.user_mapper']
 single-user-mapper = "jobbergate_agent.utils.user_mapper:SingleUserMapper"
 
 [tool.poetry.dev-dependencies]
 asynctest = "^0.13.0"
 black = "^24.3"
```

### Comparing `jobbergate_agent-5.0.0a0/PKG-INFO` & `jobbergate_agent-5.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-agent
-Version: 5.0.0a0
+Version: 5.0.0a1
 Summary: Jobbergate Agent
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: apscheduler (==3.10.3)
 Requires-Dist: auto-name-enum (>=2.0.0,<3.0.0)
 Requires-Dist: httpx (==0.24.1)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
-Requires-Dist: jobbergate-core (==5.0.0a0)
+Requires-Dist: jobbergate-core (==5.0.0a1)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: py-buzz (>=4.0.0,<5.0.0)
 Requires-Dist: pydantic (==1.10.12)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0)
```

