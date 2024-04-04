# Comparing `tmp/python_dev_utils-0.1.0.tar.gz` & `tmp/python_dev_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-0.1.0.tar", last modified: Wed Apr  3 08:55:46 2024, max compression
+gzip compressed data, was "python_dev_utils-0.1.1.tar", last modified: Thu Apr  4 10:38:52 2024, max compression
```

## Comparing `python_dev_utils-0.1.0.tar` & `python_dev_utils-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-0.1.0/LICENCE
--rw-r--r--   0        0        0        0 2024-03-19 07:17:12.960400 python_dev_utils-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-0.1.0/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-0.1.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-0.1.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      229 2024-03-26 14:07:13.958342 python_dev_utils-0.1.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-01 13:22:15.897317 python_dev_utils-0.1.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0      776 2024-03-28 08:22:11.212881 python_dev_utils-0.1.0/dev_utils/core/utils.py
--rw-r--r--   0        0        0      210 2024-03-28 10:44:02.392930 python_dev_utils-0.1.0/dev_utils/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-03-29 13:52:13.342131 python_dev_utils-0.1.0/dev_utils/profiling/containers.py
--rw-r--r--   0        0        0     2805 2024-03-29 13:59:41.103779 python_dev_utils-0.1.0/dev_utils/profiling/middlewares.py
--rw-r--r--   0        0        0     9120 2024-03-29 14:18:09.501095 python_dev_utils-0.1.0/dev_utils/profiling/profilers.py
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-0.1.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16318 2024-03-29 14:28:49.462964 python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1562 2024-03-26 14:07:50.698059 python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-03-29 14:18:20.445990 python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-03-25 07:02:41.449042 python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0    12623 2024-03-26 08:35:25.401470 python_dev_utils-0.1.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     2920 2024-04-03 08:55:46.588371 python_dev_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     9104 2024-04-01 13:25:07.596658 python_dev_utils-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-0.1.0/tests/core/__init__.py
--rw-r--r--   0        0        0      508 2024-03-26 14:08:33.510730 python_dev_utils-0.1.0/tests/core/test_guards.py
--rw-r--r--   0        0        0      933 2024-03-29 06:21:02.987051 python_dev_utils-0.1.0/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-0.1.0/tests/profiling/__init__.py
--rw-r--r--   0        0        0      349 2024-03-29 13:58:08.366680 python_dev_utils-0.1.0/tests/profiling/test_middlewares.py
--rw-r--r--   0        0        0     2723 2024-03-29 12:18:07.567058 python_dev_utils-0.1.0/tests/profiling/test_profilers.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-0.1.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    17186 2024-03-29 13:24:07.386873 python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-03-26 14:08:03.098964 python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-03-25 06:40:32.137462 python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0     7366 2024-03-25 06:19:19.846082 python_dev_utils-0.1.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      820 2024-03-29 06:17:35.440257 python_dev_utils-0.1.0/tests/types.py
--rw-r--r--   0        0        0     7174 2024-03-29 06:15:40.110095 python_dev_utils-0.1.0/tests/utils.py
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 python_dev_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-0.1.1/LICENCE
+-rw-r--r--   0        0        0     2038 2024-04-04 09:26:57.087717 python_dev_utils-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-0.1.1/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-0.1.1/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-04 10:15:44.718260 python_dev_utils-0.1.1/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-0.1.1/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      229 2024-03-26 14:07:13.958342 python_dev_utils-0.1.1/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-01 13:22:15.897317 python_dev_utils-0.1.1/dev_utils/core/logging.py
+-rw-r--r--   0        0        0      776 2024-03-28 08:22:11.212881 python_dev_utils-0.1.1/dev_utils/core/utils.py
+-rw-r--r--   0        0        0      210 2024-03-28 10:44:02.392930 python_dev_utils-0.1.1/dev_utils/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-03-29 13:52:13.342131 python_dev_utils-0.1.1/dev_utils/profiling/containers.py
+-rw-r--r--   0        0        0     2850 2024-04-04 09:56:53.374155 python_dev_utils-0.1.1/dev_utils/profiling/middlewares.py
+-rw-r--r--   0        0        0     9754 2024-04-04 10:02:43.937276 python_dev_utils-0.1.1/dev_utils/profiling/profilers.py
+-rw-r--r--   0        0        0      936 2024-04-04 09:55:26.621868 python_dev_utils-0.1.1/dev_utils/profiling/utils.py
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-0.1.1/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16331 2024-04-04 08:59:51.727121 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1562 2024-03-26 14:07:50.698059 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-03-29 14:18:20.445990 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-03-25 07:02:41.449042 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0    12623 2024-03-26 08:35:25.401470 python_dev_utils-0.1.1/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     2962 2024-04-04 10:38:52.009451 python_dev_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     9104 2024-04-01 13:25:07.596658 python_dev_utils-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-0.1.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     1589 2024-04-04 10:35:52.893988 python_dev_utils-0.1.1/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      508 2024-03-26 14:08:33.510730 python_dev_utils-0.1.1/tests/core/test_guards.py
+-rw-r--r--   0        0        0      933 2024-03-29 06:21:02.987051 python_dev_utils-0.1.1/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-0.1.1/tests/profiling/__init__.py
+-rw-r--r--   0        0        0      349 2024-03-29 13:58:08.366680 python_dev_utils-0.1.1/tests/profiling/test_middlewares.py
+-rw-r--r--   0        0        0     3027 2024-04-04 10:01:48.346733 python_dev_utils-0.1.1/tests/profiling/test_profilers.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-0.1.1/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    17186 2024-03-29 13:24:07.386873 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-03-26 14:08:03.098964 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-03-25 06:40:32.137462 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0     7366 2024-03-25 06:19:19.846082 python_dev_utils-0.1.1/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      820 2024-03-29 06:17:35.440257 python_dev_utils-0.1.1/tests/types.py
+-rw-r--r--   0        0        0     7174 2024-03-29 06:15:40.110095 python_dev_utils-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 python_dev_utils-0.1.1/PKG-INFO
```

### Comparing `python_dev_utils-0.1.0/LICENCE` & `python_dev_utils-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/core/exc.py` & `python_dev_utils-0.1.1/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/core/logging.py` & `python_dev_utils-0.1.1/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/core/utils.py` & `python_dev_utils-0.1.1/dev_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/profiling/containers.py` & `python_dev_utils-0.1.1/dev_utils/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/profiling/middlewares.py` & `python_dev_utils-0.1.1/dev_utils/profiling/middlewares.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from logging import Logger
+from pathlib import Path
 
 from fastapi import FastAPI, Request
 from sqlalchemy import Engine
 from starlette.middleware.base import RequestResponseEndpoint
 from starlette.responses import Response
 
 from dev_utils.core.logging import logger as default_logger
@@ -11,14 +12,15 @@
 
 def add_query_profiling_middleware(
     app: FastAPI,
     engine: Engine | type[Engine] = Engine,
     *,
     profiler_id: str | None = None,
     logger: Logger = default_logger,
+    report_to: str | Logger | Path = default_logger,
     log_query_stats: bool = False,
 ) -> FastAPI:
     """Add query profiling middleware to FastAPI.
 
     Note: this function also can be used with starlette instance, but only before version 1.0.0,
     because `middleware` decorator is deprecated and will be (or, maybe, already removed) in this
     version.
@@ -32,19 +34,16 @@
             engine=engine,
             profiler_id=profiler_id,
             logger=logger,
             log_query_states=log_query_stats,
         ) as profiler:
             logger.info('Profiler %s: start profiling %s', profiler.profiler_id, request.url)
             response = await call_next(request)
-        logger.info(
-            'Profiler %s result: %s',
-            profiler.profiler_id,
-            profiler.collect(),
-        )
+        profiler.report(report_to)
+        logger.info('Profiler %s finished.', profiler.profiler_id)
         return response
 
     app.middleware("http")(_profiling_middleware)
     return app
 
 
 def add_query_counter_middleware(
```

### Comparing `python_dev_utils-0.1.0/dev_utils/profiling/profilers.py` & `python_dev_utils-0.1.1/dev_utils/profiling/profilers.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import time
 import traceback
 import uuid
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence
 from contextlib import suppress
 from logging import Logger
+from pathlib import Path
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Generic, Self, TypeVar, final
 
 from sqlalchemy import event
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.asyncio import AsyncEngine
 
 from dev_utils.core.guards import all_dict_keys_are_str
 from dev_utils.core.logging import logger as default_logger
 from dev_utils.core.utils import trim_and_plain_text
 from dev_utils.profiling.containers import QueryInfo
+from dev_utils.profiling.utils import pretty_query_info
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Connection
     from sqlalchemy.engine.cursor import CursorResult
     from sqlalchemy.sql import ClauseElement
     from sqlalchemy.sql.compiler import SQLCompiler
     from sqlalchemy.util import immutabledict
@@ -164,14 +166,18 @@
         queries: list[T] = []
         with suppress(queue.Empty):
             while True:
                 queries.append(self.collector.get(block=False))
 
         return queries
 
+    def report(self, stdout: 'str | Path | Logger | None' = None) -> None:  # noqa: F841
+        """Make report about profiling."""
+        return  # pragma: no coverage
+
 
 class SQLAlchemyQueryProfiler(BaseSQLAlchemyProfiler[QueryInfo]):
     """SQLAlchemy query profiler."""
 
     def _before_exec(
         self,
         conn: 'Connection',
@@ -221,14 +227,24 @@
             end_time=end_time,
             params_dict=params_dict,
             results=results,
         )
 
         self.collector.put(query_info)
 
+    def report(self, stdout: str | Path | Logger | None = None) -> None:  # noqa: D102
+        if not stdout:  # pragma: no coverage
+            stdout = self.logger
+        data = pretty_query_info(self.collect())
+        if isinstance(stdout, Logger):
+            stdout.info(data)
+            return
+        with Path(stdout).open('a') as writer:
+            writer.write(data)
+
 
 class SQLAlchemyQueryCounter(BaseSQLAlchemyProfiler[int]):
     """SQLAlchemy query counter."""
 
     def collect(self) -> int:  # type: ignore  # noqa: D102
         if self._result is None:  # pragma: no cover
             return 0
```

### Comparing `python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import enum
 import operator as builtin_operator
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from inspect import signature
 from typing import TYPE_CHECKING, Any, final
 
-from abstractcp import Abstract, abstract_class_property
 from sqlalchemy.sql.elements import ColumnElement
 
+from dev_utils.core.abstract import Abstract, abstract_class_property
 from dev_utils.core.exc import FilterError
 from dev_utils.sqlalchemy.filters import operators as custom_operator
 from dev_utils.sqlalchemy.filters.guards import has_nested_lookups, is_dict_simple_filter_dict
 from dev_utils.sqlalchemy.utils import get_sqlalchemy_attribute, get_valid_field_names
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import DeclarativeBase
```

### Comparing `python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-0.1.1/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/pyproject.toml` & `python_dev_utils-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -163,32 +163,33 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "0.1.0"
+version = "0.1.1"
 description = "My project utils package, that I use in my projects."
-authors = []
+authors = [
+    { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
+]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 profiling = [
     "fastapi>=0.110.0",
     "sqlalchemy>=2.0.28",
 ]
 sqlalchemy_filters = [
     "sqlalchemy>=2.0.28",
-    "abstractcp>=0.9.9",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `python_dev_utils-0.1.0/tests/conftest.py` & `python_dev_utils-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/core/test_utils.py` & `python_dev_utils-0.1.1/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/profiling/test_profilers.py` & `python_dev_utils-0.1.1/tests/profiling/test_profilers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from sqlalchemy import select
 
 from dev_utils.core.utils import trim_and_plain_text
 from dev_utils.profiling import profilers
@@ -33,14 +34,25 @@
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     profiler.start()
     profiler.stop()
 
 
+def test_sync_sql_alchemy_query_profiler_report(
+    db_sync_engine: 'Engine',
+) -> None:
+    profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
+    profiler.start()
+    profiler.stop()
+    file = Path('report.txt')
+    profiler.report(file)
+    assert file.exists()
+
+
 def test_sync_sql_alchemy_query_profiler_double_stop(
     db_sync_engine: 'Engine',
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     profiler.stop()
     profiler.stop()
```

### Comparing `python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-0.1.1/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/types.py` & `python_dev_utils-0.1.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.0/tests/utils.py` & `python_dev_utils-0.1.1/tests/utils.py`

 * *Files identical despite different names*

