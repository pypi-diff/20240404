# Comparing `tmp/pybritive-1.7.0rc2.tar.gz` & `tmp/pybritive-1.7.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybritive-1.7.0rc2.tar", last modified: Fri Jan 19 14:31:04 2024, max compression
+gzip compressed data, was "pybritive-1.7.0rc3.tar", last modified: Thu Apr  4 20:09:15 2024, max compression
```

## Comparing `pybritive-1.7.0rc2.tar` & `pybritive-1.7.0rc3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.405677 pybritive-1.7.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-19 14:31:04.405677 pybritive-1.7.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-19 14:31:04.405677 pybritive-1.7.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.385677 pybritive-1.7.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.389677 pybritive-1.7.0rc2/src/pybritive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62660 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/britive_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.389677 pybritive-1.7.0rc2/src/pybritive/choices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/choices/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.393677 pybritive-1.7.0rc2/src/pybritive/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.393677 pybritive-1.7.0rc2/src/pybritive/completers/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/api_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/bash_gte_42.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/powershell_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/completers/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.397677 pybritive-1.7.0rc2/src/pybritive/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/api_method_argument_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/aws_credential_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/build_britive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12004 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/cloud_credential_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/k8s_exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/k8s_exec_credential_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/kube_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/profile_argument_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/helpers/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.401677 pybritive-1.7.0rc2/src/pybritive/options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/aws_console_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/aws_credentials_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/blocktime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/britive_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/checked_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/configure_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/configure_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/configure_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/configure_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/federation_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/force_renew.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/gcloud_key_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/justification.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/maxpolltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/silent.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/ssh_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/ssh_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/ssh_username.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/src/pybritive/options/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.405677 pybritive-1.7.0rc2/src/pybritive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-19 14:31:04.000000 pybritive-1.7.0rc2/src/pybritive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:31:04.405677 pybritive-1.7.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0100_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0200_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0300_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0400_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0450_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0500_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0600_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0700_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0800_checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0850_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_0900_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-19 14:30:53.000000 pybritive-1.7.0rc2/tests/test_1000_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.107946 pybritive-1.7.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.107946 pybritive-1.7.0rc3/src/pybritive/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63081 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/britive_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.111946 pybritive-1.7.0rc3/src/pybritive/choices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/choices/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.111946 pybritive-1.7.0rc3/src/pybritive/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.115946 pybritive-1.7.0rc3/src/pybritive/completers/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/api_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/bash_gte_42.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/powershell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/completers/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.115946 pybritive-1.7.0rc3/src/pybritive/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/api_method_argument_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/aws_credential_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/build_britive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16731 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/cloud_credential_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16747 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/k8s_exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/k8s_exec_credential_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/kube_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/profile_argument_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/helpers/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/src/pybritive/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/aws_console_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/aws_credentials_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/blocktime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/britive_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/checked_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/configure_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/configure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/configure_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/configure_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/federation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/force_renew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/gcloud_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/justification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/maxpolltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/silent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/ssh_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/ssh_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/ssh_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/src/pybritive/options/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/src/pybritive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 20:09:15.000000 pybritive-1.7.0rc3/src/pybritive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:09:15.123946 pybritive-1.7.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0100_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0200_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0300_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0400_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0450_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0500_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0600_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0700_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0800_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0850_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_0900_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 20:09:03.000000 pybritive-1.7.0rc3/tests/test_1000_logout.py
```

### Comparing `pybritive-1.7.0rc2/LICENSE` & `pybritive-1.7.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/PKG-INFO` & `pybritive-1.7.0rc3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.7.0rc2
+Version: 1.7.0rc3
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,21 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: PyYAML
 Requires-Dist: merge_args
 Requires-Dist: tabulate
 Requires-Dist: toml
 Requires-Dist: cryptography>=41.0.0
 Requires-Dist: python-dateutil
-Requires-Dist: britive>=2.24.0rc1
+Requires-Dist: britive>=2.24.0rc5
 Requires-Dist: jmespath
 Requires-Dist: pyjwt
+Provides-Extra: openshift
+Requires-Dist: beautifulsoup4; extra == "openshift"
+Provides-Extra: aws
+Requires-Dist: boto3; extra == "aws"
 
 # Britive CLI - Pure Python Implementation
 
 PyBritive is intended to be used as a CLI application for communicating with the Britive Platform.
 
 ## Installation
```

### Comparing `pybritive-1.7.0rc2/README.md` & `pybritive-1.7.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/setup.cfg` & `pybritive-1.7.0rc3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybritive
-version = 1.7.0rc2
+version = 1.7.0rc3
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python CLI for Britive
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers = 
@@ -22,24 +22,30 @@
 	requests>=2.31.0
 	PyYAML
 	merge_args
 	tabulate
 	toml
 	cryptography>=41.0.0
 	python-dateutil
-	britive>=2.24.0rc1
+	britive>=2.24.0rc5
 	jmespath
 	pyjwt
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	pybritive = pybritive.cli_interface:safe_cli
 	pybritive-aws-cred-process = pybritive.helpers.aws_credential_process:main
 	pybritive-kube-exec = pybritive.helpers.k8s_exec:main
 
+[options.extras_require]
+openshift = 
+	beautifulsoup4
+aws = 
+	boto3
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pybritive-1.7.0rc2/src/pybritive/britive_cli.py` & `pybritive-1.7.0rc3/src/pybritive/britive_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import io
 import json
 import os
 import pathlib
 from pathlib import Path
 import sys
 import uuid
-import pkg_resources
 import yaml
 import click
 import jmespath
 from britive.britive import Britive
 from britive import exceptions
 from tabulate import tabulate
 from .helpers.config import ConfigManager
@@ -165,16 +164,15 @@
         self._update_sdk_user_agent()
 
         # if user called `pybritive login` and we should get profiles...do so
         should_get_profiles = any([self.config.auto_refresh_profile_cache(), self.config.auto_refresh_kube_config()])
         if explicit and should_get_profiles:
             self._set_available_profiles()  # will handle calling cache_profiles() and construct_kube_config()
 
-        # handle printing the banner - commenting out until the banner api is released into production
-        # self._display_banner()
+        self._display_banner()
 
     def _display_banner(self):
         if self.silent:
             return
 
         if not Cache().banner_expired(tenant=self.tenant_name):  # if banner is not expired yet then nothing to do
             return
@@ -186,15 +184,16 @@
             self.print(f'*** {banner.get("messageType", "UNKNOWN")}: {banner.get("message", "<no message>")} ***')
 
     def _update_sdk_user_agent(self):
         # update the user agent to include the pybritive cli version
         user_agent = self.b.session.headers.get('User-Agent')
 
         try:
-            version = pkg_resources.get_distribution('pybritive').version
+            import pybritive
+            version = pybritive.__version__
         except Exception:
             version = 'unknown'
 
         self.b.session.headers.update({
             'User-Agent': f'pybritive/{version} {user_agent}'
         })
 
@@ -396,14 +395,17 @@
                     row.pop('Description', None)
                     row.pop('Type', None)
                     row.pop('TimeRemaining', None)
                     row.pop('TimeRemainingSeconds', None)
                     row.pop('Expiration', None)
                     if profile['2_part_profile_format_allowed']:
                         row.pop('Environment', None)
+                elif self.output_format == 'json':
+                    row['Name'] = f"{row['Application']}/{row['Environment']}/{row['Profile']}"
+
                 data.append(row)
 
         # set special list output if needed
         if self.output_format == 'list':
             self.output_format = 'list-profiles'
 
         self.print(data, ignore_silent=True)
@@ -560,14 +562,23 @@
                 mode=mode,
                 profile=profile,
                 credentials=credentials,
                 silent=silent,
                 cli=self,
                 k8s_processor=k8s_processor
             )
+        elif app_type in ['OpenShift']:
+            return printer.OpenShiftCredentialPrinter(
+                console=console,
+                mode=mode,
+                profile=profile,
+                credentials=credentials,
+                silent=silent,
+                cli=self
+            )
         else:
             return printer.GenericCloudCredentialPrinter(
                 console=console,
                 mode=mode,
                 profile=profile,
                 credentials=credentials,
                 silent=silent,
@@ -692,17 +703,17 @@
         # handle kube-exec since the profile is actually going to be passed in via another method
         # and perform some basic validation so we don't waste time performing a checkout when we
         # will not be able to return a response back to kubectl via the exec command
         if mode == 'kube-exec':
             from .helpers.k8s_exec_credential_builder import KubernetesExecCredentialProcessor
             k8s_processor = KubernetesExecCredentialProcessor()
 
-        # these 2 modes implicitly say that console access should be checked out without having to provide
+        # these 3 modes implicitly say that console access should be checked out without having to provide
         # the --console flag
-        if mode and (mode == 'console' or mode.startswith('browser')):
+        if mode and (mode == 'console' or mode.startswith('browser') or mode.startswith('os-')):
             console = True
             if mode.startswith('browser'):
                 self.browser = mode.replace('browser-', '')
             else:
                 self.browser = os.getenv('PYBRITIVE_BROWSER')
 
         self._validate_justification(justification)
@@ -747,15 +758,15 @@
         # lets check to see if we should checkin this profile first and check it out again
         if self._should_check_force_renew(app_type, force_renew, console):
             expiration = datetime.fromisoformat(credentials['expirationTime'].replace('Z', ''))
             now = datetime.utcnow()
             diff = (expiration - now).total_seconds() / 60.0
             if diff < force_renew:  # time to checkin the profile so we can refresh creds
                 self.print('checking in the profile to get renewed credentials....standby')
-                self.checkin(profile=profile)
+                self.checkin(profile=profile, console=console)
                 response = self._checkout(**params)
                 cached_credentials_found = False  # need to write new creds to cache
                 credentials = response['credentials']
 
         if alias:  # do this down here, so we know that the profile is valid and a checkout was successful
             self.config.save_profile_alias(alias=alias, profile=profile)
 
@@ -1221,20 +1232,23 @@
 
         return {
             'private_key_filename': pem_file,
             'key_pair': key_pair
         }
 
     @staticmethod
+    def build_import_exception_message(extras: str):
+        return f'required packages not found. run `pip3 install pybritive[{extras}]`'
+
+    @staticmethod
     def _ssh_aws_push_key(aws_profile, aws_region, instance_id, username, key_pair):
         try:
             import boto3
         except ImportError as e:
-            message = 'boto3 package is required. Please ensure the package is installed.'
-            raise click.ClickException(message) from e
+            raise click.ClickException(BritiveCli.build_import_exception_message('aws')) from e
 
         # we know we will be pushing the key to the instance so establish the
         # boto3 clients which are required to perform those actions
         session = boto3.Session(profile_name=aws_profile, region_name=aws_region)
         eic = session.client('ec2-instance-connect')
         ec2 = session.client('ec2')
 
@@ -1284,16 +1298,15 @@
         import requests
         import webbrowser
 
         # this is the one that may not be available so be careful
         try:
             import boto3
         except ImportError as e:
-            message = 'boto3 package is required. Please ensure the package is installed.'
-            raise click.ClickException(message) from e
+            raise click.ClickException(BritiveCli.build_import_exception_message('aws')) from e
 
         creds = boto3.Session(profile_name=profile).get_credentials()
         session_id = creds.access_key
         session_key = creds.secret_key
         session_token = creds.token
         json_creds = json.dumps({
             'sessionId': session_id,
```

### Comparing `pybritive-1.7.0rc2/src/pybritive/choices/mode.py` & `pybritive-1.7.0rc3/src/pybritive/choices/mode.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,10 +22,12 @@
         'browser-windows-default',
         'browser-macosx',
         'browser-safari',
         'browser-chrome',
         'browser-chromium',
         'kube-exec',                # bake into kubeconfig with oidc exec output and additional caching to make kubectl more performant
         'gcloudauthexec',           # will effectively execute results of gcloudauth in a sub-shell
+        'os-oclogin',               # will attempt an oidc authorization code grant flow for generating the `oc login ...` command for OpenShift
+        'os-ocloginexec',           # will attempt an oidc authorization code grant flow for generating the `oc login ...` command for OpenShift and exec the result in a subshell
     ],
     case_sensitive=False
 )
```

### Comparing `pybritive-1.7.0rc2/src/pybritive/choices/output_format.py` & `pybritive-1.7.0rc3/src/pybritive/choices/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/cli_interface.py` & `pybritive-1.7.0rc3/src/pybritive/cli_interface.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/api.py` & `pybritive-1.7.0rc3/src/pybritive/commands/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/aws.py` & `pybritive-1.7.0rc3/src/pybritive/commands/aws.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/cache.py` & `pybritive-1.7.0rc3/src/pybritive/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/checkin.py` & `pybritive-1.7.0rc3/src/pybritive/commands/checkin.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/checkout.py` & `pybritive-1.7.0rc3/src/pybritive/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/clear.py` & `pybritive-1.7.0rc3/src/pybritive/commands/clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/configure.py` & `pybritive-1.7.0rc3/src/pybritive/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/login.py` & `pybritive-1.7.0rc3/src/pybritive/commands/login.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/ls.py` & `pybritive-1.7.0rc3/src/pybritive/commands/ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/request.py` & `pybritive-1.7.0rc3/src/pybritive/commands/request.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/secret.py` & `pybritive-1.7.0rc3/src/pybritive/commands/secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/commands/ssh.py` & `pybritive-1.7.0rc3/src/pybritive/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/completers/api.py` & `pybritive-1.7.0rc3/src/pybritive/completers/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/completers/api_command.py` & `pybritive-1.7.0rc3/src/pybritive/completers/api_command.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/completers/bash_gte_42.py` & `pybritive-1.7.0rc3/src/pybritive/completers/bash_gte_42.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/completers/powershell_completion.py` & `pybritive-1.7.0rc3/src/pybritive/completers/powershell_completion.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/completers/profile.py` & `pybritive-1.7.0rc3/src/pybritive/completers/profile.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/aws_credential_process.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/aws_credential_process.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/build_britive.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/build_britive.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/cache.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/cloud_credential_printer.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/cloud_credential_printer.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import subprocess
 from pathlib import Path
 import platform
 import uuid
 import webbrowser
 import click
-import hashlib
 
 
 # trailing spaces matter as some options do not have the trailing space
 env_options = {
     'nix': 'export ',
     'winps': '$Env:',
     'wincmd': 'set '
@@ -29,27 +28,29 @@
     def __init__(self, app_type, console, mode, profile, silent, credentials, cli):
         self.cli = cli
         self.silent = silent
         self.app_type = app_type
         self.profile = profile
         self.console = console
         mode = mode or 'json'  # set a default if nothing is provided via flag --mode/-m
+        self.full_mode = mode
         helper = mode.split('-')
         self.mode = helper[0]
         self.mode_modifier = safe_list_get(mode.split('-', maxsplit=1), 1, None)
         self.credentials = credentials
         if self.mode == 'env':
             if self.mode_modifier:
                 self.env_command = env_options[self.mode_modifier]
             else:
                 self.on_windows = platform.system().lower() == 'windows'
                 self.env_command = env_options['wincmd'] if self.on_windows else env_options['nix']
+        self.modes_to_skip_console_printing = ['os-oclogin', 'os-ocloginexec']
 
     def print(self):
-        if self.console:
+        if self.console and self.full_mode not in self.modes_to_skip_console_printing:
             self.print_console()
             return
         if self.mode == 'text':
             self.print_text()
         if self.mode == 'json':
             self.print_json()
         if self.mode == 'env':
@@ -62,16 +63,18 @@
             self.print_awscredentialprocess()
         if self.mode == 'azps':
             self.print_azps()
         if self.mode == 'gcloudauth':
             self.print_gcloudauth()
         if self.mode == 'kube':
             self.print_kube()
+        if self.mode == 'os':
+            self.print_os()
         if self.mode == 'gcloudauthexec':
-            self.exec_gcloudauthexec()
+            self.print_gcloudauthexec()
 
     def print_console(self):
         url = self.credentials.get('url', self.credentials)
         if self.mode == 'browser':
             browser = self.mode_modifier or os.getenv('PYBRITIVE_BROWSER')
             webbrowser.get(using=browser).open(url)
         else:
@@ -97,18 +100,21 @@
 
     def print_azps(self):
         self._not_implemented()
 
     def print_gcloudauth(self):
         self._not_implemented()
 
-    def exec_gcloudautoauth(self):
+    def print_kube(self):
         self._not_implemented()
 
-    def print_kube(self):
+    def print_gcloudauthexec(self):
+        self._not_implemented()
+
+    def print_os(self):
         self._not_implemented()
 
     def _not_implemented(self):
         raise click.ClickException(f'Application type {self.app_type} does not support the specified mode.')
 
 
 class GenericCloudCredentialPrinter(CloudCredentialPrinter):
@@ -262,15 +268,15 @@
         path.write_text(json.dumps(self.credentials, indent=2), encoding='utf-8')
 
         self.cli.print(
             f"gcloud auth activate-service-account {self.credentials['client_email']} --key-file {str(path)}",
             ignore_silent=True
         )
 
-    def exec_gcloudauthexec(self):
+    def print_gcloudauthexec(self):
         key_file = self.cli.build_gcloud_key_file_for_gcloudauthexec(profile=self.profile)
         path = Path(self.cli.config.gcloud_key_file_path) / key_file
 
         # key file does not yet exist so write to it
         path.parent.mkdir(exist_ok=True, parents=True)
         path.write_text(json.dumps(self.credentials, indent=2), encoding='utf-8')
 
@@ -302,7 +308,108 @@
             self.cli.print(self.credentials, ignore_silent=True)
 
     def print_kube(self):
         if self.mode_modifier == 'exec':
             self.cli.print(self.k8s_processor.construct_exec_credential(self.credentials), ignore_silent=True)
         else:
             raise ValueError(f'--mode modifier {self.mode_modifier} for mode {self.mode} not supported')
+
+
+class OpenShiftCredentialPrinter(CloudCredentialPrinter):
+    def __init__(self, console, mode, profile, silent, credentials, cli):
+        super().__init__('OpenShift', console, mode, profile, silent, credentials, cli)
+
+    def print_json(self):
+        try:
+            self.cli.print(json.dumps(self.credentials, indent=2), ignore_silent=True)
+        except json.JSONDecodeError:
+            self.cli.print(self.credentials, ignore_silent=True)
+
+    def _perform_oidc_auth_code_grant_flow(self):
+        try:
+            import requests
+            from requests.adapters import HTTPAdapter
+            from urllib.parse import urlparse
+
+            try:
+                from bs4 import BeautifulSoup
+            except ImportError as e:
+                raise click.ClickException(self.cli.build_import_exception_message('openshift')) from e
+
+            class BritiveCustomHeaderAdapter(HTTPAdapter):
+                def __init__(self, headers=None, *args, **kwargs):
+                    self.headers = headers or {}
+                    super().__init__(*args, **kwargs)
+
+                def add_headers(self, request, **kwargs):
+                    for h, v in self.headers.items():
+                        request.headers.setdefault(h, v)
+
+            sdk_headers = self.cli.b.session.headers
+            tenant_fqdn = self.cli.b.tenant
+            temp_url = self.credentials['url']
+            temp_url = temp_url.replace('console-openshift-console', 'oauth-openshift')
+            parsed_url = urlparse(temp_url)
+            base_url = parsed_url.scheme + "://" + parsed_url.netloc
+            idp = self.credentials['idpName']
+
+            session = requests.session()
+
+            # set a reasonable user agent, so we can identify traffic more easily
+            session.headers.update({
+                'User-Agent': sdk_headers['User-Agent']
+            })
+
+            # create a custom adapter for the tenants fqdn and mount it
+            # this will include the authorization header, so we can "auto"
+            # authenticate to the tenant
+            adapter = BritiveCustomHeaderAdapter(headers={'Authorization': sdk_headers['Authorization']})
+            session.mount(f'https://{tenant_fqdn}/', adapter)
+
+            token_request_url = f'{base_url}/oauth/token/request'
+            idp_selection_url = session.get(token_request_url, allow_redirects=False).headers['Location']
+            idp_selected_url = f'{idp_selection_url}&idp={idp}'
+            response = session.get(idp_selected_url, allow_redirects=True)
+            # we now have a html file that we need to extract some things from
+            soup = BeautifulSoup(response.content, 'html.parser')
+            input_values = {}
+            form = soup.find('form')
+            inputs = form.find_all('input')
+            for inp in inputs:
+                name = inp.get('name')
+                value = inp.get('value')
+                if name:
+                    input_values[name] = value
+
+            form_action = form['action']
+            if form_action.startswith('/'):
+                form_action = form_action[1:]
+            response = session.post(f'{base_url}/{form_action}', data=input_values)
+
+            # and we get more html content we need to parse now
+            soup = BeautifulSoup(response.content, 'html.parser')
+
+            command = None
+            for line in soup.get_text().split('\n'):
+                if line.startswith('oc login'):
+                    command = line
+                    break
+
+            if command:
+                return command
+            else:
+                raise Exception(f'error: no `oc login` command found')
+        except Exception as e:
+            self.cli.print(f'error when attempting to perform oidc auth code grant flow: {str(e)}', ignore_silent=True)
+
+    def print_os(self):
+        if self.mode_modifier == 'oclogin':
+            command = self._perform_oidc_auth_code_grant_flow()
+            self.cli.print(command, ignore_silent=True)
+        elif self.mode_modifier == 'ocloginexec':
+            command = self._perform_oidc_auth_code_grant_flow()
+            try:
+                subprocess.run(command.split(' '), check=True)
+            except Exception as e:
+                self.cli.print(f'error running `gcloud auth activate-service-account ...`: {str(e)}')
+        else:
+            raise ValueError(f'--mode modifier {self.mode_modifier} for mode {self.mode} not supported')
```

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/config.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/config.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/credentials.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/credentials.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/encryption.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/encryption.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/k8s_exec.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/k8s_exec.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/k8s_exec_credential_builder.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/k8s_exec_credential_builder.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/kube_config_builder.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/kube_config_builder.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/profile_argument_decorator.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/profile_argument_decorator.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/helpers/split.py` & `pybritive-1.7.0rc3/src/pybritive/helpers/split.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/options/britive_options.py` & `pybritive-1.7.0rc3/src/pybritive/options/britive_options.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/options/mode.py` & `pybritive-1.7.0rc3/src/pybritive/options/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/options/output_format.py` & `pybritive-1.7.0rc3/src/pybritive/options/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/options/ssh_push_public_key.py` & `pybritive-1.7.0rc3/src/pybritive/options/ssh_push_public_key.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive/options/version.py` & `pybritive-1.7.0rc3/src/pybritive/options/version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/src/pybritive.egg-info/PKG-INFO` & `pybritive-1.7.0rc3/src/pybritive.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.7.0rc2
+Version: 1.7.0rc3
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,21 @@
 Requires-Dist: requests>=2.31.0
 Requires-Dist: PyYAML
 Requires-Dist: merge_args
 Requires-Dist: tabulate
 Requires-Dist: toml
 Requires-Dist: cryptography>=41.0.0
 Requires-Dist: python-dateutil
-Requires-Dist: britive>=2.24.0rc1
+Requires-Dist: britive>=2.24.0rc5
 Requires-Dist: jmespath
 Requires-Dist: pyjwt
+Provides-Extra: openshift
+Requires-Dist: beautifulsoup4; extra == "openshift"
+Provides-Extra: aws
+Requires-Dist: boto3; extra == "aws"
 
 # Britive CLI - Pure Python Implementation
 
 PyBritive is intended to be used as a CLI application for communicating with the Britive Platform.
 
 ## Installation
```

### Comparing `pybritive-1.7.0rc2/src/pybritive.egg-info/SOURCES.txt` & `pybritive-1.7.0rc3/src/pybritive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0200_configure.py` & `pybritive-1.7.0rc3/tests/test_0200_configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0400_ls.py` & `pybritive-1.7.0rc3/tests/test_0400_ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0500_secret.py` & `pybritive-1.7.0rc3/tests/test_0500_secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0700_checkout.py` & `pybritive-1.7.0rc3/tests/test_0700_checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0850_clear.py` & `pybritive-1.7.0rc3/tests/test_0850_clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.7.0rc2/tests/test_0900_login.py` & `pybritive-1.7.0rc3/tests/test_0900_login.py`

 * *Files identical despite different names*

