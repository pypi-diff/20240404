# Comparing `tmp/lamindb_setup-0.68.4.tar.gz` & `tmp/lamindb_setup-0.68.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.68.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.68.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.68.4.tar` & `lamindb_setup-0.68.5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     8290 2024-03-25 10:01:42.201467 lamindb_setup-0.68.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 12:04:01.937708 lamindb_setup-0.68.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 12:04:01.937784 lamindb_setup-0.68.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-02-29 12:04:01.937868 lamindb_setup-0.68.4/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 12:04:01.937945 lamindb_setup-0.68.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 12:04:01.938089 lamindb_setup-0.68.4/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 12:04:01.938164 lamindb_setup-0.68.4/README.md
--rw-r--r--   0        0        0    94332 2024-04-02 10:03:30.862359 lamindb_setup-0.68.4/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 19:17:51.102161 lamindb_setup-0.68.4/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 19:17:51.102263 lamindb_setup-0.68.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 19:17:51.102405 lamindb_setup-0.68.4/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 19:17:51.102702 lamindb_setup-0.68.4/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     2450 2024-03-18 09:44:23.350309 lamindb_setup-0.68.4/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     1913 2024-03-18 09:44:23.350808 lamindb_setup-0.68.4/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 19:17:51.103066 lamindb_setup-0.68.4/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 19:17:51.103305 lamindb_setup-0.68.4/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 19:17:51.103480 lamindb_setup-0.68.4/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-25 10:01:42.202871 lamindb_setup-0.68.4/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-19 12:58:36.468528 lamindb_setup-0.68.4/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 19:17:51.103712 lamindb_setup-0.68.4/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-11 10:42:56.000471 lamindb_setup-0.68.4/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 19:17:51.104281 lamindb_setup-0.68.4/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 19:17:51.104386 lamindb_setup-0.68.4/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-25 10:01:42.203244 lamindb_setup-0.68.4/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 19:17:51.104771 lamindb_setup-0.68.4/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 12:04:01.938771 lamindb_setup-0.68.4/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-25 10:01:42.203809 lamindb_setup-0.68.4/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 12:04:01.940681 lamindb_setup-0.68.4/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-02 10:07:21.849290 lamindb_setup-0.68.4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-07 19:17:51.105223 lamindb_setup-0.68.4/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 12:04:01.940876 lamindb_setup-0.68.4/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 12:04:01.940945 lamindb_setup-0.68.4/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:18.119868 lamindb_setup-0.68.4/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:58:52.546246 lamindb_setup-0.68.4/lamindb_setup/_close.py
--rw-r--r--   0        0        0    10793 2024-03-31 10:37:31.609599 lamindb_setup-0.68.4/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-25 10:01:42.204138 lamindb_setup-0.68.4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:58:52.546552 lamindb_setup-0.68.4/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2052 2024-03-11 10:42:56.001304 lamindb_setup-0.68.4/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1788 2024-02-29 12:04:01.941670 lamindb_setup-0.68.4/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11400 2024-03-18 09:44:23.352303 lamindb_setup-0.68.4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7356 2024-03-08 11:38:18.122077 lamindb_setup-0.68.4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:18.122391 lamindb_setup-0.68.4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:18.122834 lamindb_setup-0.68.4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-08 11:38:18.123112 lamindb_setup-0.68.4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 12:04:01.943026 lamindb_setup-0.68.4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      490 2024-03-05 13:11:55.176273 lamindb_setup-0.68.4/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     2403 2024-03-05 13:11:55.176381 lamindb_setup-0.68.4/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 13:11:55.176469 lamindb_setup-0.68.4/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 13:11:55.176553 lamindb_setup-0.68.4/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5215 2024-03-18 09:44:23.353370 lamindb_setup-0.68.4/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    11678 2024-03-25 10:01:42.204862 lamindb_setup-0.68.4/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-30 00:19:04.886366 lamindb_setup-0.68.4/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 13:11:55.177328 lamindb_setup-0.68.4/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-07 19:17:51.107799 lamindb_setup-0.68.4/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11565 2024-03-18 09:44:23.355474 lamindb_setup-0.68.4/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-18 09:44:23.355731 lamindb_setup-0.68.4/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-19 12:58:36.469141 lamindb_setup-0.68.4/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    11630 2024-03-25 10:01:42.206363 lamindb_setup-0.68.4/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-18 09:44:23.356020 lamindb_setup-0.68.4/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 19:17:51.107921 lamindb_setup-0.68.4/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 13:11:55.178221 lamindb_setup-0.68.4/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-25 10:01:42.207152 lamindb_setup-0.68.4/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     7291 2024-03-05 13:11:55.178538 lamindb_setup-0.68.4/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:18.123347 lamindb_setup-0.68.4/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-13 12:19:51.326372 lamindb_setup-0.68.4/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      308 2024-03-05 13:11:55.178881 lamindb_setup-0.68.4/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    22778 2024-04-02 09:56:45.661778 lamindb_setup-0.68.4/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4154 2024-03-28 07:58:04.166969 lamindb_setup-0.68.4/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-25 10:01:42.208566 lamindb_setup-0.68.4/pyproject.toml
--rw-r--r--   0        0        0     5492 2024-03-30 00:19:04.887726 lamindb_setup-0.68.4/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 19:17:51.108726 lamindb_setup-0.68.4/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 19:17:51.108857 lamindb_setup-0.68.4/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 19:17:51.108930 lamindb_setup-0.68.4/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 19:17:51.109001 lamindb_setup-0.68.4/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 19:17:51.109074 lamindb_setup-0.68.4/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0     2784 2024-03-25 10:01:42.208907 lamindb_setup-0.68.4/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11280 2024-03-30 00:19:04.888386 lamindb_setup-0.68.4/tests/hub-local/test_all.py
--rw-r--r--   0        0        0     1361 2024-03-25 10:01:42.209150 lamindb_setup-0.68.4/tests/hub-local/test_check_s3_storage_empty.py
--rw-r--r--   0        0        0     1149 2024-03-25 10:01:42.209500 lamindb_setup-0.68.4/tests/hub-local/test_hosted_instance_deletion_gate.py
--rw-r--r--   0        0        0      452 2024-03-07 19:17:51.109676 lamindb_setup-0.68.4/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 19:17:51.109750 lamindb_setup-0.68.4/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      285 2024-03-07 19:17:51.110002 lamindb_setup-0.68.4/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1438 2024-03-07 19:17:51.110099 lamindb_setup-0.68.4/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 19:17:51.110379 lamindb_setup-0.68.4/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-13 12:19:51.328202 lamindb_setup-0.68.4/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 19:17:51.110769 lamindb_setup-0.68.4/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-30 00:19:04.888658 lamindb_setup-0.68.4/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-28 07:58:04.167485 lamindb_setup-0.68.4/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.68.4/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-03-29 13:22:22.689587 lamindb_setup-0.68.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.68.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.68.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-02-29 20:00:56.143781 lamindb_setup-0.68.5/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.68.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.68.5/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.68.5/README.md
+-rw-r--r--   0        0        0    94692 2024-04-04 17:27:13.567863 lamindb_setup-0.68.5/docs/changelog.md
+-rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.68.5/docs/hub-cloud/01-init-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.68.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.68.5/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.68.5/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3106 2024-04-04 16:22:51.378892 lamindb_setup-0.68.5/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     2944 2024-04-04 16:22:51.379248 lamindb_setup-0.68.5/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.68.5/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.68.5/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.68.5/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.68.5/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.68.5/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.68.5/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.68.5/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.68.5/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.68.5/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.68.5/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.68.5/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.68.5/docs/index.md
+-rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.68.5/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.68.5/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-04 17:26:58.556364 lamindb_setup-0.68.5/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.68.5/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.68.5/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.68.5/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.68.5/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.68.5/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    10793 2024-03-30 23:41:21.159941 lamindb_setup-0.68.5/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.68.5/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.68.5/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2052 2024-03-09 06:05:04.472107 lamindb_setup-0.68.5/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1788 2024-02-29 20:00:56.146417 lamindb_setup-0.68.5/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11400 2024-03-29 23:29:05.334965 lamindb_setup-0.68.5/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     7356 2024-03-08 11:38:29.531124 lamindb_setup-0.68.5/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.68.5/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.68.5/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.68.5/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.68.5/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      490 2024-03-05 11:00:49.974555 lamindb_setup-0.68.5/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     2403 2024-03-05 09:37:50.121079 lamindb_setup-0.68.5/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.68.5/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.68.5/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5215 2024-03-17 22:17:13.346585 lamindb_setup-0.68.5/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    11678 2024-03-29 09:14:09.554146 lamindb_setup-0.68.5/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.68.5/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.68.5/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.68.5/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    11565 2024-03-14 17:58:31.758814 lamindb_setup-0.68.5/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.68.5/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.68.5/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    11782 2024-04-04 17:11:25.342942 lamindb_setup-0.68.5/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.68.5/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.68.5/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.68.5/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.68.5/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     7589 2024-04-04 16:22:51.380220 lamindb_setup-0.68.5/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.68.5/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.68.5/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      308 2024-03-05 11:00:49.975018 lamindb_setup-0.68.5/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    23830 2024-04-04 16:22:51.380455 lamindb_setup-0.68.5/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4154 2024-03-26 15:38:38.001047 lamindb_setup-0.68.5/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.68.5/pyproject.toml
+-rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.68.5/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.68.5/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.68.5/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.68.5/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.68.5/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.68.5/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0     2784 2024-03-22 15:00:34.134178 lamindb_setup-0.68.5/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11280 2024-03-29 23:01:12.640680 lamindb_setup-0.68.5/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0     1361 2024-03-22 15:00:34.134342 lamindb_setup-0.68.5/tests/hub-local/test_check_s3_storage_empty.py
+-rw-r--r--   0        0        0     1149 2024-03-22 15:00:34.134525 lamindb_setup-0.68.5/tests/hub-local/test_hosted_instance_deletion_gate.py
+-rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.68.5/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.68.5/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.624007 lamindb_setup-0.68.5/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1438 2024-03-07 01:53:25.976258 lamindb_setup-0.68.5/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.68.5/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.68.5/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.68.5/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.68.5/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.68.5/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.68.5/PKG-INFO
```

### Comparing `lamindb_setup-0.68.4/.github/workflows/build.yml` & `lamindb_setup-0.68.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.68.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/.gitignore` & `lamindb_setup-0.68.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/.pre-commit-config.yaml` & `lamindb_setup-0.68.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/LICENSE` & `lamindb_setup-0.68.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/changelog.md` & `lamindb_setup-0.68.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Avoid the error due to deleting the same file by multiple processes | [703](https://github.com/laminlabs/lamindb-setup/pull/703) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 | 0.68.5
+🐛 Fix directory uploads for hosted instances | [702](https://github.com/laminlabs/lamindb-setup/pull/702) | [Koncopd](https://github.com/Koncopd) | 2024-04-04 |
 🚑️ Temp fix for non-hosted buckets | [700](https://github.com/laminlabs/lamindb-setup/pull/700) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-02 |
 🍱 Add the scverse spatial hackathon bucket | [699](https://github.com/laminlabs/lamindb-setup/pull/699) | [falexwolf](https://github.com/falexwolf) | 2024-03-30 |
 ♻️ More fine-grained db credentials management | [698](https://github.com/laminlabs/lamindb-setup/pull/698) | [falexwolf](https://github.com/falexwolf) | 2024-03-29 | 0.68.2
 ✨ `upath.to_url()` | [695](https://github.com/laminlabs/lamindb-setup/pull/695) | [falexwolf](https://github.com/falexwolf) | 2024-03-28 |
 ♻️ Enable to choose skip_suffixes | [693](https://github.com/laminlabs/lamindb-setup/pull/693) | [falexwolf](https://github.com/falexwolf) | 2024-03-27 | 0.68.1
 ♻️ Refactor GCP compat | [692](https://github.com/laminlabs/lamindb-setup/pull/692) | [falexwolf](https://github.com/falexwolf) | 2024-03-26 |
 ✨ Rework synchronize, support directories | [687](https://github.com/laminlabs/lamindb-setup/pull/687) | [Koncopd](https://github.com/Koncopd) | 2024-03-23 | 0.68.0
```

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/01-init-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903159340659341%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, 'from lamindb_setup.core.upath import create_path, "*

 * *            "UPath, InstanceNotEmpty\\n'), (2, 'from lamindb_setup.core._hub_core import (\\n'), "*

 * *            "(3, '    delete_instance,\\n'), (4, '    call_with_fallback_auth,\\n'), (5, '    "*

 * *            "select_instance_by_owner_name,\\n'), (6, ')\\n')], delete: [2, 1]}}, 3: {'source': "*

 * *            '[\'try:\\n\', \'    delete_instance(f"testuser1/{instance_name}")\\n\', \'except '*

 * *            "InstanceNotEmpt […]*

```diff
@@ -19,29 +19,45 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb_setup as ln_setup\n",
-                "from lamindb_setup.core.upath import UPath\n",
-                "from lamindb_setup.core._hub_core import delete_instance\n",
+                "from lamindb_setup.core.upath import create_path, UPath, InstanceNotEmpty\n",
+                "from lamindb_setup.core._hub_core import (\n",
+                "    delete_instance,\n",
+                "    call_with_fallback_auth,\n",
+                "    select_instance_by_owner_name,\n",
+                ")\n",
                 "import pytest\n",
                 "\n",
                 "instance_name = \"my-hosted\"\n",
                 "assert ln_setup.settings.user.handle == \"testuser1\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "delete_instance(f\"testuser1/{instance_name}\")"
+                "try:\n",
+                "    delete_instance(f\"testuser1/{instance_name}\")\n",
+                "except InstanceNotEmpty:\n",
+                "    instance_with_storage = call_with_fallback_auth(\n",
+                "        select_instance_by_owner_name,\n",
+                "        owner=\"testuser1\",\n",
+                "        name=instance_name,\n",
+                "    )\n",
+                "    root = create_path(instance_with_storage[\"storage\"][\"root\"])\n",
+                "    for obj in root.rglob(\"\"):\n",
+                "        if obj.is_file():\n",
+                "            obj.unlink()\n",
+                "    delete_instance(f\"testuser1/{instance_name}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -89,27 +105,27 @@
             "source": [
                 "ln_setup.close()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py310",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9699404761904762%*

 * *Differences: {"'cells'": "{0: {'source': ['# Connect to a public instance anonymously']}, 1: {'source': "*

 * *            "['import lamindb_setup as ln_setup']}, 2: {'source': ['ln_setup.logout()']}, 3: "*

 * *            '{\'source\': [\'ln_setup.connect("laminlabs/lamindata")\']}, 4: {\'source\': [\'# for '*

 * *            "postgres instances just connecting should not initialize storage.root\\n', 'assert "*

 * *            "ln_setup.settings.storage._root is None']}, 5: {'cell_type': 'code', 'source': "*

 * *            "['ln_setup.close() […]*

```diff
@@ -1,93 +1,87 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Load hosted instance"
+                "# Connect to a public instance anonymously"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup as ln_setup\n",
-                "from lamindb_setup.core.upath import UPath\n",
-                "from lamindb_setup.core._hub_core import delete_instance\n",
-                "\n",
-                "instance_name = \"my-hosted\"\n",
-                "assert ln_setup.settings.user.handle == \"testuser1\""
+                "import lamindb_setup as ln_setup"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.connect(f\"testuser1/{instance_name}\")"
+                "ln_setup.logout()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.settings.storage.root.view_tree()"
+                "ln_setup.connect(\"laminlabs/lamindata\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "target_path = UPath(ln_setup.settings.storage.root / \"test_notebooks.py\")\n",
-                "target_path.upload_from(\"test_notebooks.py\")\n",
-                "target_path.exists()"
+                "# for postgres instances just connecting should not initialize storage.root\n",
+                "assert ln_setup.settings.storage._root is None"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Delete everything:"
+                "ln_setup.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "target_path.unlink()\n",
-                "ln_setup.delete(\"my-hosted\", force=True)\n",
-                "delete_instance(f\"testuser1/{instance_name}\")"
+                "ln_setup.login(\"testuser2\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py310",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.68.4/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-empty-init.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8211805555555556%*

 * *Differences: {"'cells'": "{0: {'source': ['# Test initialization in empty s3 bucket'], 'id': '20066735'}, 3: "*

 * *            "{'source': ['for s in root_path.iterdir():\\n', '    if s.is_file():\\n', '        "*

 * *            "s.unlink()\\n', '    elif s.is_dir():\\n', '        s.rmdir()'], 'id': 'df6e2146'}, "*

 * *            "4: {'source': ['assert list(root_path.iterdir()) == []'], 'id': '19a330ad'}, 5: "*

 * *            "{'source': ['ln_setup.init(storage=root_str)'], 'id': '81507d85'}, 6: {'source': "*

 * *            "['assert ln_s […]*

```diff
@@ -1,69 +1,111 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "20066735",
             "metadata": {},
             "source": [
-                "# Connect to a public instance anonymously"
+                "# Test initialization in empty s3 bucket"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "35db7a1b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup as ln_setup"
+                "import lamindb_setup as ln_setup\n",
+                "from lamindb_setup.core.upath import UPath"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "a4553515",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.logout()"
+                "root_str = \"s3://lamindb-setup-ci-empty-bucket\"\n",
+                "root_path = UPath(root_str, cache_regions=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "df6e2146",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.connect(\"laminlabs/lamindata\")"
+                "for s in root_path.iterdir():\n",
+                "    if s.is_file():\n",
+                "        s.unlink()\n",
+                "    elif s.is_dir():\n",
+                "        s.rmdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "19a330ad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# for postgres instances just connecting should not initialize storage.root\n",
-                "assert ln_setup.settings.storage._root is None"
+                "assert list(root_path.iterdir()) == []"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "81507d85",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.close()"
+                "ln_setup.init(storage=root_str)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "544dbae3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.login(\"testuser2\")"
+                "assert ln_setup.settings.storage.is_cloud\n",
+                "assert ln_setup.settings.storage.root_as_str == root_str\n",
+                "assert ln_setup.settings.storage.region == \"us-east-1\"\n",
+                "assert (\n",
+                "    str(ln_setup.settings.instance._sqlite_file)\n",
+                "    == f\"{root_str}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a339197a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln_setup.delete(\"lamindb-setup-ci-empty-bucket\", force=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "77859588",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for s in root_path.iterdir():\n",
+                "    if s.is_file():\n",
+                "        s.unlink()\n",
+                "    elif s.is_dir():\n",
+                "        s.rmdir()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -79,9 +121,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.17"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 5
 }
```

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.68.5/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8329427083333334%*

 * *Differences: {"'cells'": "{0: {'source': ['# Load hosted instance'], delete: ['id']}, 1: {'source': {insert: "*

 * *            "[(0, 'import shutil\\n'), (2, 'from lamindb_setup.core.upath import UPath\\n'), (3, "*

 * *            "'from lamindb_setup.core._hub_core import delete_instance\\n'), (4, '\\n'), (5, "*

 * *            '\'instance_name = "my-hosted"\\n\'), (6, \'assert ln_setup.settings.user.handle == '*

 * *            '"testuser1"\')], delete: [1]}, delete: [\'id\']}, 2: {\'source\': '*

 * *            '[\'ln_setup.connect(f"testus […]*

```diff
@@ -1,111 +1,121 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "20066735",
             "metadata": {},
             "source": [
-                "# Test initialization in empty s3 bucket"
+                "# Load hosted instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "35db7a1b",
             "metadata": {},
             "outputs": [],
             "source": [
+                "import shutil\n",
                 "import lamindb_setup as ln_setup\n",
-                "from lamindb_setup.core.upath import UPath"
+                "from lamindb_setup.core.upath import UPath\n",
+                "from lamindb_setup.core._hub_core import delete_instance\n",
+                "\n",
+                "instance_name = \"my-hosted\"\n",
+                "assert ln_setup.settings.user.handle == \"testuser1\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a4553515",
             "metadata": {},
             "outputs": [],
             "source": [
-                "root_str = \"s3://lamindb-setup-ci-empty-bucket\"\n",
-                "root_path = UPath(root_str, cache_regions=True)"
+                "ln_setup.connect(f\"testuser1/{instance_name}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "df6e2146",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for s in root_path.iterdir():\n",
-                "    if s.is_file():\n",
-                "        s.unlink()\n",
-                "    elif s.is_dir():\n",
-                "        s.rmdir()"
+                "root = ln_setup.settings.storage.root"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "19a330ad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert list(root_path.iterdir()) == []"
+                "root.view_tree()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "81507d85",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.init(storage=root_str)"
+                "target_path = root / \"test_notebooks.py\"\n",
+                "target_path.upload_from(\"test_notebooks.py\")\n",
+                "assert target_path.exists()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "544dbae3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln_setup.settings.storage.is_cloud\n",
-                "assert ln_setup.settings.storage.root_as_str == root_str\n",
-                "assert ln_setup.settings.storage.region == \"us-east-1\"\n",
-                "assert (\n",
-                "    str(ln_setup.settings.instance._sqlite_file)\n",
-                "    == f\"{root_str}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
-                ")"
+                "test_dir = UPath(\"./test-dir-upload\")\n",
+                "test_dir.mkdir()\n",
+                "(test_dir / \"file1\").touch()\n",
+                "subdir = test_dir / \"subdir\"\n",
+                "subdir.mkdir()\n",
+                "(subdir / \"file2\").touch()\n",
+                "subsubdir = subdir / \"subsubdir\"\n",
+                "subsubdir.mkdir()\n",
+                "(subsubdir / \"file3\").touch()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a339197a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.delete(\"lamindb-setup-ci-empty-bucket\", force=True)"
+                "target_dir = root / \"test-dir-upload\"\n",
+                "target_dir.upload_from(test_dir, recursive=True)\n",
+                "\n",
+                "assert target_dir.is_dir()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Delete everything:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "77859588",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for s in root_path.iterdir():\n",
-                "    if s.is_file():\n",
-                "        s.unlink()\n",
-                "    elif s.is_dir():\n",
-                "        s.rmdir()"
+                "shutil.rmtree(test_dir)\n",
+                "\n",
+                "target_path.unlink()\n",
+                "assert not target_path.exists()\n",
+                "\n",
+                "target_dir.rmdir()\n",
+                "assert not target_dir.exists()\n",
+                "\n",
+                "ln_setup.delete(\"my-hosted\", force=True)\n",
+                "delete_instance(f\"testuser1/{instance_name}\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -121,9 +131,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.17"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.68.5/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/__init__.py` & `lamindb_setup-0.68.5/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.68.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.68.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.68.5/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_cache.py` & `lamindb_setup-0.68.5/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_check_setup.py` & `lamindb_setup-0.68.5/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_close.py` & `lamindb_setup-0.68.5/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.68.5/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_delete.py` & `lamindb_setup-0.68.5/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_django.py` & `lamindb_setup-0.68.5/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_exportdb.py` & `lamindb_setup-0.68.5/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_importdb.py` & `lamindb_setup-0.68.5/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.68.5/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_migrate.py` & `lamindb_setup-0.68.5/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.68.5/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_schema.py` & `lamindb_setup-0.68.5/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.68.5/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.68.5/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,24 @@
     # we need to touch a 0-byte object in the storage location to avoid
     # permission errors from leveraging s3fs on an empty hosted storage location
     root_upath = convert_pathlike(root)
     mark_upath = root_upath / IS_INITIALIZED_KEY
     mark_upath.touch()
 
 
-def init_storage(storage: UPathStr, region: Optional[str] = None) -> "StorageSettings":
+def init_storage(storage: UPathStr) -> "StorageSettings":
     if storage is None:
         raise ValueError("storage argument can't be `None`")
     root = str(storage)  # ensure we have a string
     uid = base62(8)
-    if root == "create-s3":
+    region = None
+    if root.startswith("create-s3"):
+        if root != "create-s3":
+            assert "--" in root, "example: `create-s3--eu-central-1`"
+            region = root.replace("create-s3--", "")
         if region is None:
             region = find_closest_aws_region()
         else:
             if region not in hosted_regions:
                 raise ValueError(f"region has to be one of {hosted_regions}")
         lamin_env = os.getenv("LAMIN_ENV")
         if lamin_env is None or lamin_env == "prod":
```

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.68.5/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.68.5/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/django.py` & `lamindb_setup-0.68.5/lamindb_setup/core/django.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,14 +196,23 @@
         #                 deployed_latest_migrations=latest_migrs[0],
         #                 defined_latest_migrations=latest_migrs[1],
         #             )
         #         )
 
     # clean up temporary settings files
     if not settings_file_existed:
-        isettings._get_settings_file().unlink()
-    current_instance_settings_file().unlink()
+        try:
+            isettings._get_settings_file().unlink()
+        except FileNotFoundError:
+            pass
+    # try except is needed here and above to avoid problems due to
+    # multiple processes trying to delete this file, and for one of them
+    # it has been deleted already
+    try:
+        current_instance_settings_file().unlink()
+    except FileNotFoundError:
+        pass
     if current_settings_file_existed:
         shutil.copy(current_settings_file.with_name("_tmp.env"), current_settings_file)
 
     global IS_SETUP
     IS_SETUP = True
```

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/hashing.py` & `lamindb_setup-0.68.5/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/lamindb_setup/core/upath.py` & `lamindb_setup-0.68.5/lamindb_setup/core/upath.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     ".fcs",
     ".xslx",
     ".zarr",
     ".zrad",
 }
 
 
+TRAILING_SEP = (os.sep, os.altsep) if os.altsep is not None else os.sep
+
+
 def extract_suffix_from_path(path: Path, arg_name: Optional[str] = None) -> str:
     def process_digits(suffix: str):
         if suffix[1:].isdigit():
             return ""  # digits are no valid suffixes
         else:
             return suffix
 
@@ -156,33 +159,57 @@
     def call(self, *args, **kwargs):
         return None
 
 
 def download_to(self, path, print_progress: bool = False, **kwargs):
     """Download to a path."""
     if print_progress:
-        if not path.is_dir():
+        # can't do path.is_dir() because path doesn't exist
+        # so assume any destination without a suffix is a dir
+        # this is temporary until we have a proper progress bar for directories
+        if os.path.splitext(path)[-1] not in {"", ".zrad", ".zarr"}:
             cb = ProgressCallback("downloading")
         else:
             # todo: make proper progress bar for directories
             cb = fsspec.callbacks.NoOpCallback()
         kwargs["callback"] = cb
     self.fs.download(str(self), str(path), **kwargs)
 
 
 def upload_from(self, path, print_progress: bool = False, **kwargs):
     """Upload from a local path."""
     if print_progress:
-        if not path.is_dir():
+        if not os.path.isdir(path):
             cb = ProgressCallback("uploading")
         else:
             # todo: make proper progress bar for directories
             cb = fsspec.callbacks.NoOpCallback()
         kwargs["callback"] = cb
-    self.fs.upload(str(path), str(self), **kwargs)
+    # this weird thing is to avoid triggering create_bucket in upload
+    # if dirs are present
+    # it allows to avoid permission error
+    destination = str(self)
+    if os.path.isfile(path):
+        cleanup_cache = False
+    else:
+        bucket = self._url.netloc
+        if bucket not in self.fs.dircache:
+            self.fs.dircache[bucket] = [{}]
+            if not destination.endswith(TRAILING_SEP):  # type: ignore
+                destination += "/"
+            cleanup_cache = True
+        else:
+            cleanup_cache = False
+
+    self.fs.upload(str(path), destination, **kwargs)
+
+    if cleanup_cache:
+        # normally this is invalidated after the upload but still better to check
+        if bucket in self.fs.dircache:
+            del self.fs.dircache[bucket]
 
 
 def synchronize(self, objectpath: Path, error_no_origin: bool = True, **kwargs):
     """Sync to a local destination path."""
     # optimize the number of network requests
     if "timestamp" in kwargs:
         is_dir = False
```

### Comparing `lamindb_setup-0.68.4/noxfile.py` & `lamindb_setup-0.68.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/pyproject.toml` & `lamindb_setup-0.68.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.68.5/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.68.5/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-local/conftest.py` & `lamindb_setup-0.68.5/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-local/test_all.py` & `lamindb_setup-0.68.5/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-local/test_check_s3_storage_empty.py` & `lamindb_setup-0.68.5/tests/hub-local/test_check_s3_storage_empty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-local/test_hosted_instance_deletion_gate.py` & `lamindb_setup-0.68.5/tests/hub-local/test_hosted_instance_deletion_gate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.68.5/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/hub-prod/test_upath.py` & `lamindb_setup-0.68.5/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/storage/test_hashing.py` & `lamindb_setup-0.68.5/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/storage/test_storage_access.py` & `lamindb_setup-0.68.5/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/storage/test_storage_basis.py` & `lamindb_setup-0.68.5/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/tests/storage/test_storage_stats.py` & `lamindb_setup-0.68.5/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.4/PKG-INFO` & `lamindb_setup-0.68.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.68.4
+Version: 0.68.5
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

