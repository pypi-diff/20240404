# Comparing `tmp/paas-app-charmer-0.2.1.tar.gz` & `tmp/paas-app-charmer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paas-app-charmer-0.2.1.tar", last modified: Wed Mar 27 03:58:04 2024, max compression
+gzip compressed data, was "paas-app-charmer-1.0.0.tar", last modified: Wed Apr  3 23:20:32 2024, max compression
```

## Comparing `paas-app-charmer-0.2.1.tar` & `paas-app-charmer-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      633 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.520091 paas-app-charmer-0.2.1/paas_app_charmer/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      122 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9532 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/charm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8486 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/charm_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2904 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/observability.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/secret_storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7159 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/webserver.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/wsgi_app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4198 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/database_migration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7535 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/databases.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/django/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/django/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4190 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/django/charm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.520091 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/grafana_dashboards/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26134 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/grafana_dashboards/django.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/loki_alert_rules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/prometheus_alert_rules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      616 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.524091 paas-app-charmer-0.2.1/paas_app_charmer/flask/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      217 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/flask/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4019 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/flask/charm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.520091 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/grafana_dashboards/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26108 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/loki_alert_rules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/prometheus_alert_rules/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3755 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/paas_app_charmer/secret_storage.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      633 2024-03-27 03:58:04.000000 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2024-03-27 03:58:04.000000 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-27 03:58:04.000000 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-03-27 03:58:04.000000 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-03-27 03:58:04.000000 paas-app-charmer-0.2.1/paas_app_charmer.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2139 2024-03-27 03:57:50.000000 paas-app-charmer-0.2.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-27 03:58:04.528091 paas-app-charmer-0.2.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2024-03-27 03:57:13.000000 paas-app-charmer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/observability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/secret_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/wsgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.154874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26134 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/django.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/django/cos/prometheus_alert_rules/django.rule
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/charm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.158874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/flask.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/loki_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/loki_alert_rules/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/prometheus_alert_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/prometheus_alert_rules/flask.rule
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/paas_app_charmer/secret_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 23:20:32.000000 paas-app-charmer-1.0.0/paas_app_charmer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:20:32.162874 paas-app-charmer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 23:20:22.000000 paas-app-charmer-1.0.0/setup.py
```

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/charm.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,40 +4,49 @@
 
 """The base Gunicorn charm class for all WSGI application charms."""
 import abc
 import logging
 
 import ops
 from charms.data_platform_libs.v0.data_interfaces import DatabaseRequiresEvent
+from charms.redis_k8s.v0.redis import RedisRelationCharmEvents, RedisRequires
 from charms.traefik_k8s.v2.ingress import IngressPerAppRequirer
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
 
 from paas_app_charmer._gunicorn.charm_state import CharmState
 from paas_app_charmer._gunicorn.observability import Observability
 from paas_app_charmer._gunicorn.secret_storage import GunicornSecretStorage
 from paas_app_charmer._gunicorn.webserver import GunicornWebserver
 from paas_app_charmer._gunicorn.wsgi_app import WsgiApp
 from paas_app_charmer.database_migration import DatabaseMigration, DatabaseMigrationStatus
 from paas_app_charmer.databases import Databases, make_database_requirers
 from paas_app_charmer.exceptions import CharmConfigInvalidError
+from paas_app_charmer.helpers import load_requires
 
 logger = logging.getLogger(__name__)
 
 
 class GunicornBase(abc.ABC, ops.CharmBase):  # pylint: disable=too-many-instance-attributes
-    """Gunicorn-based charm service mixin."""
+    """Gunicorn-based charm service mixin.
+
+    Attrs:
+        on: charm events replaced by Redis ones for the Redis charm library.
+    """
 
     @abc.abstractmethod
     def get_wsgi_config(self) -> BaseModel:
         """Return the framework related configurations."""
 
     @abc.abstractmethod
     def get_cos_dir(self) -> str:
         """Return the directory with COS related files."""
 
+    on = RedisRelationCharmEvents()
+    _store = ops.StoredState()
+
     def __init__(self, framework: ops.Framework, wsgi_framework: str) -> None:
         """Initialize the instance.
 
         Args:
             framework: operator framework.
             wsgi_framework: WSGI framework name.
         """
@@ -48,20 +57,29 @@
         self._database_requirers = make_database_requirers(self, self.app.name)
         try:
             wsgi_config = self.get_wsgi_config()
         except CharmConfigInvalidError as exc:
             self._update_app_and_unit_status(ops.BlockedStatus(exc.msg))
             return
 
+        requires = load_requires()
+        if "redis" in requires and requires["redis"]["interface"] == "redis":
+            self._store.set_default(redis_relation={})
+            self._redis = RedisRequires(charm=self, _stored=self._store, relation_name="redis")
+            self.framework.observe(self.on.redis_relation_updated, self._on_redis_relation_updated)
+        else:
+            self._redis = None
+
         self._charm_state = CharmState.from_charm(
             charm=self,
             framework=wsgi_framework,
             wsgi_config=wsgi_config,
             secret_storage=self._secret_storage,
             database_requirers=self._database_requirers,
+            redis_uri=self._redis.url if self._redis is not None else None,
         )
         self._database_migration = DatabaseMigration(
             container=self.unit.get_container(self._charm_state.container_name),
             state_dir=self._charm_state.state_dir,
         )
         webserver = GunicornWebserver(
             charm_state=self._charm_state,
@@ -219,18 +237,10 @@
         """Handle the mysql's endpoints-changed event."""
         self.restart()
 
     def _on_mongodb_database_relation_broken(self, _event: ops.RelationBrokenEvent) -> None:
         """Handle the postgresql's relation-broken event."""
         self.restart()
 
-    def _on_redis_database_database_created(self, _event: DatabaseRequiresEvent) -> None:
+    def _on_redis_relation_updated(self, _event: DatabaseRequiresEvent) -> None:
         """Handle the redis's database-created event."""
         self.restart()
-
-    def _on_redis_database_endpoints_changed(self, _event: DatabaseRequiresEvent) -> None:
-        """Handle the mysql's endpoints-changed event."""
-        self.restart()
-
-    def _on_redis_database_relation_broken(self, _event: ops.RelationBrokenEvent) -> None:
-        """Handle the postgresql's relation-broken event."""
-        self.restart()
```

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/charm_state.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/charm_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         is_secret_storage_ready: whether the secret storage system is ready.
         proxy: proxy information.
         service_name: The WSGI application pebble service name.
         container_name: The name of the WSGI application container.
         base_dir: The project base directory in the WSGI application container.
         app_dir: The WSGI application directory in the WSGI application container.
         user: The UNIX user name for running the service.
-        group: The UNIX group name for running the service
+        group: The UNIX group name for running the service.
+        redis_uri: The redis uri provided by the redis charm.
     """
 
     statsd_host = "localhost:9125"
     port = 8000
     user = "_daemon_"
     group = "_daemon_"
 
@@ -66,58 +67,63 @@
         framework: str,
         webserver_config: WebserverConfig,
         is_secret_storage_ready: bool,
         app_config: dict[str, int | str | bool] | None = None,
         database_requirers: dict[str, DatabaseRequires] | None = None,
         wsgi_config: dict[str, int | str] | None = None,
         secret_key: str | None = None,
+        redis_uri: str | None = None,
     ):
         """Initialize a new instance of the CharmState class.
 
         Args:
             framework: the framework name.
             webserver_config: the Gunicorn webserver configuration.
             is_secret_storage_ready: whether the secret storage system is ready.
             app_config: User-defined configuration values for the WSGI application configuration.
             wsgi_config: The value of the WSGI application specific charm configuration.
             secret_key: The secret storage manager associated with the charm.
             database_requirers: All declared database requirers.
+            redis_uri: The redis uri provided by the redis charm.
         """
         self.framework = framework
         self.service_name = self.framework
         self.container_name = f"{self.framework}-app"
         self.base_dir = pathlib.Path(f"/{framework}")
         self.app_dir = self.base_dir / "app"
         self.state_dir = self.base_dir / "state"
         self.application_log_file = pathlib.Path(f"/var/log/{self.framework}/access.log")
         self.application_error_log_file = pathlib.Path(f"/var/log/{self.framework}/error.log")
         self.webserver_config = webserver_config
+        self.redis_uri = redis_uri
         self._wsgi_config = wsgi_config if wsgi_config is not None else {}
         self._app_config = app_config if app_config is not None else {}
         self._is_secret_storage_ready = is_secret_storage_ready
         self._secret_key = secret_key
         self._database_requirers = database_requirers if database_requirers else {}
 
     @classmethod
     def from_charm(  # pylint: disable=too-many-arguments
         cls,
         charm: ops.CharmBase,
         framework: str,
         wsgi_config: BaseModel,
         secret_storage: GunicornSecretStorage,
         database_requirers: dict[str, DatabaseRequires],
+        redis_uri: str | None = None,
     ) -> "CharmState":
         """Initialize a new instance of the CharmState class from the associated charm.
 
         Args:
             charm: The charm instance associated with this state.
             framework: The WSGI framework name.
             wsgi_config: The WSGI framework specific configurations.
             secret_storage: The secret storage manager associated with the charm.
             database_requirers: All database requirers object declared by the charm.
+            redis_uri: The redis uri provided by the redis charm.
 
         Return:
             The CharmState instance created by the provided charm.
         """
         app_config = {
             k.replace("-", "_"): v
             for k, v in charm.config.items()
@@ -130,14 +136,15 @@
             app_config=typing.cast(dict[str, str | int | bool], app_config),
             database_requirers=database_requirers,
             webserver_config=WebserverConfig.from_charm(charm),
             secret_key=(
                 secret_storage.get_secret_key() if secret_storage.is_initialized else None
             ),
             is_secret_storage_ready=secret_storage.is_initialized,
+            redis_uri=redis_uri,
         )
 
     @property
     def proxy(self) -> "ProxyConfig":
         """Get charm proxy information from juju charm environment.
 
         Returns:
```

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/observability.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/observability.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/secret_storage.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/webserver.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/webserver.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/_gunicorn/wsgi_app.py` & `paas-app-charmer-1.0.0/paas_app_charmer/_gunicorn/wsgi_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             env[secret_key_env] = self._charm_state.secret_key
         for proxy_variable in ("http_proxy", "https_proxy", "no_proxy"):
             proxy_value = getattr(self._charm_state.proxy, proxy_variable)
             if proxy_value:
                 env[proxy_variable] = str(proxy_value)
                 env[proxy_variable.upper()] = str(proxy_value)
         env.update(self._charm_state.database_uris)
+        if self._charm_state.redis_uri:
+            env["REDIS_DB_CONNECT_STRING"] = self._charm_state.redis_uri
         return env
 
     def _wsgi_layer(self) -> ops.pebble.LayerDict:
         """Generate the pebble layer definition for WSGI application.
 
         Returns:
             The pebble layer definition for WSGI application.
```

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/database_migration.py` & `paas-app-charmer-1.0.0/paas_app_charmer/database_migration.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/django/charm.py` & `paas-app-charmer-1.0.0/paas_app_charmer/django/charm.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/django/cos/grafana_dashboards/django.json` & `paas-app-charmer-1.0.0/paas_app_charmer/django/cos/grafana_dashboards/django.json`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/exceptions.py` & `paas-app-charmer-1.0.0/paas_app_charmer/exceptions.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/flask/charm.py` & `paas-app-charmer-1.0.0/paas_app_charmer/flask/charm.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/flask/cos/grafana_dashboards/flask.json` & `paas-app-charmer-1.0.0/paas_app_charmer/flask/cos/grafana_dashboards/flask.json`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer/secret_storage.py` & `paas-app-charmer-1.0.0/paas_app_charmer/secret_storage.py`

 * *Files identical despite different names*

### Comparing `paas-app-charmer-0.2.1/paas_app_charmer.egg-info/SOURCES.txt` & `paas-app-charmer-1.0.0/paas_app_charmer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 requirements.txt
 setup.py
 paas_app_charmer/__init__.py
 paas_app_charmer/database_migration.py
 paas_app_charmer/databases.py
 paas_app_charmer/exceptions.py
+paas_app_charmer/helpers.py
 paas_app_charmer/secret_storage.py
 paas_app_charmer.egg-info/PKG-INFO
 paas_app_charmer.egg-info/SOURCES.txt
 paas_app_charmer.egg-info/dependency_links.txt
 paas_app_charmer.egg-info/requires.txt
 paas_app_charmer.egg-info/top_level.txt
 paas_app_charmer/_gunicorn/__init__.py
```

### Comparing `paas-app-charmer-0.2.1/pyproject.toml` & `paas-app-charmer-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2024 Canonical Ltd.
 # See LICENSE file for licensing details.
 [project]
 name = "paas-app-charmer"
-version = "0.2.1"
+version = "1.0.0"
 description = "Companion library for PaaS app charmer."
+readme = "README.md"
 authors = [
     {name = "Canonical IS DevOps team", email="is-devops-team@canonical.com"},
 ]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
```

