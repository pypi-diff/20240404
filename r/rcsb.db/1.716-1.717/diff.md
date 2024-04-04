# Comparing `tmp/rcsb.db-1.716.tar.gz` & `tmp/rcsb.db-1.717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.716.tar", last modified: Thu Mar 21 20:08:26 2024, max compression
+gzip compressed data, was "rcsb.db-1.717.tar", last modified: Thu Apr  4 15:33:48 2024, max compression
```

## Comparing `rcsb.db-1.716.tar` & `rcsb.db-1.717.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.674178 rcsb.db-1.716/
--rw-r--r--   0 vsts      (1001) docker     (127)    30394 2024-03-21 19:42:00.000000 rcsb.db-1.716/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-03-21 19:42:00.000000 rcsb.db-1.716/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-03-21 19:42:00.000000 rcsb.db-1.716/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-03-21 20:08:26.674178 rcsb.db-1.716/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    26823 2024-03-21 19:42:00.000000 rcsb.db-1.716/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.658178 rcsb.db-1.716/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.658178 rcsb.db-1.716/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.662179 rcsb.db-1.716/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7661 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24702 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8774 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.662179 rcsb.db-1.716/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.662179 rcsb.db-1.716/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.666179 rcsb.db-1.716/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15358 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.666179 rcsb.db-1.716/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.666179 rcsb.db-1.716/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15040 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54787 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.666179 rcsb.db-1.716/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.670179 rcsb.db-1.716/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.670179 rcsb.db-1.716/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.670179 rcsb.db-1.716/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.674178 rcsb.db-1.716/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)    11601 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-21 19:42:00.000000 rcsb.db-1.716/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-21 20:08:26.674178 rcsb.db-1.716/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-21 19:46:13.000000 rcsb.db-1.716/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-03-21 20:08:26.000000 rcsb.db-1.716/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-03-21 19:42:00.000000 rcsb.db-1.716/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-03-21 20:08:26.674178 rcsb.db-1.716/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-03-21 19:42:00.000000 rcsb.db-1.716/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.966329 rcsb.db-1.717/
+-rw-r--r--   0 vsts      (1001) docker     (127)    30462 2024-04-04 15:10:22.000000 rcsb.db-1.717/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-04 15:10:22.000000 rcsb.db-1.717/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-04 15:10:22.000000 rcsb.db-1.717/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-04-04 15:33:48.966329 rcsb.db-1.717/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    26823 2024-04-04 15:10:22.000000 rcsb.db-1.717/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.950329 rcsb.db-1.717/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7661 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24702 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8774 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.954329 rcsb.db-1.717/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15040 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54787 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.958329 rcsb.db-1.717/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19129 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11601 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 15:10:22.000000 rcsb.db-1.717/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 15:33:48.962329 rcsb.db-1.717/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    28369 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 15:13:43.000000 rcsb.db-1.717/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-04 15:33:48.000000 rcsb.db-1.717/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-04-04 15:10:22.000000 rcsb.db-1.717/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-04 15:33:48.966329 rcsb.db-1.717/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-04-04 15:10:22.000000 rcsb.db-1.717/setup.py
```

### Comparing `rcsb.db-1.716/HISTORY.txt` & `rcsb.db-1.717/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -348,8 +348,8 @@
  19-May-2023  V1.711 Update DNS to PDB archive
  23-Sep-2023  V1.712 Add support for pdb_id_u cifType in DataTypeApplicationInfo
   6-Nov-2023  V1.713 Add maxStepLength argument to RepoLoadWorkflow
  21-Nov-2023  V1.714 Add support in json schema for min and unique items for sub-categories and iterable attributes
  15-Dec-2023  V1.715 Revert setting for mergeValidationReports
  19-Mar-2024  V1.716 Add quality check to PdbxLoader to ensure validation report data are loaded along with the primary data;
                      Begin updating PdbxLoader and RepoLoadEx to support weekly update workflow CLI requirements
-
+ 03-Apr-2024  V1.717 Add int_list cifType to DataTypeApplicationInfo
```

### Comparing `rcsb.db-1.716/LICENSE` & `rcsb.db-1.717/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/PKG-INFO` & `rcsb.db-1.717/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.716
+Version: 1.717
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.716/README.md` & `rcsb.db-1.717/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/ETLExec.py` & `rcsb.db-1.717/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb.db-1.717/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/RepoLoadExec.py` & `rcsb.db-1.717/rcsb/db/cli/RepoLoadExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/RepoScanExec.py` & `rcsb.db-1.717/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb.db-1.717/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb.db-1.717/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb.db-1.717/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb.db-1.717/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/cockroach/Connection.py` & `rcsb.db-1.717/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/crate/Connection.py` & `rcsb.db-1.717/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/crate/CrateDbLoader.py` & `rcsb.db-1.717/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/crate/CrateDbUtil.py` & `rcsb.db-1.717/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/define/ContentDefinition.py` & `rcsb.db-1.717/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/define/DataTypeApiProvider.py` & `rcsb.db-1.717/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb.db-1.717/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #  15-Aug-2018 jdw add mapping for JSON types based on generic 'ANY' typing.
 #  29-Sep-2018 jdw make JSON date and datetime type explicit in JSON
 #  12-Oct-2018 jdw unsuppress datetime mapping
 #   7-Jan-2019 jdw applicationName->dataTyping
 #  23-Jan-2023  bv Add uchar5 cifType to handle updates to _chem_comp.three_letter_code
 #   6-Apr-2023  bv Add entity_id_list cifType to handle _pdbx_initial_refinement_model.entity_id_list
 #  23-Sep-2023  bv Add pdb_id_u cifType to handle _em_3d_fitting_list.pdb_entry_id
+#  03-Apr-2024  bv Add int_list cifType to handle _pdbx_item_type.code for _pdbx_initial_refinement_model.entity_id_list
 ##
 """
 Manage mapping of default application data type to dictionary data types.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -65,14 +66,15 @@
         "yyyy-mm-dd:hh:mm-flex",
         "ec-type",
         "ucode-alphanum-csv",
         "int-range",
         "point_symmetry",
         "id_list",
         "entity_id_list",
+        "int_list"
         "4x3_matrix",
         "non_negative_int",
         "positive_int",
         "emd_id",
         "pdb_id",
         "pdb_id_u",
         "point_group",
@@ -118,14 +120,15 @@
         "char",
         "char",
         "char",
         "char",
         "char",
         "char",
         "char",
+        "char",
         "int",
         "int",
         "char",
         "char",
         "char",
         "char",
         "char",
@@ -169,14 +172,15 @@
         "20",
         "10",
         "25",
         "20",
         "80",
         "100",
         "100",
+        "100",
         "10",
         "10",
         "10",
         "15",
         "20",
         "200",
         "20",
@@ -205,14 +209,15 @@
         "0",
         "0",
         "0",
         "0",
         "0",
         "0",
         "0",
+        "0",
         "0",
         "0",
         "0",
         "0",
         "0",
         "0",
         "0",
```

### Comparing `rcsb.db-1.716/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb.db-1.717/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/define/SchemaDefAccess.py` & `rcsb.db-1.717/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/define/SchemaDefBuild.py` & `rcsb.db-1.717/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb.db-1.717/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb.db-1.717/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/helpers/r.py` & `rcsb.db-1.717/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mongo/Connection.py` & `rcsb.db-1.717/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mongo/ConnectionBase.py` & `rcsb.db-1.717/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mongo/DocumentLoader.py` & `rcsb.db-1.717/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mongo/MongoDbUtil.py` & `rcsb.db-1.717/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mongo/PdbxLoader.py` & `rcsb.db-1.717/rcsb/db/mongo/PdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/Connection.py` & `rcsb.db-1.717/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/ConnectionBase.py` & `rcsb.db-1.717/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/MyDbAdapter.py` & `rcsb.db-1.717/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/MyDbUtil.py` & `rcsb.db-1.717/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb.db-1.717/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb.db-1.717/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/ClusterDataPrep.py` & `rcsb.db-1.717/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/DataExchangeStatus.py` & `rcsb.db-1.717/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/DataTransformFactory.py` & `rcsb.db-1.717/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb.db-1.717/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb.db-1.717/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb.db-1.717/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/processors/SchemaDefReShape.py` & `rcsb.db-1.717/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/sql/QueryDirectives.py` & `rcsb.db-1.717/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/sql/SqlGen.py` & `rcsb.db-1.717/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb.db-1.717/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb.db-1.717/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/ProvenanceProvider.py` & `rcsb.db-1.717/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/SchemaProvider.py` & `rcsb.db-1.717/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/TextUtil.py` & `rcsb.db-1.717/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/TimeUtil.py` & `rcsb.db-1.717/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/makePathList.py` & `rcsb.db-1.717/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/utils/unescape.py` & `rcsb.db-1.717/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb.db-1.717/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/rcsb.db.egg-info/PKG-INFO` & `rcsb.db-1.717/rcsb.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.716
+Version: 1.717
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.716/rcsb.db.egg-info/SOURCES.txt` & `rcsb.db-1.717/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/requirements.txt` & `rcsb.db-1.717/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.716/setup.py` & `rcsb.db-1.717/setup.py`

 * *Files identical despite different names*

