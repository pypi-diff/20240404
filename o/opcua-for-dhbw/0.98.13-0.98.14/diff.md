# Comparing `tmp/opcua-for-dhbw-0.98.13.tar.gz` & `tmp/opcua-for-dhbw-0.98.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opcua-for-dhbw-0.98.13.tar", last modified: Thu Apr  4 15:09:16 2024, max compression
+gzip compressed data, was "opcua-for-dhbw-0.98.14.tar", last modified: Thu Apr  4 15:30:36 2024, max compression
```

## Comparing `opcua-for-dhbw-0.98.13.tar` & `opcua-for-dhbw-0.98.14.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.978799 opcua-for-dhbw-0.98.13/
--rw-rw-rw-   0        0        0     7816 2024-04-04 14:44:51.000000 opcua-for-dhbw-0.98.13/COPYING
--rw-rw-rw-   0        0        0     1170 2024-04-04 15:09:16.977780 opcua-for-dhbw-0.98.13/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2024-04-04 14:44:51.000000 opcua-for-dhbw-0.98.13/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.767662 opcua-for-dhbw-0.98.13/opcua/
--rw-rw-rw-   0        0        0      412 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.774671 opcua-for-dhbw-0.98.13/opcua/client/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/client/__init__.py
--rw-rw-rw-   0        0        0    27453 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/client/client.py
--rw-rw-rw-   0        0        0    29168 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/client/ua_client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.812307 opcua-for-dhbw-0.98.13/opcua/common/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/common/__init__.py
--rw-rw-rw-   0        0        0     3287 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/common/callback.py
--rw-rw-rw-   0        0        0    18343 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/connection.py
--rw-rw-rw-   0        0        0     3138 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/copy_node.py
--rw-rw-rw-   0        0        0    38094 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/event_objects.py
--rw-rw-rw-   0        0        0     8403 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/events.py
--rw-rw-rw-   0        0        0     5735 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/instantiate.py
--rw-rw-rw-   0        0        0    15929 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/manage_nodes.py
--rw-rw-rw-   0        0        0     2910 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/methods.py
--rw-rw-rw-   0        0        0    27183 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/node.py
--rw-rw-rw-   0        0        0     1493 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/shortcuts.py
--rw-rw-rw-   0        0        0    14670 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/structures.py
--rw-rw-rw-   0        0        0    17399 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/subscription.py
--rw-rw-rw-   0        0        0    13059 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/type_dictionary_buider.py
--rw-rw-rw-   0        0        0     9697 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/ua_utils.py
--rw-rw-rw-   0        0        0     5935 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/utils.py
--rw-rw-rw-   0        0        0    19079 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/xmlexporter.py
--rw-rw-rw-   0        0        0    18215 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/xmlimporter.py
--rw-rw-rw-   0        0        0    12362 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/common/xmlparser.py
--rw-rw-rw-   0        0        0      239 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/compat.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.818307 opcua-for-dhbw-0.98.13/opcua/crypto/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/crypto/__init__.py
--rw-rw-rw-   0        0        0    20997 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/crypto/security_policies.py
--rw-rw-rw-   0        0        0     6091 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/crypto/uacrypto.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.847307 opcua-for-dhbw-0.98.13/opcua/server/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/server/__init__.py
--rw-rw-rw-   0        0        0    31581 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/address_space.py
--rw-rw-rw-   0        0        0     4778 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/binary_server_asyncio.py
--rw-rw-rw-   0        0        0     4283 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/discovery_service.py
--rw-rw-rw-   0        0        0     4279 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/event_generator.py
--rw-rw-rw-   0        0        0    14317 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/history.py
--rw-rw-rw-   0        0        0    14612 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/history_sql.py
--rw-rw-rw-   0        0        0    18854 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/internal_server.py
--rw-rw-rw-   0        0        0    21989 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/internal_subscription.py
--rw-rw-rw-   0        0        0     5883 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/registration_service.py
--rw-rw-rw-   0        0        0    26309 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/server.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.887419 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/__init__.py
--rw-rw-rw-   0        0        0     2480 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space.py
--rw-rw-rw-   0        0        0   168721 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part10.py
--rw-rw-rw-   0        0        0   139557 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part11.py
--rw-rw-rw-   0        0        0   509385 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part12.py
--rw-rw-rw-   0        0        0    35252 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part13.py
--rw-rw-rw-   0        0        0  1622188 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part14.py
--rw-rw-rw-   0        0        0    38870 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part17.py
--rw-rw-rw-   0        0        0     7648 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part19.py
--rw-rw-rw-   0        0        0   191783 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part3.py
--rw-rw-rw-   0        0        0   825897 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part4.py
--rw-rw-rw-   0        0        0  2743543 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part5.py
--rw-rw-rw-   0        0        0    88585 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part8.py
--rw-rw-rw-   0        0        0   529118 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part9.py
--rw-rw-rw-   0        0        0     5076 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/subscription_service.py
--rw-rw-rw-   0        0        0    23960 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/uaprocessor.py
--rw-rw-rw-   0        0        0     2835 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/server/user_manager.py
--rw-rw-rw-   0        0        0    31273 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/opcua/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.911455 opcua-for-dhbw-0.98.13/opcua/ua/
--rw-rw-rw-   0        0        0      401 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/__init__.py
--rw-rw-rw-   0        0        0      731 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/ua/attribute_ids.py
--rw-rw-rw-   0        0        0  2276184 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/ua/object_ids.py
--rw-rw-rw-   0        0        0    39050 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/status_codes.py
--rw-rw-rw-   0        0        0    18687 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/ua_binary.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.917465 opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/
--rw-rw-rw-   0        0        0       44 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/__init__.py
--rw-rw-rw-   0        0        0    15885 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/_auto.py
--rw-rw-rw-   0        0        0     2526 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/_base.py
--rw-rw-rw-   0        0        0   385935 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/uaprotocol_auto.py
--rw-rw-rw-   0        0        0    11186 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/uaprotocol_hand.py
--rw-rw-rw-   0        0        0    32346 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.13/opcua/ua/uatypes.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.975781 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/
--rw-rw-rw-   0        0        0     1170 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3024 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      336 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 15:09:16.000000 opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      191 2024-04-04 15:09:16.981808 opcua-for-dhbw-0.98.13/setup.cfg
--rw-rw-rw-   0        0        0     2118 2024-04-04 15:07:49.000000 opcua-for-dhbw-0.98.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 15:09:16.973773 opcua-for-dhbw-0.98.13/tests/
--rw-rw-rw-   0        0        0      990 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.13/tests/tests.py
--rw-rw-rw-   0        0        0     6928 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_client.py
--rw-rw-rw-   0        0        0     1931 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_cmd_lines.py
--rw-rw-rw-   0        0        0    40281 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_common.py
--rw-rw-rw-   0        0        0     5952 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_crypto_connect.py
--rw-rw-rw-   0        0        0    19322 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_custom_structures.py
--rw-rw-rw-   0        0        0     4403 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_custom_structures_optional_fields.py
--rw-rw-rw-   0        0        0     1169 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_enum_struct.py
--rw-rw-rw-   0        0        0    12854 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_history.py
--rw-rw-rw-   0        0        0    30219 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_server.py
--rw-rw-rw-   0        0        0     2388 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_standard_address_space.py
--rw-rw-rw-   0        0        0    24873 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_subscriptions.py
--rw-rw-rw-   0        0        0     1108 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_uaerrors.py
--rw-rw-rw-   0        0        0    27219 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_unit.py
--rw-rw-rw-   0        0        0    17809 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.13/tests/tests_xml.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:36.098518 opcua-for-dhbw-0.98.14/
+-rw-rw-rw-   0        0        0     7816 2024-04-04 14:44:51.000000 opcua-for-dhbw-0.98.14/COPYING
+-rw-rw-rw-   0        0        0     1170 2024-04-04 15:30:36.098011 opcua-for-dhbw-0.98.14/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2024-04-04 14:44:51.000000 opcua-for-dhbw-0.98.14/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.871932 opcua-for-dhbw-0.98.14/opcua/
+-rw-rw-rw-   0        0        0      412 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.877136 opcua-for-dhbw-0.98.14/opcua/client/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/client/__init__.py
+-rw-rw-rw-   0        0        0    27453 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/client/client.py
+-rw-rw-rw-   0        0        0    29168 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/client/ua_client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.917408 opcua-for-dhbw-0.98.14/opcua/common/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/common/__init__.py
+-rw-rw-rw-   0        0        0     3287 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/common/callback.py
+-rw-rw-rw-   0        0        0    18343 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/connection.py
+-rw-rw-rw-   0        0        0     3138 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/copy_node.py
+-rw-rw-rw-   0        0        0    38094 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/event_objects.py
+-rw-rw-rw-   0        0        0     8403 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/events.py
+-rw-rw-rw-   0        0        0     5735 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/instantiate.py
+-rw-rw-rw-   0        0        0    15929 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/manage_nodes.py
+-rw-rw-rw-   0        0        0     2910 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/methods.py
+-rw-rw-rw-   0        0        0    27183 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/node.py
+-rw-rw-rw-   0        0        0     1493 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/shortcuts.py
+-rw-rw-rw-   0        0        0    14670 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/structures.py
+-rw-rw-rw-   0        0        0    17399 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/subscription.py
+-rw-rw-rw-   0        0        0    13059 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/type_dictionary_buider.py
+-rw-rw-rw-   0        0        0     9697 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/ua_utils.py
+-rw-rw-rw-   0        0        0     5935 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/utils.py
+-rw-rw-rw-   0        0        0    19079 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/xmlexporter.py
+-rw-rw-rw-   0        0        0    18215 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/xmlimporter.py
+-rw-rw-rw-   0        0        0    12362 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/common/xmlparser.py
+-rw-rw-rw-   0        0        0      239 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/compat.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.924752 opcua-for-dhbw-0.98.14/opcua/crypto/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/crypto/__init__.py
+-rw-rw-rw-   0        0        0    20997 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/crypto/security_policies.py
+-rw-rw-rw-   0        0        0     6091 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/crypto/uacrypto.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.953730 opcua-for-dhbw-0.98.14/opcua/server/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/server/__init__.py
+-rw-rw-rw-   0        0        0    31581 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/address_space.py
+-rw-rw-rw-   0        0        0     4778 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/binary_server_asyncio.py
+-rw-rw-rw-   0        0        0     4283 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/discovery_service.py
+-rw-rw-rw-   0        0        0     4279 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/event_generator.py
+-rw-rw-rw-   0        0        0    14317 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/history.py
+-rw-rw-rw-   0        0        0    14612 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/history_sql.py
+-rw-rw-rw-   0        0        0    18854 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/internal_server.py
+-rw-rw-rw-   0        0        0    21989 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/internal_subscription.py
+-rw-rw-rw-   0        0        0     5883 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/registration_service.py
+-rw-rw-rw-   0        0        0    26309 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/server.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:35.995990 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/
+-rw-rw-rw-   0        0        0        0 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/__init__.py
+-rw-rw-rw-   0        0        0     2480 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space.py
+-rw-rw-rw-   0        0        0   168721 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part10.py
+-rw-rw-rw-   0        0        0   139557 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part11.py
+-rw-rw-rw-   0        0        0   509385 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part12.py
+-rw-rw-rw-   0        0        0    35252 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part13.py
+-rw-rw-rw-   0        0        0  1622188 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part14.py
+-rw-rw-rw-   0        0        0    38870 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part17.py
+-rw-rw-rw-   0        0        0     7648 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part19.py
+-rw-rw-rw-   0        0        0   191783 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part3.py
+-rw-rw-rw-   0        0        0   825897 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part4.py
+-rw-rw-rw-   0        0        0  2743543 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part5.py
+-rw-rw-rw-   0        0        0    88585 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part8.py
+-rw-rw-rw-   0        0        0   529118 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part9.py
+-rw-rw-rw-   0        0        0     5076 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/subscription_service.py
+-rw-rw-rw-   0        0        0    23960 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/uaprocessor.py
+-rw-rw-rw-   0        0        0     2835 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/server/user_manager.py
+-rw-rw-rw-   0        0        0    31273 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/opcua/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:36.032275 opcua-for-dhbw-0.98.14/opcua/ua/
+-rw-rw-rw-   0        0        0      401 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/__init__.py
+-rw-rw-rw-   0        0        0      731 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/ua/attribute_ids.py
+-rw-rw-rw-   0        0        0  2276184 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/ua/object_ids.py
+-rw-rw-rw-   0        0        0    39050 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/status_codes.py
+-rw-rw-rw-   0        0        0    18687 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/ua_binary.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:36.039261 opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/
+-rw-rw-rw-   0        0        0       44 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/__init__.py
+-rw-rw-rw-   0        0        0    15885 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/_auto.py
+-rw-rw-rw-   0        0        0     2526 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/_base.py
+-rw-rw-rw-   0        0        0   385935 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/uaprotocol_auto.py
+-rw-rw-rw-   0        0        0    11186 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/uaprotocol_hand.py
+-rw-rw-rw-   0        0        0    32346 2024-04-04 15:06:32.000000 opcua-for-dhbw-0.98.14/opcua/ua/uatypes.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:36.060948 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/
+-rw-rw-rw-   0        0        0     1170 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3024 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      336 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 15:30:35.000000 opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      191 2024-04-04 15:30:36.102288 opcua-for-dhbw-0.98.14/setup.cfg
+-rw-rw-rw-   0        0        0     2118 2024-04-04 15:30:23.000000 opcua-for-dhbw-0.98.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:30:36.094992 opcua-for-dhbw-0.98.14/tests/
+-rw-rw-rw-   0        0        0      990 2024-04-04 14:44:52.000000 opcua-for-dhbw-0.98.14/tests/tests.py
+-rw-rw-rw-   0        0        0     6928 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_client.py
+-rw-rw-rw-   0        0        0     1931 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_cmd_lines.py
+-rw-rw-rw-   0        0        0    40281 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_common.py
+-rw-rw-rw-   0        0        0     5952 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_crypto_connect.py
+-rw-rw-rw-   0        0        0    19322 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_custom_structures.py
+-rw-rw-rw-   0        0        0     4403 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_custom_structures_optional_fields.py
+-rw-rw-rw-   0        0        0     1169 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_enum_struct.py
+-rw-rw-rw-   0        0        0    12854 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_history.py
+-rw-rw-rw-   0        0        0    30219 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_server.py
+-rw-rw-rw-   0        0        0     2388 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_standard_address_space.py
+-rw-rw-rw-   0        0        0    24873 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_subscriptions.py
+-rw-rw-rw-   0        0        0     1108 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_uaerrors.py
+-rw-rw-rw-   0        0        0    27219 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_unit.py
+-rw-rw-rw-   0        0        0    17809 2024-04-04 15:06:31.000000 opcua-for-dhbw-0.98.14/tests/tests_xml.py
```

### Comparing `opcua-for-dhbw-0.98.13/COPYING` & `opcua-for-dhbw-0.98.14/COPYING`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/PKG-INFO` & `opcua-for-dhbw-0.98.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opcua-for-dhbw
-Version: 0.98.13
+Version: 0.98.14
 Summary: Pure Python OPC-UA client and server library edited for internal purposes of DHBW Mosbach (ctrlX AUTOMATION - OPC UA Server)
 Home-page: http://freeopcua.github.io/
 Author: Olivier Roulet-Dubonnet (Edited by Adrian)
 Author-email: author@example.com
 License: GNU Lesser General Public License v3 or later
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opcua-for-dhbw-0.98.13/README.md` & `opcua-for-dhbw-0.98.14/README.md`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/client/client.py` & `opcua-for-dhbw-0.98.14/opcua/client/client.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/client/ua_client.py` & `opcua-for-dhbw-0.98.14/opcua/client/ua_client.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/callback.py` & `opcua-for-dhbw-0.98.14/opcua/common/callback.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/connection.py` & `opcua-for-dhbw-0.98.14/opcua/common/connection.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/copy_node.py` & `opcua-for-dhbw-0.98.14/opcua/common/copy_node.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/event_objects.py` & `opcua-for-dhbw-0.98.14/opcua/common/event_objects.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/events.py` & `opcua-for-dhbw-0.98.14/opcua/common/events.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/instantiate.py` & `opcua-for-dhbw-0.98.14/opcua/common/instantiate.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/manage_nodes.py` & `opcua-for-dhbw-0.98.14/opcua/common/manage_nodes.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/methods.py` & `opcua-for-dhbw-0.98.14/opcua/common/methods.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/node.py` & `opcua-for-dhbw-0.98.14/opcua/common/node.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/shortcuts.py` & `opcua-for-dhbw-0.98.14/opcua/common/shortcuts.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/structures.py` & `opcua-for-dhbw-0.98.14/opcua/common/structures.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/subscription.py` & `opcua-for-dhbw-0.98.14/opcua/common/subscription.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/type_dictionary_buider.py` & `opcua-for-dhbw-0.98.14/opcua/common/type_dictionary_buider.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/ua_utils.py` & `opcua-for-dhbw-0.98.14/opcua/common/ua_utils.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/utils.py` & `opcua-for-dhbw-0.98.14/opcua/common/utils.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/xmlexporter.py` & `opcua-for-dhbw-0.98.14/opcua/common/xmlexporter.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/xmlimporter.py` & `opcua-for-dhbw-0.98.14/opcua/common/xmlimporter.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/common/xmlparser.py` & `opcua-for-dhbw-0.98.14/opcua/common/xmlparser.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/crypto/security_policies.py` & `opcua-for-dhbw-0.98.14/opcua/crypto/security_policies.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/crypto/uacrypto.py` & `opcua-for-dhbw-0.98.14/opcua/crypto/uacrypto.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/address_space.py` & `opcua-for-dhbw-0.98.14/opcua/server/address_space.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/binary_server_asyncio.py` & `opcua-for-dhbw-0.98.14/opcua/server/binary_server_asyncio.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/discovery_service.py` & `opcua-for-dhbw-0.98.14/opcua/server/discovery_service.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/event_generator.py` & `opcua-for-dhbw-0.98.14/opcua/server/event_generator.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/history.py` & `opcua-for-dhbw-0.98.14/opcua/server/history.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/history_sql.py` & `opcua-for-dhbw-0.98.14/opcua/server/history_sql.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/internal_server.py` & `opcua-for-dhbw-0.98.14/opcua/server/internal_server.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/internal_subscription.py` & `opcua-for-dhbw-0.98.14/opcua/server/internal_subscription.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/registration_service.py` & `opcua-for-dhbw-0.98.14/opcua/server/registration_service.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/server.py` & `opcua-for-dhbw-0.98.14/opcua/server/server.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part10.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part10.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part11.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part11.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part12.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part12.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part13.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part13.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part14.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part14.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part17.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part17.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part19.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part19.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part3.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part3.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part4.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part4.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part5.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part5.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part8.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part8.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/standard_address_space/standard_address_space_part9.py` & `opcua-for-dhbw-0.98.14/opcua/server/standard_address_space/standard_address_space_part9.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/subscription_service.py` & `opcua-for-dhbw-0.98.14/opcua/server/subscription_service.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/uaprocessor.py` & `opcua-for-dhbw-0.98.14/opcua/server/uaprocessor.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/server/user_manager.py` & `opcua-for-dhbw-0.98.14/opcua/server/user_manager.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/tools.py` & `opcua-for-dhbw-0.98.14/opcua/tools.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/attribute_ids.py` & `opcua-for-dhbw-0.98.14/opcua/ua/attribute_ids.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/object_ids.py` & `opcua-for-dhbw-0.98.14/opcua/ua/object_ids.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/status_codes.py` & `opcua-for-dhbw-0.98.14/opcua/ua/status_codes.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/ua_binary.py` & `opcua-for-dhbw-0.98.14/opcua/ua/ua_binary.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/_auto.py` & `opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/_auto.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/uaerrors/_base.py` & `opcua-for-dhbw-0.98.14/opcua/ua/uaerrors/_base.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/uaprotocol_auto.py` & `opcua-for-dhbw-0.98.14/opcua/ua/uaprotocol_auto.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/uaprotocol_hand.py` & `opcua-for-dhbw-0.98.14/opcua/ua/uaprotocol_hand.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua/ua/uatypes.py` & `opcua-for-dhbw-0.98.14/opcua/ua/uatypes.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/PKG-INFO` & `opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opcua-for-dhbw
-Version: 0.98.13
+Version: 0.98.14
 Summary: Pure Python OPC-UA client and server library edited for internal purposes of DHBW Mosbach (ctrlX AUTOMATION - OPC UA Server)
 Home-page: http://freeopcua.github.io/
 Author: Olivier Roulet-Dubonnet (Edited by Adrian)
 Author-email: author@example.com
 License: GNU Lesser General Public License v3 or later
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opcua-for-dhbw-0.98.13/opcua_for_dhbw.egg-info/SOURCES.txt` & `opcua-for-dhbw-0.98.14/opcua_for_dhbw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/setup.py` & `opcua-for-dhbw-0.98.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "pytz",
     "enum34; python_version < '3'",
     "futures; python_version < '3'",
     "trollius; python_version < '3'",
 ]
 
 setup(name="opcua-for-dhbw",
-      version="0.98.13",
+      version="0.98.14",
       description="Pure Python OPC-UA client and server library edited for internal purposes of DHBW Mosbach (ctrlX AUTOMATION - OPC UA Server)",
       author="Olivier Roulet-Dubonnet (Edited by Adrian)",
       url='http://freeopcua.github.io/',
       author_email="author@example.com",
       packages=find_packages(),
       provides=["opcua_for_dhbw"],
       license="GNU Lesser General Public License v3 or later",
```

### Comparing `opcua-for-dhbw-0.98.13/tests/tests.py` & `opcua-for-dhbw-0.98.14/tests/tests.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_client.py` & `opcua-for-dhbw-0.98.14/tests/tests_client.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_cmd_lines.py` & `opcua-for-dhbw-0.98.14/tests/tests_cmd_lines.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_common.py` & `opcua-for-dhbw-0.98.14/tests/tests_common.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_crypto_connect.py` & `opcua-for-dhbw-0.98.14/tests/tests_crypto_connect.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_custom_structures.py` & `opcua-for-dhbw-0.98.14/tests/tests_custom_structures.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_custom_structures_optional_fields.py` & `opcua-for-dhbw-0.98.14/tests/tests_custom_structures_optional_fields.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_enum_struct.py` & `opcua-for-dhbw-0.98.14/tests/tests_enum_struct.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_history.py` & `opcua-for-dhbw-0.98.14/tests/tests_history.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_server.py` & `opcua-for-dhbw-0.98.14/tests/tests_server.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_standard_address_space.py` & `opcua-for-dhbw-0.98.14/tests/tests_standard_address_space.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_subscriptions.py` & `opcua-for-dhbw-0.98.14/tests/tests_subscriptions.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_uaerrors.py` & `opcua-for-dhbw-0.98.14/tests/tests_uaerrors.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_unit.py` & `opcua-for-dhbw-0.98.14/tests/tests_unit.py`

 * *Files identical despite different names*

### Comparing `opcua-for-dhbw-0.98.13/tests/tests_xml.py` & `opcua-for-dhbw-0.98.14/tests/tests_xml.py`

 * *Files identical despite different names*

