# Comparing `tmp/swh.storage-2.2.1.tar.gz` & `tmp/swh.storage-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.storage-2.2.1.tar", last modified: Fri Mar 29 20:22:32 2024, max compression
+gzip compressed data, was "swh.storage-2.2.2.tar", last modified: Thu Apr  4 10:35:58 2024, max compression
```

## Comparing `swh.storage-2.2.1.tar` & `swh.storage-2.2.2.tar`

### file list

```diff
@@ -1,378 +1,378 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.365120 swh.storage-2.2.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-03-29 20:22:25.000000 swh.storage-2.2.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-03-29 20:22:25.000000 swh.storage-2.2.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-03-29 20:22:25.000000 swh.storage-2.2.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-03-29 20:22:25.000000 swh.storage-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-03-29 20:22:25.000000 swh.storage-2.2.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-03-29 20:22:25.000000 swh.storage-2.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-03-29 20:22:25.000000 swh.storage-2.2.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-03-29 20:22:25.000000 swh.storage-2.2.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-03-29 20:22:25.000000 swh.storage-2.2.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-03-29 20:22:25.000000 swh.storage-2.2.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-03-29 20:22:32.365120 swh.storage-2.2.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-03-29 20:22:25.000000 swh.storage-2.2.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.281121 swh.storage-2.2.1/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-03-29 20:22:25.000000 swh.storage-2.2.1/bin/swh-storage-add-dir
--rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-03-29 20:22:25.000000 swh.storage-2.2.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/Makefile.local
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/archive-copies.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/extrinsic-metadata-specification.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/images/swh-archive-copies.dia
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/object-masking.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-03-29 20:22:25.000000 swh.storage-2.2.1/docs/sql-storage.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-03-29 20:22:25.000000 swh.storage-2.2.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1846 2024-03-29 20:22:25.000000 swh.storage-2.2.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-03-29 20:22:25.000000 swh.storage-2.2.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-03-29 20:22:25.000000 swh.storage-2.2.1/requirements-swh-journal.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-03-29 20:22:25.000000 swh.storage-2.2.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      406 2024-03-29 20:22:25.000000 swh.storage-2.2.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-03-29 20:22:25.000000 swh.storage-2.2.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-03-29 20:22:32.369120 swh.storage-2.2.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/TODO
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.285121 swh.storage-2.2.1/sql/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/bin/dot_add_content
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/clusters.dot
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.273121 swh.storage-2.2.1/sql/doc/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.289121 swh.storage-2.2.1/sql/json/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/entity.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/entity.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/entity_history.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/entity_history.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/fetch_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/list_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/listable_entity.list_params.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/origin_visit.metadata.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-03-29 20:22:25.000000 swh.storage-2.2.1/sql/json/tool.tool_configuration.schema.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.273121 swh.storage-2.2.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.297120 swh.storage-2.2.1/swh/storage/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4148 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.297120 swh.storage-2.2.1/swh/storage/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/dir_iterators.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6525 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/algos/snapshot.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.297120 swh.storage-2.2.1/swh/storage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2110 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4024 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5221 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20570 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/backfill.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.301120 swh.storage-2.2.1/swh/storage/cassandra/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/cql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10766 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/schema.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    86739 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cassandra/storage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14670 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3325 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/fixer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/migrate_extrinsic_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4245 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.301120 swh.storage-2.2.1/swh/storage/postgresql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/postgresql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12321 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/postgresql/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/postgresql/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    69889 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/postgresql/storage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.305120 swh.storage-2.2.1/swh/storage/proxies/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2033 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5120 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/filter.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.305120 swh.storage-2.2.1/swh/storage/proxies/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18425 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/masking/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12742 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/masking/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3229 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2586 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/proxies/validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10285 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/replay.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.305120 swh.storage-2.2.1/swh/storage/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1067 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1312 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24806 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35050 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14048 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2528 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/80-masked-objects.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.305120 swh.storage-2.2.1/swh/storage/sql/logical_replication/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/logical_replication/replication_source.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.349120 swh.storage-2.2.1/swh/storage/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/015.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/016.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/017.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/018.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/019.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/020.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/021.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/022.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/023.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/024.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/025.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/026.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/027.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/028.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/029.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/030.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/032.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/033.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/034.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/035.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/036.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/037.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/038.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/039.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/040.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/041.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/042.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/043.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/044.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/045.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/046.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/047.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/048.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/049.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/050.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/051.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/052.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/053.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/054.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/055.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/056.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/057.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/058.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/059.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/060.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/061.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/062.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/063.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/064.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/065.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/066.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/067.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/068.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/069.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/070.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/071.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/072.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/073.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/074.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/075.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/076.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/077.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/078.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/079.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/080.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/081.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/082.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/083.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/084.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/085.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/086.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/087.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/088.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/089.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/090.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/091.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/092.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/093.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/094.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/095.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/096.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/097.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/098.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/099.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/100.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/101.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/102.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/103.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/104.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/105.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/106.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/107.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/108.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/109.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/110.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/111.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/112.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/113.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/114.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/137.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/138.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/139.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/140.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/141.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/142.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/143.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/144.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/145.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/146.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/147.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/148.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/149.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/150.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/151.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/152.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/153.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/154.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/155.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/156.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/157.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/158.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/159.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/160.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/161.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/162.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/163.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/164.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/165.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/166.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/167.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/168.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/169.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/170.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/171.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/172.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/173.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/174.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/175.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/176.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/177.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/178.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/179.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/180.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/181.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/182.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/183.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/184.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/185.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/186.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/187.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/188.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/189.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/190.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/191.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/sql/upgrades/192.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.357120 swh.storage-2.2.1/swh/storage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.361120 swh.storage-2.2.1/swh/storage/tests/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_dir_iterator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13842 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/algos/test_snapshot.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.361120 swh.storage-2.2.1/swh/storage/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/data/storage.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.361120 swh.storage-2.2.1/swh/storage/tests/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18822 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9818 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30504 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/test_proxy.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5872 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/test_proxy_masking.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      960 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/masking/test_proxy_no_masking.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.365120 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20296 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25029 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    27669 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)   235228 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/storage_tests.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5205 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_backfill.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    29473 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_cassandra.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_cassandra_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_cassandra_migration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13302 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1167 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_postgresql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_postgresql_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_postgresql_flavor_mirror.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_postgresql_flavor_readreplica.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23199 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_replay.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/tests/test_validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4041 2024-03-29 20:22:25.000000 swh.storage-2.2.1/swh/storage/writer.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-29 20:22:32.365120 swh.storage-2.2.1/swh.storage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11282 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      114 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      488 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-03-29 20:22:32.000000 swh.storage-2.2.1/swh.storage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-03-29 20:22:25.000000 swh.storage-2.2.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.590465 swh.storage-2.2.2/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-04-04 10:35:53.000000 swh.storage-2.2.2/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-04-04 10:35:53.000000 swh.storage-2.2.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-04 10:35:53.000000 swh.storage-2.2.2/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-04-04 10:35:53.000000 swh.storage-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-04 10:35:53.000000 swh.storage-2.2.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-04 10:35:53.000000 swh.storage-2.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-04 10:35:53.000000 swh.storage-2.2.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-04 10:35:53.000000 swh.storage-2.2.2/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-04 10:35:53.000000 swh.storage-2.2.2/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-04-04 10:35:53.000000 swh.storage-2.2.2/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-04-04 10:35:58.590465 swh.storage-2.2.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-04-04 10:35:53.000000 swh.storage-2.2.2/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.498466 swh.storage-2.2.2/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-04-04 10:35:53.000000 swh.storage-2.2.2/bin/swh-storage-add-dir
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-04-04 10:35:53.000000 swh.storage-2.2.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.502466 swh.storage-2.2.2/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/Makefile.local
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.502466 swh.storage-2.2.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.502466 swh.storage-2.2.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/archive-copies.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/extrinsic-metadata-specification.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.502466 swh.storage-2.2.2/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/images/swh-archive-copies.dia
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/object-masking.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-04-04 10:35:53.000000 swh.storage-2.2.2/docs/sql-storage.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-04-04 10:35:53.000000 swh.storage-2.2.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1846 2024-04-04 10:35:53.000000 swh.storage-2.2.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-04-04 10:35:53.000000 swh.storage-2.2.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-04-04 10:35:53.000000 swh.storage-2.2.2/requirements-swh-journal.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-04-04 10:35:53.000000 swh.storage-2.2.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      406 2024-04-04 10:35:53.000000 swh.storage-2.2.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-04-04 10:35:53.000000 swh.storage-2.2.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-04 10:35:58.594465 swh.storage-2.2.2/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.506466 swh.storage-2.2.2/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/TODO
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.506466 swh.storage-2.2.2/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/bin/dot_add_content
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/clusters.dot
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.490466 swh.storage-2.2.2/sql/doc/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.510466 swh.storage-2.2.2/sql/json/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/entity.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/entity.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/entity_history.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/entity_history.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/fetch_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/list_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/listable_entity.list_params.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/origin_visit.metadata.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-04-04 10:35:53.000000 swh.storage-2.2.2/sql/json/tool.tool_configuration.schema.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.490466 swh.storage-2.2.2/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.514466 swh.storage-2.2.2/swh/storage/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4148 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.518466 swh.storage-2.2.2/swh/storage/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/dir_iterators.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6525 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/algos/snapshot.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.518466 swh.storage-2.2.2/swh/storage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2110 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4512 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5403 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20570 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/backfill.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.522466 swh.storage-2.2.2/swh/storage/cassandra/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/cql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10766 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/schema.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    86739 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cassandra/storage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14670 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3325 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/fixer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/migrate_extrinsic_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4245 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.522466 swh.storage-2.2.2/swh/storage/postgresql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/postgresql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12321 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/postgresql/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/postgresql/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    69889 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/postgresql/storage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.526466 swh.storage-2.2.2/swh/storage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2033 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5120 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/filter.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.526466 swh.storage-2.2.2/swh/storage/proxies/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18512 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/masking/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12742 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/masking/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3229 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2586 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/proxies/validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10285 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/replay.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.526466 swh.storage-2.2.2/swh/storage/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1067 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1312 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24806 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35050 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14048 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2528 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/80-masked-objects.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.530465 swh.storage-2.2.2/swh/storage/sql/logical_replication/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/logical_replication/replication_source.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.574465 swh.storage-2.2.2/swh/storage/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/015.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/016.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/017.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/018.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/019.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/020.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/021.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/022.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/023.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/024.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/025.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/026.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/027.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/028.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/029.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/030.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/032.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/033.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/034.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/035.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/036.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/037.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/038.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/039.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/040.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/041.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/042.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/043.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/044.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/045.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/046.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/047.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/048.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/049.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/050.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/051.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/052.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/053.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/054.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/055.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/056.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/057.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/058.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/059.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/060.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/061.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/062.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/063.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/064.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/065.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/066.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/067.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/068.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/069.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/070.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/071.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/072.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/073.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/074.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/075.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/076.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/077.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/078.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/079.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/080.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/081.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/082.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/083.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/084.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/085.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/086.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/087.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/088.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/089.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/090.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/091.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/092.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/093.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/094.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/095.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/096.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/097.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/098.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/099.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/100.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/101.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/102.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/103.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/104.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/105.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/106.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/107.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/108.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/109.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/110.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/111.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/112.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/113.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/114.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/137.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/138.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/139.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/140.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/141.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/142.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/143.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/144.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/145.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/146.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/147.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/148.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/149.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/150.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/151.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/152.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/153.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/154.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/155.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/156.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/157.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/158.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/159.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/160.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/161.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/162.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/163.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/164.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/165.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/166.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/167.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/168.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/169.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/170.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/171.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/172.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/173.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/174.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/175.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/176.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/177.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/178.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/179.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/180.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/181.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/182.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/183.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/184.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/185.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/186.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/187.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/188.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/189.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/190.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/191.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/sql/upgrades/192.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.582465 swh.storage-2.2.2/swh/storage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.586465 swh.storage-2.2.2/swh/storage/tests/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_dir_iterator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13842 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/algos/test_snapshot.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.586465 swh.storage-2.2.2/swh/storage/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/data/storage.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.586465 swh.storage-2.2.2/swh/storage/tests/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18822 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9818 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30504 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/test_proxy.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5872 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/test_proxy_masking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      960 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/masking/test_proxy_no_masking.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.590465 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20296 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25029 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    27669 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   235228 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/storage_tests.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6103 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_backfill.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    29473 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_cassandra.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_cassandra_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_cassandra_migration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13302 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1167 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_postgresql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_postgresql_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_postgresql_flavor_mirror.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_postgresql_flavor_readreplica.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23199 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_replay.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/tests/test_validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4041 2024-04-04 10:35:53.000000 swh.storage-2.2.2/swh/storage/writer.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-04 10:35:58.590465 swh.storage-2.2.2/swh.storage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11282 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      114 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      488 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-04 10:35:58.000000 swh.storage-2.2.2/swh.storage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-04-04 10:35:53.000000 swh.storage-2.2.2/tox.ini
```

### Comparing `swh.storage-2.2.1/.pre-commit-config.yaml` & `swh.storage-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/CODE_OF_CONDUCT.md` & `swh.storage-2.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/LICENSE` & `swh.storage-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/PKG-INFO` & `swh.storage-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.2.1
+Version: 2.2.2
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
```

### Comparing `swh.storage-2.2.1/README.rst` & `swh.storage-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/bin/swh-storage-add-dir` & `swh.storage-2.2.2/bin/swh-storage-add-dir`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/Makefile.local` & `swh.storage-2.2.2/docs/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/archive-copies.rst` & `swh.storage-2.2.2/docs/archive-copies.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/extrinsic-metadata-specification.rst` & `swh.storage-2.2.2/docs/extrinsic-metadata-specification.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/images/swh-archive-copies.dia` & `swh.storage-2.2.2/docs/images/swh-archive-copies.dia`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/index.rst` & `swh.storage-2.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/docs/object-masking.rst` & `swh.storage-2.2.2/docs/object-masking.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/mypy.ini` & `swh.storage-2.2.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/pyproject.toml` & `swh.storage-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/Makefile` & `swh.storage-2.2.2/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/TODO` & `swh.storage-2.2.2/sql/TODO`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/bin/db-upgrade` & `swh.storage-2.2.2/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/bin/dot_add_content` & `swh.storage-2.2.2/sql/bin/dot_add_content`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/clusters.dot` & `swh.storage-2.2.2/sql/clusters.dot`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/json/fetch_history.result.schema.json` & `swh.storage-2.2.2/sql/json/fetch_history.result.schema.json`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/sql/json/origin_visit.metadata.json` & `swh.storage-2.2.2/sql/json/origin_visit.metadata.json`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/__init__.py` & `swh.storage-2.2.2/swh/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/diff.py` & `swh.storage-2.2.2/swh/storage/algos/diff.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/dir_iterators.py` & `swh.storage-2.2.2/swh/storage/algos/dir_iterators.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/directory.py` & `swh.storage-2.2.2/swh/storage/algos/directory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/discovery.py` & `swh.storage-2.2.2/swh/storage/algos/discovery.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/origin.py` & `swh.storage-2.2.2/swh/storage/algos/origin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/revisions_walker.py` & `swh.storage-2.2.2/swh/storage/algos/revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/algos/snapshot.py` & `swh.storage-2.2.2/swh/storage/algos/snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/api/client.py` & `swh.storage-2.2.2/swh/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/api/serializers.py` & `swh.storage-2.2.2/swh/storage/api/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Decoder and encoders for swh-model objects."""
 
 from typing import Any, Callable, Dict, List, Tuple
+import uuid
 
 from swh.model import model, swhids
 from swh.storage import interface
+from swh.storage.proxies.masking.db import MaskedState, MaskedStatus
 
 
 def _encode_model_object(obj):
     d = obj.to_dict()
     d["__type__"] = type(obj).__name__
     return d
 
@@ -44,14 +46,25 @@
     return {
         "branch_found": branch_by_name_response.branch_found,
         "target": target.to_dict() if target else None,
         "aliases_followed": branch_by_name_response.aliases_followed,
     }
 
 
+def _encode_masked_status(masked_status: MaskedStatus):
+    return {
+        "state": masked_status.state.name,
+        "request": str(masked_status.request),
+    }
+
+
+def _decode_masked_status(d: Dict[str, Any]):
+    return MaskedStatus(state=MaskedState[d["state"]], request=uuid.UUID(d["request"]))
+
+
 def _decode_origin_visit_with_statuses(
     ovws: Dict[str, Any],
 ) -> interface.OriginVisitWithStatuses:
     return interface.OriginVisitWithStatuses(
         visit=model.OriginVisit(**ovws["visit"]),
         statuses=[model.OriginVisitStatus(**status) for status in ovws["statuses"]],
     )
@@ -105,14 +118,15 @@
         _encode_object_reference,
     ),
     (
         interface.SnapshotBranchByNameResponse,
         "branch_by_name_response",
         _encode_snapshot_branch_by_name_response,
     ),
+    (MaskedStatus, "masked_status", _encode_masked_status),
 ]
 
 
 DECODERS: Dict[str, Callable] = {
     "core_swhid": swhids.CoreSWHID.from_string,
     "extended_swhid": swhids.ExtendedSWHID.from_string,
     "qualified_swhid": swhids.QualifiedSWHID.from_string,
@@ -120,8 +134,9 @@
     "identifiers_enum": _decode_swhids_enum,
     "swhids_enum": _decode_swhids_enum,
     "model_enum": _decode_model_enum,
     "storage_enum": _decode_storage_enum,
     "origin_visit_with_statuses": _decode_origin_visit_with_statuses,
     "object_reference": _decode_object_reference,
     "branch_by_name_response": _decode_snapshot_branch_by_name_response,
+    "masked_status": _decode_masked_status,
 }
```

### Comparing `swh.storage-2.2.1/swh/storage/api/server.py` & `swh.storage-2.2.2/swh/storage/api/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright (C) 2015-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from functools import partial
 import logging
 import os
 from typing import Any, Dict, Optional
 
 from swh.core import config
 from swh.core.api import RPCServerApp
 from swh.core.api import encode_data_server as encode_data
 from swh.core.api import error_handler
 from swh.storage import get_storage as get_swhstorage
 
-from ..exc import StorageArgumentException
+from ..exc import NonRetryableException
 from ..interface import StorageInterface
 from ..metrics import send_metric, timed
 from .serializers import DECODERS, ENCODERS
 
 
 def get_storage():
     global storage
@@ -89,17 +90,21 @@
 
 app = StorageServerApp(
     __name__, backend_class=StorageInterface, backend_factory=get_storage
 )
 storage = None
 
 
-@app.errorhandler(StorageArgumentException)
-def argument_error_handler(exception):
-    return error_handler(exception, encode_data, status_code=400)
+@app.errorhandler(NonRetryableException)
+def non_retryable_error_handler(exception):
+    """Send all non-retryable errors with a 400 status code so the client can
+    re-raise them."""
+    return error_handler(
+        exception, partial(encode_data, extra_type_encoders=ENCODERS), status_code=400
+    )
 
 
 app.setup_psycopg2_errorhandlers()
 
 
 @app.errorhandler(Exception)
 def default_error_handler(exception):
```

### Comparing `swh.storage-2.2.1/swh/storage/backfill.py` & `swh.storage-2.2.2/swh/storage/backfill.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/common.py` & `swh.storage-2.2.2/swh/storage/cassandra/common.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/converters.py` & `swh.storage-2.2.2/swh/storage/cassandra/converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/cql.py` & `swh.storage-2.2.2/swh/storage/cassandra/cql.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/model.py` & `swh.storage-2.2.2/swh/storage/cassandra/model.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/schema.py` & `swh.storage-2.2.2/swh/storage/cassandra/schema.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cassandra/storage.py` & `swh.storage-2.2.2/swh/storage/cassandra/storage.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/cli.py` & `swh.storage-2.2.2/swh/storage/cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/exc.py` & `swh.storage-2.2.2/swh/storage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/fixer.py` & `swh.storage-2.2.2/swh/storage/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/in_memory.py` & `swh.storage-2.2.2/swh/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/interface.py` & `swh.storage-2.2.2/swh/storage/interface.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/metrics.py` & `swh.storage-2.2.2/swh/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/migrate_extrinsic_metadata.py` & `swh.storage-2.2.2/swh/storage/migrate_extrinsic_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/objstorage.py` & `swh.storage-2.2.2/swh/storage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/postgresql/converters.py` & `swh.storage-2.2.2/swh/storage/postgresql/converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/postgresql/db.py` & `swh.storage-2.2.2/swh/storage/postgresql/db.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/postgresql/storage.py` & `swh.storage-2.2.2/swh/storage/postgresql/storage.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/buffer.py` & `swh.storage-2.2.2/swh/storage/proxies/buffer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/counter.py` & `swh.storage-2.2.2/swh/storage/proxies/counter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/filter.py` & `swh.storage-2.2.2/swh/storage/proxies/filter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/masking/__init__.py` & `swh.storage-2.2.2/swh/storage/proxies/masking/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,17 +366,18 @@
 
                 with t.inner():
                     result = method(*args, **kwargs)
 
                 if result is None:
                     return None
 
-                parsed_args = inspect.getcallargs(method, *args, **kwargs)
+                signature = inspect.signature(getattr(StorageInterface, method_name))
+                bound_args = signature.bind(self, *args, **kwargs)
                 self._raise_if_masked_swhids(
-                    self._get_swhids_in_args(method_name, parsed_args)
+                    self._get_swhids_in_args(method_name, bound_args.arguments)
                 )
 
                 return result
 
         return newf
 
     RANDOM_ATTEMPTS = 5
```

### Comparing `swh.storage-2.2.1/swh/storage/proxies/masking/cli.py` & `swh.storage-2.2.2/swh/storage/proxies/masking/cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/masking/db.py` & `swh.storage-2.2.2/swh/storage/proxies/masking/db.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/record_references.py` & `swh.storage-2.2.2/swh/storage/proxies/record_references.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/retry.py` & `swh.storage-2.2.2/swh/storage/proxies/retry.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/tenacious.py` & `swh.storage-2.2.2/swh/storage/proxies/tenacious.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/proxies/validate.py` & `swh.storage-2.2.2/swh/storage/proxies/validate.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/pytest_plugin.py` & `swh.storage-2.2.2/swh/storage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/replay.py` & `swh.storage-2.2.2/swh/storage/replay.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/10-superuser-init.sql` & `swh.storage-2.2.2/swh/storage/sql/10-superuser-init.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/15-flavor.sql` & `swh.storage-2.2.2/swh/storage/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/20-enums.sql` & `swh.storage-2.2.2/swh/storage/sql/20-enums.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/30-schema.sql` & `swh.storage-2.2.2/swh/storage/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/40-funcs.sql` & `swh.storage-2.2.2/swh/storage/sql/40-funcs.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/60-indexes.sql` & `swh.storage-2.2.2/swh/storage/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/80-masked-objects.sql` & `swh.storage-2.2.2/swh/storage/sql/80-masked-objects.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/logical_replication/replication_source.sql` & `swh.storage-2.2.2/swh/storage/sql/logical_replication/replication_source.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/015.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/015.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/016.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/016.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/017.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/017.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/018.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/018.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/019.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/019.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/020.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/020.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/021.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/021.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/022.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/022.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/023.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/023.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/024.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/024.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/025.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/025.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/026.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/026.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/027.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/027.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/028.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/028.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/029.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/029.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/030.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/030.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/032.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/032.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/033.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/033.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/034.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/034.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/035.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/035.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/036.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/036.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/037.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/037.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/038.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/038.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/039.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/039.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/040.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/040.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/041.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/041.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/042.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/042.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/043.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/043.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/044.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/044.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/046.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/046.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/047.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/047.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/048.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/048.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/049.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/049.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/050.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/050.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/051.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/051.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/052.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/052.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/053.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/053.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/054.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/054.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/055.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/055.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/056.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/056.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/057.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/057.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/058.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/058.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/059.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/059.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/060.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/060.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/061.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/061.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/062.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/062.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/063.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/063.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/064.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/064.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/065.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/065.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/067.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/067.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/068.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/068.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/069.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/069.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/071.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/071.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/072.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/072.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/073.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/073.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/074.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/074.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/075.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/075.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/076.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/076.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/077.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/077.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/078.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/078.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/079.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/079.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/080.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/080.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/081.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/081.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/082.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/082.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/083.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/083.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/084.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/084.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/085.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/085.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/086.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/086.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/087.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/087.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/088.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/088.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/089.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/089.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/090.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/090.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/091.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/091.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/092.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/092.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/093.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/093.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/094.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/094.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/095.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/095.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/096.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/096.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/097.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/097.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/099.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/099.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/100.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/100.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/101.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/101.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/102.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/102.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/103.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/103.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/104.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/104.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/105.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/105.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/106.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/106.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/107.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/107.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/108.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/108.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/109.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/109.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/110.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/110.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/111.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/111.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/112.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/112.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/113.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/113.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/114.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/114.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/115.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/117.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/118.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/118.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/119.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/120.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/123.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/124.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/124.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/125.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/127.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/128.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/128.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/129.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/130.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/134.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/136.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/137.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/138.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/138.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/139.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/139.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/143.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/143.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/146.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/146.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/147.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/147.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/148.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/148.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/149.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/149.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/150.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/150.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/154.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/154.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/155.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/155.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/156.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/156.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/157.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/157.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/158.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/158.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/159.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/159.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/160.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/160.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/161.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/161.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/162.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/162.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/163.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/163.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/167.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/167.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/168.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/168.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/169.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/169.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/170.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/170.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/171.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/171.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/172.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/172.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/173.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/173.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/175.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/175.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/176.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/176.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/179.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/179.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/180.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/180.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/181.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/181.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/182.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/182.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/183.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/183.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/184.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/184.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/185.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/185.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/187.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/187.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/188.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/188.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/189.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/189.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/190.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/190.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/sql/upgrades/191.sql` & `swh.storage-2.2.2/swh/storage/sql/upgrades/191.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_diff.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_diff.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_dir_iterator.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_dir_iterator.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_directory.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_discovery.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_discovery.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_origin.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_origin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_revisions_walker.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/algos/test_snapshot.py` & `swh.storage-2.2.2/swh/storage/tests/algos/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/conftest.py` & `swh.storage-2.2.2/swh/storage/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/conftest.py` & `swh.storage-2.2.2/swh/storage/tests/masking/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/test_cli.py` & `swh.storage-2.2.2/swh/storage/tests/masking/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/test_db.py` & `swh.storage-2.2.2/swh/storage/tests/masking/test_db.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/test_proxy.py` & `swh.storage-2.2.2/swh/storage/tests/masking/test_proxy.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/test_proxy_masking.py` & `swh.storage-2.2.2/swh/storage/tests/masking/test_proxy_masking.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/masking/test_proxy_no_masking.py` & `swh.storage-2.2.2/swh/storage/tests/masking/test_proxy_no_masking.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py` & `swh.storage-2.2.2/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/storage_data.py` & `swh.storage-2.2.2/swh/storage/tests/storage_data.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/storage_tests.py` & `swh.storage-2.2.2/swh/storage/tests/storage_tests.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_api_client.py` & `swh.storage-2.2.2/swh/storage/tests/test_api_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Copyright (C) 2015-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from uuid import uuid4
+
 import psycopg2.errors
 import pytest
 
 from swh.core.api import RemoteException, TransientRemoteException
+from swh.model.swhids import ExtendedSWHID
 import swh.storage
 from swh.storage import get_storage
 import swh.storage.api.server as server
+from swh.storage.exc import MaskedObjectException
+from swh.storage.proxies.masking.db import MaskedState, MaskedStatus
 from swh.storage.tests.storage_tests import (
     TestStorageGeneratedData as _TestStorageGeneratedData,
 )
 from swh.storage.tests.storage_tests import TestStorage as _TestStorage
 
 # tests are executed using imported classes (TestStorage and
 # TestStorageGeneratedData) using overloaded swh_storage fixture
@@ -126,14 +131,31 @@
             "revision_get",
             side_effect=psycopg2.errors.QueryCanceled("too big!"),
         )
         with pytest.raises(RemoteException) as excinfo:
             swh_storage.revision_get(["\x01" * 20])
         assert not isinstance(excinfo.value, TransientRemoteException)
 
+    def test_masked_object_exception(self, app_server, swh_storage, mocker):
+        """Checks the client re-raises masking proxy exceptions"""
+        assert swh_storage.revision_get(["\x01" * 20]) == [None]
+        masked = {
+            ExtendedSWHID.from_string("swh:1:rev:" + ("01" * 20)): [
+                MaskedStatus(MaskedState.DECISION_PENDING, request=uuid4())
+            ]
+        }
+        mocker.patch.object(
+            app_server.storage._cql_runner,
+            "revision_get",
+            side_effect=MaskedObjectException(masked),
+        )
+        with pytest.raises(MaskedObjectException) as e:
+            swh_storage.revision_get(["\x01" * 20])
+        assert e.value.masked == masked
+
 
 class TestStorageApiGeneratedData(_TestStorageGeneratedData):
     @pytest.mark.skip("Not supported by Cassandra")
     def test_origin_count(self):
         pass
 
     @pytest.mark.skip("Not supported by Cassandra")
```

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_backfill.py` & `swh.storage-2.2.2/swh/storage/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_buffer.py` & `swh.storage-2.2.2/swh/storage/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_cassandra.py` & `swh.storage-2.2.2/swh/storage/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_cassandra_converters.py` & `swh.storage-2.2.2/swh/storage/tests/test_cassandra_converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_cassandra_migration.py` & `swh.storage-2.2.2/swh/storage/tests/test_cassandra_migration.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_cli.py` & `swh.storage-2.2.2/swh/storage/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_counter.py` & `swh.storage-2.2.2/swh/storage/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_exception.py` & `swh.storage-2.2.2/swh/storage/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_filter.py` & `swh.storage-2.2.2/swh/storage/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_in_memory.py` & `swh.storage-2.2.2/swh/storage/tests/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_init.py` & `swh.storage-2.2.2/swh/storage/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_kafka_writer.py` & `swh.storage-2.2.2/swh/storage/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_metrics.py` & `swh.storage-2.2.2/swh/storage/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_postgresql.py` & `swh.storage-2.2.2/swh/storage/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_postgresql_converters.py` & `swh.storage-2.2.2/swh/storage/tests/test_postgresql_converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_postgresql_flavor_mirror.py` & `swh.storage-2.2.2/swh/storage/tests/test_postgresql_flavor_mirror.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_postgresql_flavor_readreplica.py` & `swh.storage-2.2.2/swh/storage/tests/test_postgresql_flavor_readreplica.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_pytest_plugin.py` & `swh.storage-2.2.2/swh/storage/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_record_references.py` & `swh.storage-2.2.2/swh/storage/tests/test_record_references.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_replay.py` & `swh.storage-2.2.2/swh/storage/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_retry.py` & `swh.storage-2.2.2/swh/storage/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_serializers.py` & `swh.storage-2.2.2/swh/storage/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_server.py` & `swh.storage-2.2.2/swh/storage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_storage_data.py` & `swh.storage-2.2.2/swh/storage/tests/test_storage_data.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_tenacious.py` & `swh.storage-2.2.2/swh/storage/tests/test_tenacious.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_utils.py` & `swh.storage-2.2.2/swh/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/tests/test_validate.py` & `swh.storage-2.2.2/swh/storage/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/utils.py` & `swh.storage-2.2.2/swh/storage/utils.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh/storage/writer.py` & `swh.storage-2.2.2/swh/storage/writer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/swh.storage.egg-info/PKG-INFO` & `swh.storage-2.2.2/swh.storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.2.1
+Version: 2.2.2
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
```

### Comparing `swh.storage-2.2.1/swh.storage.egg-info/SOURCES.txt` & `swh.storage-2.2.2/swh.storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.storage-2.2.1/tox.ini` & `swh.storage-2.2.2/tox.ini`

 * *Files identical despite different names*

