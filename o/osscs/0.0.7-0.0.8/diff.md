# Comparing `tmp/osscs-0.0.7.tar.gz` & `tmp/osscs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osscs-0.0.7.tar", last modified: Sat Mar 30 17:51:37 2024, max compression
+gzip compressed data, was "osscs-0.0.8.tar", last modified: Thu Apr  4 04:49:08 2024, max compression
```

## Comparing `osscs-0.0.7.tar` & `osscs-0.0.8.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.517898 osscs-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-30 17:51:29.000000 osscs-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-30 17:51:37.517898 osscs-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-30 17:51:29.000000 osscs-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-30 17:51:29.000000 osscs-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 17:51:37.517898 osscs-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.505898 osscs-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.505898 osscs-0.0.7/src/osscs/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/backend/client/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/backend/client/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/client/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/client/common/base_message_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/client/message_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/backend/core/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/backend/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/common/base_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/common/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/common/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/have_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/socket_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/socket_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/core/socket_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/models/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/models/common/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/common/base_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/common/base_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/message_from_dict_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/server/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/server/common/base_message_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/server/message_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/address_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/address_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.513898 osscs-0.0.7/src/osscs/backend/storage/common/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/common/base_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/path_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/backend/storage/uuid_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.509898 osscs-0.0.7/src/osscs/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.517898 osscs-0.0.7/src/osscs/cryptography/core/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.517898 osscs-0.0.7/src/osscs/cryptography/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_key_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_key_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_rsa_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_signature_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/common/base_signature_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/cryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/encryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/key_hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/key_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/signature_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/core/signature_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.517898 osscs-0.0.7/src/osscs/cryptography/models/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-30 17:51:29.000000 osscs-0.0.7/src/osscs/cryptography/models/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:51:37.517898 osscs-0.0.7/src/osscs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-30 17:51:37.000000 osscs-0.0.7/src/osscs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-30 17:51:37.000000 osscs-0.0.7/src/osscs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 17:51:37.000000 osscs-0.0.7/src/osscs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-30 17:51:37.000000 osscs-0.0.7/src/osscs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 17:51:37.000000 osscs-0.0.7/src/osscs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 04:49:04.000000 osscs-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 04:49:08.481551 osscs-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 04:49:04.000000 osscs-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 04:49:04.000000 osscs-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:49:08.481551 osscs-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/osscs/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/client/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/common/base_message_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/client/message_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.473550 osscs-0.0.8/src/osscs/backend/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/common/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/have_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/core/socket_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/base_message_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/common/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/message_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/common/base_message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/server/message_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/address_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/address_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.477551 osscs-0.0.8/src/osscs/backend/storage/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/common/base_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/path_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/backend/storage/uuid_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.469550 osscs-0.0.8/src/osscs/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_key_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_key_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_rsa_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_signature_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/common/base_signature_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/cryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/key_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/key_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/signature_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/core/signature_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/cryptography/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/cryptography/models/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-04 04:49:04.000000 osscs-0.0.8/src/osscs/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:49:08.481551 osscs-0.0.8/src/osscs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 04:49:08.000000 osscs-0.0.8/src/osscs.egg-info/top_level.txt
```

### Comparing `osscs-0.0.7/LICENSE` & `osscs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/pyproject.toml` & `osscs-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "osscs"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="ImCocos", email="codimcocos@gmail.com" },
 ]
 description = "Open-source crypto-secure communication system"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
-  'cryptography>=42.0.3'
+  'cryptography>=42.0.3',
+  'pydantic>=2.6.4'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
```

### Comparing `osscs-0.0.7/src/osscs/backend/core/socket_listener.py` & `osscs-0.0.8/src/osscs/backend/core/socket_sender.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-import json
-from typing import Callable
-
-from osscs.backend.core.common import BaseListener
+from osscs.backend.core.common import BaseSender
 from osscs.backend.core.have_socket import HaveSocket
-from osscs.backend.core.socket_reader import SocketReader
-from osscs.backend.storage import IPv4Address, IPv6Address
 from osscs.backend.storage.common import BaseAddress
+from osscs.backend.storage import IPv4Address, IPv6Address
 
 
 TAccessedSocketAddress = IPv4Address | IPv6Address
 
 
-class SocketListener(BaseListener, HaveSocket):
+class SocketSender(HaveSocket, BaseSender):
+    '''
+    Реализация базового отправителя информации.
+    Работает с сокетами.
+    На данный момент работает только с IPv4-адресами.
+    '''
     def __init__(self) -> None:
         self.create_socket()
+    
+    def send(self, address: BaseAddress, message: bytes) -> None:
+        if not self.address_is_supported(address):
+            raise NotImplementedError
+        self._send(address, message)
 
-    def address_is_supported(self, address: BaseAddress) -> bool:
-        return isinstance(address, TAccessedSocketAddress)
-
-    def _bind(self, address: TAccessedSocketAddress) -> None:
+    def _send(self, address: TAccessedSocketAddress, msg: bytes) -> None:
         if isinstance(address, IPv4Address):
-            self.socket.bind((address.ip, address.port))
+            self.socket.sendto(msg, (address.ip, address.port))
+            return
         elif isinstance(address, IPv6Address):
             raise NotImplementedError
 
-    def listen_on(
-        self,
-        address: TAccessedSocketAddress,
-        on_message: Callable[[bytes, BaseAddress], None]
-    ) -> None:
-        self._bind(address)
-        socket_reader = SocketReader(self.socket)
-        try:
-            while True:
-                msg, peer_address = socket_reader.poll()
-
-                if not msg or not peer_address:
-                    continue
-
-                on_message(msg, peer_address)
-
-        except KeyboardInterrupt:
-            print('\nQuiting...')
-            self.close_socket()
+    def close(self) -> None:
+        self.close_socket()
+    
+    def address_is_supported(self, address: BaseAddress) -> bool:
+        return isinstance(address, TAccessedSocketAddress)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osscs-0.0.7/src/osscs/backend/core/socket_reader.py` & `osscs-0.0.8/src/osscs/backend/core/socket_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from osscs.backend.core.common import BaseReader
 from osscs.backend.storage import IPv4Address
 from osscs.backend.storage.common import BaseAddress
 
 
 class SocketReader(BaseReader):
+    '''
+    Реализация базового читателя информации.
+    Работает с сокетами.
+    '''
     def __init__(self, socket: socket.socket) -> None:
         self.socket = socket
         
     def poll(self) -> tuple[bytes, BaseAddress] | tuple[None, None]:
         while True:
             msg, peer_address = self.socket.recvfrom(2048)
             if len(msg) == 0:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osscs-0.0.7/src/osscs/backend/models/mode.py` & `osscs-0.0.8/src/osscs/backend/models/mode.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/backend/server/message_listener.py` & `osscs-0.0.8/src/osscs/backend/server/message_listener.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import json
 from typing import Callable
 
-from osscs.backend.models import MessageFromDictMapper
+from osscs.backend.models import Message
 from osscs.backend.core.common import BaseListener
 from osscs.backend.server.common import BaseMessageListener
 from osscs.backend.storage.common import BaseAddress
 
 
 class MessageListener(BaseMessageListener):
     def __init__(self, listener: BaseListener) -> None:
         self.listener = listener
     
-    def listen_on(self, address: BaseAddress, on_message: Callable[[MessageFromDictMapper, BaseAddress], None]) -> None:
+    def listen_on(self, address: BaseAddress, on_message: Callable[[Message, BaseAddress], None]) -> None:
         def wrapper(bmessage: bytes, address: BaseAddress) -> None:
+
             try:
-                dict_message = json.loads(bmessage)
-            except json.decoder.JSONDecodeError:
-                return
-            
-            try:
-                message = MessageFromDictMapper(dict_message)
-            except BaseException:
+                message = Message.model_validate_json(bmessage)
+            except BaseException as e:
+                print(e)
                 return
-            
+
             on_message(message, address)
 
         self.listener.listen_on(
             address,
             wrapper
         )
```

### Comparing `osscs-0.0.7/src/osscs/backend/storage/address_storage.py` & `osscs-0.0.8/src/osscs/backend/storage/address_storage.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/backend/storage/address_validator.py` & `osscs-0.0.8/src/osscs/backend/storage/address_validator.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/backend/storage/path_validator.py` & `osscs-0.0.8/src/osscs/backend/storage/path_validator.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/config.py` & `osscs-0.0.8/src/osscs/config.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/common/base_encryptor.py` & `osscs-0.0.8/src/osscs/cryptography/core/common/base_decryptor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from abc import ABC, abstractmethod
+from typing import Protocol
 
 from osscs.cryptography.core.common.base_key_loader import BaseRSAKeyLoader
-from osscs.cryptography.core.common.base_rsa_keys import BaseRSAPublicKey
+from osscs.cryptography.core.common.base_rsa_keys import BaseRSAPrivateKey, BaseRSAPublicKey
 
 
-class BaseEncryptor(ABC):
-    @abstractmethod
+class BaseDecryptor(Protocol):
     def __init__(
         self,
         key_loader: BaseRSAKeyLoader,
-        public_key: BaseRSAPublicKey
-    ) -> None:...
+        private_key: BaseRSAPrivateKey,
+        password: str
+    ) -> None:
+        raise NotImplementedError
     
-    @abstractmethod
-    def encrypt(self, string: str) -> bytes:...
-    
-    @abstractmethod
-    def get_10_symbols(self) -> str:...
+    def decrypt(self, data: bytes) -> str:
+        raise NotImplementedError
+
+    def public_key(self) -> BaseRSAPublicKey:
+        raise NotImplementedError
 
-    @abstractmethod
-    def get_bytes_public_key(self) -> bytes:...
+    def get_bytes_private_key(self) -> bytes:
+        raise NotImplementedError
```

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/cryptor.py` & `osscs-0.0.8/src/osscs/cryptography/core/cryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/decryptor.py` & `osscs-0.0.8/src/osscs/cryptography/core/decryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/encryptor.py` & `osscs-0.0.8/src/osscs/cryptography/core/encryptor.py`

 * *Files identical despite different names*

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/key_hasher.py` & `osscs-0.0.8/src/osscs/cryptography/core/key_hasher.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
     def string_hash_public_key(self, key: bytes | BaseRSAPublicKey) -> str:
         if isinstance(key, BaseRSAPublicKey):
             return base64.b64encode(hashlib.sha1(self.key_loader.get_bytes_public_key(key)).digest()).decode().replace('/', '')
         elif isinstance(key, bytes):
             return base64.b64encode(hashlib.sha1(key).digest()).decode().replace('/', '')
         else:
-            raise NotImplementedError
+            raise TypeError(f'Key must be bytes | BaseRSAPublicKey, not "{key.__class__.__name__}"!')
```

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/key_loader.py` & `osscs-0.0.8/src/osscs/cryptography/core/key_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import rsa
 
 from osscs.cryptography.core.common import BaseRSAPrivateKey, BaseRSAKeyLoader, BaseRSAPublicKey
 
 
 class KeyLoader(BaseRSAKeyLoader):
     def get_rsa_public_key_from_file(self, file_path: str) -> BaseRSAPublicKey | None:
         try:
@@ -39,21 +40,21 @@
                     format=serialization.PrivateFormat.PKCS8,
                     encryption_algorithm=serialization.BestAvailableEncryption(password.encode())
                 )
             )
 
     def get_rsa_public_key(self, public_key: bytes) -> BaseRSAPublicKey:
         key = serialization.load_pem_public_key(public_key)
-        if not isinstance(key, BaseRSAPublicKey):
+        if not isinstance(key, rsa.RSAPublicKey):
             raise ValueError(f'Wrong key type: {key.__class__.__name__}')
         return key
 
     def get_rsa_private_key(self, private_key: bytes, password: str) -> BaseRSAPrivateKey:
         key = serialization.load_pem_private_key(private_key, password.encode())
-        if not isinstance(key, BaseRSAPrivateKey):
+        if not isinstance(key, rsa.RSAPrivateKey):
             raise ValueError(f'Wrong key type: {key.__class__.__name__}')
         return key
 
     def get_bytes_public_key(self, public_key: BaseRSAPublicKey) -> bytes:
         return public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.PKCS1,
@@ -61,7 +62,10 @@
     
     def get_bytes_private_key(self, private_key: BaseRSAPrivateKey, password: str) -> bytes:
         return private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.PKCS8,
             encryption_algorithm=serialization.BestAvailableEncryption(password.encode())
         )
+    
+    def generate_private_key(self) -> BaseRSAPrivateKey:
+        return rsa.generate_private_key(65537, 2048)
```

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/signature_fabric.py` & `osscs-0.0.8/src/osscs/cryptography/core/signature_fabric.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         signature = self.decryptor.private_key.sign( # type: ignore
             signature_data,
             padding=self.signature_padding,
             algorithm=utils.Prehashed(chosen_hash)
         )
 
         return Signature(
-            self.encryptor.get_bytes_public_key(),
-            signature,
-            signature_data
+            public_key=self.encryptor.get_bytes_public_key(),
+            signature=signature,
+            signature_data=signature_data
         )
```

### Comparing `osscs-0.0.7/src/osscs/cryptography/core/signature_verifier.py` & `osscs-0.0.8/src/osscs/cryptography/core/signature_verifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from cryptography import exceptions
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import utils
 from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric import rsa
 
-from osscs.cryptography.core.common import BaseSignatureVerifier
-from osscs.cryptography.core.common.base_encryptor import BaseEncryptor
-from osscs.cryptography.core.common.base_rsa_keys import BaseRSAPublicKey
+from osscs.cryptography.core.common import BaseSignatureVerifier, BaseEncryptor, BaseRSAKeyLoader
 from osscs.cryptography.models.signature import Signature
 
 
 class SignatureVerifier(BaseSignatureVerifier):
-    def __init__(self, encryptor: BaseEncryptor) -> None:
+    def __init__(self, encryptor: BaseEncryptor, key_loader: BaseRSAKeyLoader) -> None:
         self.encryptor = encryptor
+        self.key_loader = key_loader
 
         self.signature_padding = padding.PSS(
             mgf=padding.MGF1(hashes.SHA256()),
             salt_length=padding.PSS.MAX_LENGTH
         )
 
     def __call__(self, signature: Signature) -> bool:
         try:
-            public_key = self.encryptor.key_loader.get_rsa_public_key(signature.public_key)
-            if not isinstance(public_key, BaseRSAPublicKey):
-                raise ValueError(f'Wrong key')
+            public_key = self.key_loader.get_rsa_public_key(signature.public_key)
+            if not isinstance(public_key, rsa.RSAPublicKey):
+                raise ValueError(f'Wrong key: {public_key.__class__.__name__}')
             public_key.verify(
                 signature.signature,
                 signature.signature_data,
                 padding=self.signature_padding,
                 algorithm=utils.Prehashed(hashes.SHA256())
             )
             return True
```

### Comparing `osscs-0.0.7/src/osscs.egg-info/SOURCES.txt` & `osscs-0.0.8/src/osscs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 src/osscs/backend/core/socket_sender.py
 src/osscs/backend/core/common/__init__.py
 src/osscs/backend/core/common/base_listener.py
 src/osscs/backend/core/common/base_reader.py
 src/osscs/backend/core/common/base_sender.py
 src/osscs/backend/models/__init__.py
 src/osscs/backend/models/message.py
-src/osscs/backend/models/message_from_dict_mapper.py
+src/osscs/backend/models/message_preparer.py
 src/osscs/backend/models/mode.py
 src/osscs/backend/models/user.py
 src/osscs/backend/models/common/__init__.py
-src/osscs/backend/models/common/base_message.py
+src/osscs/backend/models/common/base_message_preparer.py
 src/osscs/backend/models/common/base_user.py
 src/osscs/backend/server/__init__.py
 src/osscs/backend/server/message_listener.py
 src/osscs/backend/server/common/__init__.py
 src/osscs/backend/server/common/base_message_listener.py
 src/osscs/backend/storage/__init__.py
 src/osscs/backend/storage/address_storage.py
@@ -53,8 +53,9 @@
 src/osscs/cryptography/core/common/base_encryptor.py
 src/osscs/cryptography/core/common/base_key_hasher.py
 src/osscs/cryptography/core/common/base_key_loader.py
 src/osscs/cryptography/core/common/base_rsa_keys.py
 src/osscs/cryptography/core/common/base_signature_fabric.py
 src/osscs/cryptography/core/common/base_signature_verifier.py
 src/osscs/cryptography/models/__init__.py
-src/osscs/cryptography/models/signature.py
+src/osscs/cryptography/models/signature.py
+src/osscs/types/__init__.py
```

