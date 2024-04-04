# Comparing `tmp/unionai-0.1.8.tar.gz` & `tmp/unionai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unionai-0.1.8.tar", last modified: Mon Mar 25 18:46:51 2024, max compression
+gzip compressed data, was "unionai-0.1.9.tar", last modified: Tue Mar 26 20:59:16 2024, max compression
```

## Comparing `unionai-0.1.8.tar` & `unionai-0.1.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-25 18:46:46.000000 unionai-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-25 18:46:46.000000 unionai-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-25 18:46:51.522654 unionai-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-25 18:46:46.000000 unionai-0.1.8/README_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.510654 unionai-0.1.8/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-03-25 18:46:46.000000 unionai-0.1.8/licenses/APL.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-25 18:46:46.000000 unionai-0.1.8/licenses/BSL.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-25 18:46:46.000000 unionai-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:46:51.522654 unionai-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:46:46.000000 unionai-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.510654 unionai-0.1.8/unionai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/_interceptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.510654 unionai-0.1.8/unionai/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/artifacts/_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/artifacts/_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/artifacts/_triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.510654 unionai-0.1.8/unionai/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/_get.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/cli/_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.514654 unionai-0.1.8/unionai/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/configuration/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.514654 unionai-0.1.8/unionai/filesystems/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/filesystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/filesystems/_async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/filesystems/_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/filesystems/_unionfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/filesystems/_unionmetafs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.514654 unionai-0.1.8/unionai/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.514654 unionai-0.1.8/unionai/internal/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)    18340 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.514654 unionai-0.1.8/unionai/internal/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/common/list_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/common/list_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/common/list_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.518654 unionai-0.1.8/unionai/internal/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_definition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_definition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_definition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_payload_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_payload_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_payload_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/app_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/enums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/enums_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/identity/enums_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.518654 unionai-0.1.8/unionai/internal/objectstore/
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/definition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/definition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/definition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/metadata_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/metadata_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/metadata_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/objectstore_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/objectstore_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/objectstore_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/payload_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/payload_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/objectstore/payload_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/unionai/internal/secret/
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/definition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/definition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/definition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/payload_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/payload_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/payload_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/secret_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/secret_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/secret/secret_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.506654 unionai-0.1.8/unionai/internal/validate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/unionai/internal/validate/validate/
--rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/validate/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/internal/validate/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/unionai/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/remote/_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/unionai/ucimage/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/ucimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-03-25 18:46:46.000000 unionai-0.1.8/unionai/ucimage/_image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:46:51.522654 unionai-0.1.8/unionai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 18:46:51.000000 unionai-0.1.8/unionai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.798872 unionai-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-26 20:59:11.000000 unionai-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-26 20:59:11.000000 unionai-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-26 20:59:16.798872 unionai-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-26 20:59:11.000000 unionai-0.1.9/README_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.782871 unionai-0.1.9/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-03-26 20:59:11.000000 unionai-0.1.9/licenses/APL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-26 20:59:11.000000 unionai-0.1.9/licenses/BSL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-26 20:59:11.000000 unionai-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:59:16.798872 unionai-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:59:11.000000 unionai-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/artifacts/_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/artifacts/_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/artifacts/_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/cli/_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/configuration/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/filesystems/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/filesystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/filesystems/_async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/filesystems/_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/filesystems/_unionfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/filesystems/_unionmetafs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.786872 unionai-0.1.9/unionai/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.790871 unionai-0.1.9/unionai/internal/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18340 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.790871 unionai-0.1.9/unionai/internal/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/common/list_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/common/list_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/common/list_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.790871 unionai-0.1.9/unionai/internal/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_definition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_definition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_definition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_payload_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_payload_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_payload_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/app_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/enums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/enums_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/identity/enums_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.794871 unionai-0.1.9/unionai/internal/objectstore/
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/definition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/definition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/definition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/metadata_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/metadata_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/metadata_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/objectstore_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/objectstore_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/objectstore_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/payload_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/payload_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/objectstore/payload_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.794871 unionai-0.1.9/unionai/internal/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/definition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/definition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/definition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/payload_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/payload_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/payload_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/secret_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/secret_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/secret/secret_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.782871 unionai-0.1.9/unionai/internal/validate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.794871 unionai-0.1.9/unionai/internal/validate/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/validate/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/internal/validate/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.794871 unionai-0.1.9/unionai/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/remote/_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.798872 unionai-0.1.9/unionai/ucimage/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/ucimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-03-26 20:59:11.000000 unionai-0.1.9/unionai/ucimage/_image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:59:16.798872 unionai-0.1.9/unionai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 20:59:16.000000 unionai-0.1.9/unionai.egg-info/top_level.txt
```

### Comparing `unionai-0.1.8/CHANGELOG.md` & `unionai-0.1.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## [Unreleased] - TBA
 
+## [v0.1.9] - 2024-03-26
+
+- Adds `verbose` and `x-request-id` for debugging.
+
 ## [v0.1.8] - 2024-03-25
 
 - Install `unionai` by default in the image builder.
 
 ## [v0.1.7] - 2024-03-25
 
 * Adds Image Build related mapping of Union serverless FQDN to Google Artifact registry base URLs.
```

### Comparing `unionai-0.1.8/PKG-INFO` & `unionai-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unionai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Adds Union Cloud specific functionality to Flytekit
 Author-email: unionai <oss@union.ai>
 License: Source code in this repository is licensed under the Business Source
         License 1.1 (BSL) and the Apache License 2.0 (APL). A copy of each
         license can be found in the licenses directory. Source code in a
         given file is licensed under the BSL and the copyright belongs to
         Union Systems, Inc. unless otherwise noted at the beginning of the
```

### Comparing `unionai-0.1.8/licenses/APL.txt` & `unionai-0.1.9/licenses/APL.txt`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/licenses/BSL.txt` & `unionai-0.1.9/licenses/BSL.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                       A “Compute Orchestration Service” is a commercial
                       offering that allows third parties (other than your
                       employees and contractors) to access the functionality
                       of the Licensed Work by creating workflows, tasks, or
                       computer programs whose source code are controlled by
                       such third parties.
 
-Change Date:          2028-03-25
+Change Date:          2028-03-26
 
 Change License:       Apache License, Version 2.0
 
 For information about alternative licensing arrangements for the Software,
 please visit: https://union.ai/
 
 Notice
```

### Comparing `unionai-0.1.8/pyproject.toml` & `unionai-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/_config.py` & `unionai-0.1.9/unionai/_config.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/_interceptor.py` & `unionai-0.1.9/unionai/_interceptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import logging
+import random
+import string
 from collections import namedtuple
 from collections.abc import Sequence
 from contextlib import suppress
 from typing import Any
 
 import grpc
 from flyteidl.service.admin_pb2_grpc import AdminServiceStub
 from flyteidl.service.dataproxy_pb2_grpc import DataProxyServiceStub
 from flyteidl.service.signal_pb2_grpc import SignalServiceStub
 from flytekit.clients.auth_helper import get_authenticated_channel
 from flytekit.clients.friendly import SynchronousFlyteClient
 from flytekit.configuration import PlatformConfig
 
+logger = logging.getLogger("unionai")
+
 
 class ConcreteClientCallDetails(
     namedtuple(
         "ConcreteClientCallDetails",
         (
             "method",
             "timeout",
@@ -39,34 +44,40 @@
             set_org(value, org=org)
 
     if isinstance(obj, Sequence) and not isinstance(obj, str):
         for value in obj:
             set_org(value, org=org)
 
 
+def generate_random_str(N):
+    return "".join(random.choice(string.ascii_letters) for _ in range(N))
+
+
 class OrgInterceptor(grpc.UnaryUnaryClientInterceptor):
     """Interceptor that adds org metadata into the grpc call."""
 
     def __init__(self, org: str):
         self.org = org
 
     def intercept_unary_unary(self, continuation, client_call_details, request):
+        request_id = f"u-{generate_random_str(20)}"
         old_metadata = client_call_details.metadata or []
-        new_metadata = old_metadata + [("x-user-active-org", self.org)]
+        new_metadata = old_metadata + [("x-user-active-org", self.org), ("x-request-id", request_id)]
         new_details = ConcreteClientCallDetails(
             method=client_call_details.method,
             timeout=client_call_details.timeout,
             metadata=new_metadata,
             credentials=client_call_details.credentials,
             wait_for_ready=client_call_details.wait_for_ready,
             compression=client_call_details.compression,
         )
 
         # Inject org into every IDL requests
         set_org(request, org=self.org)
+        logger.debug(f"request: {type(request)}, x-request-id: {request_id}, contents:\n{request}")
         return continuation(new_details, request)
 
 
 def update_client_with_interceptor(client: SynchronousFlyteClient, org: str) -> SynchronousFlyteClient:
     """Updates SynchronousFlyteClient inplace with an interceptor with org."""
     if org == "":
         # There is no org, so no need to intercept
```

### Comparing `unionai-0.1.8/unionai/artifacts/_artifact.py` & `unionai-0.1.9/unionai/artifacts/_artifact.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/artifacts/_card.py` & `unionai-0.1.9/unionai/artifacts/_card.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/artifacts/_triggers.py` & `unionai-0.1.9/unionai/artifacts/_triggers.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/cli/_create.py` & `unionai-0.1.9/unionai/cli/_create.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/cli/_delete.py` & `unionai-0.1.9/unionai/cli/_delete.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/cli/_get.py` & `unionai-0.1.9/unionai/cli/_get.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/cli/_update.py` & `unionai-0.1.9/unionai/cli/_update.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/configuration/_plugin.py` & `unionai-0.1.9/unionai/configuration/_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """All imports to unionai in this file should be in the function definition.
 
 This plugin is loaded by flytekit, so any imports to unionai can lead to circular imports.
 """
 
+import logging
 from typing import Optional
 
 import click
 from click import Group, Option
 from flytekit.remote import FlyteRemote
 
 
@@ -52,17 +53,30 @@
 
             # Only register image builder for serverless
             cfg_obj = _get_config_obj(value)
             if unionai._config._is_serverless_endpoint(cfg_obj.platform.endpoint):
                 _register_union_image_builder()
             return value
 
+        def _cli_verbose_callback(ctx, param, value):
+            """Configure logger based on value."""
+            if not value:
+                return value
+            logger = logging.getLogger("unionai")
+            handler = logging.StreamHandler()
+            logger.addHandler(handler)
+            logger.setLevel(logging.DEBUG)
+
+            return value
+
         for p in main.params:
             if p.name == "config":
                 p.callback = _cli_main_config_callback
+            if p.name == "verbose":
+                p.callback = _cli_verbose_callback
 
         # Configure org at the top level:
         def _set_org(ctx, param, value):
             _UNIONAI_CONFIG.org = value
 
         main.params.append(
             click.Option(
```

### Comparing `unionai-0.1.8/unionai/filesystems/_async_utils.py` & `unionai-0.1.9/unionai/filesystems/_async_utils.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/filesystems/_endpoint.py` & `unionai-0.1.9/unionai/filesystems/_endpoint.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/filesystems/_unionfs.py` & `unionai-0.1.9/unionai/filesystems/_unionfs.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/filesystems/_unionmetafs.py` & `unionai-0.1.9/unionai/filesystems/_unionmetafs.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2.py` & `unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2.pyi` & `unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/artifacts/artifacts_pb2_grpc.py` & `unionai-0.1.9/unionai/internal/artifacts/artifacts_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/common/list_pb2.py` & `unionai-0.1.9/unionai/internal/common/list_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/common/list_pb2.pyi` & `unionai-0.1.9/unionai/internal/common/list_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_definition_pb2.py` & `unionai-0.1.9/unionai/internal/identity/app_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_definition_pb2.pyi` & `unionai-0.1.9/unionai/internal/identity/app_definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_payload_pb2.py` & `unionai-0.1.9/unionai/internal/identity/app_payload_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_payload_pb2.pyi` & `unionai-0.1.9/unionai/internal/identity/app_payload_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_service_pb2.py` & `unionai-0.1.9/unionai/internal/identity/app_service_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/app_service_pb2_grpc.py` & `unionai-0.1.9/unionai/internal/identity/app_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/enums_pb2.py` & `unionai-0.1.9/unionai/internal/identity/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/identity/enums_pb2.pyi` & `unionai-0.1.9/unionai/internal/identity/enums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/definition_pb2.py` & `unionai-0.1.9/unionai/internal/objectstore/definition_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/definition_pb2.pyi` & `unionai-0.1.9/unionai/internal/objectstore/definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/metadata_service_pb2.py` & `unionai-0.1.9/unionai/internal/objectstore/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/metadata_service_pb2_grpc.py` & `unionai-0.1.9/unionai/internal/objectstore/metadata_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/objectstore_service_pb2.py` & `unionai-0.1.9/unionai/internal/objectstore/objectstore_service_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/objectstore_service_pb2_grpc.py` & `unionai-0.1.9/unionai/internal/objectstore/objectstore_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/payload_pb2.py` & `unionai-0.1.9/unionai/internal/objectstore/payload_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/objectstore/payload_pb2.pyi` & `unionai-0.1.9/unionai/internal/objectstore/payload_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/definition_pb2.py` & `unionai-0.1.9/unionai/internal/secret/definition_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/definition_pb2.pyi` & `unionai-0.1.9/unionai/internal/secret/definition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/payload_pb2.py` & `unionai-0.1.9/unionai/internal/secret/payload_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/payload_pb2.pyi` & `unionai-0.1.9/unionai/internal/secret/payload_pb2.pyi`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/secret_pb2.py` & `unionai-0.1.9/unionai/internal/secret/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/secret/secret_pb2_grpc.py` & `unionai-0.1.9/unionai/internal/secret/secret_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/internal/validate/validate/validate_pb2.py` & `unionai-0.1.9/unionai/internal/validate/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/remote/_remote.py` & `unionai-0.1.9/unionai/remote/_remote.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai/ucimage/_image_builder.py` & `unionai-0.1.9/unionai/ucimage/_image_builder.py`

 * *Files identical despite different names*

### Comparing `unionai-0.1.8/unionai.egg-info/PKG-INFO` & `unionai-0.1.9/unionai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unionai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Adds Union Cloud specific functionality to Flytekit
 Author-email: unionai <oss@union.ai>
 License: Source code in this repository is licensed under the Business Source
         License 1.1 (BSL) and the Apache License 2.0 (APL). A copy of each
         license can be found in the licenses directory. Source code in a
         given file is licensed under the BSL and the copyright belongs to
         Union Systems, Inc. unless otherwise noted at the beginning of the
```

### Comparing `unionai-0.1.8/unionai.egg-info/SOURCES.txt` & `unionai-0.1.9/unionai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

