# Comparing `tmp/pyvserv-1.0.2.tar.gz` & `tmp/pyvserv-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvserv-1.0.2.tar", last modified: Sun Mar 31 09:47:10 2024, max compression
+gzip compressed data, was "pyvserv-1.0.3.tar", last modified: Thu Apr  4 07:48:56 2024, max compression
```

## Comparing `pyvserv-1.0.2.tar` & `pyvserv-1.0.3.tar`

### file list

```diff
@@ -1,89 +1,86 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.392542 pyvserv-1.0.2/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.2/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    10193 2024-03-31 09:47:10.388542 pyvserv-1.0.2/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     9656 2024-03-15 11:39:21.000000 pyvserv-1.0.2/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.376541 pyvserv-1.0.2/pyvclient/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:10.000000 pyvserv-1.0.2/pyvclient/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      509 2024-03-11 08:27:21.000000 pyvserv-1.0.2/pyvclient/bulkren.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3921 2024-03-09 10:49:47.000000 pyvserv-1.0.2/pyvclient/chall.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.2/pyvclient/loadtest.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4889 2024-03-17 10:22:21.000000 pyvserv-1.0.2/pyvclient/pyvcli_acc.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3979 2024-03-02 11:01:52.000000 pyvserv-1.0.2/pyvclient/pyvcli_akey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4200 2024-03-17 10:21:55.000000 pyvserv-1.0.2/pyvclient/pyvcli_bigget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5698 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_cd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     8835 2024-03-17 10:21:31.000000 pyvserv-1.0.2/pyvclient/pyvcli_cli.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3595 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_fdel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3689 2024-03-17 10:21:00.000000 pyvserv-1.0.2/pyvclient/pyvcli_fget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3916 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_file.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3928 2024-03-02 14:08:46.000000 pyvserv-1.0.2/pyvclient/pyvcli_fput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3739 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_gethelp.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1990 2024-02-25 14:49:13.000000 pyvserv-1.0.2/pyvclient/pyvcli_hello.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2097 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_id.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6005 2024-03-11 12:10:04.000000 pyvserv-1.0.2/pyvclient/pyvcli_ihost.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4119 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_login.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5016 2024-03-17 10:20:16.000000 pyvserv-1.0.2/pyvclient/pyvcli_ls.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4891 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_lsd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3958 2024-03-17 10:19:24.000000 pyvserv-1.0.2/pyvclient/pyvcli_mkdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3907 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_pass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_ping.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4612 2024-03-01 13:57:24.000000 pyvserv-1.0.2/pyvclient/pyvcli_qr.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     8517 2024-03-17 10:16:21.000000 pyvserv-1.0.2/pyvclient/pyvcli_replic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5599 2024-03-17 10:12:42.000000 pyvserv-1.0.2/pyvclient/pyvcli_rget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4396 2024-03-17 10:15:52.000000 pyvserv-1.0.2/pyvclient/pyvcli_rlist.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5802 2024-03-14 11:50:16.000000 pyvserv-1.0.2/pyvclient/pyvcli_rput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6401 2024-03-02 15:00:25.000000 pyvserv-1.0.2/pyvclient/pyvcli_sess.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7033 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_sess_tout.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2680 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_tout.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3348 2024-03-17 00:44:33.000000 pyvserv-1.0.2/pyvclient/pyvcli_uadd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4215 2024-03-17 07:30:55.000000 pyvserv-1.0.2/pyvclient/pyvcli_uchpass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3187 2024-03-17 06:46:46.000000 pyvserv-1.0.2/pyvclient/pyvcli_udel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3566 2024-03-17 01:28:17.000000 pyvserv-1.0.2/pyvclient/pyvcli_uena.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3528 2024-03-12 08:26:46.000000 pyvserv-1.0.2/pyvclient/pyvcli_uini.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     1101 2024-03-12 08:36:38.000000 pyvserv-1.0.2/pyvclient/pyvcli_utils.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2600 2024-02-25 16:08:36.000000 pyvserv-1.0.2/pyvclient/pyvcli_ver.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.380541 pyvserv-1.0.2/pyvcommon/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:18.000000 pyvserv-1.0.2/pyvcommon/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10832 2024-03-03 15:44:52.000000 pyvserv-1.0.2/pyvcommon/comline.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.2/pyvcommon/crysupp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.2/pyvcommon/genstrerr.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14912 2024-03-17 10:10:30.000000 pyvserv-1.0.2/pyvcommon/pyclisup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.2/pyvcommon/pycrypt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6671 2024-03-11 08:42:22.000000 pyvserv-1.0.2/pyvcommon/pydata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    23021 2024-03-17 07:27:39.000000 pyvserv-1.0.2/pyvcommon/pyservsup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.2/pyvcommon/pysyslog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.2/pyvcommon/pyv2fa.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10240 2024-03-31 09:39:31.000000 pyvserv-1.0.2/pyvcommon/pyvhash.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.2/pyvcommon/pywrap.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9353 2024-03-31 09:38:00.000000 pyvserv-1.0.2/pyvcommon/support.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.380541 pyvserv-1.0.2/pyvgui/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:37:55.000000 pyvserv-1.0.2/pyvgui/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.384541 pyvserv-1.0.2/pyvgui/guilib/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:42:21.000000 pyvserv-1.0.2/pyvgui/guilib/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14657 2024-03-16 15:57:54.000000 pyvserv-1.0.2/pyvgui/guilib/mainwin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5883 2024-03-11 07:30:45.000000 pyvserv-1.0.2/pyvgui/guilib/mainwinserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9305 2024-03-16 16:07:42.000000 pyvserv-1.0.2/pyvgui/guilib/mainwintally.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.2/pyvgui/guilib/pgui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.2/pyvgui/guilib/pymenu.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3524 2024-03-16 14:48:37.000000 pyvserv-1.0.2/pyvgui/pyvcpanel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3019 2024-03-16 15:59:27.000000 pyvserv-1.0.2/pyvgui/pyvservui.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3534 2024-03-16 15:39:10.000000 pyvserv-1.0.2/pyvgui/pyvtally.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.388542 pyvserv-1.0.2/pyvserv.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    10193 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)     1866 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)      242 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/requires.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-03-31 09:47:10.000000 pyvserv-1.0.2/pyvserv.egg-info/top_level.txt
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.388542 pyvserv-1.0.2/pyvserver/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:04.000000 pyvserv-1.0.2/pyvserver/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    55635 2024-03-17 06:44:25.000000 pyvserv-1.0.2/pyvserver/pyvfunc.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    11352 2024-03-11 14:27:18.000000 pyvserv-1.0.2/pyvserver/pyvpuller.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    11364 2024-03-11 14:18:05.000000 pyvserv-1.0.2/pyvserver/pyvreplic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    19046 2024-03-14 14:12:57.000000 pyvserv-1.0.2/pyvserver/pyvserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13799 2024-03-17 05:17:57.000000 pyvserv-1.0.2/pyvserver/pyvstate.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-31 09:47:10.388542 pyvserv-1.0.2/pyvtools/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:46:04.000000 pyvserv-1.0.2/pyvtools/__init__.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4811 2024-03-11 08:51:24.000000 pyvserv-1.0.2/pyvtools/pyvgenkey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2507 2024-03-11 08:52:17.000000 pyvserv-1.0.2/pyvtools/pyvgenkeys.py
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-03-31 09:47:10.392542 pyvserv-1.0.2/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     2749 2024-03-31 09:46:54.000000 pyvserv-1.0.2/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.664012 pyvserv-1.0.3/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.3/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    14003 2024-04-04 07:48:56.660012 pyvserv-1.0.3/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13441 2024-04-04 07:48:11.000000 pyvserv-1.0.3/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.520001 pyvserv-1.0.3/pyvclient/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:10.000000 pyvserv-1.0.3/pyvclient/__init__.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.3/pyvclient/loadtest.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3979 2024-03-02 11:01:52.000000 pyvserv-1.0.3/pyvclient/pyvcli_akey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4767 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_bigget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5698 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_cd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     9981 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_cli.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3595 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_fdel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3689 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_fget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3916 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_file.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3745 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_fput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4087 2024-04-02 09:10:12.000000 pyvserv-1.0.3/pyvclient/pyvcli_gethelp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2328 2024-04-02 08:13:29.000000 pyvserv-1.0.3/pyvclient/pyvcli_hello.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2097 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_id.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6005 2024-03-11 12:10:04.000000 pyvserv-1.0.3/pyvclient/pyvcli_ihost.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4119 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_login.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5016 2024-03-17 10:20:16.000000 pyvserv-1.0.3/pyvclient/pyvcli_ls.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4891 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_lsd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3958 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_mkdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3907 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_pass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_ping.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3599 2024-04-02 15:41:33.000000 pyvserv-1.0.3/pyvclient/pyvcli_qr.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     9414 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_replic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5940 2024-04-02 09:10:50.000000 pyvserv-1.0.3/pyvclient/pyvcli_rget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4814 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_rlist.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6511 2024-04-02 08:59:15.000000 pyvserv-1.0.3/pyvclient/pyvcli_rput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6401 2024-03-02 15:00:25.000000 pyvserv-1.0.3/pyvclient/pyvcli_sess.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7033 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_sess_tout.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2680 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_tout.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3348 2024-03-17 00:44:33.000000 pyvserv-1.0.3/pyvclient/pyvcli_uadd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4215 2024-03-17 07:30:55.000000 pyvserv-1.0.3/pyvclient/pyvcli_uchpass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3187 2024-03-17 06:46:46.000000 pyvserv-1.0.3/pyvclient/pyvcli_udel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3566 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_uena.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3432 2024-04-02 09:29:19.000000 pyvserv-1.0.3/pyvclient/pyvcli_uini.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4869 2024-04-02 10:38:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_uman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2725 2024-04-02 16:14:25.000000 pyvserv-1.0.3/pyvclient/pyvcli_ver.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.608008 pyvserv-1.0.3/pyvcommon/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:18.000000 pyvserv-1.0.3/pyvcommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10832 2024-03-03 15:44:52.000000 pyvserv-1.0.3/pyvcommon/comline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.3/pyvcommon/crysupp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.3/pyvcommon/genstrerr.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14953 2024-04-02 10:45:49.000000 pyvserv-1.0.3/pyvcommon/pyclisup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.3/pyvcommon/pycrypt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6671 2024-03-11 08:42:22.000000 pyvserv-1.0.3/pyvcommon/pydata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    23396 2024-04-04 02:24:00.000000 pyvserv-1.0.3/pyvcommon/pyservsup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.3/pyvcommon/pysyslog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.3/pyvcommon/pyv2fa.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10237 2024-04-04 06:05:08.000000 pyvserv-1.0.3/pyvcommon/pyvhash.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.3/pyvcommon/pywrap.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9527 2024-04-01 14:21:20.000000 pyvserv-1.0.3/pyvcommon/support.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.616008 pyvserv-1.0.3/pyvgui/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:37:55.000000 pyvserv-1.0.3/pyvgui/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.628009 pyvserv-1.0.3/pyvgui/guilib/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:42:21.000000 pyvserv-1.0.3/pyvgui/guilib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14657 2024-03-16 15:57:54.000000 pyvserv-1.0.3/pyvgui/guilib/mainwin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.3/pyvgui/guilib/mainwinserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9305 2024-03-16 16:07:42.000000 pyvserv-1.0.3/pyvgui/guilib/mainwintally.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.3/pyvgui/guilib/pgui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.3/pyvgui/guilib/pymenu.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3104 2024-04-03 07:29:15.000000 pyvserv-1.0.3/pyvgui/pyvcpanel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2682 2024-04-03 07:32:33.000000 pyvserv-1.0.3/pyvgui/pyvservui.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3089 2024-04-03 07:47:23.000000 pyvserv-1.0.3/pyvgui/pyvtally.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.660012 pyvserv-1.0.3/pyvserv.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    14003 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)     1801 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)      598 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/requires.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/top_level.txt
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.648011 pyvserv-1.0.3/pyvserver/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:04.000000 pyvserv-1.0.3/pyvserver/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    56484 2024-04-04 03:20:07.000000 pyvserv-1.0.3/pyvserver/pyvfunc.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    10855 2024-04-03 07:15:57.000000 pyvserv-1.0.3/pyvserver/pyvpuller.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    10940 2024-04-03 07:59:18.000000 pyvserv-1.0.3/pyvserver/pyvreplic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    20718 2024-04-04 05:56:40.000000 pyvserv-1.0.3/pyvserver/pyvserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14047 2024-04-04 03:19:43.000000 pyvserv-1.0.3/pyvserver/pyvstate.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.656012 pyvserv-1.0.3/pyvtools/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:46:04.000000 pyvserv-1.0.3/pyvtools/__init__.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.3/pyvtools/pyvgenkey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2507 2024-03-11 08:52:17.000000 pyvserv-1.0.3/pyvtools/pyvgenkeys.py
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-04 07:48:56.664012 pyvserv-1.0.3/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4076 2024-04-04 05:10:28.000000 pyvserv-1.0.3/setup.py
```

### Comparing `pyvserv-1.0.2/LICENSE` & `pyvserv-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/PKG-INFO` & `pyvserv-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.2
+Version: 1.0.3
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyvpacker
 Requires-Dist: pydbase
 Requires-Dist: pycryptodome
 Requires-Dist: pyvecc
+Requires-Dist: pyvguicom
 
 #  PyvServer
+
 ## 	Fully encrypted TCP/IP server.
 
  &nbsp; &nbsp; PyvServ is an encrypting TCP/IP server written in Python. The
 encryption algorithm is AES. (Advanced Encryption Standard) The key exchange
 uses ECC. (Elliptic curve) The server can be fully administered from the
 protocol side.
 
@@ -85,16 +87,14 @@
  PyvServ has replication facilities via a client based 'I have You have'
  mechanism featuring encrypted transport. It is also capable of replication
  on a 'replicate when received' mechanism. The replicated records are marked
  with a replication count, so replication does not enter looping. By default,
  the replicated records are not replicated any further, assuming a flat
  structure of replication.
 
- Project is still in motion, but a lot of it is usable.
-
 #### Installation:
 
     pip install pyvserv
 
  Dependencies:
 
  Most linux systems already have all the dependencies by default. Some dependencies
@@ -105,92 +105,167 @@
  The firewall needs to be opened for incoming connections on port xxxx
 
 For example (assuming port 6666):
 
     sudo iptables -A INPUT -p tcp --dport 6666
     sudo iptables -A INPUT -p tcp --sport 6666
 
- Please note that this is not a recommendation, it is a port we used during development.
+ Please note that this is not a recommendation, it is a port we used during
+ development.
+
+#### Start server
+
+ The python server can be added to the system servers with the Makefile targets
+'make genservice' and 'make instservice'
+ The scripts will generate the service file to run under current user's
+ credentials, and install it onto the running system. (requires sudo)
 
 #### Platform:
 
-    This project was developed on Ubuntu 22.x. Most linux distributions should work.
+ This project was developed on Ubuntu 22.x. Most linux distributions should work.
+It is ported to Windows MSYS2, with all major functions operating as expected.
+
+ On Fedora, the service files need to be re-written to accomodate the
+quirk that the Fedora systectl does not allow user executables. Install
+the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
+to use pyvserv with  particular data directory, use the -r option.
 
-#### Working parts:
+#### Quick map:
 
-    Server.     subdir: pyvserver       -- Server has most of the commands done
+    Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
-    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     Test Suite. subdir: pyvclient/tests -- official pytest tests
+    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
 installation from github, replicating directory structure on the local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
-    type ./pyvserv.py  -D
-
-    The -D option stands for development mode. The server will not ask for
-    2FA authentication.
+    type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
-    type ./pyvcli_hello.py
+    type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
     Server initial: ['OK', 'pyvserv 1.0 ready']
     resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
     Server quit response: ['OK', 'Bye', '11812']
 
 Quick rundown of the above test:
 
-1.) Server responds to connection
-2.) Delivers OK status, hello message, server serial number, and a unique id
-3.) Server signs off. This interaction is typical of all the commands.
+    1.) Server responds to connection with signin message
+    2.) Delivers OK status, hello message, server serial number, and a unique id
+    3.) Server signs off. Repeats unique id / session number.
 
- The unique ID is the session's thread ID and it is not cryptographically secure;
+This interaction is typical of all the commands.
+
+The unique ID is the session's thread ID and it is not cryptographically secure;
+Mostly useful for identifying the session on the client side.
 
  The best way to learn about the operation of the server is to look at the
 sample client examples in the client source tree. (Files named pyvcli_*)
 
+## The pip install
+
+ Scripts are provided for the server, and some test clients. The
+  server can be started as
+
+    pyvserver
+
+ The -P option is for non Developer mode, enabling 2FA authentication.
+ (two factor authentication)
+
+ The command line client can be started as:
+
+    pyvcli_cli
+
+  In the command line client most of the server functions can be exercised.
+See the pyvcli_* utils for more examples of driving the server.
+
+## Command line help
+
+    Usage: pyvserv.py [options]
+
+    Options:
+            -n   --host                 -  Set server hostname / interface.
+            -r   --dataroot  dataroot   -  Set data root for server.
+            -P   --pmode                -  Production mode ON. (allow 2FA)
+            -l   --loglevel             -  Log level (0 - 10) default = 1
+            -m   --mem                  -  Show memory trace.
+            -N   --norepl               -  No replication. (for testing)
+            -d   --debug     debug      -  Debug level 0-10
+            -p   --port      port       -  Listen on port
+            -v   --verbose              -  Verbose
+            -q   --quiet                -  Quiet
+            -V   --version              -  Print Version
+            -h   --help                 -  Show Help
+
+## Client command line help example:
+
+ While most command line clients have their own help screen, here as a typical
+client utility's help screen:
+
+    Usage: pyvcli_uman.py [options]
+
+    Options:    -d level  - Debug level 0-10
+                -p        - Port to use (default: 6666)
+                -l login  - Login Name; default: 'user'
+                -s lpass  - Login Pass; default: '1234'
+                -u user   - User Name; default: 'user'
+                -a        - Add user. Must be unique.
+                -r        - Remove user (one of add or remove needed.
+                -u user   - User Name; default: 'user'
+                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -m        - Add admin instead of regular user
+                -v        - Verbose
+                -q        - Quiet
+                -h        - Help
+
 ## Testing:
 
  All pytest cases pass. Note that the for the pytest client tests one needs to
  start the 'pyvserv.py' server.
  The server --port and --dataroot option can ba used to start the server in an alternate
  universe. Please make sure it does not interfere with production.
 
-   More test coming soon ....
-
-    ============================= test session starts ==============================
+    ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
-    rootdir: /home/peterglen/pgpygtk/pyvserv
-    collected 9 items
+    rootdir: /home/<homedir>/pgpygtk/pyvserv
+    collected 15 items
 
-    test_afirst.py .                                                         [ 11%]
-    test_file.py .                                                           [ 22%]
+    test_afirst.py .                                                         [  6%]
+    test_file.py ..                                                          [ 20%]
+    test_hello.py .                                                          [ 26%]
     test_help.py .                                                           [ 33%]
-    test_id.py .                                                             [ 44%]
-    test_key.py .                                                            [ 55%]
-    test_login.py .                                                          [ 66%]
-    test_sess.py ..                                                          [ 88%]
+    test_id.py .                                                             [ 40%]
+    test_key.py .                                                            [ 46%]
+    test_login.py .                                                          [ 53%]
+    test_noadmn.py .                                                         [ 60%]
+    test_rget.py .                                                           [ 66%]
+    test_rput.py .                                                           [ 73%]
+    test_sess.py ..                                                          [ 86%]
+    test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
-    ============================== 9 passed in 1.35s ===============================
+    ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the test directory. The pyvcli_* files may also
+Additional tests can be found in the tests/ directory. The pyvcli_* files may also
 serve as test cases.
 
+More test coming soon ....
+
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
@@ -199,23 +274,39 @@
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
   All views monitor the live files, on the default setup, without interfering
 with any of the operations.
 
+## Windows compatibility
+
+ Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+functionalities are ported. The file locking mechanism works, and all the
+pytests pass. Naturally, logging and readline etc ... works with the usual
+windows caveat.
+
+  For the GUI functions install the PyGobject subsystem. Instructions can
+be found very easily for that. Below, a screenshot of the pyvserv control panel
+in MSYS2.
+
+![Screen Shot](winscreen.png)
+
+The project is functional in MSYS2, but for real deployment we recommend Linux.
+
 ## History:
 
  Recent history kept, for the full list of changes consult the github site.
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
+    1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
 
 ## Statistics
 
     Project name
         pyvserv
     Report Period
         2018-12-31 20:50:04 to 2024-03-15 04:47:25
```

### Comparing `pyvserv-1.0.2/README.md` & `pyvserv-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  PyvServer
+
 ## 	Fully encrypted TCP/IP server.
 
  &nbsp; &nbsp; PyvServ is an encrypting TCP/IP server written in Python. The
 encryption algorithm is AES. (Advanced Encryption Standard) The key exchange
 uses ECC. (Elliptic curve) The server can be fully administered from the
 protocol side.
 
@@ -67,16 +68,14 @@
  PyvServ has replication facilities via a client based 'I have You have'
  mechanism featuring encrypted transport. It is also capable of replication
  on a 'replicate when received' mechanism. The replicated records are marked
  with a replication count, so replication does not enter looping. By default,
  the replicated records are not replicated any further, assuming a flat
  structure of replication.
 
- Project is still in motion, but a lot of it is usable.
-
 #### Installation:
 
     pip install pyvserv
 
  Dependencies:
 
  Most linux systems already have all the dependencies by default. Some dependencies
@@ -87,92 +86,167 @@
  The firewall needs to be opened for incoming connections on port xxxx
 
 For example (assuming port 6666):
 
     sudo iptables -A INPUT -p tcp --dport 6666
     sudo iptables -A INPUT -p tcp --sport 6666
 
- Please note that this is not a recommendation, it is a port we used during development.
+ Please note that this is not a recommendation, it is a port we used during
+ development.
+
+#### Start server
+
+ The python server can be added to the system servers with the Makefile targets
+'make genservice' and 'make instservice'
+ The scripts will generate the service file to run under current user's
+ credentials, and install it onto the running system. (requires sudo)
 
 #### Platform:
 
-    This project was developed on Ubuntu 22.x. Most linux distributions should work.
+ This project was developed on Ubuntu 22.x. Most linux distributions should work.
+It is ported to Windows MSYS2, with all major functions operating as expected.
+
+ On Fedora, the service files need to be re-written to accomodate the
+quirk that the Fedora systectl does not allow user executables. Install
+the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
+to use pyvserv with  particular data directory, use the -r option.
 
-#### Working parts:
+#### Quick map:
 
-    Server.     subdir: pyvserver       -- Server has most of the commands done
+    Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
-    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     Test Suite. subdir: pyvclient/tests -- official pytest tests
+    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
 installation from github, replicating directory structure on the local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
-    type ./pyvserv.py  -D
-
-    The -D option stands for development mode. The server will not ask for
-    2FA authentication.
+    type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
-    type ./pyvcli_hello.py
+    type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
     Server initial: ['OK', 'pyvserv 1.0 ready']
     resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
     Server quit response: ['OK', 'Bye', '11812']
 
 Quick rundown of the above test:
 
-1.) Server responds to connection
-2.) Delivers OK status, hello message, server serial number, and a unique id
-3.) Server signs off. This interaction is typical of all the commands.
+    1.) Server responds to connection with signin message
+    2.) Delivers OK status, hello message, server serial number, and a unique id
+    3.) Server signs off. Repeats unique id / session number.
 
- The unique ID is the session's thread ID and it is not cryptographically secure;
+This interaction is typical of all the commands.
+
+The unique ID is the session's thread ID and it is not cryptographically secure;
+Mostly useful for identifying the session on the client side.
 
  The best way to learn about the operation of the server is to look at the
 sample client examples in the client source tree. (Files named pyvcli_*)
 
+## The pip install
+
+ Scripts are provided for the server, and some test clients. The
+  server can be started as
+
+    pyvserver
+
+ The -P option is for non Developer mode, enabling 2FA authentication.
+ (two factor authentication)
+
+ The command line client can be started as:
+
+    pyvcli_cli
+
+  In the command line client most of the server functions can be exercised.
+See the pyvcli_* utils for more examples of driving the server.
+
+## Command line help
+
+    Usage: pyvserv.py [options]
+
+    Options:
+            -n   --host                 -  Set server hostname / interface.
+            -r   --dataroot  dataroot   -  Set data root for server.
+            -P   --pmode                -  Production mode ON. (allow 2FA)
+            -l   --loglevel             -  Log level (0 - 10) default = 1
+            -m   --mem                  -  Show memory trace.
+            -N   --norepl               -  No replication. (for testing)
+            -d   --debug     debug      -  Debug level 0-10
+            -p   --port      port       -  Listen on port
+            -v   --verbose              -  Verbose
+            -q   --quiet                -  Quiet
+            -V   --version              -  Print Version
+            -h   --help                 -  Show Help
+
+## Client command line help example:
+
+ While most command line clients have their own help screen, here as a typical
+client utility's help screen:
+
+    Usage: pyvcli_uman.py [options]
+
+    Options:    -d level  - Debug level 0-10
+                -p        - Port to use (default: 6666)
+                -l login  - Login Name; default: 'user'
+                -s lpass  - Login Pass; default: '1234'
+                -u user   - User Name; default: 'user'
+                -a        - Add user. Must be unique.
+                -r        - Remove user (one of add or remove needed.
+                -u user   - User Name; default: 'user'
+                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -m        - Add admin instead of regular user
+                -v        - Verbose
+                -q        - Quiet
+                -h        - Help
+
 ## Testing:
 
  All pytest cases pass. Note that the for the pytest client tests one needs to
  start the 'pyvserv.py' server.
  The server --port and --dataroot option can ba used to start the server in an alternate
  universe. Please make sure it does not interfere with production.
 
-   More test coming soon ....
-
-    ============================= test session starts ==============================
+    ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
-    rootdir: /home/peterglen/pgpygtk/pyvserv
-    collected 9 items
+    rootdir: /home/<homedir>/pgpygtk/pyvserv
+    collected 15 items
 
-    test_afirst.py .                                                         [ 11%]
-    test_file.py .                                                           [ 22%]
+    test_afirst.py .                                                         [  6%]
+    test_file.py ..                                                          [ 20%]
+    test_hello.py .                                                          [ 26%]
     test_help.py .                                                           [ 33%]
-    test_id.py .                                                             [ 44%]
-    test_key.py .                                                            [ 55%]
-    test_login.py .                                                          [ 66%]
-    test_sess.py ..                                                          [ 88%]
+    test_id.py .                                                             [ 40%]
+    test_key.py .                                                            [ 46%]
+    test_login.py .                                                          [ 53%]
+    test_noadmn.py .                                                         [ 60%]
+    test_rget.py .                                                           [ 66%]
+    test_rput.py .                                                           [ 73%]
+    test_sess.py ..                                                          [ 86%]
+    test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
-    ============================== 9 passed in 1.35s ===============================
+    ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the test directory. The pyvcli_* files may also
+Additional tests can be found in the tests/ directory. The pyvcli_* files may also
 serve as test cases.
 
+More test coming soon ....
+
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
@@ -181,23 +255,39 @@
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
   All views monitor the live files, on the default setup, without interfering
 with any of the operations.
 
+## Windows compatibility
+
+ Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+functionalities are ported. The file locking mechanism works, and all the
+pytests pass. Naturally, logging and readline etc ... works with the usual
+windows caveat.
+
+  For the GUI functions install the PyGobject subsystem. Instructions can
+be found very easily for that. Below, a screenshot of the pyvserv control panel
+in MSYS2.
+
+![Screen Shot](winscreen.png)
+
+The project is functional in MSYS2, but for real deployment we recommend Linux.
+
 ## History:
 
  Recent history kept, for the full list of changes consult the github site.
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
+    1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
 
 ## Statistics
 
     Project name
         pyvserv
     Report Period
         2018-12-31 20:50:04 to 2024-03-15 04:47:25
```

### Comparing `pyvserv-1.0.2/pyvclient/loadtest.py` & `pyvserv-1.0.3/pyvclient/loadtest.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_acc.py` & `pyvserv-1.0.3/pyvclient/pyvcli_ls.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, datetime
 
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5
+from Crypto.PublicKey import RSA
 from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
@@ -88,33 +89,15 @@
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Response:", resp3)
-    resp3 = hand.client(["tout",] , conf.sess_key, False)
-    print("Response:", resp3)
-
-    coms = [ \
-        "ver",           "id",            "hello",         "helo",
-        "help",          "xkey",          "ekey",          "akey",
-        "uini",          "kadd",          "user",          "pass",
-        "sess",          "tout",          "file",          "mkdir",
-        "data",          "fget",          "fput",          "del",
-        "uadd",          "uena",          "aadd",          "udel",
-        "ls",            "lsd",           "cd",            "pwd",
-        "stat",          "buff",          "chpass",        ]
-
-    # test out of order commands
-    for aa in coms:
-        print("exec", aa + ':', end=" ")
-        resp3 = hand.client([aa,] , conf.sess_key, False)
-        print("Response:", resp3)
+    print("Hello Response:", resp3)
 
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3)
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
@@ -130,30 +113,55 @@
     ret =  hand.login("admin", "1234", conf)
     if ret[0] != "OK":
         print ("Server login fail:", ret)
         hand.client(["quit"], conf.sess_key)
         hand.close();
         sys.exit(0)
 
-    print("-------------------------------------")
-
     cresp = hand.client(["buff", "10000000",], conf.sess_key)
     print ("Server buff response:", cresp)
     if cresp[0] != "OK":
         print("Error on buff command", cresp[1])
         hand.client(["quit"], conf.sess_key)
         hand.close();
         sys.exit(0)
 
+    cresp = hand.client(["ls", ], conf.sess_key)
+    print ("Server  ls response:", cresp)
+    if cresp[0] != "OK":
+        print("Error on listing directory:", cresp[1])
+        hand.client(["quit"], conf.sess_key)
+        hand.close();
+        sys.exit(0)
 
-     # test in order commands now good
-    for aa in coms:
-        print("exec", aa + ':', end=" ")
-        resp3 = hand.client([aa,] , conf.sess_key, False)
-        print("Response:", resp3)
+    ''' Stat return values are as in python os.stat() + OK and name prefix
+    "OK", fname (1),
+    st_mode (2), st_ino, st_dev, st_nlink
+    st_uid, st_gid, st_size (8)
+    st_atime (9), st_mtime, st_ctime
+    st_atime_ns
+    st_mtime_ns
+    st_ctime_ns '''
+
+    print ("Server stat response:")
+    for aa in cresp[1:]:
+        bb = support.unescape(aa)
+        cresp2 = hand.client(["stat", aa], conf.sess_key)
+        #print("cresp2", cresp2)
+        if cresp2[0] != "OK":
+            print("Bad entry from remote", cresp2)
+        else:
+            ddd = datetime.datetime.fromtimestamp(int(cresp2[10]))
+            print ("%s %-24s %-8d %s" %
+                (
+                support.mode2str(int(cresp2[2])), support.unescape(cresp2[1]),
+                        int(cresp2[8]), ddd)
+                )
+            #int(cresp2[9]), int(cresp2[10]), int(cresp2[11])
+            #print(ddd)
 
     hand.client(["quit",],conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_akey.py` & `pyvserv-1.0.3/pyvclient/pyvcli_akey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_bigget.py` & `pyvserv-1.0.3/pyvclient/pyvcli_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 #!/usr/bin/env python
 
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
-
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
 base = os.path.dirname(os.path.realpath(__file__))
@@ -26,121 +21,123 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
-    print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
-    ["f:",  "file",     6666,   None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["n",   "plain",    0,      None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
-    #print(dir(conf))
-
-    #if conf.comm:
-    #    print("Save to filename", conf.comm)
-
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
-    #hand.comm  = conf.comm
-
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #resp3 = hand.client(["id",] , "", False)
-    #print("ID Response:", resp3[1])
+    if conf.verbose:
+        resp3 = hand.client(["hello",] , "", False)
+        print("Hello Response:", resp3[1])
 
-    #ret = ["OK",];  conf.sess_key = ""
+    #conf.sess_key = ""    #ret = ["OK",]
     ret = hand.start_session(conf)
+
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
-
-    if conf.sess_key:
-        print("Post session, session key:", conf.sess_key[:12], "...")
-
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello Response:", resp3)
+    #print("Post session, all is encrypted")
 
     # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
-
-    cresp = hand.login("admin", "1234", conf)
-    print ("Server login response:", cresp)
+    resp4 = hand.client(["hello",], conf.sess_key)
+    if conf.verbose:
+        print("Hello (plain) Response:", resp4)
+        #print("Hello (encrypted) Response:", resp4[1])
+
+    cresp = hand.client(["user", "admin"], conf.sess_key)
+    #print ("Server user response:", cresp[1])
+
+    cresp = hand.client(["pass", "1234"], conf.sess_key)
+    #print ("Server pass response:", cresp[1])
+
+    if conf.verbose:
+        cresp = hand.client(["ls", ], conf.sess_key)
+        print ("Server  ls response:", cresp)
+
+    cresp = hand.client(["file", "zeros"], conf.sess_key)
+    print ("Server file response:", cresp)
+    if cresp[0] != "OK":
+        #print("Err: ", cresp)
+        cresp = hand.client(["quit", ], conf.sess_key)
+        print ("Server quit response:", cresp)
+        sys.exit(0)
 
-    #cresp = hand.client(["ls", ], conf.sess_key)
-    #print ("Server  ls response:", cresp)
+    fp = open("zeros_local", "rb")
+    offs = 0
+    while 1:
+        buf = fp.read(1024)
+        #print("sending", buf)
+        cresp = hand.client(["data", offs, buf], conf.sess_key)
+        if conf.verbose:
+            print ("Server data response:", cresp)
+        if cresp[0] != "OK":
+            print("Cannot send", cresp)
+            break
+        blen = len(buf)
+        if blen == 0:
+            break
 
-    #cresp = hand.client(["buff", "10", ], conf.sess_key)
-    #print ("Server buff response:", cresp)
-    #if cresp[0] != "OK":
-    #    print("Error on buff command", cresp[1])
-    #    hand.client(["quit"], conf.sess_key)
-    #    hand.close();
-    #    sys.exit(0)
-
-    #zfile = "zeros"
-    #ret2 = hand.getfile(zfile, zfile+"_local", conf.sess_key)
-    #print ("Server  fget response:", ret2)
-
-    bfile ="bigfile"
-    print("Started bigfile ...", bfile)
-    ttt = time.time()
-    ret = hand.getfile(bfile, bfile + "_local", conf.sess_key)
-    filesize = support.fsize(bfile+ "_local")
-    print("filesize", filesize)
-    rate = filesize / (time.time() - ttt)
-    print ("Server fget response:", ret, "time %.2f kbytes/sec" % (rate/1024))
+        offs += blen
 
     cresp = hand.client(["quit", ], conf.sess_key)
     print ("Server quit response:", cresp)
 
     sys.exit(0)
 
 
+
+
+
+
+
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_cd.py` & `pyvserv-1.0.3/pyvclient/pyvcli_cd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_cli.py` & `pyvserv-1.0.3/pyvclient/pyvcli_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,40 @@
 #!/usr/bin/env python
 
-import sys, os, readline, atexit
+import sys, os, atexit
+
+try:
+    import readline
+except:
+    pass
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
+# ------------------------------------------------------------------------
+# Test client for the pyserv project.
+
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
+
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
+
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
+
 __doc__ = \
 ''' Test unit for pyvserv. Command line interpreter. This interface is similar
     to the FTP client interface. Some functions are sent through directly,
     and some functions are interpreted via client helpers.
     All encryption functionality is exercised as the real client would.
     The command that starts with the exclamation point is executed
     in the local shell.
@@ -51,26 +76,14 @@
         qr                              -- Get qrcode image for 2fa
         twofa                           -- Two factor authentication
         dmode                           -- Get dmode (Developer Mode) flag
         ihave                           -- The 'i have you have' protocol entry point
         ihost                           -- Add / delete replicator host
 
 '''
-
-# ------------------------------------------------------------------------
-# Test client for the pyserv project. Download file.
-
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
-
-from pyvcli_utils import *
-
-from pyvcommon import support, pycrypt, pyclisup
-from pyvcommon import pysyslog, comline
-
 # ------------------------------------------------------------------------
 # Globals
 
 version = 1.0
 
 # ------------------------------------------------------------------------
 
@@ -78,17 +91,20 @@
 
     ''' Provide local help '''
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
+    print( "            -l login  - Login Name; default: 'user'")
+    print( "            -s lpass  - Login Pass; default: '1234'")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
+    print( "            -x comm   - Execute command and quit")
     print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
 
@@ -97,14 +113,17 @@
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",    None],      \
+    ["x:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
@@ -132,60 +151,73 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    atexit.register(atexit_func, hand, conf)
+    atexit.register(pyclisup.atexit_func, hand, conf)
 
-    #resp3 = hand.client(["id",] , "", False)
-    #print("ID Response:", resp3[1])
+    resp3 = hand.client(["id",] , "", False)
+    if not conf.quiet:
+        print("ID Response:", resp3[1])
 
     conf.sess_key = ""
     #ret = ["OK",];  conf.sess_key = ""
     resp3 = hand.start_session(conf)
     if resp3[0] != "OK":
         print("Error on setting session:", resp3[1])
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
 
     if conf.sess_key:
-        print(" ------ Post session, session key:", conf.sess_key[:12], "...")
+        if not conf.quiet:
+            print(" ------ Post session, session key:", conf.sess_key[:12], "...")
 
     resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello Resp:", resp3)
-
-    # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
+    if not conf.quiet:
+        print("Hello Resp:", resp3)
 
-    cresp = hand.login("admin", "1234", conf)
-    print ("Login resp:", cresp)
+    cresp = hand.login(conf.login, conf.lpass, conf)
+    if not conf.quiet:
+        print ("Login resp:", cresp)
+    if cresp[0] != "OK":
+        print("Error on logging in, exiting.")
+        sys.exit(1)
 
     # Start a new session for the rest of the work
     resp3 = hand.start_session(conf)
     if resp3[0] != "OK":
         print("Error on setting session:", resp3[1])
         sys.exit(0)
 
     if conf.sess_key:
-        print(" ------ Post session, session key:", conf.sess_key[:12], "...")
+        if not conf.quiet:
+            print(" ------ Post session, session key:", conf.sess_key[:12], "...")
 
     resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello2 Resp:", resp3)
+    if not conf.quiet:
+        print("Hello2 Resp:", resp3)
 
     # Interactive, need more time
     hand.client(["tout", "30",], conf.sess_key)
 
-    print ("Enter commands, Ctrl-C or 'done' to quit. Prefix local commands with '!'")
-
-    mainloop(conf, hand)
+    if conf.comm:
+        import shlex
+        #print("exec:", conf.comm)
+        commx = shlex.split(conf.comm)
+        if not conf.quiet:
+            print("Issue:", commx)
+        resp = hand.client([*commx], conf.sess_key)
+        print("resp:", resp)
+    else:
+        print ("Enter commands, Ctrl-C or 'done' to quit. Prefix local commands with '!'")
+        mainloop(conf, hand)
 
     sys.exit(0)
 
 
 def mainloop(conf, hand):
 
     ''' Loop through commands and provide interpretation / execution on
@@ -244,7 +276,9 @@
                     print ("Server response:", cresp)
         except:
             print(sys.exc_info())
             break
 
 if __name__ == '__main__':
     mainfunct()
+
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_fdel.py` & `pyvserv-1.0.3/pyvclient/pyvcli_fdel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_fget.py` & `pyvserv-1.0.3/pyvclient/pyvcli_fget.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_file.py` & `pyvserv-1.0.3/pyvclient/pyvcli_login.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,138 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+from __future__ import print_function
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Download file.
+# Test client for the pyserv project. Encrypt test.
 
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
+from Crypto.Hash import SHA512
+import  os, sys, getopt, signal, select, socket, time, struct
+import  random, stat
+
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_v1_5
+from Crypto.PublicKey import RSA
+from Crypto.Hash import SHA
+from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
-# Globals
-
-version = 1.0
-
-# ------------------------------------------------------------------------
+# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p port   - Port to use (default: 6666)")
+    print( "            -l level  - Log level (default: 0)")
+    print( "            -c file   - Save comm to file")
+    print( "            -s        - Showkey")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
+    #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", version)
+    print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
+    ["c:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
+    ["s",   "showkey",  "",     None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
+    if conf.comm:
+        print("Save to filename", conf.comm)
+
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
+    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    if conf.verbose:
-        resp3 = hand.client(["hello",] , "", False)
-        print("Hello Response:", resp3[1])
+    resp3 = hand.client(["hello", "world"] , "", False)
+    print("Hello Response: ", resp3)
 
-    #conf.sess_key = ""    #ret = ["OK",]
     ret = hand.start_session(conf)
 
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
+    print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
     #print("Post session, all is encrypted")
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    if conf.verbose:
-        print("Hello (plain) Response:", resp4)
-        #print("Hello (encrypted) Response:", resp4[1])
+    print("Server hello Response:", resp4[1])
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print ("Server user response:", cresp[1])
+    print ("Server user  response:", cresp)
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
+    print ("Server pass  response:", cresp)
 
-    if conf.verbose:
-        cresp = hand.client(["ls", ], conf.sess_key)
-        print ("Server  ls response:", cresp)
-
-    cresp = hand.client(["file", "zeros"], conf.sess_key)
-    print ("Server file response:", cresp)
-    if cresp[0] != "OK":
-        #print("Err: ", cresp)
-        cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
-        sys.exit(0)
+    #resp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass  response:", cresp)
 
-    fp = open("zeros_local", "rb")
-    offs = 0
-    while 1:
-        buf = fp.read(1024)
-        #print("sending", buf)
-        cresp = hand.client(["data", offs, buf], conf.sess_key)
-        if conf.verbose:
-            print ("Server data response:", cresp)
-        if cresp[0] != "OK":
-            print("Cannot send", cresp)
-            break
-        blen = len(buf)
-        if blen == 0:
-            break
-
-        offs += blen
-
-    cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
-
-    sys.exit(0)
+    #resp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass response:", cresp)
 
+    #cresp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass response:", cresp[1])
+    #if(cresp[1][:2] != "OK"): sys.exit(1)
 
+    #cresp = hand.client(["pass", "1234"], conf.sess_key)
+    #print ("Server pass  response:", cresp[1])
 
+    #cresp = hand.client(["hello", "1234"], conf.sess_key)
+    #print ("Server hello response:", cresp[1])
 
+    cresp = hand.client(["quit",],conf.sess_key)
+    print ("Server quit  response:", cresp[1])
+    hand.close();
 
+    sys.exit(0)
 
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_fput.py` & `pyvserv-1.0.3/pyvclient/pyvcli_fput.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -f fname  - Send file")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
@@ -83,23 +83,18 @@
 
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
-    #print("Post session, all is encrypted")
-
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
     if conf.verbose:
         print("Hello (plain) Response:", resp4)
-        #print("Hello (encrypted) Response:", resp4[1])
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
     #print ("Server user response:", cresp[1])
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
     #print ("Server pass response:", cresp[1])
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_gethelp.py` & `pyvserv-1.0.3/pyvclient/pyvcli_gethelp.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,27 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. User add.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
 myhandler = None
 mydathand = None
 pgdebug = 0
@@ -103,15 +111,15 @@
         print( "Received: '%s'" % response)
 
     return response
 '''
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
@@ -143,17 +151,13 @@
         print ("Server response:", resp)
 
     hand.client(["quit",])
     hand.close();
 
     sys.exit(0)
 
-# EOF
-
-
-
-
-
-
-
+#def mainfunct():
 
+if __name__ == '__main__':
+    mainfunct()
 
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_hello.py` & `pyvserv-1.0.3/pyvclient/pyvcli_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 #!/usr/bin/env python3
 
 from __future__ import print_function
 
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
+
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
 base = os.path.dirname(os.path.realpath(__file__))
@@ -62,15 +67,15 @@
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     if conf.quiet == False:
         respini = hand.pb.decode_data(resp2[1])[0]
         print ("Server initial:", respini)
 
-    resp = hand.client(["hello"])
+    resp = hand.client(["id"])
     if conf.quiet == False:
         print("resp", resp)
 
     resp2 = hand.client(["quit"])
     if conf.quiet == False:
         print ("Server quit response:", resp2)
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_id.py` & `pyvserv-1.0.3/pyvclient/pyvcli_hello.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python3
 
 from __future__ import print_function
 
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
-
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
 optarr =  comline.optarr
 optarr.append ( ["p:",  "port",     6666,   None, "Port to use (default: 6666)"] )
 
 #print (optarr)
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
     if sys.version_info[0] < 3:
         print("Warning! This script was meant for python 3.x")
         time.sleep(1)
 
     args = conf.comline(sys.argv[1:])
 
@@ -67,20 +70,23 @@
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     if conf.quiet == False:
         respini = hand.pb.decode_data(resp2[1])[0]
         print ("Server initial:", respini)
 
-    resp = hand.client(["id"])
+    resp = hand.client(["hello"])
     if conf.quiet == False:
         print("resp", resp)
 
     resp2 = hand.client(["quit"])
     if conf.quiet == False:
         print ("Server quit response:", resp2)
 
     hand.close();
 
     sys.exit(0)
 
+if __name__ == '__main__':
+    mainfunct()
+
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_ihost.py` & `pyvserv-1.0.3/pyvclient/pyvcli_ihost.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_login.py` & `pyvserv-1.0.3/pyvclient/pyvcli_pass.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
+
+'''
+# test encrypt with large keys
+rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
+        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
+sss = bluepy.encrypt(rrr, conf.sess_key)
+ttt = bluepy.decrypt(sss, conf.sess_key)
+print (rrr)
+print (ttt)
+'''
+
 # ------------------------------------------------------------------------
 # Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
@@ -83,56 +94,45 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello", "world"] , "", False)
-    print("Hello Response: ", resp3)
+    resp3 = hand.client(["hello",] , "", False)
+    print("Hello Response:", resp3[1])
 
     ret = hand.start_session(conf)
 
+    #if ret[0] == "OK":
+    #    print("Sess Key ACCEPTED:",  ret[1])
+
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
-    #print("Post session, all is encrypted")
+    #print("Sess Key ACCEPTED:",  resp3[1])
+    print("Post session, all is encrypted")
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    print("Server hello Response:", resp4[1])
+    print("Hello sess Response:", resp4)
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    print ("Server user  response:", cresp)
+    print ("Server user response:", cresp[1])
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    print ("Server pass  response:", cresp)
-
-    #resp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass  response:", cresp)
-
-    #resp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass response:", cresp)
-
-    #cresp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
-    #if(cresp[1][:2] != "OK"): sys.exit(1)
-
-    #cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass  response:", cresp[1])
+    print ("Server pass response:", cresp[1])
 
-    #cresp = hand.client(["hello", "1234"], conf.sess_key)
-    #print ("Server hello response:", cresp[1])
+    #cresp = hand.client(["chpass", "1234"], conf.sess_key)
+    #print ("Server chpass response:", cresp[1])
 
-    cresp = hand.client(["quit",],conf.sess_key)
-    print ("Server quit  response:", cresp[1])
+    hand.client(["quit",], conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_ls.py` & `pyvserv-1.0.3/pyvclient/pyvcli_uman.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,168 +1,151 @@
-#!/usr/bin/env python3
-
-from __future__ import print_function
-
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
+#!/usr/bin/env python
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project. User add.
 
-from Crypto.Hash import SHA512
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, datetime
-
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
-from Crypto import Random
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
-# Functions from command line
+# Globals
+
+version = 1.0
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -s        - Showkey")
+    print( "            -p        - Port to use (default: 6666)")
+    print( "            -l login  - Login Name; default: 'user'")
+    print( "            -s lpass  - Login Pass; default: '1234'")
+    print( "            -u user   - User Name; default: 'user'")
+    print( "            -a        - Add user. Must be unique.")
+    print( "            -r        - Remove user (one of add or remove needed.")
+    print( "            -u user   - User Name; default: 'user'")
+    print( "            -p pass   - User pssword; default: '1234' (!!! for tests only)")
+    print( "            -m        - Add admin instead of regular user")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
-    #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", support.version)
+    print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",    None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["m",   "admin",    0,          None],      \
+    ["a",   "add",      0,          None],      \
+    ["r",   "remove",    0,         None],      \
+    ["u:",  "userx",    "user",     None],      \
+    ["p:",  "passx",    "1234",     None],      \
+    ["t",   "prompt",    0,         None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
+conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def    mainfunct():
 
-    args = conf.comline(sys.argv[1:])
+    '''if  sys.version_info[0] < 3:
+        print(("Needs python 3 or better."))
+        sys.exit(1)'''
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    args = conf.comline(sys.argv[1:])
 
-    pyclisup.verbose = conf.verbose
-    pyclisup.pgdebug = conf.pgdebug
+    if not conf.add and not conf.remove:
+        print("One of Add / Remove [ -a | -r ] should be specified.")
+        sys.exit()
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello Response:", resp3)
-
-    ret = hand.start_session(conf)
-    if ret[0] != "OK":
-        print("Error on setting session:", resp3)
-        hand.client(["quit"])
-        hand.close();
-        sys.exit(0)
+    resp3 = hand.start_session(conf)
+    print("Sess Response:", resp3)
 
-    # Make a note of the session key
-    #print("Session Key ACCEPTED:",  ret, )
-    print("Session, with key:", conf.sess_key[:12], "...")
-
-    # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
-
-    ret =  hand.login("admin", "1234", conf)
-    if ret[0] != "OK":
-        print ("Server login fail:", ret)
-        hand.client(["quit"], conf.sess_key)
-        hand.close();
-        sys.exit(0)
+    resp3 = hand.client(["hello",] , conf.sess_key, False)
+    print("Hello sess Response:", resp3[1])
 
-    cresp = hand.client(["buff", "10000000",], conf.sess_key)
-    print ("Server buff response:", cresp)
-    if cresp[0] != "OK":
-        print("Error on buff command", cresp[1])
+    resp = hand.client(["user", conf.login], conf.sess_key)
+    print("user Response:", resp)
+    if resp[0] != "OK":
         hand.client(["quit"], conf.sess_key)
         hand.close();
-        sys.exit(0)
 
-    cresp = hand.client(["ls", ], conf.sess_key)
-    print ("Server  ls response:", cresp)
-    if cresp[0] != "OK":
-        print("Error on listing directory:", cresp[1])
+    resp = hand.client(["pass", conf.lpass], conf.sess_key)
+    print("pass Response:", resp)
+    if resp[0] != "OK":
         hand.client(["quit"], conf.sess_key)
         hand.close();
-        sys.exit(0)
+        print("Error on authentication, exiting.")
+        sys.exit(1)
 
-    ''' Stat return values are as in python os.stat() + OK and name prefix
-    "OK", fname (1),
-    st_mode (2), st_ino, st_dev, st_nlink
-    st_uid, st_gid, st_size (8)
-    st_atime (9), st_mtime, st_ctime
-    st_atime_ns
-    st_mtime_ns
-    st_ctime_ns '''
-
-    print ("Server stat response:")
-    for aa in cresp[1:]:
-        bb = support.unescape(aa)
-        cresp2 = hand.client(["stat", aa], conf.sess_key)
-        #print("cresp2", cresp2)
-        if cresp2[0] != "OK":
-            print("Bad entry from remote", cresp2)
+    if conf.prompt:
+        import getpass
+        #print("Pass for new user %s:" % conf.userx, end = " ");
+        #sys.stdout.flush()
+        #strx = input()
+        strx = getpass.getpass("Pass for new user %s: " % conf.userx)
+        if not strx:
+            print("Aborting ...")
+            sys.exit(0)
+        conf.passx = strx
+    if conf.add:
+        if conf.admin:
+            resp = hand.client(["aadd", conf.userx, conf.passx], conf.sess_key)
         else:
-            ddd = datetime.datetime.fromtimestamp(int(cresp2[10]))
-            print ("%s %-24s %-8d %s" %
-                (
-                support.mode2str(int(cresp2[2])), support.unescape(cresp2[1]),
-                        int(cresp2[8]), ddd)
-                )
-            #int(cresp2[9]), int(cresp2[10]), int(cresp2[11])
-            #print(ddd)
+            resp = hand.client(["uadd", conf.userx, conf.passx], conf.sess_key)
+        print("uadd Response:", resp)
+    elif conf.remove:
+        resp = hand.client(["udel", conf.userx, conf.passx], conf.sess_key)
+        print("udel Response:", resp)
 
-    hand.client(["quit",],conf.sess_key)
+    hand.client(["quit"], conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
-# EOF
+if __name__ == '__main__':
+    mainfunct()
 
+
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_lsd.py` & `pyvserv-1.0.3/pyvclient/pyvcli_lsd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_mkdir.py` & `pyvserv-1.0.3/pyvclient/pyvcli_mkdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level   - Debug level 0-10")
     print( "            -c dirname - Directory to create. default: test_3")
-    print( "            -p         - Port to use (default: 9999)")
+    print( "            -p         - Port to use (default: 6666)")
     print( "            -v         - Verbose")
     print( "            -q         - Quiet")
     print( "            -n         - No encryption (plain)")
     print( "            -h         - Help")
     print()
     sys.exit(0)
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_pass.py` & `pyvserv-1.0.3/pyvclient/pyvcli_bigget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,138 +1,166 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
-from __future__ import print_function
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project. Download file.
 
-from Crypto.Hash import SHA512
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
-
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
-from Crypto import Random
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
+# ------------------------------------------------------------------------
+# Globals
 
-'''
-# test encrypt with large keys
-rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
-        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
-sss = bluepy.encrypt(rrr, conf.sess_key)
-ttt = bluepy.decrypt(sss, conf.sess_key)
-print (rrr)
-print (ttt)
-'''
+version = 1.0
 
 # ------------------------------------------------------------------------
-# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -s        - Showkey")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
+    print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
-    #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", support.version)
+    print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
+    ["f:",  "file",     6666,   None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
+    ["n",   "plain",    0,      None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    #print(dir(conf))
+
+    #if conf.comm:
+    #    print("Save to filename", conf.comm)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
+
+    #hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello",] , "", False)
-    print("Hello Response:", resp3[1])
+    #resp3 = hand.client(["id",] , "", False)
+    #print("ID Response:", resp3[1])
 
+    #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
-
-    #if ret[0] == "OK":
-    #    print("Sess Key ACCEPTED:",  ret[1])
-
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
-    print("Post session, all is encrypted")
 
-    # Session estabilished, try a simple command
-    resp4 = hand.client(["hello",], conf.sess_key)
-    print("Hello sess Response:", resp4)
-
-    cresp = hand.client(["user", "admin"], conf.sess_key)
-    print ("Server user response:", cresp[1])
+    if conf.sess_key:
+        if not conf.quiet:
+            print("Post session, session key:", conf.sess_key[:12], "...")
+
+    resp3 = hand.client(["hello", ],  conf.sess_key, False)
+    if not conf.quiet:
+        print("Hello Response:", resp3)
 
-    cresp = hand.client(["pass", "1234"], conf.sess_key)
-    print ("Server pass response:", cresp[1])
+    # Session estabilished, try a simple command
+    #resp4 = hand.client(["hello",], conf.sess_key)
+    #print("Hello Response:", resp4[1])
 
-    #cresp = hand.client(["chpass", "1234"], conf.sess_key)
-    #print ("Server chpass response:", cresp[1])
+    cresp = hand.login("admin", "1234", conf)
+    if not conf.quiet:
+        print ("Server login response:", cresp)
+
+    bigfname = "bigfile"    # Use this name for cleaning it
+    bigbuff = b"a" * 1024
+    # Create bigfile
+    fp = open(bigfname, "wb")
+    for aa in range(1024 * 20):
+        fp.write(bigbuff)
+    fp.close()
+
+    # Put big file up
+    print("Started file UP ...", )
+    ttt = time.time()
+    resp = hand.putfile(bigfname, "", conf.sess_key)
+    filesize = support.fsize(bigfname)
+    rate = filesize / (time.time() - ttt)
+    if not conf.quiet:
+        print("filesize", filesize)
+    if resp[0] != "OK":
+        print ("fput resp:", resp)
+        cresp = hand.client(["quit", ], conf.sess_key)
+        print ("Server quit response:", cresp)
+        sys.exit()
+    print ("fput response:", resp, "time %.2f kbytes/sec" % (rate/1024))
+
+    print("Started bigfile DOWN")
+    ttt = time.time()
+    ret = hand.getfile(bigfname, bigfname + "_local", conf.sess_key)
+    filesize = support.fsize(bigfname + "_local")
+    if not conf.quiet:
+        print("filesize", filesize)
+    rate = filesize / (time.time() - ttt)
+    print ("fget response:", ret, "time %.2f kbytes/sec" % (rate/1024))
+
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
+
+    ret = os.system("diff " + bigfname + " " + bigfname + "_local")
+    if ret:
+        print("Error: Files Differ", ret)
+    else:
+        print("Files Compare OK")
 
-    hand.client(["quit",], conf.sess_key)
-    hand.close();
+    os.remove(bigfname)
+    os.remove(bigfname + "_local")
 
     sys.exit(0)
 
-# EOF
-
+ # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_ping.py` & `pyvserv-1.0.3/pyvclient/pyvcli_ping.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_qr.py` & `pyvserv-1.0.3/pyvclient/pyvcli_qr.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 import readline
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Download file.
+# Test client for the pyserv project.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-#sys.path.append(os.path.join(base,  '../pyvcommon'))
-sys.path.append(os.path.join(base,  '..'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
@@ -29,15 +36,16 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
+    print( "            -f file   - Upload new QR image file")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
@@ -45,32 +53,31 @@
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
-    ["f:",  "file",     6666,   None],      \
+    ["f:",  "file",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
     ["n",   "plain",    0,      None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-def mainfunc():
+def mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
     #print(vars(conf))
-
     #if conf.comm:
     #    print("Save to filename", conf.comm)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
@@ -78,76 +85,45 @@
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
-    #hand.comm  = conf.comm
-
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["qr",] , "", False)
-    #print("QR Response:", resp3[1])
-    fp = open("qr.png", 'wb')
-    fp.write(resp3[1])
-    fp.close()
-
-    hand.sock.shutdown(socket.SHUT_RDWR)
-    sys.exit(0)
+    conf.sess_key = ""
+    #ret = ["OK",];  conf.sess_key = ""
+    resp3 = hand.start_session(conf)
+    if resp3[0] != "OK":
+        print("Error on setting session:", resp3[1])
+        sys.exit(0)
+
+    if conf.file:
+        fp = open(conf.file, "rb")
+        buff = fp.read()
+        fp.close()
+        #print("len:", len(buff))
+        resp3 = hand.client(["qr", buff], conf.sess_key, False)
+        print("QR UP Response:", resp3)
+    else:
+        resp3 = hand.client(["qr",], conf.sess_key, False)
+        #print("QR Response:", resp3)
+        fp = open("qr.png", 'wb')
+        if type(resp3[1]) != type(b""):
+            resp3[1] = resp3[1].encode()
+        fp.write(resp3[1])
+        fp.close()
 
-def mainloop(conf, hand):
+    hand.client(["quit"], conf.sess_key)
+    hand.close();
 
-    while(True):
-        try:
-            onecom = input(">> ")
-            #print ("'" + onecom.split() + "'")
-            ss = onecom.split()
-            if ss  != []:
-                # process commands that need additional data
-                if ss[0] == "done":
-                    break
-                elif ss[0] == "sess":
-                    cresp = hand.start_session(conf)
-                    if conf.sess_key:
-                        print("Post session, session key:", conf.sess_key[:12], "...")
-
-                elif ss[0] == "fget":
-                    if len(ss) < 2:
-                        print("Use: fget fname")
-                        continue
-                    ret2 = hand.getfile(ss[1], "", conf.sess_key)
-                    print ("Server fget response:", ret2)
-
-                elif ss[0] == "fput":
-                    if len(ss) < 2:
-                        print("Use: fput fname")
-                        continue
-                    ret2 = hand.putfile(ss[1], "", conf.sess_key)
-                    print ("Server fput response:", ret2)
-
-                elif ss[0] == "file":
-                    if not os.path.isfile(ss[1]):
-                        print("File must exist.")
-                        continue
-                    cresp = hand.start_session(conf)
-                    if conf.sess_key:
-                        print("Post session, session key:", conf.sess_key[:12], "...")
-                if ss[0][0] == "!":
-                    #print ("local command")
-                    os.system(ss[0][1:] + " " + " ".join(ss[1:]))
-                    continue
-                else:
-                    # No wrapper needed
-                    cresp = hand.client(ss, conf.sess_key)
-                print ("Server response:", cresp)
-
-        except:
-            print(sys.exc_info())
-            break
+    sys.exit(0)
 
 if __name__ == '__main__':
-    mainfunc()
+    mainfunct()
+
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_replic.py` & `pyvserv-1.0.3/pyvclient/pyvcli_replic.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,46 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat, datetime, atexit
 
-from pyvcli_utils import *
+#from pyvcli_utils import *
+
+# This repairs the path from local run to pip run.
+# Remove pip version for local tests
+
+try:
+    from pyvcommon import support
+    #print("sf", sf)
+    # Get Parent of module root
+    sf = os.path.dirname(support.__file__)
+    sf = os.path.dirname(sf)
+    sys.path.append(os.path.join(sf, "pyvcommon"))
+    sys.path.append(os.path.join(sf, "pyvserver"))
+except:
+    #print("pathching")
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    sys.path.append(os.path.join(base,  '..', "pyvserver"))
+    from pyvcommon import support
+
+def atexit_func(hand, conf):
+
+    ''' Severe connection on exit '''
+
+    try:
+        print("Atexit")
+        cresp = hand.client(["quit", ], conf.sess_key)
+        print ("Server quit response:", cresp)
+        hand.close();
+    except:
+        pass
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 hand = None
 hand2 = None
 
@@ -28,15 +59,15 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_rget.py` & `pyvserv-1.0.3/pyvclient/pyvcli_rget.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,27 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat, datetime
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
 version = 1.0
 
 # ------------------------------------------------------------------------
@@ -58,15 +66,15 @@
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def    mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
     #print(dir(conf))
 
     #if conf.comm:
     #    print("Save to filename", conf.comm)
@@ -170,8 +178,11 @@
                 #print("aa", aa)
                 dec = hand.pb.decode_data(aa[1])
                 print("dec:", dec[0]['header'], dec[0]['now'], dec[0]['payload'])
 
     cresp = hand.client(["quit", ], conf.sess_key)
     print ("Server quit response:", cresp)
 
+if __name__ == '__main__':
+    mainfunct()
+
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_rlist.py` & `pyvserv-1.0.3/pyvclient/pyvcli_rlist.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,24 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat, datetime, uuid, atexit
 
-from pyvcli_utils import *
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
@@ -25,15 +34,15 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -s        - Start time. Format: 'Y-m-d H:M'")
     print( "            -i        - Interval in minutes. (Default: 1 day)")
     print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
@@ -56,15 +65,15 @@
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
     #print(dir(conf))
 
     #if conf.comm:
     #    print("Save to filename", conf.comm)
@@ -83,15 +92,15 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    atexit.register(atexit_func, hand, conf)
+    atexit.register(pyclisup.atexit_func, hand, conf)
 
     #resp3 = hand.client(["id",] , "", False)
     #print("ID Response:", resp3[1])
 
     #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
     if ret[0] != "OK":
@@ -139,8 +148,11 @@
         if cresp[0] == "OK":
             for aa in cresp[1]:
                 #print("aa", aa)
                 if aa:
                     ttt = pyservsup.uuid2date(uuid.UUID(aa))
                     print(aa, ":", ttt)
 
+if __name__ == '__main__':
+    mainfunct()
+
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_rput.py` & `pyvserv-1.0.3/pyvclient/pyvcli_sess.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 #!/usr/bin/env python3
 
+#from __future__ import print_function
+
+from pyvecc.Key import Key
+
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, uuid, atexit
-
-#from Crypto.Hash import SHA512
-#from Crypto.PublicKey import RSA
-#from Crypto.Cipher import PKCS1_v1_5
-#from Crypto.PublicKey import RSA
-#from Crypto.Hash import SHA
+import  random, stat, base64
 
+from Crypto.Hash import SHA256
 from Crypto import Random
 
-from pyvcli_utils import *
+base = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
-from pyvcommon import support, pycrypt, pyservsup, pyclisup, pyvhash
-from pyvcommon import pysyslog, comline
-
-import pyvpacker
+import support, pycrypt, pyservsup, pyclisup
+import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p port   - Port to use (default: 6666)")
     print( "            -l level  - Log level (default: 0)")
     print( "            -c file   - Save comm to file")
-    print( "            -k keyval - Put this key")
-    print( "            -n        - Number of records to put")
+    print( "            -s        - Showkey")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
@@ -49,25 +46,24 @@
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
     ["c:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["k:",  "putkey",   "",     None],      \
-    ["n:",  "numrec",   1,     None],      \
+    ["s",   "showkey",  "",     None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-def mainfunct():
+if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
     #print(vars(conf))
 
     if conf.comm:
         print("Save to filename", conf.comm)
 
@@ -80,117 +76,146 @@
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
     hand.comm  = conf.comm
 
-    atexit.register(atexit_func, hand, conf)
+    try:
+        respc = hand.connect(ip, conf.port)
+    except:
+        print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
+        sys.exit(1)
+
+    #print("IP:", ip, respc);
+    #print("Initial:", respc);
 
-    actstr = ["register", "unregister", "cast", "uncast", ]
-    act = actstr[random.randint(0, len(actstr)-1)]
+    resp = hand.client(["akey"], conf.sess_key)
+    #print("akey response", resp)
 
-    ttt = time.time()
-    pvh = pyvhash.BcData()
-    pvh.addpayload({"Vote": random.randint(0, 10), "UID":  str(uuid.uuid1()), })
-    pvh.addpayload({"SubVote": random.randint(0, 10), "TUID":  str(uuid.uuid1()), })
-    pvh.addpayload({"Action": act , "RUID":  str(uuid.uuid1()), })
-    #print(pvh.datax)
+    if resp[0] != "OK":
+        print("Error on getting key:", resp[1])
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
+
+    #if conf.pgdebug > 4:
+    #    print ("Server response2:\n" +  "'" + resp[1].decode("cp437") +  "'\n")
+
+    hhh = SHA256.new();
+    #hhh.update(bytes(resp[2], "utf-8"))
+    hhh.update(resp[2].encode())
+
+    if conf.pgdebug > 3:
+        print("Hash1:  '" + resp[1] + "'")
+        print("Hash2:  '" + hhh.hexdigest() + "'")
+
+    # Remember key
+    if hhh.hexdigest() !=  resp[1]:
+        print("Tainted key, aborting.")
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
+
+    hand.pkey = resp[2]
 
-    if conf.putkey:
-        pvh.datax['header'] = conf.putkey
+    #if conf.quiet == False:
+    #     print("Key response:", resp[0], resp[2][:32], "...")
 
-    pvh.hasharr();    pvh.powarr()
+    if conf.pgdebug > 4:
+         print(hand.pkey)
 
-    if not pvh.checkhash():
-        print("Error on hashing payload .. retrying ...")
-    elif not pvh.checkpow():
-        print("Error on POW payload .. retrying ...")
+    hand.pkey = resp[2]
+    #print("got FIRST key", hand.pkey)
 
-    if conf.verbose:
-        print(pvh.datax)
+    if conf.pgdebug > 2:
+        print ("Server response:", "'" + hhh.hexdigest() + "'")
 
-    #print("Chain cnt", pvh.cnt)
-    #print("chain %.3fms" % ((time.time() - ttt) * 1000) )
+    #if conf.showkey or conf.pgdebug > 5:
+    #    #print("Key:")
 
     try:
-        respc = hand.connect(ip, conf.port)
+        #hand.pubkey = RSA.importKey(hand.pkey)
+        hand.pubkey = Key.import_pub(hand.pkey)
+        if conf.pgdebug > 4:
+            print (hand.pubkey)
     except:
-        print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
-        sys.exit(1)
+        print("Cannot import public key.")
+        support.put_exception("import key")
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
 
-    resp3 = hand.client(["hello", "world"] , "", False)
-    print("Hello Resp:", resp3)
+    resp0 = hand.client(["hello",], )
+    print("Hello Plain:", resp0)
 
-    ret = hand.start_session(conf)
+    # Generate communication key
+    conf.sess_key = base64.b64encode(Random.new().read(128))
+    sss = SHA256.new(); sss.update(conf.sess_key)
 
-    if ret[0] != "OK":
-        print("Error on setting session:", resp3[1])
-        sys.exit(0)
+    if conf.pgdebug > 2:
+        support.shortdump("conf.sess_key", conf.sess_key )
 
-    # Make a note of the session key
-    if conf.verbose:
-        print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
+    sess_keyx  = hand.pubkey.encrypt(conf.sess_key)
+
+    ttt = SHA256.new(); ttt.update(sess_keyx.encode())
 
-    #print(" ----- Post session, all is encrypted ----- ")
+    if conf.pgdebug > 2:
+        support.shortdump("sess_keyx", sess_keyx )
+
+    resp3 = hand.client(["sess", sss.hexdigest(), ttt.hexdigest(), sess_keyx], "", False)
+    #print("Sess Response:", resp3)
 
-    #resp4 = hand.client(["tout", "30",], conf.sess_key)
-    #if resp4[0] != "OK":
-    #    print("Server tout Response:", resp4)
-    #    sys.exit()
+    if resp3[0] != "OK":
+        print("Error on setting session:", resp3)
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
+
+    # Make a note of the session key
+    print("Session key:", conf.sess_key[:24] , "..." )
 
-    #ttt = time.time()
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    #print("hello %.3fms" % ((time.time() - ttt) * 1000) )
-    if resp4[0] != "OK":
-        print("Server hello resp:", resp4[1])
-        sys.exit()
+    print("Encrypted Resp:", resp4)
 
-    #ttt = time.time()
-    cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print("user %.3fms" % ((time.time() - ttt) * 1000) )
-    print ("Server user respo:", cresp)
-
-    #ttt = time.time()
-    cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print("pass %.3fms" % ((time.time() - ttt) * 1000) )
-    if cresp[0] != "OK":
-        print("Cannot log on")
-        sys.exit(1)
-    print ("Server pass resp:", cresp)
+    # --------------------------------------------------------------------
+    # Generate communication key, second session and second run
 
-    cresp = hand.client(["dmode",], conf.sess_key)
-    #print("dmode", cresp)
-    if cresp[1] == '0':
-        print("Enter twofa code: (ret to skip)", end = "")
-        sesscode = input()
-        if sesscode:
-            cresp = hand.client(["twofa", sesscode], conf.sess_key)
-            print ("Server twofa resp:", cresp)
-            if cresp[0] != OK:
-                print ("Server twofa failed")
-                sys.exit(0)
-
-    # Interactive, need more time
-    #tout = hand.client(["tout", "200",], conf.sess_key)
-    #print (tout)
+    conf.sess_key2 = base64.b64encode(Random.new().read(128))
+    sss2 = SHA256.new(); sss2.update(conf.sess_key2)
 
     if conf.pgdebug > 2:
-        print(pvh.datax)
+        support.shortdump("conf.sess_key2", conf.sess_key2 )
 
-    if hand.verbose:
-        print("Sending Data:", pvh.datax)
+    sess_keyx2 = hand.pubkey.encrypt(conf.sess_key2)
+    ttt2 = SHA256.new(); ttt2.update(sess_keyx2.encode())
 
-    #ttt = time.time()
-    for aa in range(conf.numrec):
-        cresp = hand.client(["rput", "vote", pvh.datax], conf.sess_key)
-        print ("Server rput response:", cresp)
-    #print("rput %.3fms" % ((time.time() - ttt) * 1000) )
+    if conf.pgdebug > 2:
+        support.shortdump("sess_keyx2", sess_keyx2 )
 
-    sys.exit(0)
+    if conf.pgdebug > 3:
+        print("key  Hexdigest", sss2.hexdigest()[:16])
+        print("sess Hexdigest", ttt2.hexdigest()[:16])
 
-if __name__ == '__main__':
-    mainfunct()
+    resp4 = hand.client(["sess", sss2.hexdigest(), ttt2.hexdigest(), sess_keyx2],
+                                conf.sess_key, False)
+    if resp4[0] != "OK":
+        print("Err: ", resp4)
+        cresp = hand.client(["quit", ], conf.sess_key)
+        print ("Server quit response:", cresp)
+        sys.exit(0)
+
+    conf.sess_key = conf.sess_key2
+    # Make a note of the session key
+    print("Session key:", conf.sess_key[:24] , "..." )
+
+    # Session estabilished, try a simple command
+    resp5 = hand.client(["hello",], conf.sess_key)
+    print("Hello2 Response:", resp5)
 
-# EOF
+    hand.client(["quit",],conf.sess_key)
+    hand.close();
+
+    sys.exit(0)
 
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_sess.py` & `pyvserv-1.0.3/pyvclient/pyvcli_sess_tout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 #!/usr/bin/env python3
 
-#from __future__ import print_function
-
-from pyvecc.Key import Key
+from __future__ import print_function
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, base64
+import  random, stat
 
-from Crypto.Hash import SHA256
+from Crypto.Hash import SHA512
+from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_v1_5
+from Crypto.PublicKey import RSA
+from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
+'''
+# test encrypt with large keys
+rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
+        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
+sss = bluepy.encrypt(rrr, conf.sess_key)
+ttt = bluepy.decrypt(sss, conf.sess_key)
+print (rrr)
+print (ttt)
+'''
+
 # ------------------------------------------------------------------------
 # Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
@@ -58,15 +70,14 @@
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
-    #print(vars(conf))
 
     if conf.comm:
         print("Save to filename", conf.comm)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
@@ -85,29 +96,33 @@
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     #print("IP:", ip, respc);
     #print("Initial:", respc);
 
-    resp = hand.client(["akey"], conf.sess_key)
+    resp = hand.client(["akey"])
     #print("akey response", resp)
 
     if resp[0] != "OK":
         print("Error on getting key:", resp[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
+    if conf.verbose:
+        print("Got akey hash:", "'" + resp[1] + "'")
+        pass
+
     #if conf.pgdebug > 4:
     #    print ("Server response2:\n" +  "'" + resp[1].decode("cp437") +  "'\n")
 
-    hhh = SHA256.new();
-    #hhh.update(bytes(resp[2], "utf-8"))
-    hhh.update(resp[2].encode())
+    hhh = SHA512.new();
+    hhh.update(resp[2])
+    #hhh.update(bytes(resp[2], "cp437"))
 
     if conf.pgdebug > 3:
         print("Hash1:  '" + resp[1] + "'")
         print("Hash2:  '" + hhh.hexdigest() + "'")
 
     # Remember key
     if hhh.hexdigest() !=  resp[1]:
@@ -120,102 +135,112 @@
 
     #if conf.quiet == False:
     #     print("Key response:", resp[0], resp[2][:32], "...")
 
     if conf.pgdebug > 4:
          print(hand.pkey)
 
-    hand.pkey = resp[2]
-    #print("got FIRST key", hand.pkey)
-
     if conf.pgdebug > 2:
         print ("Server response:", "'" + hhh.hexdigest() + "'")
 
-    #if conf.showkey or conf.pgdebug > 5:
-    #    #print("Key:")
+    if conf.showkey or conf.pgdebug > 5:
+        #print("Key:")
+        print(hand.pkey)
 
     try:
-        #hand.pubkey = RSA.importKey(hand.pkey)
-        hand.pubkey = Key.import_pub(hand.pkey)
+        hand.pubkey = RSA.importKey(hand.pkey)
         if conf.pgdebug > 4:
             print (hand.pubkey)
     except:
         print("Cannot import public key.")
         support.put_exception("import key")
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     resp0 = hand.client(["hello",], )
-    print("Hello Plain:", resp0)
+    print("Hello (unencrypted) Response:", resp0[1])
+
+    #if conf.pgdebug > 1:
+    #    print("Got pub key", hand.pubkey, "size =", hand.pubkey.size_in_bits())
 
     # Generate communication key
-    conf.sess_key = base64.b64encode(Random.new().read(128))
-    sss = SHA256.new(); sss.update(conf.sess_key)
+    conf.sess_key = Random.new().read(512)
+    sss = SHA512.new(); sss.update(conf.sess_key)
+
+    cipher = PKCS1_v1_5.new(hand.pubkey)
+    #print ("cipher", cipher.can_encrypt())
 
     if conf.pgdebug > 2:
         support.shortdump("conf.sess_key", conf.sess_key )
 
-    sess_keyx  = hand.pubkey.encrypt(conf.sess_key)
-
-    ttt = SHA256.new(); ttt.update(sess_keyx.encode())
+    sess_keyx = cipher.encrypt(conf.sess_key)
+    ttt = SHA512.new(); ttt.update(sess_keyx)
 
     if conf.pgdebug > 2:
         support.shortdump("sess_keyx", sess_keyx )
 
     resp3 = hand.client(["sess", sss.hexdigest(), ttt.hexdigest(), sess_keyx], "", False)
     #print("Sess Response:", resp3)
 
     if resp3[0] != "OK":
-        print("Error on setting session:", resp3)
+        print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    print("Session key:", conf.sess_key[:24] , "..." )
+    #print(resp3[1])
+    support.shortdump(" All is encrypted with", conf.sess_key )
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    print("Encrypted Resp:", resp4)
+    print("Hello (encrypted) Response:", resp4[1])
 
     # --------------------------------------------------------------------
     # Generate communication key, second session and second run
 
-    conf.sess_key2 = base64.b64encode(Random.new().read(128))
-    sss2 = SHA256.new(); sss2.update(conf.sess_key2)
+    conf.sess_key2 = Random.new().read(512)
+    sss2 = SHA512.new(); sss2.update(conf.sess_key2)
+
+    #cipher = PKCS1_v1_5.new(hand.pubkey)
+    #print ("cipher", cipher.can_encrypt())
 
     if conf.pgdebug > 2:
         support.shortdump("conf.sess_key2", conf.sess_key2 )
 
-    sess_keyx2 = hand.pubkey.encrypt(conf.sess_key2)
-    ttt2 = SHA256.new(); ttt2.update(sess_keyx2.encode())
+    sess_keyx2 = cipher.encrypt(conf.sess_key2)
+    ttt2 = SHA512.new(); ttt2.update(sess_keyx2)
 
     if conf.pgdebug > 2:
-        support.shortdump("sess_keyx2", sess_keyx2 )
+        support.shortdump("sess_keyx", sess_keyx )
 
-    if conf.pgdebug > 3:
-        print("key  Hexdigest", sss2.hexdigest()[:16])
-        print("sess Hexdigest", ttt2.hexdigest()[:16])
+    #print("Key Hexdigest", ttt2.hexdigest()[:16])
 
     resp4 = hand.client(["sess", sss2.hexdigest(), ttt2.hexdigest(), sess_keyx2],
                                 conf.sess_key, False)
+
     if resp4[0] != "OK":
         print("Err: ", resp4)
         cresp = hand.client(["quit", ], conf.sess_key)
         print ("Server quit response:", cresp)
         sys.exit(0)
 
-    conf.sess_key = conf.sess_key2
     # Make a note of the session key
-    print("Session key:", conf.sess_key[:24] , "..." )
+    #print(resp4[1])
+    support.shortdump(" All is encrypted with", conf.sess_key2 )
 
     # Session estabilished, try a simple command
-    resp5 = hand.client(["hello",], conf.sess_key)
-    print("Hello2 Response:", resp5)
+    resp5 = hand.client(["hello",], conf.sess_key2)
+    print("Hello (encrypted2) Response:", resp5)
+
+    time.sleep(10)
+
+    resp5 = hand.client(["hello",], conf.sess_key2)
+    print("Hello (encrypted2) Response:", resp5)
 
-    hand.client(["quit",],conf.sess_key)
+    hand.client(["quit",],conf.sess_key2)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_tout.py` & `pyvserv-1.0.3/pyvclient/pyvcli_tout.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_uadd.py` & `pyvserv-1.0.3/pyvclient/pyvcli_uadd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_uchpass.py` & `pyvserv-1.0.3/pyvclient/pyvcli_uchpass.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_udel.py` & `pyvserv-1.0.3/pyvclient/pyvcli_udel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_uena.py` & `pyvserv-1.0.3/pyvclient/pyvcli_uena.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_uini.py` & `pyvserv-1.0.3/pyvclient/pyvcli_uini.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,44 +4,32 @@
 import sys
 if  sys.version_info[0] < 3:
     print(("Needs python 3 or better."))
     sys.exit(1)
 
 __doc__ =\
 '''
-    Test client for the pyserv project. Default user initializer.
+    Test client for the pyvserv project. Default user initialiser.
     This command can only be used from the local network, loopback
     interface. The command is used to create the initial user,
-    and will not run if the is a user present already.
+    and will not do anything if there is a user present already.
 
 '''
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
 # This repairs the path from local run to pip run.
-# Remove pip version for local tests
 try:
     from pyvcommon import support
-
-    # Get Parent of module root
-    sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
-    print("sf", sf)
-    sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
-
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
-    sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
@@ -49,42 +37,46 @@
 version = 1.0
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
-    print( "Options:    -d level  - Debug level 0-10")
+    print( "Options:    -d level  - Debug level 0-10 default: 0")
     print( "            -p        - Port to use (default: 6666)")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -h        - Help")
+    print( "            -v        - Verbose. Present more info")
+    print( "            -u user   - User Name; default: 'admin'")
+    print( "            -p pass   - Password; default: '1234' (!!! for tests only)")
+    print( "            -q        - Quiet. Prrsent less info")
+    print( "            -h        - Help (this screen)")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["u:",  "userx",    "admin",    None],      \
+    ["p:",  "passx",    "1234",     None],      \
+    ["t",   "test",     "x",        None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def    mainfunct():
 
     ''' Initialize test user 'admin' with password '1234'
     Naturally, this is for testing. '''
 
 
     args = conf.comline(sys.argv[1:])
 
@@ -99,25 +91,27 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello",] , "", False)
-    print("Hello Response:", resp3)
+    #print("Connect Response:", respc)
 
     resp3 = hand.start_session(conf)
     print("Sess Response:", resp3)
 
     resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello sess Response:", resp3[1])
+    #print("Hello sess Response:", resp3[1])
 
-    resp = hand.client(["uini", "admin", "1234"], conf.sess_key)
-    print("uini resp", resp)
+    resp = hand.client(["uini", conf.userx, conf.passx], conf.sess_key)
+    print("resp", resp)
 
     hand.client(["quit"], conf.sess_key)
-
     hand.close();
 
     sys.exit(0)
 
+if __name__ == '__main__':
+    mainfunct()
+
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvclient/pyvcli_ver.py` & `pyvserv-1.0.3/pyvgui/pyvservui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,91 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
+from __future__ import absolute_import
 from __future__ import print_function
 
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
-# ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# This repairs the path from local run to pip run.
+# Remove pip version for local tests
+try:
+    from pyvcommon import support
+
+    # Get Parent of module root
+    sf = os.path.dirname(support.__file__)
+    sf = os.path.dirname(sf)
+    #print("sf", sf)
+    sys.path.append(os.path.join(sf, "pyvcommon"))
+    sys.path.append(os.path.join(sf, "pyvserver"))
+    sys.path.append(os.path.join(sf, "pyvgui"))
+    sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
+
+except:
+    #print("pip inc")
+    base = os.path.dirname(__file__)
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    sys.path.append(os.path.join(base,  '..', "pyvserver"))
+    sys.path.append(os.path.join(base, "..", "pyvgui"))
+    sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
+    from pyvcommon import support
+
+from pyvguicom import sutil
+# Get Parent of module root
+sf = os.path.dirname(sutil.__file__)
+sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
+from pyvcommon import support, comline, pywrap
+from pyvcommon import pydata, pyservsup,  crysupp
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+from guilib import mainwinserv
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+# ------------------------------------------------------------------------
+# Globals
 
-version = "1,0"
+version = "0.00"
 
 # ------------------------------------------------------------------------
-# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
+    print( "            -p        - Port to use (default: 9999)")
     print( "            -v        - Verbose")
+    print( "            -V        - Version")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
+# ------------------------------------------------------------------------
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
+    ["p:",  "port",     9999,   None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
-conf = comline.Config(optarr)
+conf = comline.ConfigLong(optarr)
 
-# ------------------------------------------------------------------------
+def mainfunct():
 
-if __name__ == '__main__':
-
-    if sys.version_info[0] < 3:
-        print("Warning! This script was meant for python 3.x")
-        time.sleep(1)
-
-    #if  sys.version_info[0] < 3:
-    #    print("Needs python 3 or better.")
-    #    sys.exit(1)
-    #
     args = conf.comline(sys.argv[1:])
-
-    if len(args) == 0:
-        ip = '127.0.0.1'
-    else:
-        ip = args[0]
-
-    hand = pyclisup.CliSup()
-    hand.verbose = conf.verbose
-    hand.pgdebug = conf.pgdebug
-
-    try:
-        resp2 = hand.connect(ip, conf.port)
-    except:
-        support.put_exception("On connect")
-        print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
-        sys.exit(1)
-
-    #if conf.quiet == False:
-    #    print ("Server initial:", resp2)
-
-    resp = hand.client(["ver"])
-
-    if conf.quiet == False:
-        print ("Server response:", resp)
-
-    hand.client(["quit"])
-    hand.close()
-
+    mw = mainwinserv.MainWin()
+    mw.main()
     sys.exit(0)
 
-# EOF
-
-
-
-
-
-
-
-
-
-
-
+if __name__ == '__main__':
+    mainfunct()
 
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvcommon/comline.py` & `pyvserv-1.0.3/pyvcommon/comline.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/crysupp.py` & `pyvserv-1.0.3/pyvcommon/crysupp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/genstrerr.py` & `pyvserv-1.0.3/pyvcommon/genstrerr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/pyclisup.py` & `pyvserv-1.0.3/pyvcommon/pyclisup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,20 @@
 #from __future__ import print_function
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, socket, datetime
 
 from pyvecc.Key import Key
 
-#base = os.path.dirname(os.path.realpath(__file__))
-#sys.path.append(os.path.join('..', 'pyvcommon'))
-#sys.path.append(os.path.join('.', 'pyvcommon'))
-
 import pydata, pyservsup, crysupp, support, comline, pywrap
 
 import pyvpacker
 
 from Crypto import Random
 from Crypto.Cipher import AES
-#from Crypto.Hash import SHA512
-#from Crypto.Hash import SHA
 from Crypto.Hash import SHA256
 
 from Crypto.PublicKey import ECC
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5
 from Crypto.Cipher import PKCS1_OAEP
 
@@ -483,8 +477,20 @@
             #self.client(["quit"])
             #self.close();
             return resp3
 
         self.sess = True
         return resp3
 
+def atexit_func(hand, conf):
+
+    ''' Severe connection on exit '''
+
+    try:
+        #print("Atexit")
+        cresp = hand.client(["quit", ], conf.sess_key)
+        #print ("Server quit response:", cresp)
+        hand.close();
+    except:
+        pass
+
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvcommon/pycrypt.py` & `pyvserv-1.0.3/pyvcommon/pycrypt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/pydata.py` & `pyvserv-1.0.3/pyvcommon/pydata.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/pyservsup.py` & `pyvserv-1.0.3/pyvcommon/pyservsup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
 import os, sys, string, time, traceback, random, uuid
-import datetime, base64, fcntl
+import datetime, base64
+
+try:
+    import fcntl
+except:
+    fcntl = None
 
 #base = os.path.dirname(os.path.realpath(__file__))
 #sys.path.append(os.path.join(base, '../pyvcommon'))
 
 import support, pyclisup, crysupp, pysyslog
 
 #from Crypto.Hash import SHA512
@@ -37,14 +42,16 @@
 chainfname  = "initial"
 repfname    = "pyvreplic"
 logfname    = "pyvserver"
 
 lock_pgdebug = 0
 lock_locktout = 5
 
+# Configure the server by customizing this class
+
 class   Global_Vars:
 
     def __init__(self, scriptname, dataroot):
 
         # Underscore names are definitions - others are calculated
 
         self.verbose = 0
@@ -97,17 +104,21 @@
         self._softmkdir(self.logdir, "Log dir")
 
         self.lockfname = self.tmpdir + os.sep + "lockfile"
         self.passfile = self.passdir + os.sep + self._passfile
         self.idfile = self.myhome + self._idfile
 
         self.siteid     =  None
-        self.throttle   =  10       # seconds
-        self.instance   =  15       # max instace from one IP/host
-        self.maxthdat   =  100      # max data in throttle var
+
+        # These are presets for testing, use larger values for production
+        self.throt_sec        =  5    # seconds for conn frequency
+        self.throt_maxsec     =  6    # seconds max life in cache
+        self.throt_instances  =  5    # max instaces from one IP/host
+        self.throt_maxdat     =  10   # max data length in throttle var
+        self.throt_time       =  3    # throttle by this many sec
 
         #print("init globals");
         #global globals
         #globals = self
         pass
 
     # Soft make dir
@@ -240,18 +251,20 @@
                 if 1: #lock_pgdebug > 1:
                     print("Lock held too long pid =", os.getpid(), cnt)
                 self.unlock()
                 break
             cnt += 1
             time.sleep(1)
         # Lock NOW
-        fcntl.lockf(self.fpx, fcntl.LOCK_EX)
+        if fcntl:
+            fcntl.lockf(self.fpx, fcntl.LOCK_EX)
 
     def unlock(self):
-        fcntl.lockf(self.fpx, fcntl.LOCK_UN)
+        if fcntl:
+            fcntl.lockf(self.fpx, fcntl.LOCK_UN)
 
 # ------------------------------------------------------------------------
 # This class will maintain a passwd database, similar to
 #  the system database
 
 class Passwd():
```

### Comparing `pyvserv-1.0.2/pyvcommon/pysyslog.py` & `pyvserv-1.0.3/pyvcommon/pysyslog.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/pyv2fa.py` & `pyvserv-1.0.3/pyvcommon/pyv2fa.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/pyvhash.py` & `pyvserv-1.0.3/pyvcommon/pyvhash.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 def DefPayload():
     return {PayLoad : { "Default": "None"}}
 
 def DefHeader():
     return {Header : str(uuid.uuid1())}
 
 def DefNow():
-    dt = datetime.datetime.utcnow()
+    dt = datetime.datetime.now()
     fdt = dt.strftime('%a, %d %b %Y %H:%M:%S`')
     return {'now' : fdt}
 
 def DefRep():
     return {Repli : 0}
 
 class NoProof(Exception):
```

### Comparing `pyvserv-1.0.2/pyvcommon/pywrap.py` & `pyvserv-1.0.3/pyvcommon/pywrap.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvcommon/support.py` & `pyvserv-1.0.3/pyvcommon/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,20 +160,29 @@
                 state = 1; back += aa
             else:
                 aaa += aa
 
     return aaa
 
 # ------------------------------------------------------------------------
-# Remove dup //
 
 def dirclean(strx):
+
+    '''  Remove duplicate //
+
+      History:
+        Mon 01.Apr.2024 added c: path exception for MSYS2
+    '''
+
     rrr = ""; aaa = strx.split("/")
     for aa in aaa:
-        if aa != "": rrr += "/" + aa
+        if len(aa) > 1 and aa[1] == ":":
+            rrr += aa
+        elif aa != "":
+            rrr += "/" + aa
     return rrr
 
 # ------------------------------------------------------------------------
 # Change directory to up (..)
 
 def chup(strx):
     # Stage 1: clean
```

### Comparing `pyvserv-1.0.2/pyvgui/guilib/mainwin.py` & `pyvserv-1.0.3/pyvgui/guilib/mainwin.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvgui/guilib/mainwinserv.py` & `pyvserv-1.0.3/pyvgui/guilib/mainwinserv.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from pgui import *
 
 base = os.path.dirname(os.path.realpath(__file__))
 #sys.path.append(os.path.join(base, '../../'))
 
 sys.path.append('../../')
 
-from pycommon.pgutils import  *
-from pycommon.pggui import  *
-from pycommon.pgsimp import  *
+from pyvguicom import pgutils # import  *
+from pyvguicom import pggui   #import  *
+from pyvguicom import pgsimp  #import  *
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
@@ -124,24 +124,24 @@
         hbox2 = Gtk.HBox()
         lab3 = Gtk.Label("");  hbox2.pack_start(lab3, 0, 0, 0)
         lab4 = Gtk.Label("");  hbox2.pack_start(lab4, 0, 0, 0)
         vbox.pack_start(hbox2, False, 0, 0)
 
 
         hbox3 = Gtk.HBox()
-        self.edit = SimpleEdit();
+        self.edit = pgsimp.SimpleEdit();
 
         scroll = Gtk.ScrolledWindow()
         scroll.add(self.edit)
         scroll.set_policy(Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
         hbox3.pack_start(scroll, True, True, 6)
         vbox.pack_start(hbox3, True, True, 2)
 
         hbox3a = Gtk.HBox()
-        self.edita = SimpleEdit();
+        self.edita = pgsimp.SimpleEdit();
         scrolla = Gtk.ScrolledWindow()
         scrolla.add(self.edita)
         scrolla.set_policy(Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
         hbox3a.pack_start(scrolla, True, True, 6)
         vbox.pack_start(hbox3a, True, True, 2)
 
         vbox.pack_start(hbox4, False, 0, 6)
```

### Comparing `pyvserv-1.0.2/pyvgui/guilib/mainwintally.py` & `pyvserv-1.0.3/pyvgui/guilib/mainwintally.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvgui/guilib/pgui.py` & `pyvserv-1.0.3/pyvgui/guilib/pgui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvgui/guilib/pymenu.py` & `pyvserv-1.0.3/pyvgui/guilib/pymenu.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.2/pyvgui/pyvcpanel.py` & `pyvserv-1.0.3/pyvgui/pyvcpanel.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,40 +18,31 @@
 
     # Get Parent of module root
     sf = os.path.dirname(support.__file__)
     sf = os.path.dirname(sf)
     #print("sf", sf)
     sys.path.append(os.path.join(sf, "pyvcommon"))
     sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pydbase"))
     sys.path.append(os.path.join(sf, "pyvgui"))
     sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
 
 except:
-    base = os.path.dirname(os.path.realpath(__file__))
+    base = os.path.dirname(__file__)
+    #print("base:", base)
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base,  '..', "pydbase"))
     sys.path.append(os.path.join(base,  "..", "pyvgui"))
     sys.path.append(os.path.join(base,  "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-try:
-    from pyvguicom import sutil
-    # Get Parent of module root
-    sf = os.path.dirname(sutil.__file__)
-    sf = os.path.dirname(sf)
-    sys.path.append(os.path.join(sf, "pyvguicom"))
-except:
-    #print("import", sys.exc_info())
-    base = os.path.dirname(os.path.realpath(__file__))
-    sys.path.append(os.path.join(base, "..", "..", "pyvguicom"))
-    sys.path.append(os.path.join(base, "..", "..", "pyvguicom", "pyvguicom"))
-    from pyvguicom import sutil
+from pyvguicom import sutil
+# Get Parent of module root
+sf = os.path.dirname(sutil.__file__)
+sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
 #print("Load:", sys.path[-1])
 
 from pyvcommon import support, comline, pywrap
 from pyvcommon import pydata, pyservsup,  crysupp
 from pyvserver import pyvstate
 from pyvserver import pyvfunc
```

### Comparing `pyvserv-1.0.2/pyvgui/pyvservui.py` & `pyvserv-1.0.3/pyvgui/pyvtally.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
-from __future__ import absolute_import
-from __future__ import print_function
+import os, sys
 
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
+if  sys.version_info[0] < 3:
+        print("Needs python 3 or better.")
+        sys.exit(1)
+
+import getopt, signal, select, socket, time, struct
+import random, string, stat, base64, random, datetime
+
+import pyvpacker
 
 # This repairs the path from local run to pip run.
 # Remove pip version for local tests
 try:
     from pyvcommon import support
 
     # Get Parent of module root
     sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
+    sf = os.path.dirname(sf )
     #print("sf", sf)
     sys.path.append(os.path.join(sf, "pyvcommon"))
     sys.path.append(os.path.join(sf, "pyvserver"))
     sys.path.append(os.path.join(sf, "pyvgui"))
     sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
 
 except:
-    base = os.path.dirname(os.path.realpath(__file__))
+    base = os.path.dirname(__file__)
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    sys.path.append(os.path.join(base, "..", "pyvgui"))
-    sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
+    sys.path.append(os.path.join(base,  "..", "pyvgui"))
+    sys.path.append(os.path.join(base,  "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-try:
-    from pyvguicom import sutil
-    # Get Parent of module root
-    sf = os.path.dirname(sutil.__file__)
-    sf = os.path.dirname(sf)
-    sys.path.append(os.path.join(sf, "pyvguicom"))
-except:
-    #print(sys.exc_info())
-    base = os.path.dirname(os.path.realpath(__file__))
-    sys.path.append(os.path.join(base, "..", "..", "pyvguicom"))
-    sys.path.append(os.path.join(base, "..", "..", "pyvguicom", "pyvguicom"))
-    from pyvguicom import sutil
-
+from pyvguicom import sutil
+# Get Parent of module root
+sf = os.path.dirname(sutil.__file__)
+sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
 #print("Load:", sys.path[-1])
 
 from pyvcommon import support, comline, pywrap
 from pyvcommon import pydata, pyservsup,  crysupp
+from pyvserver import pyvstate
+from pyvserver import pyvfunc
+from guilib import mainwintally
 
-from guilib import mainwinserv
-
-# ------------------------------------------------------------------------
+# -----------------------------------------------------------------------
 # Globals
 
-version = "0.00"
+version = "1.00"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
@@ -74,28 +71,34 @@
 # ------------------------------------------------------------------------
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     9999,   None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "debug=",   "pgdebug",  0,      None],      \
+    ["p:",  "port=",    "port",     9999,   None],      \
+    ["v",   "verbose",  "verbose",  0,      None],      \
+    ["q",   "quiet",    "quiet",    0,      None],      \
+    ["r:",  "dataroot=", "droot",   "pyvserver",     None],      \
+    ["V",   "version",  None,       None,   pversion],  \
+    ["h",   "help",     None,       None,   phelp]      \
 
 conf = comline.ConfigLong(optarr)
 
 def mainfunct():
-
+    #print("pyvcpanel started ...")
     args = conf.comline(sys.argv[1:])
-    mw = mainwinserv.MainWin()
+    #print("args", args)
+
+    pyservsup.globals  = pyservsup.Global_Vars(__file__, conf.droot)
+    pyservsup.globals.conf = conf
+
+    mw = mainwintally.MainWin()
     mw.main()
     sys.exit(0)
 
 if __name__ == '__main__':
+
     mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvserv.egg-info/PKG-INFO` & `pyvserv-1.0.3/pyvserv.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.2
+Version: 1.0.3
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyvpacker
 Requires-Dist: pydbase
 Requires-Dist: pycryptodome
 Requires-Dist: pyvecc
+Requires-Dist: pyvguicom
 
 #  PyvServer
+
 ## 	Fully encrypted TCP/IP server.
 
  &nbsp; &nbsp; PyvServ is an encrypting TCP/IP server written in Python. The
 encryption algorithm is AES. (Advanced Encryption Standard) The key exchange
 uses ECC. (Elliptic curve) The server can be fully administered from the
 protocol side.
 
@@ -85,16 +87,14 @@
  PyvServ has replication facilities via a client based 'I have You have'
  mechanism featuring encrypted transport. It is also capable of replication
  on a 'replicate when received' mechanism. The replicated records are marked
  with a replication count, so replication does not enter looping. By default,
  the replicated records are not replicated any further, assuming a flat
  structure of replication.
 
- Project is still in motion, but a lot of it is usable.
-
 #### Installation:
 
     pip install pyvserv
 
  Dependencies:
 
  Most linux systems already have all the dependencies by default. Some dependencies
@@ -105,92 +105,167 @@
  The firewall needs to be opened for incoming connections on port xxxx
 
 For example (assuming port 6666):
 
     sudo iptables -A INPUT -p tcp --dport 6666
     sudo iptables -A INPUT -p tcp --sport 6666
 
- Please note that this is not a recommendation, it is a port we used during development.
+ Please note that this is not a recommendation, it is a port we used during
+ development.
+
+#### Start server
+
+ The python server can be added to the system servers with the Makefile targets
+'make genservice' and 'make instservice'
+ The scripts will generate the service file to run under current user's
+ credentials, and install it onto the running system. (requires sudo)
 
 #### Platform:
 
-    This project was developed on Ubuntu 22.x. Most linux distributions should work.
+ This project was developed on Ubuntu 22.x. Most linux distributions should work.
+It is ported to Windows MSYS2, with all major functions operating as expected.
+
+ On Fedora, the service files need to be re-written to accomodate the
+quirk that the Fedora systectl does not allow user executables. Install
+the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
+to use pyvserv with  particular data directory, use the -r option.
 
-#### Working parts:
+#### Quick map:
 
-    Server.     subdir: pyvserver       -- Server has most of the commands done
+    Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
-    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     Test Suite. subdir: pyvclient/tests -- official pytest tests
+    Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
 installation from github, replicating directory structure on the local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
-    type ./pyvserv.py  -D
-
-    The -D option stands for development mode. The server will not ask for
-    2FA authentication.
+    type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
-    type ./pyvcli_hello.py
+    type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
     Server initial: ['OK', 'pyvserv 1.0 ready']
     resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
     Server quit response: ['OK', 'Bye', '11812']
 
 Quick rundown of the above test:
 
-1.) Server responds to connection
-2.) Delivers OK status, hello message, server serial number, and a unique id
-3.) Server signs off. This interaction is typical of all the commands.
+    1.) Server responds to connection with signin message
+    2.) Delivers OK status, hello message, server serial number, and a unique id
+    3.) Server signs off. Repeats unique id / session number.
 
- The unique ID is the session's thread ID and it is not cryptographically secure;
+This interaction is typical of all the commands.
+
+The unique ID is the session's thread ID and it is not cryptographically secure;
+Mostly useful for identifying the session on the client side.
 
  The best way to learn about the operation of the server is to look at the
 sample client examples in the client source tree. (Files named pyvcli_*)
 
+## The pip install
+
+ Scripts are provided for the server, and some test clients. The
+  server can be started as
+
+    pyvserver
+
+ The -P option is for non Developer mode, enabling 2FA authentication.
+ (two factor authentication)
+
+ The command line client can be started as:
+
+    pyvcli_cli
+
+  In the command line client most of the server functions can be exercised.
+See the pyvcli_* utils for more examples of driving the server.
+
+## Command line help
+
+    Usage: pyvserv.py [options]
+
+    Options:
+            -n   --host                 -  Set server hostname / interface.
+            -r   --dataroot  dataroot   -  Set data root for server.
+            -P   --pmode                -  Production mode ON. (allow 2FA)
+            -l   --loglevel             -  Log level (0 - 10) default = 1
+            -m   --mem                  -  Show memory trace.
+            -N   --norepl               -  No replication. (for testing)
+            -d   --debug     debug      -  Debug level 0-10
+            -p   --port      port       -  Listen on port
+            -v   --verbose              -  Verbose
+            -q   --quiet                -  Quiet
+            -V   --version              -  Print Version
+            -h   --help                 -  Show Help
+
+## Client command line help example:
+
+ While most command line clients have their own help screen, here as a typical
+client utility's help screen:
+
+    Usage: pyvcli_uman.py [options]
+
+    Options:    -d level  - Debug level 0-10
+                -p        - Port to use (default: 6666)
+                -l login  - Login Name; default: 'user'
+                -s lpass  - Login Pass; default: '1234'
+                -u user   - User Name; default: 'user'
+                -a        - Add user. Must be unique.
+                -r        - Remove user (one of add or remove needed.
+                -u user   - User Name; default: 'user'
+                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -m        - Add admin instead of regular user
+                -v        - Verbose
+                -q        - Quiet
+                -h        - Help
+
 ## Testing:
 
  All pytest cases pass. Note that the for the pytest client tests one needs to
  start the 'pyvserv.py' server.
  The server --port and --dataroot option can ba used to start the server in an alternate
  universe. Please make sure it does not interfere with production.
 
-   More test coming soon ....
-
-    ============================= test session starts ==============================
+    ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
-    rootdir: /home/peterglen/pgpygtk/pyvserv
-    collected 9 items
+    rootdir: /home/<homedir>/pgpygtk/pyvserv
+    collected 15 items
 
-    test_afirst.py .                                                         [ 11%]
-    test_file.py .                                                           [ 22%]
+    test_afirst.py .                                                         [  6%]
+    test_file.py ..                                                          [ 20%]
+    test_hello.py .                                                          [ 26%]
     test_help.py .                                                           [ 33%]
-    test_id.py .                                                             [ 44%]
-    test_key.py .                                                            [ 55%]
-    test_login.py .                                                          [ 66%]
-    test_sess.py ..                                                          [ 88%]
+    test_id.py .                                                             [ 40%]
+    test_key.py .                                                            [ 46%]
+    test_login.py .                                                          [ 53%]
+    test_noadmn.py .                                                         [ 60%]
+    test_rget.py .                                                           [ 66%]
+    test_rput.py .                                                           [ 73%]
+    test_sess.py ..                                                          [ 86%]
+    test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
-    ============================== 9 passed in 1.35s ===============================
+    ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the test directory. The pyvcli_* files may also
+Additional tests can be found in the tests/ directory. The pyvcli_* files may also
 serve as test cases.
 
+More test coming soon ....
+
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
@@ -199,23 +274,39 @@
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
   All views monitor the live files, on the default setup, without interfering
 with any of the operations.
 
+## Windows compatibility
+
+ Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+functionalities are ported. The file locking mechanism works, and all the
+pytests pass. Naturally, logging and readline etc ... works with the usual
+windows caveat.
+
+  For the GUI functions install the PyGobject subsystem. Instructions can
+be found very easily for that. Below, a screenshot of the pyvserv control panel
+in MSYS2.
+
+![Screen Shot](winscreen.png)
+
+The project is functional in MSYS2, but for real deployment we recommend Linux.
+
 ## History:
 
  Recent history kept, for the full list of changes consult the github site.
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
+    1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
 
 ## Statistics
 
     Project name
         pyvserv
     Report Period
         2018-12-31 20:50:04 to 2024-03-15 04:47:25
```

### Comparing `pyvserv-1.0.2/pyvserv.egg-info/SOURCES.txt` & `pyvserv-1.0.3/pyvserv.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 LICENSE
 README.md
 setup.py
 pyvclient/__init__.py
-pyvclient/bulkren.py
-pyvclient/chall.py
 pyvclient/loadtest.py
-pyvclient/pyvcli_acc.py
 pyvclient/pyvcli_akey.py
 pyvclient/pyvcli_bigget.py
 pyvclient/pyvcli_cd.py
 pyvclient/pyvcli_cli.py
 pyvclient/pyvcli_fdel.py
 pyvclient/pyvcli_fget.py
 pyvclient/pyvcli_file.py
@@ -33,15 +30,15 @@
 pyvclient/pyvcli_sess_tout.py
 pyvclient/pyvcli_tout.py
 pyvclient/pyvcli_uadd.py
 pyvclient/pyvcli_uchpass.py
 pyvclient/pyvcli_udel.py
 pyvclient/pyvcli_uena.py
 pyvclient/pyvcli_uini.py
-pyvclient/pyvcli_utils.py
+pyvclient/pyvcli_uman.py
 pyvclient/pyvcli_ver.py
 pyvcommon/__init__.py
 pyvcommon/comline.py
 pyvcommon/crysupp.py
 pyvcommon/genstrerr.py
 pyvcommon/pyclisup.py
 pyvcommon/pycrypt.py
```

### Comparing `pyvserv-1.0.2/pyvserver/pyvfunc.py` & `pyvserv-1.0.3/pyvserver/pyvfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python
 
 #from __future__ import print_function
 #from __future__ import absolute_import
 
-import pyotp
+try:
+    import pyotp
+except:
+    pyotp = None
 
 import os, sys, getopt, signal, select, string
 import datetime,  time, stat, base64, uuid
 
 from pyvecc.Key import Key
 
 #from Crypto.Cipher import PKCS1_v1_5
@@ -226,34 +229,40 @@
     dname = ""; sss = ""
     if len(strx) < 2:
         strx.append(".")
     try:
         dname = support.unescape(strx[1]);
     except:
         pass
-    dname2 = self.resp.cwd + os.sep + self.resp.dir + os.sep + dname
-    dname2 = support.dirclean(dname2)
 
+    dname2 = self.resp.cwd + os.sep + self.resp.dir + os.sep + dname
     #print("dname2", dname2)
 
+    dname2 = support.dirclean(dname2)
+    #print("dname2c", dname2)
+
     response = [OK]
     try:
         ddd = os.listdir(dname2)
         for aa in ddd:
             try:
                 aaa = dname2 + os.sep + aa
                 if stat.S_ISREG(os.stat(aaa)[stat.ST_MODE]):
                     # Escape spaces
                     response.append(aa) #support.escape(aa))
             except:
                 print( "Cannot stat ", aaa, str(sys.exc_info()[1]) )
 
     except:
-        support.put_exception("ls ")
-        response = [ERR, "No such directory.", strx[0]]
+        # Perhaps the user meant the file:
+        if os.path.isfile(dname2):
+            response = [OK, strx[1], strx[0]]
+        else:
+            support.put_exception("ls ")
+            response = [ERR, "No such directory.", strx[1]]
 
     #print("response", response)
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_fget_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
@@ -1062,17 +1071,18 @@
     self.resp.datahandler.putencode(res, self.resp.ekey)
 
 
 def get_id_func(self, strx):
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_id_func()", strx)
     res = []
-    res.append(OK);    res.append("%s" % pyservsup.globals.siteid)
+    res.append(OK);   res.append("%s" % pyservsup.globals.siteid)
+    res.append("ID")
     if pyservsup.globals.conf.pgdebug > 2:
-        print( "get_ver_func->output", "'" + res + "'")
+        print( "get_ver_func->output", res)
     self.resp.datahandler.putencode(res, self.resp.ekey)
 
 #@support.timeit
 def get_hello_func(self, strx):
     if pyservsup.globals.conf.pgdebug > 3:
         print( "get_hello_func()", strx)
     strres = [OK, "Hello", str(pyservsup.globals.siteid), self.name]
@@ -1664,45 +1674,62 @@
     #print( xstr)
     #pysyslog.syslog(xstr)
     #self.resp.datahandler.putencode("OK Got data", self.resp.ekey)
     self.resp.datahandler.putencode([OK,  "Got data"], self.resp.ekey)
 
 def get_qr_func(self, strx):
 
-    #print("QRfunc called")
+    if pyservsup.globals.conf.pgdebug > 1:
+        print("QRfunc called", len(strx))
 
-    fp = open('qr.png', 'rb')
-    buff = fp.read()
-    fp.close()
-    self.resp.datahandler.putencode([OK, buff], self.resp.ekey)
+    #print("cwd:", self.resp.cwd)
+    if len(strx) == 1:
+        fp = open('qr.png', 'rb')
+        buff = fp.read()
+        fp.close()
+        self.resp.datahandler.putencode([OK, buff], self.resp.ekey)
+    else:
+        if type(strx[1]) != type(b""):
+            strx[1] = strx[1].encode()
+        fp = open('qr.png', 'wb')
+        fp.write(strx[1])
+        fp.close()
+        self.resp.datahandler.putencode([OK, "Written new QR image", len(strx[1])], self.resp.ekey)
 
 def get_twofa_func(self, strx):
 
-    #print("get_twofa_func called")
+    if pyservsup.globals.conf.pgdebug > 1:
+        print("get_twofa_func called")
 
     retval = True
     if len(strx) < 2:
         response = [ERR, "Must pass 2fa code.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     key = "pyvserverkey"
+
+    if not pyotp:
+        self.resp.datahandler.putencode(["ERR", "2FA lib not installed"],  self.resp.ekey)
+        return
+
     totp = pyotp.TOTP(key)
     res = totp.verify(strx[1])
+
     if not res:
         self.resp.datahandler.putencode(["ERR", "Invalid 2FA code"],  self.resp.ekey)
     else:
         self.resp.datahandler.putencode(["OK", "Code Auth OK",],  self.resp.ekey)
         retval = False
 
     return retval
 
 def get_dmode_func(self, strx):
 
-    flag = pyservsup.globals.conf.dmode
+    flag = not pyservsup.globals.conf.pmode
     self.resp.datahandler.putencode(["OK", "%d" % flag],  self.resp.ekey)
 
 def get_help_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_help_func()", strx)
 
@@ -1718,18 +1745,19 @@
                 harr.append(OK)
                 harr.append(aa[5])
                 ff = True
                 break
         if not ff:
                 harr.append(ERR)
                 harr.append("No such command")
-                harr.appnd(strx[0])
+                harr.append(strx[0])
 
     if pyservsup.globals.conf.pgdebug > 2:
         print( "get_help_func->output", harr)
 
     self.resp.datahandler.putencode(harr, self.resp.ekey)
 
 if __name__ == '__main__':
+    print("This module was not meant to use as main")
     pass
 
-# EOF
+# EOF
```

### Comparing `pyvserv-1.0.2/pyvserver/pyvpuller.py` & `pyvserv-1.0.3/pyvserver/pyvpuller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,47 @@
 #!/usr/bin/env python3
 
-import os, sys, threading, time
-
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..'))
-
-import sys
+import os, sys
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
-import os, getopt, signal, select, string, time
+import getopt, signal, select, string, time
 import tarfile, subprocess, struct, platform
-import socket, threading, tracemalloc, inspect
-
-if sys.version_info[0] < 3:
-    import SocketServer as socketserver
-else:
-    import socketserver
+import socket, threading, tracemalloc, inspect, socketserver
 
 import pyvpacker
 
 # This repairs the path from local run to pip run.
-# Remove pip version for local tests
 try:
     from pyvcommon import support
-
     # Get Parent of module root
-    sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
-    #print("sf", sf)
-    sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
-
+    base = os.path.dirname(support.__file__)
+    #print("base:", base)
+    sys.path.append(os.path.join(base, "..", "pyvcommon"))
+    sys.path.append(os.path.join(base, "..", "pyvserver"))
 except:
     base = os.path.dirname(os.path.realpath(__file__))
+    print("local base", base)
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-#for aa in sys.path:
-#    print(aa)
-
-print("Load:", sys.path[-1])
+#print("Load:", sys.path[-1])
 
 from pyvcommon import support, pyservsup, pyclisup
 from pyvcommon import pydata, pysyslog, comline, pyvhash
 
 from pydbase import twincore, twinchain
 
-replicname = "replic.pydb"
-datafname = "initial.pydb"
-ihostfname = "ihosts.pydb"
+replicname  = "replic.pydb"
+datafname   = "initial.pydb"
+ihostfname  = "ihosts.pydb"
 
 MAX_DBSIZE = 20                 # Size of DB when vacuum
 
 class Blank(): pass
 
 class Puller():
 
@@ -88,15 +68,15 @@
     #            xcore = aa[1]
     #            break
     #    if not xcore:
     #        xcore = dbcreator(fname)
     #        dbarr.append((fname, xcore))
     #    return xcore
 
-    def rep_run(self):
+    def pull_run(self):
 
         ''' Main entry point for replication. '''
 
         while True:
 
             #if self.pgdebug > 5:
             #    print("Replicator cycle", time.time())
@@ -345,19 +325,17 @@
     pyservsup.globals.conf = conf
 
     slogfile = os.path.join(pyservsup.globals.myhome, "log", "pyvserver.log")
     rlogfile = os.path.join(pyservsup.globals.myhome, "log", "pyvreplic.log")
     pysyslog.init_loggers(
             ("system", slogfile), ("replic", rlogfile))
 
-
     pysyslog.repliclog("Puller started")
-
     print("Started puller")
-    repl = Replicator(conf.verbose, conf.pgdebug)
+    repl = Puller(conf.verbose, conf.pgdebug)
     repl.pull_run()
 
 if __name__ == '__main__':
 
     mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvserver/pyvreplic.py` & `pyvserv-1.0.3/pyvserver/pyvreplic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,40 @@
 #!/usr/bin/env python3
 
-import os, sys, threading, time
-
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..'))
-
-import sys
+import os, sys
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
-import os, getopt, signal, select, string, time
+import getopt, signal, select, string, time
 import tarfile, subprocess, struct, platform
-import socket, threading, tracemalloc, inspect
-
-if sys.version_info[0] < 3:
-    import SocketServer as socketserver
-else:
-    import socketserver
+import socket, threading, tracemalloc, inspect, socketserver
 
 import pyvpacker
 
 # This repairs the path from local run to pip run.
 # Remove pip version for local tests
 try:
     from pyvcommon import support
-
     # Get Parent of module root
-    sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
-    #print("sf", sf)
-    sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    #print("base", base)
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base, "..", "pyvcommon"))
+    sys.path.append(os.path.join(base, "..", "pyvserver"))
 
 except:
     base = os.path.dirname(os.path.realpath(__file__))
+    #print("local base", base)
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-#for aa in sys.path:
-#    print(aa)
-
-print("Load:", sys.path[-1])
-
 from pyvcommon import support, pyservsup, pyclisup
 from pyvcommon import pydata, pysyslog, comline, pyvhash
 
 from pydbase import twincore, twinchain
 
 replicname = "replic.pydb"
 datafname = "initial.pydb"
```

### Comparing `pyvserv-1.0.2/pyvserver/pyvserv.py` & `pyvserv-1.0.3/pyvserver/pyvserv.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,36 @@
 import sys
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
 import os, getopt, signal, select, string, time
-import tarfile, subprocess, struct, platform
-import socket, threading, tracemalloc, inspect
+import subprocess,  platform, queue, ctypes
+import socket, threading, tracemalloc, copy, random
+
+import multiprocessing as mp
+
+try:
+    import fcntl
+except:
+    fcntl = None
 
 if sys.version_info[0] < 3:
     import SocketServer as socketserver
 else:
     import socketserver
 
 import pyvpacker
 
-# Create a placeholder
+#import gi
+#gi.require_version("Gtk", "3.0")
+#from gi.repository import GLib
+
+# Create a placeholder for the main server var
 server = None
 
 progname = os.path.split(sys.argv[0])[1]
 
 # This repairs the path from local run to pip run.
 # Remove pip version for local tests
 try:
@@ -33,108 +44,130 @@
 
     # Get Parent of module root
     sf = os.path.dirname(support.__file__)
     sf = os.path.dirname(sf)
     #print("sf", sf)
     sys.path.append(os.path.join(sf, "pyvcommon"))
     sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
-
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-#for aa in sys.path:
-#    print(aa)
-
-print("Load:", sys.path[-1])
-
 from pyvcommon import support, pyservsup, pyclisup
 from pyvcommon import pydata, pysyslog, comline
 
 from pyvserver import pyvstate
 from pyvserver import pyvfunc
 
-version = "1.0"
+# Update it from setup
+version = "1.0.3"
 
 mydata = {}
 
 # ------------------------------------------------------------------------
 
 class InvalidArg(Exception):
 
     ''' Exception for bad arguments '''
 
     def __init__(self, message):
          self.message = message
 
-# ------------------------------------------------------------------------
+# Using globals here; class instances fooled by threading
+#gl_sem = threading.Semaphore()
+#gl_queue = queue.Queue()
+#global gl_queue
+#gl_queue.put((peer, now))
+#print("qsize", gl_queue.qsize)
 
-connlist = []
-sem = threading.Semaphore()
+# ------------------------------------------------------------------------
 
-def throttle(peer):
+class Throttle():
 
-    '''  Catch clients that are connecting too fast. This is a crude
-         implementation, will need serious uppdate on large volume production
+    '''  Catch clients that are connecting too fast. This needs a serious
+        upgrade if in large volume production.
     '''
+    def __init__(self):
+
+        if fcntl:
+            # This is for forkmixin
+            self.sem  = mp.Semaphore()
+            self.man  = mp.Manager()
+            self.connlist = self.man.list()
+        else:
+            self.sem     = threading.Semaphore()
+            self.connlist = []
+
+    def throttle(self, peer):
+
+        '''
+            Catch clients that are connecting too fast.
+            Throttle to N sec frequency, if number of connections from
+            the same ip exceeds throt_instances.
+        '''
+
+        wantsleep = 0; sss = 0;
+        now = time.time()
+        self.sem.acquire()
+
+        for aa in self.connlist:
+            if aa[0] == peer[0]:
+                if now - aa[1] <  pyservsup.globals.throt_sec:
+                    sss += 1
+
+        if sss >  pyservsup.globals.throt_instances:
+            # Clean old entries fot this host
+            for aa in range(len(self.connlist)-1, -1 ,-1):
+                if self.connlist[aa][0] == peer[0]:
+                    if now - self.connlist[aa][1] > pyservsup.globals.throt_sec:
+                        del self.connlist[aa]
+            wantsleep = pyservsup.globals.throt_time
+
+        # Clean throtle data periodically
+        if len(self.connlist) > pyservsup.globals.throt_maxdat:
+            #print("Cleaning throttle list", len(self.connlist))
+            for aa in range(len(self.connlist)-1, -1 ,-1):
+                if now - self.connlist[aa][1] > pyservsup.globals.throt_maxsec:
+                    del self.connlist[aa]
+
+        # Flatten list for the multiprocessing context manager
+        self.connlist.append((peer[0], now))
 
-    global connlist, sem
-    #print("throttle", peer)
+        #print("connlist", self.connlist)  # Make sure it cycles
+        #print()
 
-    # Throttle to 10 sec frequency
-    now = time.time()
-    sem.acquire()
-    sss = 0; slept = False
-    for aa in connlist:
-        if aa[0][0] == peer[0]:
-            if now - aa[1] <  pyservsup.globals.throttle:
-                sss += 1
-    if sss >  pyservsup.globals.instance:
-        for aa in range(len(connlist)-1, -1 ,-1):
-            if connlist[aa][0][0] == peer[0]:
-                if now - connlist[aa][1] > pyservsup.globals.throttle:
-                    del connlist[aa]
-        time.sleep(5.)
-        slept = True
-
-    # Clean throtle data periodically
-    if len(connlist) > pyservsup.globals.maxthdat:
-        for aa in range(len(connlist)-1, -1 ,-1):
-            if connlist[aa][0][0] == peer[0]:
-                if now - connlist[aa][1] > pyservsup.globals.throttle:
-                    del connlist[aa]
-    connlist.append((peer, now))
-    #print(connlist)
-    sem.release()
-    return slept
+        self.sem.release()
+        return wantsleep
+
+# The one and only instance
+gl_throttle = Throttle()
 
 class ThreadedTCPRequestHandler(socketserver.BaseRequestHandler):
 
     ''' Request handler. '''
 
     def __init__(self, a1, a2, a3):
+
+        self.verbose = conf.verbose
+        self.a1 = a1
         self.a2 = a2
         self.fname = ""
         self.user = ""
         self.cwd = os.getcwd()
         self.dir = ""
         self.ekey = ""
-        self.verbose = conf.verbose
 
-        ttt = throttle(a1.getpeername())
-        if self.verbose:
-            if ttt > 0:
-                print ("Throttle sleep",  a1.getpeername())
+        ttt = gl_throttle.throttle(self.a1.getpeername())
+        if ttt > 0:
+            if self.verbose > 0:
+                print("Throttle sleep",  a1.getpeername())
+            time.sleep(ttt)
 
         socketserver.BaseRequestHandler.__init__(self, a1, a2, a3)
 
     def setup(self):
 
         ''' Start server '''
 
@@ -148,17 +181,14 @@
 
         self.name  = str(cur_thread._native_id) #name #getName()
         #self.name  = cur_thread.name #getName()
         #print( "Logoff '" + usr + "'", cli)
         if self.verbose:
             print( "Connection from ", self.a2, "as", self.name)
 
-        #if pgdebug > 1:
-        #    put_debug("Connection from %s" % self.a2)
-
         self.statehandler = pyvstate.StateHandler(self)
         self.statehandler.verbose = conf.verbose
         self.statehandler.pglog = conf.pglog
         self.statehandler.pgdebug = conf.pgdebug
         self.statehandler.name    = self.name
 
         #print(self.request)
@@ -244,18 +274,25 @@
         if conf.pglog > 0:
             pysyslog.syslog("Logoff '" + usr + "' " + cli)
 
         #server.socket.shutdown(socket.SHUT_RDWR)
         #server.socket.close()
 
 # ------------------------------------------------------------------------
-# Override stock methods
+# Override stock methods. Windows has no ForkinMixin
+
+if not fcntl:
+    mixin = socketserver.ThreadingMixIn
+else:
+    mixin = socketserver.ForkingMixIn
 
-#class ThreadedTCPServer(socketserver.ThreadingMixIn, socketserver.TCPServer):
-class ThreadedTCPServer(socketserver.ForkingMixIn, socketserver.TCPServer):
+# Overriding it for throttle development
+#mixin = socketserver.ThreadingMixIn
+
+class ThreadedTCPServer(mixin, socketserver.TCPServer):
 
     ''' Overridden socket server '''
 
     #def __init__(self, arg1, arg2):
     #    self._BaseServer__shutdown_request = True
 
     def stop(self):
@@ -426,15 +463,14 @@
             snapshot = tracemalloc.take_snapshot()
             top_stats = snapshot.statistics('lineno')
 
         if self.verbose:
             print("ended thread", self.name)
 
 
-
 def simple_server(HOST, PORT):
 
     ''' This was a test server, left it in for future refernence.
         It was marginally faster than the stock version, also less features,
          so the stock servers stayed.
     '''
 
@@ -446,60 +482,65 @@
         while True:
             client, addr = server.accept()
             client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
             serve_one(client, addr, args)
 
 # ------------------------------------------------------------------------
 
-optarr =  comline.optarrlong
-optarr.append ( ["e",   "detach=",   "detach",      0,       None, "Detach from terminal"] )
+optarr =  [] #comline.optarrlong
+#optarr.append ( ["e",   "detach=",   "detach",      0,       None, "Detach from terminal."] )
+optarr.append ( ["n:",  "host",      "host",   "127.0.0.1",  None, "Set server hostname / interface."] )
+optarr.append ( ["r:",  "dataroot=", "droot",  "pyvserver",  None, "Set data root for server. "] )
+optarr.append ( ["P",   "pmode",     "pmode",       0,       None, "Production mode ON. (allow 2FA)"] )
 optarr.append ( ["l:",  "loglevel",  "pglog",       1,       None, "Log level (0 - 10) default = 1"] )
-optarr.append ( ["n:",  "host",      "host",   "127.0.0.1",  None, "Set server hostname"] )
-optarr.append ( ["r:",  "dataroot=", "droot",  "pyvserver",  None, "Root for server data"] )
 optarr.append ( ["m",   "mem",       "mem",         0,       None, "Show memory trace."] )
-optarr.append ( ["D",   "dmode",     "dmode",       0,       None, "Dev mode (no twofa)"] )
-optarr.append ( ["N",   "norepl",    "norepl",      0,       None, "No replication (for test)"] )
+optarr.append ( ["N",   "norepl",    "norepl",      0,       None, "No replication. (for testing)"] )
+
+for aa in comline.optarrlong:
+    optarr.append(aa)
+
+comline.optarrlong = optarr
+
+# Tue 02.Apr.2024 made devmode default
 
 #print (optarr)
 comline.setargs("")
 comline.setfoot("Use quotes for argument separations.")
 
 conf = comline.ConfigLong(optarr)
 #conf.printvars()
 
-
 def mainfunct():
 
     ''' Main entry point. The pip install will call this script. '''
 
     if sys.version_info[0] < 3:
-        print("Warning! This script was meant for python 3.x")
+        print("This script was meant for python 3.x")
         time.sleep(.1)
         sys.exit(0)
 
     args = conf.comline(sys.argv[1:])
     #print(args)
 
     # Print comline args
     if conf.pgdebug > 7:
         for aa in vars(conf):
-            if aa != "optarr":
-                print(aa, "=", getattr(conf, aa), end = "   ")
+            if aa != "_optarr":
+                print(aa, "=", getattr(conf, aa), end = "    ")
         print()
 
-    if conf.verbose:
-        pass
-        #print("This script:     ", os.path.realpath(__file__))
-        #print("Full path argv:  ", os.path.abspath(sys.argv[0]))
-        #print("Script name:     ", __file__)
-        #print("Exec argv:       ", sys.argv[0])
+    if conf.pgdebug > 4:
+        print("This script:     ", os.path.realpath(__file__))
+        print("Full path argv:  ", os.path.abspath(sys.argv[0]))
+        print("Script name:     ", __file__)
+        print("Exec argv:       ", sys.argv[0])
 
     pyservsup.globals  = pyservsup.Global_Vars(__file__, conf.droot)
     pyservsup.globals.conf = conf
-    pyservsup.globals.lockfname += "_" + str(conf.port)  # Lock file + port
+    pyservsup.globals.lockfname += "_" + str(conf.port) + "_" + str(conf.host)
     pyservsup.globals._softmkdir(pyservsup.globals.myhome)
 
     # Change directory to the data dir
     os.chdir(pyservsup.globals.myhome)
     #print("cwd", os.getcwd())
 
     pyservsup.globals.config(pyservsup.globals.myhome, conf)
@@ -516,26 +557,33 @@
     try:
         keyfroot = pyservsup.pickkey(pyservsup.globals.keydir)
     except:
         #print("No keys generated yet. Please run pyvgenkey.py first.")
         exec = os.path.dirname(os.path.split(pyservsup.globals._script_home)[0]) + os.sep
         exec += "../pyvtools/pyvgenkey.py"
         print("Notice: Generating key in", "'" + pyservsup.globals.keydir + "'")
-        print("For added security please generate more keys with 'pyvgenkeys'");
-        if conf.pgdebug > 2:
-            print("Exec:  ", exec)
-
         try:
-            os.system("%s -q -m %s " % (exec, pyservsup.globals.myhome))
-            #if conf.verbose:
-                #print("exc", sys.exc_info())
-                #support.put_exception("Generating keys")
+            if conf.pgdebug > 2:
+                print("Generating keys", exec)
+            # Early out for no script
+            if not os.path.isfile(exec):
+                raise
+            ret = subprocess.Popen([exec, "-q", "-m", pyservsup.globals.myhome])
         except:
-            print("Could not generate key. Keydir was", pyservsup.globals.keydir)
-            sys.exit(1)
+            try:
+                # Try with full install version
+                #print("Executing with installed version")
+                exec = "pyvgenkey"
+                ret = subprocess.Popen([exec, "-q", "-m", pyservsup.globals.myhome])
+            except:
+                print("Could not generate key. Keydir was:", pyservsup.globals.keydir)
+                print("Please try again manually with the 'pvgenkey' utility.")
+
+            print("For added security please generate more keys with 'pyvgenkeys'");
+            #sys.exit(1)
 
     iii = pyservsup.create_read_idfile(pyservsup.globals.idfile)
     if not iii:
         print("Cannot read / create site ID, exiting.")
         sys.exit(1)
 
     pyservsup.globals.siteid = iii
@@ -546,15 +594,15 @@
     # Set termination handlers, so lock will be deleted
     signal.signal(signal.SIGTERM, terminate)
     signal.signal(signal.SIGINT, soft_terminate)
     try:
         signal.signal(signal.SIGUSR1, usersig)
         signal.signal(signal.SIGUSR2, usersig2)
     except:
-        print("User signal may not be available.")
+        print("User signals may not be available.")
 
     sys.stdout = support.Unbuffered(sys.stdout)
     sys.stderr = support.Unbuffered(sys.stderr)
 
     # Comline processed, go
     support.lock_process(pyservsup.globals.lockfname)
 
@@ -564,65 +612,73 @@
     slogfile = os.path.join(pyservsup.globals.logdir, pyservsup.logfname + ".log")
     rlogfile = os.path.join(pyservsup.globals.logdir, pyservsup.repfname +".log")
 
     pysyslog.init_loggers(
             ("system", slogfile), ("replic", rlogfile))
     #pysyslog.syslog("Started Server")
 
-    # Port 0 would mean to select an arbitrary unused port
-    HOST, PORT = conf.host, conf.port
-
     if not conf.quiet:
+        if not pyservsup.globals.conf.pmode:
+            print("Warning! Devmode ON. Use -P to allow 2FA auth")
         try:
             import distro
             strx = distro.name()
         except:
             strx = "Win or Unkn."
 
         print("MainSiteID:      ", pyservsup.globals.siteid)
-        print("Server running: ", "'"+HOST+"'", "Port:", PORT)
+        print("Server running: ", "'"+conf.host+"'", "Port:", conf.port)
         pyver = support.list2str(sys.version_info) #[0:3], ".")
         print("Running python", platform.python_version(), "on", platform.system(), strx)
 
-        pyvstate.init_state_table()
+    pyvstate.init_state_table()
+
+    # Parse multiple host (interace) options (disabled)
+    #hostarr = []
+    #import shlex
+    #hostarr = shlex.split(conf.host)
+    #print("hostarr", hostarr)
+
+    global server
     try:
-        global server
-        server = ThreadedTCPServer((HOST, PORT), ThreadedTCPRequestHandler)
+        server = ThreadedTCPServer((conf.host, conf.port), ThreadedTCPRequestHandler)
         server.allow_reuse_address = True
         ip, port = server.server_address
         server.allow_reuse_address = True
         server.verbose = conf.verbose
 
         # Start a thread with the server -- that thread will then start one
         # or more threads for each request
         server_thread = threading.Thread(target=server.serve_forever)
 
         # Exit the server thread when the main thread terminates
         server_thread.verbose = conf.verbose
-        #server_thread.setDaemon(True)
         server_thread.daemon = True
         #server_thread.paydir =  pyservsup.globals.paydir
         server_thread.start()
 
     except:
-        print( "Cannot start server. ", sys.exc_info()[1])
+        print( "Cannot start server. ", sys.exc_info())
         if conf.pglog > 0:
-            pysyslog.syslog("Cannot start server " + str(sys.exc_info()[1]) )
-
-        #print("Try again later.")
-        terminate(None, None)
-        #sys.exit(1)
+            pysyslog.syslog("Cannot start server ", sys.exc_info())
+            #print("Try again later.")
+            #terminate(None, None)
+            sys.exit(1)
 
     #if conf.pglog > 0:
-    #    pysyslog.syslog("Started Server")
+    #     pysyslog.syslog("Started Server")
 
     if conf.pglog > 0:
-        pysyslog.syslog("Server started. Devmode %d" % conf.dmode)
+        pysyslog.syslog("Server started. Prodmode %d" % conf.pmode)
 
-    # Block
     #simple_server(HOST, PORT)
+    # Block
     server.serve_forever()
 
+    #if conf.detach:
+    #    print("Detach from terminal:)
+
+
 if __name__ == '__main__':
     mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.2/pyvserver/pyvstate.py` & `pyvserv-1.0.3/pyvserver/pyvstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
 from Crypto.Hash import SHA512
 import os, sys, getopt, signal, select, string, time, stat, base64
-import inspect, fcntl, multiprocessing
+import inspect, multiprocessing
+
+try:
+    import fcntl
+except:
+    fcntl = None
 
 import pyvpacker
 
 import pyservsup, pyclisup, support
 import crysupp, pysyslog, pywrap
 
 from pyvfunc import *
@@ -106,72 +111,71 @@
 # function is executed. The new state set to end_state
 
 def init_state_table():
 
     global state_table
     #print("pystate init table")
     # This is to develop without entering auth code every time
-    if pyservsup.globals.conf.dmode:
-        print("Warning! devmode ON")
+    if not pyservsup.globals.conf.pmode:
         minauth =  auth_pass
     else:
         minauth =  auth_twofa
 
     state_table = \
     [
-    # Command; start_state; end_state; min_auth; action func;   help func
-    ("ver",     all_in,     none_in,    initial,  get_ver_func,   vers_help),
-    ("id",      all_in,     none_in,    initial,  get_id_func,    id_help),
-    ("hello",   all_in,     none_in,    initial,  get_hello_func, hello_help),
-    ("helo",    all_in,     none_in,    initial,  get_hello_func, hello_help),
-    ("quit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
-    ("exit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
-    ("help",    all_in,     none_in,    initial,  get_help_func,  help_help),
-    #("xkey",    all_in,     none_in,    initial,  get_xkey_func,  ekey_help),
-    #("ekey",    all_in,     none_in,    initial,  get_ekey_func,  ekey_help),
-    ("akey",    all_in,     none_in,    initial,  get_akey_func,  akey_help),
-    ("uini",    all_in,     none_in,    initial,  get_uini_func,  uini_help),
-    #("kadd",    all_in,     none_in,    initial,  get_kadd_func,  kadd_help),
-    ("user",    all_in,     none_in,    initial,  get_user_func,  user_help),
-    ("pass",    all_in,     auth_pass,  initial,  get_pass_func,  pass_help),
-    ("logout",  all_in,     initial,    auth_pass,get_logout_func,  logout_help),
-    ("sess",    all_in,     none_in,    initial,  get_sess_func,  sess_help),
-    ("tout",    all_in,     none_in,    initial,  get_tout_func,  tout_help),
-    ("qr",      all_in,     none_in,    initial,  get_qr_func,    qr_help),
-    ("chpass",  all_in,  none_in,    auth_pass, get_chpass_func,  chpass_help),
-    ("file",    all_in,  none_in,    auth_pass, put_file_func, file_help),
-    ("mkdir",   all_in,  none_in,    auth_pass, get_mkdir_func, file_help),
-    ("data",    all_in,  none_in,    auth_pass, put_data_func,  data_help),
-    ("fget",    all_in,  none_in,    auth_pass, get_fget_func,  fget_help),
-    ("fput",    all_in,  none_in,    auth_pass, get_fput_func,  fput_help),
-    ("del",     all_in,  none_in,    auth_pass, get_del_func,   del_help),
-    ("uadd",    all_in,  none_in,    auth_pass, get_uadd_func,  uadd_help),
-    ("uena",    all_in,  none_in,    auth_pass, get_uena_func,  uena_help),
-    ("aadd",    all_in,  none_in,    auth_pass, get_aadd_func,  aadd_help),
-    ("udel",    all_in,  none_in,    auth_pass, get_udel_func,  udel_help),
-    ("ls",      all_in,  none_in,    auth_pass, get_ls_func,    lsls_help),
-    ("lsd",     all_in,  none_in,    auth_pass, get_lsd_func,   lsld_help),
-    ("cd",      all_in,  none_in,    auth_pass, get_cd_func,    cdcd_help),
-    ("pwd",     all_in,  none_in,    auth_pass, get_pwd_func,   pwdd_help),
-    ("stat",    all_in,  none_in,    auth_pass, get_stat_func,  stat_help),
-    ("buff",    all_in,  none_in,    auth_pass, get_buff_func,  buff_help),
-    ("twofa",   all_in,  auth_twofa, auth_pass, get_twofa_func,  twofa_help),
-
-    ("dmode",   all_in,  none_in,    initial, get_dmode_func,  dmode_help),
-    ("ihave",   all_in,  none_in,    initial, get_ihave_func,  ihave_help),
-    ("ihost",   all_in,  none_in,    initial, get_ihost_func,  ihost_help),
-
-    # Following the two factor auth commands. Disabled during development
-    ("rput",     all_in,  none_in,    minauth,   get_rput_func,   rput_help),
-    ("rcheck",   all_in,  none_in,    minauth,   get_rcheck_func,  rcheck_help),
-    ("rlist",    all_in,  none_in,    auth_pass, get_rlist_func,  rlist_help),
-    ("rcount",   all_in,  none_in,    auth_pass, get_rcount_func, rcount_help),
-    ("rsize",    all_in,  none_in,    auth_pass, get_rsize_func,  rsize_help),
-    ("rget",     all_in,  none_in,    auth_pass, get_rget_func,   rget_help),
-    ("rhave",    all_in,  none_in,    auth_pass, get_rhave_func,   rhave_help),
+        # Command; start_state; end_state; min_auth; action func;   help func
+        ("ver",     all_in,     none_in,    initial,  get_ver_func,   vers_help),
+        ("id",      all_in,     none_in,    initial,  get_id_func,    id_help),
+        ("hello",   all_in,     none_in,    initial,  get_hello_func, hello_help),
+        ("helo",    all_in,     none_in,    initial,  get_hello_func, hello_help),
+        ("quit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
+        ("exit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
+        ("help",    all_in,     none_in,    initial,  get_help_func,  help_help),
+        #("xkey",    all_in,     none_in,    initial,  get_xkey_func,  ekey_help),
+        #("ekey",    all_in,     none_in,    initial,  get_ekey_func,  ekey_help),
+        ("akey",    all_in,     none_in,    initial,  get_akey_func,  akey_help),
+        ("uini",    all_in,     none_in,    initial,  get_uini_func,  uini_help),
+        #("kadd",    all_in,     none_in,    initial,  get_kadd_func,  kadd_help),
+        ("user",    all_in,     none_in,    initial,  get_user_func,  user_help),
+        ("pass",    all_in,     auth_pass,  initial,  get_pass_func,  pass_help),
+        ("logout",  all_in,     initial,    auth_pass,get_logout_func,  logout_help),
+        ("sess",    all_in,     none_in,    initial,  get_sess_func,  sess_help),
+        ("tout",    all_in,     none_in,    initial,  get_tout_func,  tout_help),
+        ("qr",      all_in,     none_in,    initial,  get_qr_func,    qr_help),
+        ("chpass",  all_in,  none_in,    auth_pass, get_chpass_func,  chpass_help),
+        ("file",    all_in,  none_in,    auth_pass, put_file_func, file_help),
+        ("mkdir",   all_in,  none_in,    auth_pass, get_mkdir_func, file_help),
+        ("data",    all_in,  none_in,    auth_pass, put_data_func,  data_help),
+        ("fget",    all_in,  none_in,    auth_pass, get_fget_func,  fget_help),
+        ("fput",    all_in,  none_in,    auth_pass, get_fput_func,  fput_help),
+        ("del",     all_in,  none_in,    auth_pass, get_del_func,   del_help),
+        ("uadd",    all_in,  none_in,    auth_pass, get_uadd_func,  uadd_help),
+        ("uena",    all_in,  none_in,    auth_pass, get_uena_func,  uena_help),
+        ("aadd",    all_in,  none_in,    auth_pass, get_aadd_func,  aadd_help),
+        ("udel",    all_in,  none_in,    auth_pass, get_udel_func,  udel_help),
+        ("ls",      all_in,  none_in,    auth_pass, get_ls_func,    lsls_help),
+        ("lsd",     all_in,  none_in,    auth_pass, get_lsd_func,   lsld_help),
+        ("cd",      all_in,  none_in,    auth_pass, get_cd_func,    cdcd_help),
+        ("pwd",     all_in,  none_in,    auth_pass, get_pwd_func,   pwdd_help),
+        ("stat",    all_in,  none_in,    auth_pass, get_stat_func,  stat_help),
+        ("buff",    all_in,  none_in,    auth_pass, get_buff_func,  buff_help),
+        ("twofa",   all_in,  auth_twofa, auth_pass, get_twofa_func,  twofa_help),
+
+        ("dmode",   all_in,  none_in,    initial, get_dmode_func,  dmode_help),
+        ("ihave",   all_in,  none_in,    initial, get_ihave_func,  ihave_help),
+        ("ihost",   all_in,  none_in,    initial, get_ihost_func,  ihost_help),
+
+        # Following the two factor auth commands. Disabled during development
+        ("rput",     all_in,  none_in,    minauth,   get_rput_func,   rput_help),
+        ("rcheck",   all_in,  none_in,    minauth,   get_rcheck_func,  rcheck_help),
+        ("rlist",    all_in,  none_in,    auth_pass, get_rlist_func,  rlist_help),
+        ("rcount",   all_in,  none_in,    auth_pass, get_rcount_func, rcount_help),
+        ("rsize",    all_in,  none_in,    auth_pass, get_rsize_func,  rsize_help),
+        ("rget",     all_in,  none_in,    auth_pass, get_rget_func,   rget_help),
+        ("rhave",    all_in,  none_in,    auth_pass, get_rhave_func,   rhave_help),
     ]
 # ------------------------------------------------------------------------
 
 class StateHandler():
 
     def __init__(self, resp):
 
@@ -191,21 +195,23 @@
         while True:
             if os.path.isfile(self.lockname):
                 time.sleep(1)
             else:
                 break
         try:
             self.fpx = open(self.lockname, "wb")
-            fcntl.lockf(self.fpx, fcntl.LOCK_EX)
+            if fcntl:
+                fcntl.lockf(self.fpx, fcntl.LOCK_EX)
         except:
             print(sys.exc_info())
             pass
 
     def dellock(self):
-        fcntl.lockf(self.fpx, fcntl.LOCK_EX)
+        if fcntl:
+            fcntl.lockf(self.fpx, fcntl.LOCK_EX)
         try:
             self.fpx.close()
             os.unlink(self.lockname)
         except:
             print(sys.exc_info())
             pass
```

### Comparing `pyvserv-1.0.2/pyvtools/pyvgenkey.py` & `pyvserv-1.0.3/pyvtools/pyvgenkey.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,31 +30,23 @@
 
     # Get Parent of module root
     sf = os.path.dirname(support.__file__)
     sf = os.path.dirname(sf)
     #print("sf", sf)
     sys.path.append(os.path.join(sf, "pyvcommon"))
     sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
 
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-#for aa in sys.path:
-#    print(aa)
-
-print("Load:", sys.path[-1])
-
+#print("Load:", sys.path[-1])
 
 from pyvcommon import pyservsup
 
 import argparse
 
 parser = argparse.ArgumentParser(description='Genetrate ECC keypair for pyvserv')
```

### Comparing `pyvserv-1.0.2/pyvtools/pyvgenkeys.py` & `pyvserv-1.0.3/pyvtools/pyvgenkeys.py`

 * *Files identical despite different names*

