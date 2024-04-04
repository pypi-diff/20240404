# Comparing `tmp/osscs-0.0.8.tar.gz` & `tmp/osscs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osscs-0.0.8.tar", last modified: Thu Apr  4 04:49:08 2024, max compression
+gzip compressed data, was "osscs-0.0.9.tar", last modified: Thu Apr  4 18:56:59 2024, max compression
```

## Comparing `osscs-0.0.8.tar` & `osscs-0.0.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 04:49:04.000000 osscs-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 04:49:08.481551 osscs-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 04:49:04.000000 osscs-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 04:49:04.000000 osscs-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:49:08.481551 osscs-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/osscs/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/client/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/client/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/common/base_message_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/message_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/core/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/have_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/models/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/models/common/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/base_message_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/base_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/message_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/server/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/common/base_message_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/message_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/address_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/address_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/storage/common/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/common/base_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/path_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/uuid_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/osscs/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/core/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_key_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_key_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_rsa_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_signature_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_signature_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/cryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/key_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/key_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/signature_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/signature_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/models/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/models/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/types/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.797294 osscs-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 18:56:54.000000 osscs-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 18:56:59.797294 osscs-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 18:56:54.000000 osscs-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 18:56:54.000000 osscs-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:56:59.797294 osscs-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.781294 osscs-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.785294 osscs-0.0.9/src/osscs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.781294 osscs-0.0.9/src/osscs/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.785294 osscs-0.0.9/src/osscs/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.785294 osscs-0.0.9/src/osscs/backend/client/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/client/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/client/common/base_message_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/client/message_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.785294 osscs-0.0.9/src/osscs/backend/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/common/base_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/common/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/common/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/have_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/socket_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/socket_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/core/socket_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/common/base_message_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/common/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/message_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/server/common/base_message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/server/message_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.789294 osscs-0.0.9/src/osscs/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/address_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/address_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs/backend/storage/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/common/base_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/path_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/backend/storage/uuid_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.785294 osscs-0.0.9/src/osscs/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs/cryptography/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs/cryptography/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_key_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_key_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_rsa_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_signature_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/common/base_signature_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/cryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/key_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/key_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/signature_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/core/signature_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs/cryptography/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/cryptography/models/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-04 18:56:54.000000 osscs-0.0.9/src/osscs/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:56:59.793294 osscs-0.0.9/src/osscs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 18:56:59.000000 osscs-0.0.9/src/osscs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-04 18:56:59.000000 osscs-0.0.9/src/osscs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:56:59.000000 osscs-0.0.9/src/osscs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 18:56:59.000000 osscs-0.0.9/src/osscs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 18:56:59.000000 osscs-0.0.9/src/osscs.egg-info/top_level.txt
```

### Comparing `osscs-0.0.8/LICENSE` & `osscs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/PKG-INFO` & `osscs-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osscs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open-source crypto-secure communication system
 Author-email: ImCocos <codimcocos@gmail.com>
 Project-URL: Homepage, https://github.com/imcocos/ritatop
 Project-URL: Issues, https://github.com/imcocos/ritatop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osscs-0.0.8/README.md` & `osscs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/pyproject.toml` & `osscs-0.0.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "osscs"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="ImCocos", email="codimcocos@gmail.com" },
 ]
 description = "Open-source crypto-secure communication system"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `osscs-0.0.8/src/osscs/backend/client/common/base_message_sender.py` & `osscs-0.0.9/src/osscs/backend/client/common/base_message_sender.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/client/message_sender.py` & `osscs-0.0.9/src/osscs/backend/client/message_sender.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/common/base_listener.py` & `osscs-0.0.9/src/osscs/backend/core/common/base_listener.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/common/base_sender.py` & `osscs-0.0.9/src/osscs/backend/core/common/base_sender.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/have_socket.py` & `osscs-0.0.9/src/osscs/backend/core/have_socket.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/socket_listener.py` & `osscs-0.0.9/src/osscs/backend/core/socket_listener.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/socket_reader.py` & `osscs-0.0.9/src/osscs/backend/core/socket_reader.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/core/socket_sender.py` & `osscs-0.0.9/src/osscs/backend/core/socket_sender.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/models/common/base_message_preparer.py` & `osscs-0.0.9/src/osscs/backend/models/common/base_message_preparer.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/models/message.py` & `osscs-0.0.9/src/osscs/backend/models/message.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/models/message_preparer.py` & `osscs-0.0.9/src/osscs/backend/models/message_preparer.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/models/mode.py` & `osscs-0.0.9/src/osscs/backend/models/mode.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/server/message_listener.py` & `osscs-0.0.9/src/osscs/backend/server/message_listener.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/storage/address_storage.py` & `osscs-0.0.9/src/osscs/backend/storage/address_storage.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/storage/address_validator.py` & `osscs-0.0.9/src/osscs/backend/storage/address_validator.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/storage/key_storage.py` & `osscs-0.0.9/src/osscs/backend/storage/key_storage.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/backend/storage/path_validator.py` & `osscs-0.0.9/src/osscs/backend/storage/path_validator.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/config.py` & `osscs-0.0.9/src/osscs/config.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/common/base_decryptor.py` & `osscs-0.0.9/src/osscs/cryptography/core/common/base_decryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/common/base_encryptor.py` & `osscs-0.0.9/src/osscs/cryptography/core/common/base_encryptor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Protocol
 
-from osscs.cryptography.core.common.base_key_loader import BaseRSAKeyLoader
-from osscs.cryptography.core.common.base_rsa_keys import BaseRSAPublicKey
+from osscs.cryptography.core.common import BaseRSAKeyLoader, BaseRSAPublicKey
 
 
 class BaseEncryptor(Protocol):
     def __init__(
         self,
         key_loader: BaseRSAKeyLoader,
         public_key: BaseRSAPublicKey
```

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/common/base_key_loader.py` & `osscs-0.0.9/src/osscs/cryptography/core/common/base_key_loader.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/cryptor.py` & `osscs-0.0.9/src/osscs/cryptography/core/cryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/decryptor.py` & `osscs-0.0.9/src/osscs/cryptography/core/decryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/encryptor.py` & `osscs-0.0.9/src/osscs/cryptography/core/encryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/key_hasher.py` & `osscs-0.0.9/src/osscs/cryptography/core/key_hasher.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/key_loader.py` & `osscs-0.0.9/src/osscs/cryptography/core/key_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,21 @@
                     format=serialization.PrivateFormat.PKCS8,
                     encryption_algorithm=serialization.BestAvailableEncryption(password.encode())
                 )
             )
 
     def get_rsa_public_key(self, public_key: bytes) -> BaseRSAPublicKey:
         key = serialization.load_pem_public_key(public_key)
-        if not isinstance(key, rsa.RSAPublicKey):
+        if not isinstance(key, BaseRSAPublicKey):
             raise ValueError(f'Wrong key type: {key.__class__.__name__}')
         return key
 
     def get_rsa_private_key(self, private_key: bytes, password: str) -> BaseRSAPrivateKey:
         key = serialization.load_pem_private_key(private_key, password.encode())
-        if not isinstance(key, rsa.RSAPrivateKey):
+        if not isinstance(key, BaseRSAPrivateKey):
             raise ValueError(f'Wrong key type: {key.__class__.__name__}')
         return key
 
     def get_bytes_public_key(self, public_key: BaseRSAPublicKey) -> bytes:
         return public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.PKCS1,
```

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/signature_fabric.py` & `osscs-0.0.9/src/osscs/cryptography/core/signature_fabric.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/cryptography/core/signature_verifier.py` & `osscs-0.0.9/src/osscs/cryptography/core/signature_verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cryptography import exceptions
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import utils
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.asymmetric import rsa
 
-from osscs.cryptography.core.common import BaseSignatureVerifier, BaseEncryptor, BaseRSAKeyLoader
+from osscs.cryptography.core.common import BaseSignatureVerifier, BaseEncryptor, BaseRSAKeyLoader, BaseRSAPublicKey
 from osscs.cryptography.models.signature import Signature
 
 
 class SignatureVerifier(BaseSignatureVerifier):
     def __init__(self, encryptor: BaseEncryptor, key_loader: BaseRSAKeyLoader) -> None:
         self.encryptor = encryptor
         self.key_loader = key_loader
@@ -17,15 +17,15 @@
             mgf=padding.MGF1(hashes.SHA256()),
             salt_length=padding.PSS.MAX_LENGTH
         )
 
     def __call__(self, signature: Signature) -> bool:
         try:
             public_key = self.key_loader.get_rsa_public_key(signature.public_key)
-            if not isinstance(public_key, rsa.RSAPublicKey):
+            if not isinstance(public_key, BaseRSAPublicKey):
                 raise ValueError(f'Wrong key: {public_key.__class__.__name__}')
             public_key.verify(
                 signature.signature,
                 signature.signature_data,
                 padding=self.signature_padding,
                 algorithm=utils.Prehashed(hashes.SHA256())
             )
```

### Comparing `osscs-0.0.8/src/osscs/cryptography/models/signature.py` & `osscs-0.0.9/src/osscs/cryptography/models/signature.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs/types/__init__.py` & `osscs-0.0.9/src/osscs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.8/src/osscs.egg-info/PKG-INFO` & `osscs-0.0.9/src/osscs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osscs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Open-source crypto-secure communication system
 Author-email: ImCocos <codimcocos@gmail.com>
 Project-URL: Homepage, https://github.com/imcocos/ritatop
 Project-URL: Issues, https://github.com/imcocos/ritatop/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osscs-0.0.8/src/osscs.egg-info/SOURCES.txt` & `osscs-0.0.9/src/osscs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

