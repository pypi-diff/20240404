# Comparing `tmp/mitogen-0.3.5.tar.gz` & `tmp/mitogen-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitogen-0.3.5.tar", last modified: Thu Mar 28 16:18:29 2024, max compression
+gzip compressed data, was "mitogen-0.3.6.tar", last modified: Thu Apr  4 12:55:07 2024, max compression
```

## Comparing `mitogen-0.3.5.tar` & `mitogen-0.3.6.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.324579 mitogen-0.3.5/
--rw-r--r--   0 alex       (501) staff       (20)     1465 2022-06-24 21:10:35.000000 mitogen-0.3.5/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       16 2022-06-24 21:04:22.000000 mitogen-0.3.5/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     1776 2024-03-28 16:18:29.324522 mitogen-0.3.5/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      495 2022-06-24 21:10:35.000000 mitogen-0.3.5/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.315965 mitogen-0.3.5/ansible_mitogen/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/affinity.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.316071 mitogen-0.3.5/ansible_mitogen/compat/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    39600 2023-07-28 23:27:24.000000 mitogen-0.3.5/ansible_mitogen/connection.py
--rw-r--r--   0 alex       (501) staff       (20)     3851 2024-03-28 16:09:46.000000 mitogen-0.3.5/ansible_mitogen/loaders.py
--rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/logging.py
--rw-r--r--   0 alex       (501) staff       (20)    21499 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/mixins.py
--rw-r--r--   0 alex       (501) staff       (20)     9588 2024-03-28 16:10:59.000000 mitogen-0.3.5/ansible_mitogen/module_finder.py
--rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/parsing.py
--rw-r--r--   0 alex       (501) staff       (20)    22044 2023-07-02 18:42:28.000000 mitogen-0.3.5/ansible_mitogen/planner.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.316156 mitogen-0.3.5/ansible_mitogen/plugins/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/plugins/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.316470 mitogen-0.3.5/ansible_mitogen/plugins/action/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/plugins/action/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/action/mitogen_fetch.py
--rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/action/mitogen_get_stack.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.318596 mitogen-0.3.5/ansible_mitogen/plugins/connection/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_buildah.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_doas.py
--rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_docker.py
--rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_jail.py
--rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_kubectl.py
--rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_local.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_lxd.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_machinectl.py
--rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_podman.py
--rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_setns.py
--rw-r--r--   0 alex       (501) staff       (20)     3301 2024-03-28 16:09:46.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_ssh.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_su.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_sudo.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.319247 mitogen-0.3.5/ansible_mitogen/plugins/strategy/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/ansible_mitogen/plugins/strategy/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen.py
--rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_free.py
--rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
--rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-24 21:10:35.000000 mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_linear.py
--rw-r--r--   0 alex       (501) staff       (20)    24921 2024-03-28 16:09:46.000000 mitogen-0.3.5/ansible_mitogen/process.py
--rw-r--r--   0 alex       (501) staff       (20)    37900 2024-03-28 16:10:59.000000 mitogen-0.3.5/ansible_mitogen/runner.py
--rw-r--r--   0 alex       (501) staff       (20)    20647 2023-08-10 08:38:54.000000 mitogen-0.3.5/ansible_mitogen/services.py
--rw-r--r--   0 alex       (501) staff       (20)    12611 2024-03-28 16:09:46.000000 mitogen-0.3.5/ansible_mitogen/strategy.py
--rw-r--r--   0 alex       (501) staff       (20)    25091 2023-08-10 08:38:54.000000 mitogen-0.3.5/ansible_mitogen/target.py
--rw-r--r--   0 alex       (501) staff       (20)    27116 2024-03-28 16:09:46.000000 mitogen-0.3.5/ansible_mitogen/transport_config.py
--rw-r--r--   0 alex       (501) staff       (20)      604 2024-03-28 16:10:59.000000 mitogen-0.3.5/ansible_mitogen/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.323002 mitogen-0.3.5/mitogen/
--rw-r--r--   0 alex       (501) staff       (20)     4145 2024-03-28 16:10:59.000000 mitogen-0.3.5/mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2681 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/buildah.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.323983 mitogen-0.3.5/mitogen/compat/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.5/mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    20406 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/compat/pkgutil.py
--rw-r--r--   0 alex       (501) staff       (20)    17572 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/compat/tokenize.py
--rw-r--r--   0 alex       (501) staff       (20)   151746 2024-03-28 16:10:59.000000 mitogen-0.3.5/mitogen/core.py
--rw-r--r--   0 alex       (501) staff       (20)     6699 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/debug.py
--rw-r--r--   0 alex       (501) staff       (20)     4958 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/doas.py
--rw-r--r--   0 alex       (501) staff       (20)     3085 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/docker.py
--rw-r--r--   0 alex       (501) staff       (20)    15577 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/fakessh.py
--rw-r--r--   0 alex       (501) staff       (20)     8436 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/fork.py
--rw-r--r--   0 alex       (501) staff       (20)     2537 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/jail.py
--rw-r--r--   0 alex       (501) staff       (20)     2561 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/kubectl.py
--rw-r--r--   0 alex       (501) staff       (20)     2853 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     2844 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/lxd.py
--rw-r--r--   0 alex       (501) staff       (20)    55088 2024-03-28 16:10:59.000000 mitogen-0.3.5/mitogen/master.py
--rw-r--r--   0 alex       (501) staff       (20)     5093 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/minify.py
--rw-r--r--   0 alex       (501) staff       (20)     6624 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/os_fork.py
--rw-r--r--   0 alex       (501) staff       (20)    98171 2024-03-28 16:10:59.000000 mitogen-0.3.5/mitogen/parent.py
--rw-r--r--   0 alex       (501) staff       (20)     2730 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/podman.py
--rw-r--r--   0 alex       (501) staff       (20)     5392 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/profiler.py
--rw-r--r--   0 alex       (501) staff       (20)    12325 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/select.py
--rw-r--r--   0 alex       (501) staff       (20)    41699 2024-03-28 16:10:59.000000 mitogen-0.3.5/mitogen/service.py
--rw-r--r--   0 alex       (501) staff       (20)     8450 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/setns.py
--rw-r--r--   0 alex       (501) staff       (20)    10892 2024-03-28 16:09:56.000000 mitogen-0.3.5/mitogen/ssh.py
--rw-r--r--   0 alex       (501) staff       (20)     5656 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/su.py
--rw-r--r--   0 alex       (501) staff       (20)    12089 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/sudo.py
--rw-r--r--   0 alex       (501) staff       (20)     7133 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/unix.py
--rw-r--r--   0 alex       (501) staff       (20)     7167 2023-08-10 08:38:54.000000 mitogen-0.3.5/mitogen/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.324329 mitogen-0.3.5/mitogen.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1776 2024-03-28 16:18:29.000000 mitogen-0.3.5/mitogen.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2430 2024-03-28 16:18:29.000000 mitogen-0.3.5/mitogen.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-03-28 16:18:29.000000 mitogen-0.3.5/mitogen.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-03-28 16:18:29.000000 mitogen-0.3.5/mitogen.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       24 2024-03-28 16:18:29.000000 mitogen-0.3.5/mitogen.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)      206 2024-03-28 16:18:29.324783 mitogen-0.3.5/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     3591 2024-03-28 16:10:59.000000 mitogen-0.3.5/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-28 16:18:29.324160 mitogen-0.3.5/tests/
--rw-r--r--   0 alex       (501) staff       (20)    20874 2024-03-28 16:10:59.000000 mitogen-0.3.5/tests/testlib.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793728 mitogen-0.3.6/
+-rw-r--r--   0 alex       (501) staff       (20)     1465 2022-06-24 21:10:35.000000 mitogen-0.3.6/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       16 2022-06-24 21:04:22.000000 mitogen-0.3.6/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-04 12:55:07.793673 mitogen-0.3.6/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      495 2022-06-24 21:10:35.000000 mitogen-0.3.6/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.782550 mitogen-0.3.6/ansible_mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/affinity.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.782931 mitogen-0.3.6/ansible_mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    39735 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/connection.py
+-rw-r--r--   0 alex       (501) staff       (20)     3851 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/loaders.py
+-rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)    21609 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/mixins.py
+-rw-r--r--   0 alex       (501) staff       (20)     9588 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/module_finder.py
+-rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/parsing.py
+-rw-r--r--   0 alex       (501) staff       (20)    22044 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/planner.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.783031 mitogen-0.3.6/ansible_mitogen/plugins/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.783524 mitogen-0.3.6/ansible_mitogen/plugins/action/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_fetch.py
+-rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_get_stack.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.785716 mitogen-0.3.6/ansible_mitogen/plugins/connection/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_buildah.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_docker.py
+-rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_local.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_machinectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_setns.py
+-rw-r--r--   0 alex       (501) staff       (20)     3301 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_su.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_sudo.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.786339 mitogen-0.3.6/ansible_mitogen/plugins/strategy/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen.py
+-rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_free.py
+-rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
+-rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_linear.py
+-rw-r--r--   0 alex       (501) staff       (20)    24921 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/process.py
+-rw-r--r--   0 alex       (501) staff       (20)    37900 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/runner.py
+-rw-r--r--   0 alex       (501) staff       (20)    20677 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/services.py
+-rw-r--r--   0 alex       (501) staff       (20)    12611 2024-03-28 16:09:46.000000 mitogen-0.3.6/ansible_mitogen/strategy.py
+-rw-r--r--   0 alex       (501) staff       (20)    25091 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/target.py
+-rw-r--r--   0 alex       (501) staff       (20)    27116 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/transport_config.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.786566 mitogen-0.3.6/ansible_mitogen/utils/
+-rw-r--r--   0 alex       (501) staff       (20)      604 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2586 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/utils/unsafe.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.791856 mitogen-0.3.6/mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)     4145 2024-04-04 12:53:20.000000 mitogen-0.3.6/mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2681 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/buildah.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.792865 mitogen-0.3.6/mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    20406 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/compat/pkgutil.py
+-rw-r--r--   0 alex       (501) staff       (20)    17572 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/compat/tokenize.py
+-rw-r--r--   0 alex       (501) staff       (20)   151746 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/core.py
+-rw-r--r--   0 alex       (501) staff       (20)     6699 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/debug.py
+-rw-r--r--   0 alex       (501) staff       (20)     4958 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     3085 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/docker.py
+-rw-r--r--   0 alex       (501) staff       (20)    15577 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/fakessh.py
+-rw-r--r--   0 alex       (501) staff       (20)     8436 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/fork.py
+-rw-r--r--   0 alex       (501) staff       (20)     2537 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     2561 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     2853 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     2844 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)    55088 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/master.py
+-rw-r--r--   0 alex       (501) staff       (20)     5093 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/minify.py
+-rw-r--r--   0 alex       (501) staff       (20)     6624 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/os_fork.py
+-rw-r--r--   0 alex       (501) staff       (20)    98171 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/parent.py
+-rw-r--r--   0 alex       (501) staff       (20)     2730 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     5392 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/profiler.py
+-rw-r--r--   0 alex       (501) staff       (20)    12325 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/select.py
+-rw-r--r--   0 alex       (501) staff       (20)    41699 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/service.py
+-rw-r--r--   0 alex       (501) staff       (20)     8450 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/setns.py
+-rw-r--r--   0 alex       (501) staff       (20)    10892 2024-03-28 16:09:56.000000 mitogen-0.3.6/mitogen/ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     5656 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/su.py
+-rw-r--r--   0 alex       (501) staff       (20)    12089 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/sudo.py
+-rw-r--r--   0 alex       (501) staff       (20)     7133 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/unix.py
+-rw-r--r--   0 alex       (501) staff       (20)     7694 2024-04-04 12:53:20.000000 mitogen-0.3.6/mitogen/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793492 mitogen-0.3.6/mitogen.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2471 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       24 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)      206 2024-04-04 12:55:07.793921 mitogen-0.3.6/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     3591 2024-03-28 16:31:39.000000 mitogen-0.3.6/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793123 mitogen-0.3.6/tests/
+-rw-r--r--   0 alex       (501) staff       (20)    20874 2024-03-28 16:31:39.000000 mitogen-0.3.6/tests/testlib.py
```

### Comparing `mitogen-0.3.5/LICENSE` & `mitogen-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/PKG-INFO` & `mitogen-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.5
+Version: 0.3.6
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.5 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.6 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
 hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
 Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
```

### Comparing `mitogen-0.3.5/ansible_mitogen/affinity.py` & `mitogen-0.3.6/ansible_mitogen/affinity.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/connection.py` & `mitogen-0.3.6/ansible_mitogen/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,22 @@
 import time
 
 import ansible.constants as C
 import ansible.errors
 import ansible.plugins.connection
 
 import mitogen.core
-import mitogen.utils
 
 import ansible_mitogen.mixins
 import ansible_mitogen.parsing
 import ansible_mitogen.process
 import ansible_mitogen.services
 import ansible_mitogen.target
 import ansible_mitogen.transport_config
+import ansible_mitogen.utils.unsafe
 
 
 LOG = logging.getLogger(__name__)
 
 task_vars_msg = (
     'could not recover task_vars. This means some connection '
     'settings may erroneously be reset to their defaults. '
@@ -793,15 +793,15 @@
         description of the returned dictionary.
         """
         try:
             dct = mitogen.service.call(
                 call_context=self.binding.get_service_context(),
                 service_name='ansible_mitogen.services.ContextService',
                 method_name='get',
-                stack=mitogen.utils.cast(list(stack)),
+                stack=ansible_mitogen.utils.unsafe.cast(list(stack)),
             )
         except mitogen.core.CallError:
             LOG.warning('Connection failed; stack configuration was:\n%s',
                         pprint.pformat(stack))
             raise
 
         if dct['msg']:
@@ -844,15 +844,15 @@
         # However nothing I've found uses it, it's not even assigned.
         if self.connected:
             return
 
         inventory_name, stack = self._build_stack()
         worker_model = ansible_mitogen.process.get_worker_model()
         self.binding = worker_model.get_binding(
-            mitogen.utils.cast(inventory_name)
+            ansible_mitogen.utils.unsafe.cast(inventory_name)
         )
         self._connect_stack(stack)
 
     def _put_connection(self):
         """
         Forget everything we know about the connected context. This function
         cannot be called _reset() since that name is used as a public API by
@@ -929,15 +929,15 @@
         worker_model = ansible_mitogen.process.get_worker_model()
         binding = worker_model.get_binding(inventory_name)
         try:
             mitogen.service.call(
                 call_context=binding.get_service_context(),
                 service_name='ansible_mitogen.services.ContextService',
                 method_name='reset',
-                stack=mitogen.utils.cast(list(stack)),
+                stack=ansible_mitogen.utils.unsafe.cast(list(stack)),
             )
         finally:
             binding.close()
 
     # Compatibility with Ansible 2.4 wait_for_connection plug-in.
     _reset = reset
 
@@ -1007,16 +1007,16 @@
             (return code, stdout bytes, stderr bytes)
 
         Ansible connection plugin method.
         """
         emulate_tty = (not in_data and sudoable)
         rc, stdout, stderr = self.get_chain().call(
             ansible_mitogen.target.exec_command,
-            cmd=mitogen.utils.cast(cmd),
-            in_data=mitogen.utils.cast(in_data),
+            cmd=ansible_mitogen.utils.unsafe.cast(cmd),
+            in_data=ansible_mitogen.utils.unsafe.cast(in_data),
             chdir=mitogen_chdir or self.get_default_cwd(),
             emulate_tty=emulate_tty,
         )
 
         stderr += b'Shared connection to %s closed.%s' % (
             self._play_context.remote_addr.encode(),
             (b'\r\n' if emulate_tty else b'\n'),
@@ -1035,15 +1035,15 @@
 
         Ansible connection plugin method.
         """
         self._connect()
         ansible_mitogen.target.transfer_file(
             context=self.context,
             # in_path may be AnsibleUnicode
-            in_path=mitogen.utils.cast(in_path),
+            in_path=ansible_mitogen.utils.unsafe.cast(in_path),
             out_path=out_path
         )
 
     def put_data(self, out_path, data, mode=None, utimes=None):
         """
         Implement put_file() by caling the corresponding ansible_mitogen.target
         function in the target, transferring small files inline. This is
@@ -1053,15 +1053,15 @@
         :param str out_path:
             Remote filesystem path to write.
         :param byte data:
             File contents to put.
         """
         self.get_chain().call_no_reply(
             ansible_mitogen.target.write_path,
-            mitogen.utils.cast(out_path),
+            ansible_mitogen.utils.unsafe.cast(out_path),
             mitogen.core.Blob(data),
             mode=mode,
             utimes=utimes,
         )
 
     #: Maximum size of a small file before switching to streaming
     #: transfer. This should really be the same as
@@ -1115,15 +1115,15 @@
                                      utimes=(st.st_atime, st.st_mtime))
 
         self._connect()
         mitogen.service.call(
             call_context=self.binding.get_service_context(),
             service_name='mitogen.service.FileService',
             method_name='register',
-            path=mitogen.utils.cast(in_path)
+            path=ansible_mitogen.utils.unsafe.cast(in_path)
         )
 
         # For now this must remain synchronous, as the action plug-in may have
         # passed us a temporary file to transfer. A future FileService could
         # maintain an LRU list of open file descriptors to keep the temporary
         # file alive, but that requires more work.
         self.get_chain().call(
```

### Comparing `mitogen-0.3.5/ansible_mitogen/loaders.py` & `mitogen-0.3.6/ansible_mitogen/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'module_utils_loader',
     'shell_loader',
     'strategy_loader',
 ]
 
 
 ANSIBLE_VERSION_MIN = (2, 10)
-ANSIBLE_VERSION_MAX = (2, 13)
+ANSIBLE_VERSION_MAX = (2, 14)
 
 NEW_VERSION_MSG = (
     "Your Ansible version (%s) is too recent. The most recent version\n"
     "supported by Mitogen for Ansible is %s.x. Please check the Mitogen\n"
     "release notes to see if a new version is available, otherwise\n"
     "subscribe to the corresponding GitHub issue to be notified when\n"
     "support becomes available.\n"
```

### Comparing `mitogen-0.3.5/ansible_mitogen/logging.py` & `mitogen-0.3.6/ansible_mitogen/logging.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/mixins.py` & `mitogen-0.3.6/ansible_mitogen/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 import ansible
 import ansible.constants
 import ansible.plugins
 import ansible.plugins.action
 
 import mitogen.core
 import mitogen.select
-import mitogen.utils
 
 import ansible_mitogen.connection
 import ansible_mitogen.planner
 import ansible_mitogen.target
 import ansible_mitogen.utils
+import ansible_mitogen.utils.unsafe
 
 from ansible.module_utils._text import to_text
 
 try:
     from ansible.utils.unsafe_proxy import wrap_var
 except ImportError:
     from ansible.vars.unsafe_proxy import wrap_var
@@ -183,15 +183,15 @@
         """
         Determine if `path` exists by directly invoking os.path.exists() in the
         target user account.
         """
         LOG.debug('_remote_file_exists(%r)', path)
         return self._connection.get_chain().call(
             ansible_mitogen.target.file_exists,
-            mitogen.utils.cast(path)
+            ansible_mitogen.utils.unsafe.cast(path)
         )
 
     def _configure_module(self, module_name, module_args, task_vars=None):
         """
         Mitogen does not use the Ansiballz framework. This call should never
         happen when ActionMixin is active, so crash if it does.
         """
@@ -320,15 +320,15 @@
                 return self._connection.homedir
             if path.startswith('~/'):
                 # ~/.ansible -> /home/dmw/.ansible
                 return os.path.join(self._connection.homedir, path[2:])
         # ~root/.ansible -> /root/.ansible
         return self._connection.get_chain(use_login=(not sudoable)).call(
             os.path.expanduser,
-            mitogen.utils.cast(path),
+            ansible_mitogen.utils.unsafe.cast(path),
         )
 
     def get_task_timeout_secs(self):
         """
         Return the task "async:" value, portable across 2.4-2.5.
         """
         try:
@@ -383,19 +383,19 @@
             self._connection.context = None
 
         self._connection._connect()
         result = ansible_mitogen.planner.invoke(
             ansible_mitogen.planner.Invocation(
                 action=self,
                 connection=self._connection,
-                module_name=mitogen.core.to_text(module_name),
-                module_args=mitogen.utils.cast(module_args),
+                module_name=ansible_mitogen.utils.unsafe.cast(mitogen.core.to_text(module_name)),
+                module_args=ansible_mitogen.utils.unsafe.cast(module_args),
                 task_vars=task_vars,
                 templar=self._templar,
-                env=mitogen.utils.cast(env),
+                env=ansible_mitogen.utils.unsafe.cast(env),
                 wrap_async=wrap_async,
                 timeout_secs=self.get_task_timeout_secs(),
             )
         )
 
         if tmp and delete_remote_tmp and ansible_mitogen.utils.ansible_version[:2] < (2, 5):
             # Built-in actions expected tmpdir to be cleaned up automatically
```

### Comparing `mitogen-0.3.5/ansible_mitogen/module_finder.py` & `mitogen-0.3.6/ansible_mitogen/module_finder.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/parsing.py` & `mitogen-0.3.6/ansible_mitogen/parsing.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/planner.py` & `mitogen-0.3.6/ansible_mitogen/planner.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/action/mitogen_fetch.py` & `mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_fetch.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/action/mitogen_get_stack.py` & `mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_get_stack.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_buildah.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_doas.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_docker.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_docker.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_jail.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_kubectl.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_local.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_local.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_lxc.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxc.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_lxd.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_machinectl.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_machinectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_podman.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_setns.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_ssh.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_ssh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_su.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_su.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/connection/mitogen_sudo.py` & `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_sudo.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen.py` & `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_free.py` & `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py` & `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/plugins/strategy/mitogen_linear.py` & `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/process.py` & `mitogen-0.3.6/ansible_mitogen/process.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/runner.py` & `mitogen-0.3.6/ansible_mitogen/runner.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/services.py` & `mitogen-0.3.6/ansible_mitogen/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 import sys
 import threading
 
 import ansible.constants
 
 import mitogen.core
 import mitogen.service
-import mitogen.utils
 import ansible_mitogen.loaders
 import ansible_mitogen.module_finder
 import ansible_mitogen.target
+import ansible_mitogen.utils.unsafe
 
 
 LOG = logging.getLogger(__name__)
 
 # Force load of plugin to ensure ConfigManager has definitions loaded. Done
 # during module import to ensure a single-threaded environment; PluginLoader
 # is not thread-safe.
@@ -87,15 +87,15 @@
         remote_tmp = options.get('remote_tmp') or ansible.constants.DEFAULT_REMOTE_TMP
         system_tmpdirs = options.get('system_tmpdirs', ('/var/tmp', '/tmp'))
     except AttributeError:
         # 2.3
         remote_tmp = ansible.constants.DEFAULT_REMOTE_TMP
         system_tmpdirs = ('/var/tmp', '/tmp')
 
-    return mitogen.utils.cast([remote_tmp] + list(system_tmpdirs))
+    return ansible_mitogen.utils.unsafe.cast([remote_tmp] + list(system_tmpdirs))
 
 
 def key_from_dict(**kwargs):
     """
     Return a unique string representation of a dict as quickly as possible.
     Used to generated deduplication keys from a request.
     """
```

### Comparing `mitogen-0.3.5/ansible_mitogen/strategy.py` & `mitogen-0.3.6/ansible_mitogen/strategy.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/target.py` & `mitogen-0.3.6/ansible_mitogen/target.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/transport_config.py` & `mitogen-0.3.6/ansible_mitogen/transport_config.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/ansible_mitogen/utils.py` & `mitogen-0.3.6/ansible_mitogen/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/__init__.py` & `mitogen-0.3.6/mitogen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 On the Mitogen master, this is imported from ``mitogen/__init__.py`` as would
 be expected. On the slave, it is built dynamically during startup.
 """
 
 
 #: Library version as a tuple.
-__version__ = (0, 3, 5)
+__version__ = (0, 3, 6)
 
 
 #: This is :data:`False` in slave contexts. Previously it was used to prevent
 #: re-execution of :mod:`__main__` in single file programs, however that now
 #: happens automatically.
 is_master = True
```

### Comparing `mitogen-0.3.5/mitogen/buildah.py` & `mitogen-0.3.6/mitogen/buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/compat/pkgutil.py` & `mitogen-0.3.6/mitogen/compat/pkgutil.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/compat/tokenize.py` & `mitogen-0.3.6/mitogen/compat/tokenize.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/core.py` & `mitogen-0.3.6/mitogen/core.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/debug.py` & `mitogen-0.3.6/mitogen/debug.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/doas.py` & `mitogen-0.3.6/mitogen/doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/docker.py` & `mitogen-0.3.6/mitogen/docker.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/fakessh.py` & `mitogen-0.3.6/mitogen/fakessh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/fork.py` & `mitogen-0.3.6/mitogen/fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/jail.py` & `mitogen-0.3.6/mitogen/jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/kubectl.py` & `mitogen-0.3.6/mitogen/kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/lxc.py` & `mitogen-0.3.6/mitogen/lxc.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/lxd.py` & `mitogen-0.3.6/mitogen/lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/master.py` & `mitogen-0.3.6/mitogen/master.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/minify.py` & `mitogen-0.3.6/mitogen/minify.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/os_fork.py` & `mitogen-0.3.6/mitogen/os_fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/parent.py` & `mitogen-0.3.6/mitogen/parent.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/podman.py` & `mitogen-0.3.6/mitogen/podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/profiler.py` & `mitogen-0.3.6/mitogen/profiler.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/select.py` & `mitogen-0.3.6/mitogen/select.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/service.py` & `mitogen-0.3.6/mitogen/service.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/setns.py` & `mitogen-0.3.6/mitogen/setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/ssh.py` & `mitogen-0.3.6/mitogen/ssh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/su.py` & `mitogen-0.3.6/mitogen/su.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/sudo.py` & `mitogen-0.3.6/mitogen/sudo.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/unix.py` & `mitogen-0.3.6/mitogen/unix.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/mitogen/utils.py` & `mitogen-0.3.6/mitogen/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -186,37 +186,51 @@
     mitogen.core.Blob,
     mitogen.core.Secret,
 )
 
 
 def cast(obj):
     """
+    Return obj (or a copy) with subtypes of builtins cast to their supertype.
+    Subtypes of those in :data:`PASSTHROUGH` are not modified.
+
     Many tools love to subclass built-in types in order to implement useful
     functionality, such as annotating the safety of a Unicode string, or adding
-    additional methods to a dict. However, cPickle loves to preserve those
-    subtypes during serialization, resulting in CallError during :meth:`call
+    additional methods to a dict. However :py:mod:`pickle` serializes these
+    exactly, leading to :exc:`mitogen.CallError` during :meth:`Context.call
     <mitogen.parent.Context.call>` in the target when it tries to deserialize
     the data.
 
     This function walks the object graph `obj`, producing a copy with any
     custom sub-types removed. The functionality is not default since the
     resulting walk may be computationally expensive given a large enough graph.
 
+    Raises :py:exc:`TypeError` if an unknown subtype is encountered, or
+    casting does not return the desired supertype.
+
     See :ref:`serialization-rules` for a list of supported types.
 
     :param obj:
         Object to undecorate.
     :returns:
         Undecorated object.
     """
     if isinstance(obj, dict):
         return dict((cast(k), cast(v)) for k, v in iteritems(obj))
     if isinstance(obj, (list, tuple)):
         return [cast(v) for v in obj]
     if isinstance(obj, PASSTHROUGH):
         return obj
     if isinstance(obj, mitogen.core.UnicodeType):
-        return mitogen.core.UnicodeType(obj)
+        return _cast(obj, mitogen.core.UnicodeType)
     if isinstance(obj, mitogen.core.BytesType):
-        return mitogen.core.BytesType(obj)
+        return _cast(obj, mitogen.core.BytesType)
 
     raise TypeError("Cannot serialize: %r: %r" % (type(obj), obj))
+
+
+def _cast(obj, desired_type):
+    result = desired_type(obj)
+    if type(result) is not desired_type:
+        raise TypeError("Cast of %r to %r failed, got %r"
+                        % (type(obj), desired_type, type(result)))
+    return result
```

### Comparing `mitogen-0.3.5/mitogen.egg-info/PKG-INFO` & `mitogen-0.3.6/mitogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.5
+Version: 0.3.6
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.5 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.6 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
 hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
 Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
```

### Comparing `mitogen-0.3.5/mitogen.egg-info/SOURCES.txt` & `mitogen-0.3.6/mitogen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 ansible_mitogen/planner.py
 ansible_mitogen/process.py
 ansible_mitogen/runner.py
 ansible_mitogen/services.py
 ansible_mitogen/strategy.py
 ansible_mitogen/target.py
 ansible_mitogen/transport_config.py
-ansible_mitogen/utils.py
 ansible_mitogen/compat/__init__.py
 ansible_mitogen/plugins/__init__.py
 ansible_mitogen/plugins/action/__init__.py
 ansible_mitogen/plugins/action/mitogen_fetch.py
 ansible_mitogen/plugins/action/mitogen_get_stack.py
 ansible_mitogen/plugins/connection/__init__.py
 ansible_mitogen/plugins/connection/mitogen_buildah.py
@@ -40,14 +39,16 @@
 ansible_mitogen/plugins/connection/mitogen_su.py
 ansible_mitogen/plugins/connection/mitogen_sudo.py
 ansible_mitogen/plugins/strategy/__init__.py
 ansible_mitogen/plugins/strategy/mitogen.py
 ansible_mitogen/plugins/strategy/mitogen_free.py
 ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
 ansible_mitogen/plugins/strategy/mitogen_linear.py
+ansible_mitogen/utils/__init__.py
+ansible_mitogen/utils/unsafe.py
 mitogen/__init__.py
 mitogen/buildah.py
 mitogen/core.py
 mitogen/debug.py
 mitogen/doas.py
 mitogen/docker.py
 mitogen/fakessh.py
```

### Comparing `mitogen-0.3.5/setup.py` & `mitogen-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.5/tests/testlib.py` & `mitogen-0.3.6/tests/testlib.py`

 * *Files identical despite different names*

