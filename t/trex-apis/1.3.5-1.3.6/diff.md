# Comparing `tmp/trex-apis-1.3.5.tar.gz` & `tmp/trex-apis-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-apis-1.3.5.tar", last modified: Fri Mar 15 03:28:20 2024, max compression
+gzip compressed data, was "trex-apis-1.3.6.tar", last modified: Thu Apr  4 11:19:36 2024, max compression
```

## Comparing `trex-apis-1.3.5.tar` & `trex-apis-1.3.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2024-03-15 03:28:20.000000 trex-apis-1.3.5/PKG-INFO
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1628 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/top_level.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.3.5/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2024-03-15 03:28:08.000000 trex-apis-1.3.5/setup.py
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-03-15 03:28:20.000000 trex-apis-1.3.5/setup.cfg
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.3.5/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7539 2023-12-13 05:36:24.000000 trex-apis-1.3.5/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.3.5/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.3.5/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.3.5/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.3.5/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.3.5/trexapi/decorators/api_decorators.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1156 2024-01-03 02:31:28.000000 trex-apis-1.3.5/trexapi/conf.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.3.5/trexapi/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)     9242 2024-03-14 09:07:57.000000 trex-apis-1.3.5/trexapi/utils/redemption_catalogue_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)    79248 2024-01-29 13:58:07.000000 trex-apis-1.3.5/trexapi/utils/reward_transaction_helper.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.3.5/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2983 2024-01-03 03:38:30.000000 trex-apis-1.3.5/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.3.5/trexapi/utils/push_notification_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.3.5/trexapi/libs/flask_auth_wrapper.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.3.5/trexapi/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-03-15 03:28:20.000000 trex-apis-1.3.5/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)    82820 2024-02-29 15:51:55.000000 trex-apis-1.3.5/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-01-25 03:26:42.000000 trex-apis-1.3.5/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.3.5/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    16728 2024-01-19 03:44:19.000000 trex-apis-1.3.5/trexapi/controllers/voucher_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.3.5/trexapi/controllers/rating_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27474 2024-01-29 10:13:52.000000 trex-apis-1.3.5/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.3.5/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22414 2024-02-07 06:33:19.000000 trex-apis-1.3.5/trexapi/controllers/merchant_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.3.5/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.3.5/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7436 2024-01-30 09:36:58.000000 trex-apis-1.3.5/trexapi/controllers/message_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.3.5/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.3.5/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7080 2023-12-04 14:21:25.000000 trex-apis-1.3.5/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10501 2024-02-05 02:35:34.000000 trex-apis-1.3.5/trexapi/controllers/redemption_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14912 2024-01-26 08:21:50.000000 trex-apis-1.3.5/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.3.5/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    44555 2023-12-13 09:05:54.000000 trex-apis-1.3.5/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.3.5/trexapi/controllers/prepaid_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    14268 2024-02-05 07:27:46.000000 trex-apis-1.3.5/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.3.5/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.3.5/trexapi/controllers/user_reward_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.933993 trex-apis-1.3.6/
+-rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-04 11:19:36.933871 trex-apis-1.3.6/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.3.6/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-04 11:19:36.934613 trex-apis-1.3.6/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2024-04-04 11:19:22.000000 trex-apis-1.3.6/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.933346 trex-apis-1.3.6/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      444 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1628 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2024-04-04 11:19:36.000000 trex-apis-1.3.6/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.897688 trex-apis-1.3.6/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.3.6/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1269 2024-04-03 14:24:11.000000 trex-apis-1.3.6/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.920644 trex-apis-1.3.6/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.3.6/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4523 2023-05-23 05:00:09.000000 trex-apis-1.3.6/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7080 2023-12-04 14:21:25.000000 trex-apis-1.3.6/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    44555 2023-12-13 09:05:54.000000 trex-apis-1.3.6/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.3.6/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.3.6/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14912 2024-01-26 08:21:50.000000 trex-apis-1.3.6/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14268 2024-02-05 07:27:46.000000 trex-apis-1.3.6/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22414 2024-02-07 06:33:19.000000 trex-apis-1.3.6/trexapi/controllers/merchant_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7436 2024-01-30 09:36:58.000000 trex-apis-1.3.6/trexapi/controllers/message_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11609 2024-01-30 15:20:28.000000 trex-apis-1.3.6/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.3.6/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    24944 2023-05-23 09:32:47.000000 trex-apis-1.3.6/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8448 2024-02-01 01:40:55.000000 trex-apis-1.3.6/trexapi/controllers/prepaid_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5450 2024-01-24 14:48:05.000000 trex-apis-1.3.6/trexapi/controllers/rating_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    10501 2024-02-05 02:35:34.000000 trex-apis-1.3.6/trexapi/controllers/redemption_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27474 2024-01-29 10:13:52.000000 trex-apis-1.3.6/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13578 2024-01-25 03:26:42.000000 trex-apis-1.3.6/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.3.6/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    84469 2024-04-04 07:59:04.000000 trex-apis-1.3.6/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2996 2024-01-19 04:06:09.000000 trex-apis-1.3.6/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    16728 2024-01-19 03:44:19.000000 trex-apis-1.3.6/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.922490 trex-apis-1.3.6/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.3.6/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11971 2024-03-01 01:12:37.000000 trex-apis-1.3.6/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.925890 trex-apis-1.3.6/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.3.6/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7539 2023-12-13 05:36:24.000000 trex-apis-1.3.6/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.3.6/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.3.6/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4548 2023-11-22 08:18:38.000000 trex-apis-1.3.6/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.927009 trex-apis-1.3.6/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.3.6/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.3.6/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-04 11:19:36.931432 trex-apis-1.3.6/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.3.6/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2983 2024-01-03 03:38:30.000000 trex-apis-1.3.6/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      501 2024-01-30 09:47:06.000000 trex-apis-1.3.6/trexapi/utils/push_notification_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9242 2024-03-14 09:07:57.000000 trex-apis-1.3.6/trexapi/utils/redemption_catalogue_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    79248 2024-01-29 13:58:07.000000 trex-apis-1.3.6/trexapi/utils/reward_transaction_helper.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `trex-apis-1.3.5/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.3.6/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/setup.py` & `trex-apis-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.3.5',
+     version='1.3.6',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.3.5/trexapi/forms/sales_api_forms.py` & `trex-apis-1.3.6/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/forms/customer_api_forms.py` & `trex-apis-1.3.6/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/forms/reward_api_forms.py` & `trex-apis-1.3.6/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/forms/user_api_forms.py` & `trex-apis-1.3.6/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/decorators/api_decorators.py` & `trex-apis-1.3.6/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/utils/redemption_catalogue_helper.py` & `trex-apis-1.3.6/trexapi/utils/redemption_catalogue_helper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.3.6/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/utils/api_helpers.py` & `trex-apis-1.3.6/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.3.6/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/user_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/user_api_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from flask import Blueprint, request
 import logging
 from trexlib.utils.log_util import get_tracelog
 from trexmodel.utils.model.model_util import create_db_client
 from datetime import datetime, timedelta
 from trexlib.utils.string_util import is_not_empty, random_number, random_string,\
-    is_empty
+    is_empty, boolify
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from werkzeug.datastructures import ImmutableMultiDict
 from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm,\
     OutletReviewsForm
-from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL, MOBILE_APP_NAME
+from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL, MOBILE_APP_NAME,\
+    USE_VERIFICATION_REQUEST_ID
 from trexmail.email_helper import trigger_send_email
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher,\
     CustomerPointReward, CustomerEntitledTierRewardSummary
 from trexapi.utils.api_helpers import generate_user_auth_token
 from trexapi.decorators.api_decorators import user_auth_token_required,\
@@ -1148,15 +1149,19 @@
             reference_code = request.headers.get('x-reference-code')
             logger.debug('reference_code from header=%s', reference_code)
             logger.debug('reference_code from database=%s', user_acct.reference_code)
             
             if reference_code == user_acct.reference_code:
                 email_vc_expiry_datetime    = _generate_email_expiry_datetime()
                 email_vc                    = random_number(6)
-                email_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                
+                if USE_VERIFICATION_REQUEST_ID:
+                    email_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                else:
+                    email_vc_prefix             = ''
                 
                 send_email_verification_code_email(email, email_vc, email_vc_prefix)
                 
                 return create_rest_message(status_code=StatusCode.OK, 
                                        #email_vc_expiry_datetime          = str(email_vc_expiry_datetime),
                                        expiry_datetime      = email_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                        prefix               = email_vc_prefix,
@@ -1171,17 +1176,19 @@
 
 def _generate_email_expiry_datetime():
     return datetime.utcnow() + timedelta(minutes=int(os.environ.get('EMAIL_EXPIRY_LENGTH_IN_MINUTE')))
     
 @user_api_bp.route('/reset-mobile-phone-vc', methods=['PUT'])
 @user_auth_token_required
 def reset_mobile_phone_verification_code(reference_code):
-    mobile_phone = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
+    mobile_phone    = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
+    send_method     = request.args.get('send_method') or request.form.get('send_method') or request.json.get('send_method')
 
     logger.debug('mobile_phone=%s', mobile_phone)
+    logger.debug('send_method=%s', send_method)
     logger.debug('reference_code=%s', reference_code)
     
     if is_not_empty(mobile_phone):
         db_client                           = create_db_client(caller_info="reset_mobile_phone_verification_code")
         user_acct                           = None
         
         with db_client.context():
@@ -1194,17 +1201,21 @@
                 #logger.debug('reset_mobile_phone_verification_code: found user account by mobile_phone=%s', mobile_phone)    
                 #is_mobile_phone_verified           = user_acct.is_mobile_phone_verified
                 
                 with db_client.context():
                     user_by_mobile_phone.reset_mobile_phone_vc()
                     
                 logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', user_by_mobile_phone.mobile_phone_vc_expiry_datetime)
-                logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_by_mobile_phone.mobile_phone_vc)   
+                logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_by_mobile_phone.mobile_phone_vc)
+                logger.debug('reset_mobile_phone_verification_code: USE_VERIFICATION_REQUEST_ID=%s', USE_VERIFICATION_REQUEST_ID)   
                 
-                mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                if boolify(USE_VERIFICATION_REQUEST_ID):
+                    mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                else:
+                    mobile_phone_vc_prefix = ''
                 
                 send_mobile_phone_verification_code_sms(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix)
                 
                 return create_rest_message(status_code=StatusCode.OK, 
                                            expiry_datetime      = user_by_mobile_phone.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                            code                 = user_by_mobile_phone.mobile_phone_vc,
                                            prefix               = mobile_phone_vc_prefix,
@@ -1215,18 +1226,22 @@
             with db_client.context():
                 user_acct    = User.get_by_reference_code(reference_code)
             
             if user_acct is not None:
                 with db_client.context():
                     user_acct.reset_mobile_phone_vc()
                     
-                mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                if boolify(USE_VERIFICATION_REQUEST_ID):
+                    mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+                else:
+                    mobile_phone_vc_prefix = ''
                 
                 logger.debug('reset_mobile_phone_verification_code: mobile_phone_vc_expiry_datetime=%s', user_acct.mobile_phone_vc_expiry_datetime)
                 logger.debug('reset_mobile_phone_verification_code: verification code=%s', user_acct.mobile_phone_vc)    
+                logger.debug('reset_mobile_phone_verification_code: USE_VERIFICATION_REQUEST_ID=%s', USE_VERIFICATION_REQUEST_ID)
                 
                 send_mobile_phone_verification_code_sms(mobile_phone, user_acct.mobile_phone_vc, mobile_phone_vc_prefix)
                 
                 return create_rest_message(status_code=StatusCode.OK, 
                                            expiry_datetime      = user_acct.mobile_phone_vc_expiry_datetime.strftime('%d-%m-%Y %H:%M:%S'),
                                            code                 = user_acct.mobile_phone_vc,
                                            prefix               = mobile_phone_vc_prefix,
@@ -1346,18 +1361,20 @@
     else:
         logger.warn('reset_password_post: email is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST) 
     
 @user_api_bp.route('/request-reset-password-via-mobile-phone', methods=['POST'])
 def request_reset_password_via_mobile_phone_post():
     mobile_phone = request.args.get('mobile_phone') or request.form.get('mobile_phone') or request.json.get('mobile_phone')
+    send_method = request.args.get('send_method') or request.form.get('send_method') or request.json.get('send_method')
     
     logger.debug('request_reset_password_via_mobile_phone_post: going to reset mobile_phone verification code by mobile phone=%s', mobile_phone)
 
     logger.debug('mobile_phone=%s', mobile_phone)
+    logger.debug('send_method=%s', send_method)
     
     if is_not_empty(mobile_phone):
         db_client                           = create_db_client(caller_info="request_reset_password_via_mobile_phone_post")
         
         with db_client.context():
             user_by_mobile_phone    = User.get_by_mobile_phone(mobile_phone)
         
@@ -1368,15 +1385,18 @@
                 user_by_mobile_phone.reset_mobile_phone_vc()
                 
                 
                 
             logger.debug('request_reset_password_via_mobile_phone_post debug: mobile_phone_vc_expiry_datetime=%s', user_by_mobile_phone.mobile_phone_vc_expiry_datetime)
             logger.debug('request_reset_password_via_mobile_phone_post debug: verification code=%s', user_by_mobile_phone.mobile_phone_vc)   
             
-            mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+            if boolify(USE_VERIFICATION_REQUEST_ID):
+                mobile_phone_vc_prefix             = random_string(4, is_human_mistake_safe=True)
+            else:
+                mobile_phone_vc_prefix = ''
             
             send_mobile_phone_verification_code_sms(mobile_phone, user_by_mobile_phone.mobile_phone_vc, mobile_phone_vc_prefix)
             
             with db_client.context():
                 reset_password_token = '%s-%s' % (mobile_phone_vc_prefix, user_by_mobile_phone.mobile_phone_vc)
                 logger.debug('request_reset_password_via_mobile_phone_post debug: reset_password_token=%s', reset_password_token)
                 user_by_mobile_phone.set_reset_password_token(reset_password_token)
@@ -1455,35 +1475,40 @@
             logger.info('Invalid voucher redeem code')
             return create_rest_message('Invalid voucher redeem code', status_code=StatusCode.BAD_REQUEST)
     else:
         logger.info('Missing voucher redeem code')
         return create_rest_message('Missing voucher redeem code', status_code=StatusCode.BAD_REQUEST)
 
 def send_email_verification_code_email(email, verification_code, request_id):
+    
+    final_verification_code = verification_code
+    if is_not_empty(request_id):
+        final_verification_code = '%s-%s' % (request_id, verification_code)
+        
+    
     message = '''
                 Dear,
                 
                 Please enter below code to verify your email for {mobile_app_name}.
                 
                 
-                {request_id}-{verification_code}
+                {verification_code}
                 
                 
                 The code will be expired after {email_expiry_in_minute} minutes.
                 
                 Cheers,
                 {application_name} Team
                 
                 
                 ***Please do not reply to this email. This is an auto-generated email.***
     
-            '''.format(email=email, verification_code=verification_code, 
+            '''.format(email=email, verification_code=final_verification_code, 
                        application_name=APPLICATION_NAME,
                        mobile_app_name=MOBILE_APP_NAME,
-                       request_id = request_id, 
                        email_expiry_in_minute=os.environ.get('EMAIL_EXPIRY_LENGTH_IN_MINUTE'))
     
     subject      = 'Email Verification from {mobile_app_name}'.format(mobile_app_name=MOBILE_APP_NAME)
     
     logger.info('DEPLOYMENT_MODE=%s', DEPLOYMENT_MODE)
     
     logger.info(message)
@@ -1491,17 +1516,21 @@
     if DEPLOYMENT_MODE==PRODUCTION_MODE:
         trigger_send_email(recipient_address = email, subject=subject, message=message)
     else:
         logger.debug('not send email for development or local mode')
         
         
 def send_mobile_phone_verification_code_sms(mobile_phone, verification_code, request_id):
-    message = '{mobile_app_name} {request_id}-{verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
+    if is_not_empty(request_id):
+        message = '{mobile_app_name} {request_id}-{verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
                        request_id = request_id, 
                        expiry_in_minute=os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE'))
+    else:
+        message = '{mobile_app_name} {verification_code} is your Verification Code. It will be expired after {expiry_in_minute} minutes'.format(mobile_app_name=MOBILE_APP_NAME, verification_code=verification_code, 
+                       expiry_in_minute=os.environ.get('MOBILE_PHONE_EXPIRY_LENGTH_IN_MINUTE'))
     
     logger.info('DEPLOYMENT_MODE=%s', DEPLOYMENT_MODE)
     
     logger.info('sms message: %s', message)
     
     if DEPLOYMENT_MODE in (PRODUCTION_MODE, DEMO_MODE):
         logger.info('Going to send sms to %s', mobile_phone)
```

### Comparing `trex-apis-1.3.5/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/rating_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/rating_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/merchant_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/merchant_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/message_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/message_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/app_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/redemption_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/redemption_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/prepaid_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/prepaid_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.3.5/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.3.6/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

