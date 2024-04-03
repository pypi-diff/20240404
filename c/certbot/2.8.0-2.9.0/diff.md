# Comparing `tmp/certbot-2.8.0.tar.gz` & `tmp/certbot-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-2.8.0.tar", last modified: Tue Dec  5 19:13:53 2023, max compression
+gzip compressed data, was "certbot-2.9.0.tar", last modified: Thu Feb  8 19:45:18 2024, max compression
```

## Comparing `certbot-2.8.0.tar` & `certbot-2.9.0.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.303259 certbot-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)   119261 2023-12-05 19:13:52.000000 certbot-2.8.0/CHANGELOG.md
--rw-rw-r--   0 willg     (1000) willg     (1000)    11456 2023-12-05 19:13:52.000000 certbot-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      267 2023-12-05 19:13:52.000000 certbot-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     8079 2023-12-05 19:13:53.303259 certbot-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)     4264 2023-12-05 19:13:52.000000 certbot-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.283259 certbot-2.8.0/certbot/
--rw-rw-r--   0 willg     (1000) willg     (1000)      113 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.283259 certbot-2.8.0/certbot/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)      184 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14642 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/account.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    21072 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/auth_handler.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    18597 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cert_manager.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/cli/
--rw-rw-r--   0 willg     (1000) willg     (1000)    25858 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4024 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/cli_constants.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9128 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/cli_utils.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1073 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/group_adder.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    23926 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/helpful.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2055 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/paths_parser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     6210 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/plugins_parsing.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4162 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/subparsers.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5223 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/cli/verb_help.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    36975 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/client.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7616 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/constants.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/display/
--rw-rw-r--   0 willg     (1000) willg     (1000)       33 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/display/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2578 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/display/completer.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      811 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/display/dummy_readline.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    22469 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/display/obj.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3456 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/display/util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4484 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/eff.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7452 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/error_handler.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    10644 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/hooks.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    10226 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/lock.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15384 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/log.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    73405 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/main.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/plugins/
--rw-rw-r--   0 willg     (1000) willg     (1000)       23 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    11272 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/disco.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    11966 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/manual.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1579 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/null.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15772 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/selection.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9340 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/standalone.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15984 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/plugins/webroot.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    26160 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/renewal.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3706 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/snap_config.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    53441 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/storage.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       20 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14284 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/account_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    25036 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/auth_handler_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    31115 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/cert_manager_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    26212 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/cli_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    46400 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/client_test.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/tests/compat/
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/compat/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    27416 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/compat/filesystem_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1747 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/compat/misc_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      604 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/compat/os_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7862 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/configuration_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    18932 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/crypto_util_test.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.287259 certbot-2.8.0/certbot/_internal/tests/display/
--rw-rw-r--   0 willg     (1000) willg     (1000)       28 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3716 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/completer_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5153 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/internal_util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    13201 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/obj_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    20275 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/ops_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2375 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/display/util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     6676 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/eff_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5202 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/error_handler_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1956 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/errors_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4983 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/helpful_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    17948 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/hook_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5060 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/lock_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15949 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/log_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)   120795 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/main_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    17535 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/ocsp_test.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.291259 certbot-2.8.0/certbot/_internal/tests/plugins/
--rw-rw-r--   0 willg     (1000) willg     (1000)       28 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14446 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/common_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    11418 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/disco_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     8522 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/dns_common_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2340 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/enhancements_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7425 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/manual_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      674 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/null_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9958 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/selection_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     6817 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/standalone_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5541 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/storage_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1511 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15386 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/plugins/webroot_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14936 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/renewal_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5509 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/renewupdater_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    17001 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/reverter_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    45136 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/storage_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    24762 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/tests/util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4747 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/_internal/updater.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2024 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/achallenges.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.291259 certbot-2.8.0/certbot/compat/
--rw-rw-r--   0 willg     (1000) willg     (1000)      249 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/compat/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1797 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/compat/_path.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    30470 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/compat/filesystem.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5412 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/compat/misc.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9511 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/compat/os.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    19114 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/configuration.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    24587 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/crypto_util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.291259 certbot-2.8.0/certbot/display/
--rw-rw-r--   0 willg     (1000) willg     (1000)       33 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/display/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    13522 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/display/ops.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7268 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/display/util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2786 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/errors.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15584 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/interfaces.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      535 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/main.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15052 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/ocsp.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.291259 certbot-2.8.0/certbot/plugins/
--rw-rw-r--   0 willg     (1000) willg     (1000)       23 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    17516 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/common.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14028 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/dns_common.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    12954 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/dns_common_lexicon.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2635 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/dns_test_common.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    15716 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/dns_test_common_lexicon.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     6809 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/enhancements.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4294 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/storage.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1811 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/plugins/util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/py.typed
--rw-rw-r--   0 willg     (1000) willg     (1000)    22069 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/reverter.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      424 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/ssl-dhparams.pem
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.291259 certbot-2.8.0/certbot/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       42 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2763 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/acme_util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/certbot/tests/testdata/
--rw-rw-r--   0 willg     (1000) willg     (1000)      642 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/README
--rw-rw-r--   0 willg     (1000) willg     (1000)      952 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert-5sans_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      623 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert-nosans_nistp256.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      786 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert-san_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1200 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_2048.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      709 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      887 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_512_bad.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2400 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_fullchain_2048.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1208 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_intermediate_1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1208 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_intermediate_2.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1220 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cert_leaf.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)       25 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/cli.ini
--rw-rw-r--   0 willg     (1000) willg     (1000)      502 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-6sans_512.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      676 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-6sans_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      420 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-nonames_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      277 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-nosans_512.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      493 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-nosans_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      452 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-nosans_nistp256.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      574 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr-san_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      281 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr_512.der
--rw-rw-r--   0 willg     (1000) willg     (1000)      452 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/csr_512.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      302 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ec_prime256v1_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      359 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ec_secp384r1_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      436 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ec_secp521r1_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      227 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/nistp256_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2273 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ocsp_certificate.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2247 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ocsp_issuer_certificate.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1671 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/ocsp_responder_certificate.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      190 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/os-release
--rw-rw-r--   0 willg     (1000) willg     (1000)     1708 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/rsa2048_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      298 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/rsa256_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      493 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/rsa512_key.pem
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/certbot/tests/testdata/sample-archive/
--rw-rw-r--   0 willg     (1000) willg     (1000)     1736 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive/cert1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1123 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive/chain1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2859 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive/fullchain1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1704 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive/privkey1.pem
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/
--rw-rw-r--   0 willg     (1000) willg     (1000)     1050 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/cert1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1208 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/chain1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2258 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/fullchain1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      241 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/privkey1.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1877 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-renewal-ancient.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      553 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-renewal-deprecated-option.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1970 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-renewal-ec.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1911 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/sample-renewal.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       54 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/testdata/webrootconftest.ini
--rw-rw-r--   0 willg     (1000) willg     (1000)    18166 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/tests/util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    25674 2023-12-05 19:13:52.000000 certbot-2.8.0/certbot/util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.299259 certbot-2.8.0/certbot.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     8079 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)     7652 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      291 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      910 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        8 2023-12-05 19:13:53.000000 certbot-2.8.0/certbot.egg-info/top_level.txt
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/docs/
--rw-rw-r--   0 willg     (1000) willg     (1000)        9 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)     7073 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/Makefile
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/docs/_static/
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/_static/.gitignore
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/docs/_templates/
--rw-rw-r--   0 willg     (1000) willg     (1000)     2004 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/_templates/footer.html
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/docs/api/
--rw-rw-r--   0 willg     (1000) willg     (1000)      148 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.achallenges.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      166 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.compat.filesystem.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      148 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.compat.misc.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      180 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.compat.os.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      247 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.compat.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      150 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.crypto_util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      148 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.display.ops.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      224 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.display.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      151 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.display.util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      133 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.errors.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      145 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.interfaces.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      127 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.main.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      131 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.ocsp.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      157 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.common.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      171 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.dns_common.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      197 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.dns_common_lexicon.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      188 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.dns_test_common.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      214 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.dns_test_common_lexicon.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      175 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.enhancements.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      432 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      160 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.storage.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      151 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.plugins.util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      139 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.reverter.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      424 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      162 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.tests.acme_util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      220 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.tests.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      145 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.tests.util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      127 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api/certbot.util.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      100 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/api.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     4701 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/challenges.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)    15001 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/ciphers.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)    41234 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/cli-help.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)     2001 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/compatibility.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)    10308 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/conf.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    26849 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/contributing.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      347 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/index.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     5935 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/install.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      258 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/intro.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     7259 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/make.bat
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.295259 certbot-2.8.0/docs/man/
--rw-rw-r--   0 willg     (1000) willg     (1000)      751 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/man/certbot.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     2861 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/packaging.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      147 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/resources.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)    57589 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/using.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     1712 2023-12-05 19:13:52.000000 certbot-2.8.0/docs/what.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.299259 certbot-2.8.0/examples/
--rw-rw-r--   0 willg     (1000) willg     (1000)       36 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)     1283 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/cli.ini
--rw-rw-r--   0 willg     (1000) willg     (1000)      453 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/dev-cli.ini
--rwxrwxr-x   0 willg     (1000) willg     (1000)      721 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/generate-csr.sh
--rw-rw-r--   0 willg     (1000) willg     (1000)      114 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/openssl.cnf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:53.299259 certbot-2.8.0/examples/plugins/
--rw-rw-r--   0 willg     (1000) willg     (1000)      674 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/plugins/certbot_example_plugins.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      378 2023-12-05 19:13:52.000000 certbot-2.8.0/examples/plugins/setup.py
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:13:53.303259 certbot-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     4550 2023-12-05 19:13:52.000000 certbot-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.347083 certbot-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)   119682 2024-02-08 19:45:17.000000 certbot-2.9.0/CHANGELOG.md
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11456 2024-02-08 19:45:17.000000 certbot-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      267 2024-02-08 19:45:17.000000 certbot-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     8130 2024-02-08 19:45:18.347083 certbot-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4264 2024-02-08 19:45:17.000000 certbot-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.327083 certbot-2.9.0/certbot/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      113 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.327083 certbot-2.9.0/certbot/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      184 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14642 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/account.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    21072 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/auth_handler.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18597 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cert_manager.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.327083 certbot-2.9.0/certbot/_internal/cli/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    25926 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4024 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/cli_constants.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11286 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/cli_utils.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1073 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/group_adder.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22702 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/helpful.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2055 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/paths_parser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6210 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/plugins_parsing.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4162 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/subparsers.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5223 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/cli/verb_help.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    36975 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/client.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7616 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/constants.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.331083 certbot-2.9.0/certbot/_internal/display/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       33 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/display/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2578 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/display/completer.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      811 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/display/dummy_readline.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22469 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/display/obj.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3456 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/display/util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4484 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/eff.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7452 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/error_handler.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10644 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/hooks.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10226 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/lock.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15384 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/log.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    74966 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/main.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.331083 certbot-2.9.0/certbot/_internal/plugins/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       23 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11272 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/disco.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11966 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/manual.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1579 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/null.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15772 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/selection.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9340 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/standalone.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15984 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/plugins/webroot.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    26160 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/renewal.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3706 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/snap_config.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    53441 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/storage.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.331083 certbot-2.9.0/certbot/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       20 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14284 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/account_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    25036 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/auth_handler_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    31115 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/cert_manager_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    26212 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/cli_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    46400 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/client_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.331083 certbot-2.9.0/certbot/_internal/tests/compat/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/compat/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    27416 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/compat/filesystem_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1747 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/compat/misc_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      604 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/compat/os_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7862 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/configuration_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18934 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/crypto_util_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.331083 certbot-2.9.0/certbot/_internal/tests/display/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       28 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3716 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/completer_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5153 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/internal_util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13201 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/obj_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    20275 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/ops_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2375 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/display/util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6676 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/eff_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5202 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/error_handler_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1956 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/errors_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4983 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/helpful_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    17948 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/hook_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5060 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/lock_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15949 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/log_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)   123854 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/main_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    17535 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/ocsp_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.335083 certbot-2.9.0/certbot/_internal/tests/plugins/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       28 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14446 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/common_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11418 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/disco_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8522 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/dns_common_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2340 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/enhancements_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7425 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/manual_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      674 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/null_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9958 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/selection_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6817 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/standalone_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5541 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/storage_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1511 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15386 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/plugins/webroot_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14936 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/renewal_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5509 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/renewupdater_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    17001 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/reverter_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    45136 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/storage_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24762 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/tests/util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4747 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/_internal/updater.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2024 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/achallenges.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.335083 certbot-2.9.0/certbot/compat/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      249 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/compat/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1797 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/compat/_path.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    30470 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/compat/filesystem.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5412 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/compat/misc.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9511 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/compat/os.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    19114 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/configuration.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24587 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/crypto_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.335083 certbot-2.9.0/certbot/display/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       33 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/display/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13522 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/display/ops.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7268 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/display/util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2786 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/errors.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15584 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/interfaces.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      535 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/main.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15052 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/ocsp.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.335083 certbot-2.9.0/certbot/plugins/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       23 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    17525 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/common.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14028 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/dns_common.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12954 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/dns_common_lexicon.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2635 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/dns_test_common.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15716 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/dns_test_common_lexicon.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6809 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/enhancements.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4294 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/storage.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1811 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/plugins/util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/py.typed
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22069 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/reverter.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      424 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/ssl-dhparams.pem
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.335083 certbot-2.9.0/certbot/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       42 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2763 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/acme_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.339083 certbot-2.9.0/certbot/tests/testdata/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      642 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/README
+-rw-rw-r--   0 erica     (1001) erica     (1001)      952 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert-5sans_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      623 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert-nosans_nistp256.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      786 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert-san_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1200 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_2048.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      709 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      887 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_512_bad.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2400 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_fullchain_2048.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1208 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_intermediate_1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1208 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_intermediate_2.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1220 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cert_leaf.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)       25 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/cli.ini
+-rw-rw-r--   0 erica     (1001) erica     (1001)      502 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-6sans_512.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      676 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-6sans_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      420 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-nonames_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      277 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-nosans_512.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      493 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-nosans_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      452 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-nosans_nistp256.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      574 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr-san_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      281 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr_512.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      452 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/csr_512.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      302 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ec_prime256v1_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      359 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ec_secp384r1_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      436 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ec_secp521r1_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      227 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/nistp256_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2273 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ocsp_certificate.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2247 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ocsp_issuer_certificate.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1671 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/ocsp_responder_certificate.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      190 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/os-release
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1708 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/rsa2048_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      298 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/rsa256_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      493 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/rsa512_key.pem
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.339083 certbot-2.9.0/certbot/tests/testdata/sample-archive/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1736 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive/cert1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1123 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive/chain1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2859 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive/fullchain1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1704 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive/privkey1.pem
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.339083 certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1050 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/cert1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1208 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/chain1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2258 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/fullchain1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      241 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/privkey1.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1877 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-renewal-ancient.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      553 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-renewal-deprecated-option.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1970 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-renewal-ec.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1911 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/sample-renewal.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       54 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/testdata/webrootconftest.ini
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18166 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/tests/util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    25674 2024-02-08 19:45:17.000000 certbot-2.9.0/certbot/util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/certbot.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     8130 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7652 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      291 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      910 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        8 2024-02-08 19:45:18.000000 certbot-2.9.0/certbot.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.339083 certbot-2.9.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7073 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/Makefile
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.339083 certbot-2.9.0/docs/_static/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/_static/.gitignore
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/docs/_templates/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2004 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/_templates/footer.html
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/docs/api/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      148 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.achallenges.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      166 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.compat.filesystem.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      148 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.compat.misc.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      180 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.compat.os.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      247 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.compat.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      150 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.crypto_util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      148 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.display.ops.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      224 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.display.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      151 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.display.util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      133 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.errors.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      145 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.interfaces.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      127 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.main.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      131 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.ocsp.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      157 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.common.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      171 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.dns_common.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      197 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.dns_common_lexicon.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      188 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.dns_test_common.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      214 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.dns_test_common_lexicon.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      175 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.enhancements.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      432 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      160 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.storage.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      151 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.plugins.util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      139 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.reverter.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      424 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      162 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.tests.acme_util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      220 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.tests.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      145 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.tests.util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      127 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api/certbot.util.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      100 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4701 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/challenges.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)    15001 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/ciphers.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)    41235 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/cli-help.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2001 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/compatibility.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10307 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    26849 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/contributing.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      347 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5935 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/install.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      258 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/intro.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7259 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/make.bat
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/docs/man/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      751 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/man/certbot.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2861 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/packaging.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      147 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/resources.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)    57724 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/using.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1712 2024-02-08 19:45:17.000000 certbot-2.9.0/docs/what.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/examples/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       36 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1283 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/cli.ini
+-rw-rw-r--   0 erica     (1001) erica     (1001)      453 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/dev-cli.ini
+-rwxrwxr-x   0 erica     (1001) erica     (1001)      721 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/generate-csr.sh
+-rw-rw-r--   0 erica     (1001) erica     (1001)      114 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/openssl.cnf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:18.343083 certbot-2.9.0/examples/plugins/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      674 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/plugins/certbot_example_plugins.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      378 2024-02-08 19:45:17.000000 certbot-2.9.0/examples/plugins/setup.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:18.347083 certbot-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4600 2024-02-08 19:45:17.000000 certbot-2.9.0/setup.py
```

### Comparing `certbot-2.8.0/CHANGELOG.md` & `certbot-2.9.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Certbot change log
 
 Certbot adheres to [Semantic Versioning](https://semver.org/).
 
+## 2.9.0 - 2024-02-08
+
+### Added
+
+* Support for Python 3.12 was added.
+
+### Changed
+
+*
+
+### Fixed
+
+* Updates `joinpath` syntax to only use one addition per call, because the multiple inputs
+  version was causing mypy errors on Python 3.10.
+* Makes the `reconfigure` verb actually use the staging server for the dry run to check the new
+  configuration.
+
+More details about these changes can be found on our GitHub repo.
+
 ## 2.8.0 - 2023-12-05
 
 ### Added
 
 * Added support for [Alpine Linux](https://www.alpinelinux.org) distribution when is used the apache plugin
 
 ### Changed
```

### Comparing `certbot-2.8.0/LICENSE.txt` & `certbot-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/PKG-INFO` & `certbot-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot
-Version: 2.8.0
+Version: 2.9.0
 Summary: ACME client
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,23 +14,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: acme>=2.8.0
+Requires-Dist: acme>=2.9.0
 Requires-Dist: ConfigArgParse>=1.5.3
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: cryptography>=3.2.1
 Requires-Dist: distro>=1.0.1
 Requires-Dist: importlib_resources>=1.3.1; python_version < "3.9"
 Requires-Dist: importlib_metadata>=4.6; python_version < "3.10"
 Requires-Dist: josepy>=1.13.0
```

### Comparing `certbot-2.8.0/README.rst` & `certbot-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/account.py` & `certbot-2.9.0/certbot/_internal/account.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/auth_handler.py` & `certbot-2.9.0/certbot/_internal/auth_handler.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cert_manager.py` & `certbot-2.9.0/certbot/_internal/cert_manager.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/__init__.py` & `certbot-2.9.0/certbot/_internal/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from certbot._internal.cli.cli_utils import config_help
 from certbot._internal.cli.cli_utils import CustomHelpFormatter
 from certbot._internal.cli.cli_utils import flag_default
 from certbot._internal.cli.cli_utils import HelpfulArgumentGroup
 from certbot._internal.cli.cli_utils import nonnegative_int
 from certbot._internal.cli.cli_utils import parse_preferred_challenges
 from certbot._internal.cli.cli_utils import read_file
+from certbot._internal.cli.cli_utils import set_test_server_options
 from certbot._internal.cli.group_adder import _add_all_groups
 from certbot._internal.cli.helpful import HelpfulArgumentParser
 from certbot._internal.cli.paths_parser import _paths_parser
 from certbot._internal.cli.plugins_parsing import _plugins_parsing
 from certbot._internal.cli.subparsers import _create_subparsers
 from certbot._internal.cli.verb_help import VERB_HELP
 from certbot._internal.cli.verb_help import VERB_HELP_MAP
```

### Comparing `certbot-2.8.0/certbot/_internal/cli/cli_constants.py` & `certbot-2.9.0/certbot/_internal/cli/cli_constants.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/cli_utils.py` & `certbot-2.9.0/certbot/_internal/cli/cli_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Certbot command line util function"""
 import argparse
 import copy
+import glob
 import inspect
 from typing import Any
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
@@ -246,7 +247,52 @@
         int_value = int(value)
     except ValueError:
         raise argparse.ArgumentTypeError("value must be an integer")
 
     if int_value < 0:
         raise argparse.ArgumentTypeError("value must be non-negative")
     return int_value
+
+def set_test_server_options(verb: str, config: configuration.NamespaceConfig) -> None:
+    """Updates server, break_my_certs, staging, tos, and
+    register_unsafely_without_email in config as necessary to prepare
+    to use the test server.
+
+    We have --staging/--dry-run; perform sanity check and set config.server
+
+    :param str verb: subcommand called
+
+    :param config: parsed command line arguments
+    :type config: configuration.NamespaceConfig
+
+    :raises errors.Error: if non-default server is used and --staging is set
+    :raises errors.Error: if inapplicable verb is used and --dry-run is set
+    """
+
+    # Flag combinations should produce these results:
+    #                             | --staging      | --dry-run   |
+    # ------------------------------------------------------------
+    # | --server acme-v02         | Use staging    | Use staging |
+    # | --server acme-staging-v02 | Use staging    | Use staging |
+    # | --server <other>          | Conflict error | Use <other> |
+
+    default_servers = (flag_default("server"), constants.STAGING_URI)
+
+    if config.staging and config.server not in default_servers:
+        raise errors.Error("--server value conflicts with --staging")
+
+    if config.server == flag_default("server"):
+        config.server = constants.STAGING_URI
+        # If the account has already been loaded (such as by calling reconstitute before this),
+        # clear it so that we don't try to use the prod account on the staging server.
+        config.account = None
+
+    if config.dry_run:
+        if verb not in ["certonly", "renew", "reconfigure"]:
+            raise errors.Error("--dry-run currently only works with the "
+                               "'certonly' or 'renew' subcommands (%r)" % verb)
+        config.break_my_certs = config.staging = True
+        if glob.glob(os.path.join(config.config_dir, constants.ACCOUNTS_DIR, "*")):
+            # The user has a prod account, but might not have a staging
+            # one; we don't want to start trying to perform interactive registration
+            config.tos = True
+            config.register_unsafely_without_email = True
```

### Comparing `certbot-2.8.0/certbot/_internal/cli/group_adder.py` & `certbot-2.9.0/certbot/_internal/cli/group_adder.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/helpful.py` & `certbot-2.9.0/certbot/_internal/cli/helpful.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Certbot command line argument parser"""
 
 import argparse
 import functools
-import glob
 import sys
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -22,19 +21,19 @@
 from certbot._internal.cli.cli_constants import COMMAND_OVERVIEW
 from certbot._internal.cli.cli_constants import HELP_AND_VERSION_USAGE
 from certbot._internal.cli.cli_constants import SHORT_USAGE
 from certbot._internal.cli.cli_utils import add_domains
 from certbot._internal.cli.cli_utils import CustomHelpFormatter
 from certbot._internal.cli.cli_utils import flag_default
 from certbot._internal.cli.cli_utils import HelpfulArgumentGroup
+from certbot._internal.cli.cli_utils import set_test_server_options
 from certbot._internal.cli.verb_help import VERB_HELP
 from certbot._internal.cli.verb_help import VERB_HELP_MAP
 from certbot._internal.display import obj as display_obj
 from certbot._internal.plugins import disco
-from certbot.compat import os
 from certbot.configuration import ArgumentSource
 from certbot.configuration import NamespaceConfig
 
 
 class HelpfulArgumentParser:
     """Argparse Wrapper.
 
@@ -314,41 +313,18 @@
         if isinstance(config.key_type, list) and len(config.key_type) > 1:
             raise errors.Error(
                 "Only *one* --key-type type may be provided at this time.")
 
         return config
 
     def set_test_server(self, config: NamespaceConfig) -> None:
-        """We have --staging/--dry-run; perform sanity check and set config.server"""
-
-        # Flag combinations should produce these results:
-        #                             | --staging      | --dry-run   |
-        # ------------------------------------------------------------
-        # | --server acme-v02         | Use staging    | Use staging |
-        # | --server acme-staging-v02 | Use staging    | Use staging |
-        # | --server <other>          | Conflict error | Use <other> |
-
-        default_servers = (flag_default("server"), constants.STAGING_URI)
-
-        if config.staging and config.server not in default_servers:
-            raise errors.Error("--server value conflicts with --staging")
-
-        if config.server == flag_default("server"):
-            config.server = constants.STAGING_URI
-
-        if config.dry_run:
-            if self.verb not in ["certonly", "renew"]:
-                raise errors.Error("--dry-run currently only works with the "
-                                   "'certonly' or 'renew' subcommands (%r)" % self.verb)
-            config.break_my_certs = config.staging = True
-            if glob.glob(os.path.join(config.config_dir, constants.ACCOUNTS_DIR, "*")):
-                # The user has a prod account, but might not have a staging
-                # one; we don't want to start trying to perform interactive registration
-                config.tos = True
-                config.register_unsafely_without_email = True
+        """Updates server, break_my_certs, staging, tos, and
+        register_unsafely_without_email in config as necessary to prepare
+        to use the test server."""
+        return set_test_server_options(self.verb, config)
 
     def handle_csr(self, config: NamespaceConfig) -> None:
         """Process a --csr flag."""
         if config.verb != "certonly":
             raise errors.Error("Currently, a CSR file may only be specified "
                                "when obtaining a new or replacement "
                                "via the certonly command. Please try the "
```

### Comparing `certbot-2.8.0/certbot/_internal/cli/paths_parser.py` & `certbot-2.9.0/certbot/_internal/cli/paths_parser.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/plugins_parsing.py` & `certbot-2.9.0/certbot/_internal/cli/plugins_parsing.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/subparsers.py` & `certbot-2.9.0/certbot/_internal/cli/subparsers.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/cli/verb_help.py` & `certbot-2.9.0/certbot/_internal/cli/verb_help.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/client.py` & `certbot-2.9.0/certbot/_internal/client.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/constants.py` & `certbot-2.9.0/certbot/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/display/completer.py` & `certbot-2.9.0/certbot/_internal/display/completer.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/display/dummy_readline.py` & `certbot-2.9.0/certbot/_internal/display/dummy_readline.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/display/obj.py` & `certbot-2.9.0/certbot/_internal/display/obj.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/display/util.py` & `certbot-2.9.0/certbot/_internal/display/util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/eff.py` & `certbot-2.9.0/certbot/_internal/eff.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/error_handler.py` & `certbot-2.9.0/certbot/_internal/error_handler.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/hooks.py` & `certbot-2.9.0/certbot/_internal/hooks.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/lock.py` & `certbot-2.9.0/certbot/_internal/lock.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/log.py` & `certbot-2.9.0/certbot/_internal/log.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/main.py` & `certbot-2.9.0/certbot/_internal/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1723,18 +1723,16 @@
             "domains from the command to continue reconfiguring. You can specify which certificate "
             "you want on the command line with flag --cert-name instead.")
     # While we could technically allow domains to be used to specify the certificate in addition to
     # --cert-name, there's enough complexity with matching certs to domains that it's not worth it,
     # to say nothing of the difficulty in explaining what exactly this subcommand can modify
 
 
-    # To make sure that the requested changes work, do a dry run. While setting up the dry run,
-    # we will set all the needed fields in config, which will then be saved upon success.
-    config.dry_run = True
-
+    # To make sure that the requested changes work, we're going to do a dry run, and only save
+    # upon success. First, modify the config as the user requested.
     if not config.certname:
         certname_question = "Which certificate would you like to reconfigure?"
         config.certname = cert_manager.get_certnames(
             config, "reconfigure", allow_multiple=False,
             custom_prompt=certname_question)[0]
 
     certname = config.certname
@@ -1768,25 +1766,52 @@
         renewal_candidate = renewal.reconstitute(lineage_config, renewal_file)
     except Exception as e:  # pylint: disable=broad-except
         raise errors.ConfigurationError(f"Renewal configuration file {renewal_file} "
             f"(cert: {certname}) produced an unexpected error: {e}.")
     if not renewal_candidate:
         raise errors.ConfigurationError("Could not load certificate. See logs for errors.")
 
+    renewalparams = orig_renewal_conf['renewalparams']
+    # If server was set but hasn't changed and no account is loaded,
+    # load the old account because reconstitute won't have
+    if lineage_config.set_by_user('server') and lineage_config.server == renewalparams['server']\
+        and lineage_config.account is None:
+        lineage_config.account = renewalparams['account']
+    for param in ('account', 'server',):
+        if getattr(lineage_config, param) != renewalparams.get(param):
+            msg = ("Using reconfigure to change the ACME account or server is not supported. "
+                   "If you would like to do so, use renew with the --force-renewal flag instead "
+                   "of reconfigure. Note that doing so will count against any rate limits. For "
+                   "more information on this method, see "
+                   "https://certbot.org/renew-reconfiguration")
+            raise errors.ConfigurationError(msg)
+
     # this is where lineage_config gets fully filled out (e.g. --apache will set auth and installer)
     installer, auth = plug_sel.choose_configurator_plugins(lineage_config, plugins, "certonly")
-    le_client = _init_le_client(lineage_config, auth, installer)
+
+    # make a deep copy of lineage_config because we're about to modify it for a test dry run
+    dry_run_lineage_config = copy.deepcopy(lineage_config)
+
+    # we also set noninteractive_mode to more accurately simulate renewal (since `certbot renew`
+    # implies noninteractive mode) and to avoid prompting the user as changes made to
+    # dry_run_lineage_config beyond this point will not be applied to the original lineage_config
+    dry_run_lineage_config.noninteractive_mode = True
+    dry_run_lineage_config.dry_run = True
+    cli.set_test_server_options("reconfigure", dry_run_lineage_config)
+
+    le_client = _init_le_client(dry_run_lineage_config, auth, installer)
 
     # renews cert as dry run to test that the new values are ok
     # at this point, renewal_candidate.configuration has the old values, but will use
     # the values from lineage_config when doing the dry run
-    _get_and_save_cert(le_client, lineage_config, certname=certname,
+    _get_and_save_cert(le_client, dry_run_lineage_config, certname=certname,
         lineage=renewal_candidate)
 
     # this function will update lineage.configuration with the new values, and save it to disk
+    # use the pre-dry-run version
     renewal_candidate.save_new_config_values(lineage_config)
 
     _report_reconfigure_results(renewal_file, orig_renewal_conf)
 
 
 @contextmanager
 def make_displayer(config: configuration.NamespaceConfig
```

### Comparing `certbot-2.8.0/certbot/_internal/plugins/disco.py` & `certbot-2.9.0/certbot/_internal/plugins/disco.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/plugins/manual.py` & `certbot-2.9.0/certbot/_internal/plugins/manual.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/plugins/null.py` & `certbot-2.9.0/certbot/_internal/plugins/null.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/plugins/selection.py` & `certbot-2.9.0/certbot/_internal/plugins/selection.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/plugins/standalone.py` & `certbot-2.9.0/certbot/_internal/plugins/standalone.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/plugins/webroot.py` & `certbot-2.9.0/certbot/_internal/plugins/webroot.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/renewal.py` & `certbot-2.9.0/certbot/_internal/renewal.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/snap_config.py` & `certbot-2.9.0/certbot/_internal/snap_config.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/storage.py` & `certbot-2.9.0/certbot/_internal/storage.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/account_test.py` & `certbot-2.9.0/certbot/_internal/tests/account_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/auth_handler_test.py` & `certbot-2.9.0/certbot/_internal/tests/auth_handler_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/cert_manager_test.py` & `certbot-2.9.0/certbot/_internal/tests/cert_manager_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/cli_test.py` & `certbot-2.9.0/certbot/_internal/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/client_test.py` & `certbot-2.9.0/certbot/_internal/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/compat/filesystem_test.py` & `certbot-2.9.0/certbot/_internal/tests/compat/filesystem_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/compat/misc_test.py` & `certbot-2.9.0/certbot/_internal/tests/compat/misc_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/compat/os_test.py` & `certbot-2.9.0/certbot/_internal/tests/compat/os_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/configuration_test.py` & `certbot-2.9.0/certbot/_internal/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/crypto_util_test.py` & `certbot-2.9.0/certbot/_internal/tests/crypto_util_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     """Tests for certbot.crypto_util.make_key."""
 
     def test_rsa(self):  # pylint: disable=no-self-use
         # RSA Key Type Test
         from certbot.crypto_util import make_key
 
         # Do not test larger keys as it takes too long.
-        OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, make_key(1024))
+        OpenSSL.crypto.load_privatekey(OpenSSL.crypto.FILETYPE_PEM, make_key(2048))
 
     def test_ec(self):  # pylint: disable=no-self-use
         # ECDSA Key Type Tests
         from certbot.crypto_util import make_key
 
         for (name, bits) in [('secp256r1', 256), ('secp384r1', 384), ('secp521r1', 521)]:
             pkey = OpenSSL.crypto.load_privatekey(
@@ -181,30 +181,30 @@
             )
             assert pkey.bits() == bits
 
     def test_bad_key_sizes(self):
         from certbot.crypto_util import make_key
 
         # Try a bad key size for RSA and ECDSA
-        with pytest.raises(errors.Error, match='Unsupported RSA key length: 512'):
-            make_key(bits=512, key_type='rsa')
+        with pytest.raises(errors.Error, match='Unsupported RSA key length: 1024'):
+            make_key(bits=1024, key_type='rsa')
 
     def test_bad_elliptic_curve_name(self):
         from certbot.crypto_util import make_key
         with pytest.raises(errors.Error, match='Unsupported elliptic curve: nothere'):
             make_key(elliptic_curve="nothere", key_type='ecdsa')
 
     def test_bad_key_type(self):
         from certbot.crypto_util import make_key
 
         # Try a bad --key-type
         with pytest.raises(errors.Error,
                            match=re.escape('Invalid key_type specified: unf.  Use [rsa|ecdsa]')):
             OpenSSL.crypto.load_privatekey(
-                OpenSSL.crypto.FILETYPE_PEM, make_key(1024, key_type='unf'))
+                OpenSSL.crypto.FILETYPE_PEM, make_key(2048, key_type='unf'))
 
 
 class VerifyCertSetup(unittest.TestCase):
     """Refactoring for verification tests."""
 
     def setUp(self):
         self.renewable_cert = mock.MagicMock()
```

### Comparing `certbot-2.8.0/certbot/_internal/tests/display/completer_test.py` & `certbot-2.9.0/certbot/_internal/tests/display/completer_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/display/internal_util_test.py` & `certbot-2.9.0/certbot/_internal/tests/display/internal_util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/display/obj_test.py` & `certbot-2.9.0/certbot/_internal/tests/display/obj_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/display/ops_test.py` & `certbot-2.9.0/certbot/_internal/tests/display/ops_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/display/util_test.py` & `certbot-2.9.0/certbot/_internal/tests/display/util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/eff_test.py` & `certbot-2.9.0/certbot/_internal/tests/eff_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/error_handler_test.py` & `certbot-2.9.0/certbot/_internal/tests/error_handler_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/errors_test.py` & `certbot-2.9.0/certbot/_internal/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/helpful_test.py` & `certbot-2.9.0/certbot/_internal/tests/helpful_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/hook_test.py` & `certbot-2.9.0/certbot/_internal/tests/hook_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/lock_test.py` & `certbot-2.9.0/certbot/_internal/tests/lock_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/log_test.py` & `certbot-2.9.0/certbot/_internal/tests/log_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/main_test.py` & `certbot-2.9.0/certbot/_internal/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1679,5872 +1679,6063 @@
 000068e0: 2020 2020 2020 2020 2020 5b72 656e 6577            [renew
 000068f0: 616c 7061 7261 6d73 5d0a 2020 2020 2020  alparams].      
 00006900: 2020 2020 2020 6163 636f 756e 7420 3d20        account = 
 00006910: 6565 3433 3633 3464 6230 6161 3465 3638  ee43634db0aa4e68
 00006920: 3034 6631 3532 6265 3339 3939 3065 3661  04f152be39990e6a
 00006930: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
 00006940: 7665 7220 3d20 6874 7470 733a 2f2f 6163  ver = https://ac
-00006950: 6d65 2d73 7461 6769 6e67 2d76 3032 2e61  me-staging-v02.a
-00006960: 7069 2e6c 6574 7365 6e63 7279 7074 2e6f  pi.letsencrypt.o
-00006970: 7267 2f64 6972 6563 746f 7279 0a20 2020  rg/directory.   
-00006980: 2020 2020 2020 2020 2061 7574 6865 6e74           authent
-00006990: 6963 6174 6f72 203d 206e 6769 6e78 0a20  icator = nginx. 
-000069a0: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
-000069b0: 6c6c 6572 203d 206e 6769 6e78 0a20 2020  ller = nginx.   
-000069c0: 2020 2020 2020 2020 206b 6579 5f74 7970           key_typ
-000069d0: 6520 3d20 7273 610a 2020 2020 2020 2020  e = rsa.        
-000069e0: 2222 220a 2020 2020 2020 2020 7769 7468  """.        with
-000069f0: 206f 7065 6e28 7365 6c66 2e72 656e 6577   open(self.renew
-00006a00: 616c 5f66 696c 652c 2027 7727 2920 6173  al_file, 'w') as
-00006a10: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-00006a20: 662e 7772 6974 6528 6f72 6967 696e 616c  f.write(original
-00006a30: 5f63 6f6e 6669 6729 0a20 2020 2020 2020  _config).       
-00006a40: 2077 6974 6820 6f70 656e 2873 656c 662e   with open(self.
-00006a50: 7265 6e65 7761 6c5f 6669 6c65 2c20 2772  renewal_file, 'r
-00006a60: 2729 2061 7320 663a 0a20 2020 2020 2020  ') as f:.       
-00006a70: 2020 2020 2073 656c 662e 6f72 6967 696e       self.origin
-00006a80: 616c 5f63 6f6e 6669 6720 3d20 636f 6e66  al_config = conf
-00006a90: 6967 6f62 6a2e 436f 6e66 6967 4f62 6a28  igobj.ConfigObj(
-00006aa0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-00006ab0: 2020 2065 6e63 6f64 696e 673d 2775 7466     encoding='utf
-00006ac0: 2d38 272c 2064 6566 6175 6c74 5f65 6e63  -8', default_enc
-00006ad0: 6f64 696e 673d 2775 7466 2d38 2729 0a0a  oding='utf-8')..
-00006ae0: 0a20 2020 2064 6566 2074 6561 7244 6f77  .    def tearDow
-00006af0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00006b00: 2073 7570 6572 2829 2e74 6561 7244 6f77   super().tearDow
-00006b10: 6e28 290a 2020 2020 2020 2020 7365 6c66  n().        self
-00006b20: 2e67 6574 5f75 7469 6c69 7479 5f70 6174  .get_utility_pat
-00006b30: 6368 2e73 746f 7028 290a 2020 2020 2020  ch.stop().      
-00006b40: 2020 666f 7220 7061 7463 6820 696e 2073    for patch in s
-00006b50: 656c 662e 7061 7463 6865 7273 2e76 616c  elf.patchers.val
-00006b60: 7565 7328 293a 0a20 2020 2020 2020 2020  ues():.         
-00006b70: 2020 2070 6174 6368 2e73 746f 7028 290a     patch.stop().
-00006b80: 0a20 2020 2064 6566 205f 6361 6c6c 2873  .    def _call(s
-00006b90: 656c 662c 2070 6173 7365 645f 6172 6773  elf, passed_args
-00006ba0: 293a 0a20 2020 2020 2020 2066 756c 6c5f  ):.        full_
-00006bb0: 6172 6773 203d 2070 6173 7365 645f 6172  args = passed_ar
-00006bc0: 6773 202b 205b 272d 2d63 6f6e 6669 672d  gs + ['--config-
-00006bd0: 6469 7227 2c20 7365 6c66 2e63 6f6e 6669  dir', self.confi
-00006be0: 675f 6469 725d 0a20 2020 2020 2020 2070  g_dir].        p
-00006bf0: 6c75 6769 6e73 203d 2064 6973 636f 2e50  lugins = disco.P
-00006c00: 6c75 6769 6e73 5265 6769 7374 7279 2e66  luginsRegistry.f
-00006c10: 696e 645f 616c 6c28 290a 2020 2020 2020  ind_all().      
-00006c20: 2020 636f 6e66 6967 203d 2063 6c69 2e70    config = cli.p
-00006c30: 7265 7061 7265 5f61 6e64 5f70 6172 7365  repare_and_parse
-00006c40: 5f61 7267 7328 706c 7567 696e 732c 2066  _args(plugins, f
-00006c50: 756c 6c5f 6172 6773 290a 0a20 2020 2020  ull_args)..     
-00006c60: 2020 2066 726f 6d20 6365 7274 626f 742e     from certbot.
-00006c70: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2069  _internal.main i
-00006c80: 6d70 6f72 7420 7265 636f 6e66 6967 7572  mport reconfigur
-00006c90: 650a 2020 2020 2020 2020 7265 636f 6e66  e.        reconf
-00006ca0: 6967 7572 6528 636f 6e66 6967 2c20 706c  igure(config, pl
-00006cb0: 7567 696e 7329 0a0a 2020 2020 2020 2020  ugins)..        
-00006cc0: 7769 7468 206f 7065 6e28 7365 6c66 2e72  with open(self.r
-00006cd0: 656e 6577 616c 5f66 696c 652c 2027 7227  enewal_file, 'r'
-00006ce0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00006cf0: 2020 2020 7570 6461 7465 645f 636f 6e66      updated_conf
-00006d00: 203d 2063 6f6e 6669 676f 626a 2e43 6f6e   = configobj.Con
-00006d10: 6669 674f 626a 2866 2c20 656e 636f 6469  figObj(f, encodi
-00006d20: 6e67 3d27 7574 662d 3827 2c20 6465 6661  ng='utf-8', defa
-00006d30: 756c 745f 656e 636f 6469 6e67 3d27 7574  ult_encoding='ut
-00006d40: 662d 3827 290a 0a20 2020 2020 2020 2072  f-8')..        r
-00006d50: 6574 7572 6e20 7570 6461 7465 645f 636f  eturn updated_co
-00006d60: 6e66 0a0a 2020 2020 6465 6620 7465 7374  nf..    def test
-00006d70: 5f64 6f6d 6169 6e73 5f73 6574 2873 656c  _domains_set(sel
-00006d80: 6629 3a0a 2020 2020 2020 2020 7769 7468  f):.        with
-00006d90: 2070 7974 6573 742e 7261 6973 6573 2865   pytest.raises(e
-00006da0: 7272 6f72 732e 436f 6e66 6967 7572 6174  rrors.Configurat
-00006db0: 696f 6e45 7272 6f72 293a 0a20 2020 2020  ionError):.     
-00006dc0: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-00006dd0: 6c28 272d 2d63 6572 742d 6e61 6d65 2063  l('--cert-name c
-00006de0: 6572 7431 202d 6420 6f6e 652e 6365 7274  ert1 -d one.cert
-00006df0: 2e63 6f6d 272e 7370 6c69 7428 2929 0a0a  .com'.split())..
-00006e00: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-00006e10: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00006e20: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
-00006e30: 6765 745f 6365 7274 6e61 6d65 7327 290a  get_certnames').
-00006e40: 2020 2020 6465 6620 7465 7374 5f61 736b      def test_ask
-00006e50: 735f 666f 725f 6365 7274 6e61 6d65 2873  s_for_certname(s
-00006e60: 656c 662c 206d 6f63 6b5f 6365 7274 5f6d  elf, mock_cert_m
-00006e70: 616e 6167 6572 293a 0a20 2020 2020 2020  anager):.       
-00006e80: 206e 616d 6564 5f6d 6f63 6b20 3d20 6d6f   named_mock = mo
-00006e90: 636b 2e4d 6f63 6b28 290a 2020 2020 2020  ck.Mock().      
-00006ea0: 2020 6e61 6d65 645f 6d6f 636b 2e6e 616d    named_mock.nam
-00006eb0: 6520 3d20 276e 6769 6e78 270a 0a20 2020  e = 'nginx'..   
-00006ec0: 2020 2020 2073 656c 662e 6d6f 636b 735b       self.mocks[
-00006ed0: 2770 6963 6b5f 696e 7374 616c 6c65 7227  'pick_installer'
-00006ee0: 5d2e 7265 7475 726e 5f76 616c 7565 203d  ].return_value =
-00006ef0: 206e 616d 6564 5f6d 6f63 6b0a 2020 2020   named_mock.    
-00006f00: 2020 2020 7365 6c66 2e6d 6f63 6b73 5b27      self.mocks['
-00006f10: 7069 636b 5f61 7574 6827 5d2e 7265 7475  pick_auth'].retu
-00006f20: 726e 5f76 616c 7565 203d 206e 616d 6564  rn_value = named
-00006f30: 5f6d 6f63 6b0a 2020 2020 2020 2020 7365  _mock.        se
-00006f40: 6c66 2e6d 6f63 6b73 5b27 6669 6e64 5f69  lf.mocks['find_i
-00006f50: 6e69 7427 5d2e 7265 7475 726e 5f76 616c  nit'].return_val
-00006f60: 7565 203d 206e 616d 6564 5f6d 6f63 6b0a  ue = named_mock.
-00006f70: 2020 2020 2020 2020 6d6f 636b 5f63 6572          mock_cer
-00006f80: 745f 6d61 6e61 6765 722e 7265 7475 726e  t_manager.return
-00006f90: 5f76 616c 7565 203d 205b 2765 7861 6d70  _value = ['examp
-00006fa0: 6c65 2e63 6f6d 275d 0a20 2020 2020 2020  le.com'].       
-00006fb0: 2073 656c 662e 5f63 616c 6c28 272d 2d6e   self._call('--n
-00006fc0: 6769 6e78 272e 7370 6c69 7428 2929 0a20  ginx'.split()). 
-00006fd0: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
-00006fe0: 636b 5f63 6572 745f 6d61 6e61 6765 722e  ck_cert_manager.
-00006ff0: 6361 6c6c 5f63 6f75 6e74 203d 3d20 310a  call_count == 1.
-00007000: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
-00007010: 6461 7465 5f63 6f6e 6669 6775 7261 746f  date_configurato
-00007020: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-00007030: 206e 616d 6564 5f6d 6f63 6b20 3d20 6d6f   named_mock = mo
-00007040: 636b 2e4d 6f63 6b28 290a 2020 2020 2020  ck.Mock().      
-00007050: 2020 6e61 6d65 645f 6d6f 636b 2e6e 616d    named_mock.nam
-00007060: 6520 3d20 2761 7061 6368 6527 0a0a 2020  e = 'apache'..  
-00007070: 2020 2020 2020 7365 6c66 2e6d 6f63 6b73        self.mocks
-00007080: 5b27 7069 636b 5f69 6e73 7461 6c6c 6572  ['pick_installer
-00007090: 275d 2e72 6574 7572 6e5f 7661 6c75 6520  '].return_value 
-000070a0: 3d20 6e61 6d65 645f 6d6f 636b 0a20 2020  = named_mock.   
-000070b0: 2020 2020 2073 656c 662e 6d6f 636b 735b       self.mocks[
-000070c0: 2770 6963 6b5f 6175 7468 275d 2e72 6574  'pick_auth'].ret
-000070d0: 7572 6e5f 7661 6c75 6520 3d20 6e61 6d65  urn_value = name
-000070e0: 645f 6d6f 636b 0a20 2020 2020 2020 2073  d_mock.        s
-000070f0: 656c 662e 6d6f 636b 735b 2766 696e 645f  elf.mocks['find_
-00007100: 696e 6974 275d 2e72 6574 7572 6e5f 7661  init'].return_va
-00007110: 6c75 6520 3d20 6e61 6d65 645f 6d6f 636b  lue = named_mock
-00007120: 0a0a 2020 2020 2020 2020 6e65 775f 636f  ..        new_co
-00007130: 6e66 6967 203d 2073 656c 662e 5f63 616c  nfig = self._cal
-00007140: 6c28 272d 2d63 6572 742d 6e61 6d65 2065  l('--cert-name e
-00007150: 7861 6d70 6c65 2e63 6f6d 202d 2d61 7061  xample.com --apa
-00007160: 6368 6527 2e73 706c 6974 2829 290a 2020  che'.split()).  
-00007170: 2020 2020 2020 6173 7365 7274 206e 6577        assert new
-00007180: 5f63 6f6e 6669 675b 2772 656e 6577 616c  _config['renewal
-00007190: 7061 7261 6d73 275d 5b27 6175 7468 656e  params']['authen
-000071a0: 7469 6361 746f 7227 5d20 3d3d 2027 6170  ticator'] == 'ap
-000071b0: 6163 6865 270a 0a20 2020 2040 6d6f 636b  ache'..    @mock
-000071c0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-000071d0: 5f69 6e74 6572 6e61 6c2e 686f 6f6b 732e  _internal.hooks.
-000071e0: 7661 6c69 6461 7465 5f68 6f6f 6b73 2729  validate_hooks')
-000071f0: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
-00007200: 6461 7465 5f68 6f6f 6b73 2873 656c 662c  date_hooks(self,
-00007210: 2075 6e75 7365 645f 7661 6c69 6461 7465   unused_validate
-00007220: 5f68 6f6f 6b73 293a 0a20 2020 2020 2020  _hooks):.       
-00007230: 2061 7373 6572 7420 2770 7265 5f68 6f6f   assert 'pre_hoo
-00007240: 6b27 206e 6f74 2069 6e20 7365 6c66 2e6f  k' not in self.o
-00007250: 7269 6769 6e61 6c5f 636f 6e66 6967 0a20  riginal_config. 
-00007260: 2020 2020 2020 2023 2074 6573 7420 7365         # test se
-00007270: 740a 2020 2020 2020 2020 6e65 775f 636f  t.        new_co
-00007280: 6e66 6967 203d 2073 656c 662e 5f63 616c  nfig = self._cal
-00007290: 6c28 272d 2d63 6572 742d 6e61 6d65 2065  l('--cert-name e
-000072a0: 7861 6d70 6c65 2e63 6f6d 202d 2d70 7265  xample.com --pre
-000072b0: 2d68 6f6f 6b27 2e73 706c 6974 2829 202b  -hook'.split() +
-000072c0: 205b 2765 6368 6f20 7072 6527 5d29 0a20   ['echo pre']). 
-000072d0: 2020 2020 2020 2061 7373 6572 7420 6e65         assert ne
-000072e0: 775f 636f 6e66 6967 5b27 7265 6e65 7761  w_config['renewa
-000072f0: 6c70 6172 616d 7327 5d5b 2770 7265 5f68  lparams']['pre_h
-00007300: 6f6f 6b27 5d20 3d3d 2027 6563 686f 2070  ook'] == 'echo p
-00007310: 7265 270a 2020 2020 2020 2020 2320 7465  re'.        # te
-00007320: 7374 2075 7064 6174 650a 2020 2020 2020  st update.      
+00006950: 6d65 2d76 3032 2e61 7069 2e6c 6574 7365  me-v02.api.letse
+00006960: 6e63 7279 7074 2e6f 7267 2f64 6972 6563  ncrypt.org/direc
+00006970: 746f 7279 0a20 2020 2020 2020 2020 2020  tory.           
+00006980: 2061 7574 6865 6e74 6963 6174 6f72 203d   authenticator =
+00006990: 206e 6769 6e78 0a20 2020 2020 2020 2020   nginx.         
+000069a0: 2020 2069 6e73 7461 6c6c 6572 203d 206e     installer = n
+000069b0: 6769 6e78 0a20 2020 2020 2020 2020 2020  ginx.           
+000069c0: 206b 6579 5f74 7970 6520 3d20 7273 610a   key_type = rsa.
+000069d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000069e0: 2020 2020 7769 7468 206f 7065 6e28 7365      with open(se
+000069f0: 6c66 2e72 656e 6577 616c 5f66 696c 652c  lf.renewal_file,
+00006a00: 2027 7727 2920 6173 2066 3a0a 2020 2020   'w') as f:.    
+00006a10: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00006a20: 6f72 6967 696e 616c 5f63 6f6e 6669 6729  original_config)
+00006a30: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+00006a40: 656e 2873 656c 662e 7265 6e65 7761 6c5f  en(self.renewal_
+00006a50: 6669 6c65 2c20 2772 2729 2061 7320 663a  file, 'r') as f:
+00006a60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006a70: 662e 6f72 6967 696e 616c 5f63 6f6e 6669  f.original_confi
+00006a80: 6720 3d20 636f 6e66 6967 6f62 6a2e 436f  g = configobj.Co
+00006a90: 6e66 6967 4f62 6a28 662c 0a20 2020 2020  nfigObj(f,.     
+00006aa0: 2020 2020 2020 2020 2020 2065 6e63 6f64             encod
+00006ab0: 696e 673d 2775 7466 2d38 272c 2064 6566  ing='utf-8', def
+00006ac0: 6175 6c74 5f65 6e63 6f64 696e 673d 2775  ault_encoding='u
+00006ad0: 7466 2d38 2729 0a0a 0a20 2020 2064 6566  tf-8')...    def
+00006ae0: 2074 6561 7244 6f77 6e28 7365 6c66 293a   tearDown(self):
+00006af0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00006b00: 2e74 6561 7244 6f77 6e28 290a 2020 2020  .tearDown().    
+00006b10: 2020 2020 7365 6c66 2e67 6574 5f75 7469      self.get_uti
+00006b20: 6c69 7479 5f70 6174 6368 2e73 746f 7028  lity_patch.stop(
+00006b30: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
+00006b40: 7463 6820 696e 2073 656c 662e 7061 7463  tch in self.patc
+00006b50: 6865 7273 2e76 616c 7565 7328 293a 0a20  hers.values():. 
+00006b60: 2020 2020 2020 2020 2020 2070 6174 6368             patch
+00006b70: 2e73 746f 7028 290a 0a20 2020 2064 6566  .stop()..    def
+00006b80: 205f 6361 6c6c 2873 656c 662c 2070 6173   _call(self, pas
+00006b90: 7365 645f 6172 6773 293a 0a20 2020 2020  sed_args):.     
+00006ba0: 2020 2066 756c 6c5f 6172 6773 203d 2070     full_args = p
+00006bb0: 6173 7365 645f 6172 6773 202b 205b 272d  assed_args + ['-
+00006bc0: 2d63 6f6e 6669 672d 6469 7227 2c20 7365  -config-dir', se
+00006bd0: 6c66 2e63 6f6e 6669 675f 6469 725d 0a20  lf.config_dir]. 
+00006be0: 2020 2020 2020 2070 6c75 6769 6e73 203d         plugins =
+00006bf0: 2064 6973 636f 2e50 6c75 6769 6e73 5265   disco.PluginsRe
+00006c00: 6769 7374 7279 2e66 696e 645f 616c 6c28  gistry.find_all(
+00006c10: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00006c20: 203d 2063 6c69 2e70 7265 7061 7265 5f61   = cli.prepare_a
+00006c30: 6e64 5f70 6172 7365 5f61 7267 7328 706c  nd_parse_args(pl
+00006c40: 7567 696e 732c 2066 756c 6c5f 6172 6773  ugins, full_args
+00006c50: 290a 0a20 2020 2020 2020 2066 726f 6d20  )..        from 
+00006c60: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00006c70: 6c2e 6d61 696e 2069 6d70 6f72 7420 7265  l.main import re
+00006c80: 636f 6e66 6967 7572 650a 2020 2020 2020  configure.      
+00006c90: 2020 7265 636f 6e66 6967 7572 6528 636f    reconfigure(co
+00006ca0: 6e66 6967 2c20 706c 7567 696e 7329 0a0a  nfig, plugins)..
+00006cb0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+00006cc0: 6e28 7365 6c66 2e72 656e 6577 616c 5f66  n(self.renewal_f
+00006cd0: 696c 652c 2027 7227 2920 6173 2066 3a0a  ile, 'r') as f:.
+00006ce0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00006cf0: 7465 645f 636f 6e66 203d 2063 6f6e 6669  ted_conf = confi
+00006d00: 676f 626a 2e43 6f6e 6669 674f 626a 2866  gobj.ConfigObj(f
+00006d10: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
+00006d20: 3827 2c20 6465 6661 756c 745f 656e 636f  8', default_enco
+00006d30: 6469 6e67 3d27 7574 662d 3827 290a 0a20  ding='utf-8').. 
+00006d40: 2020 2020 2020 2072 6574 7572 6e20 7570         return up
+00006d50: 6461 7465 645f 636f 6e66 0a0a 2020 2020  dated_conf..    
+00006d60: 6465 6620 7465 7374 5f64 6f6d 6169 6e73  def test_domains
+00006d70: 5f73 6574 2873 656c 6629 3a0a 2020 2020  _set(self):.    
+00006d80: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+00006d90: 7261 6973 6573 2865 7272 6f72 732e 436f  raises(errors.Co
+00006da0: 6e66 6967 7572 6174 696f 6e45 7272 6f72  nfigurationError
+00006db0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00006dc0: 656c 662e 5f63 616c 6c28 272d 2d63 6572  elf._call('--cer
+00006dd0: 742d 6e61 6d65 2063 6572 7431 202d 6420  t-name cert1 -d 
+00006de0: 6f6e 652e 6365 7274 2e63 6f6d 272e 7370  one.cert.com'.sp
+00006df0: 6c69 7428 2929 0a0a 2020 2020 406d 6f63  lit())..    @moc
+00006e00: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00006e10: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
+00006e20: 6d61 6e61 6765 722e 6765 745f 6365 7274  manager.get_cert
+00006e30: 6e61 6d65 7327 290a 2020 2020 6465 6620  names').    def 
+00006e40: 7465 7374 5f61 736b 735f 666f 725f 6365  test_asks_for_ce
+00006e50: 7274 6e61 6d65 2873 656c 662c 206d 6f63  rtname(self, moc
+00006e60: 6b5f 6365 7274 5f6d 616e 6167 6572 293a  k_cert_manager):
+00006e70: 0a20 2020 2020 2020 206e 616d 6564 5f6d  .        named_m
+00006e80: 6f63 6b20 3d20 6d6f 636b 2e4d 6f63 6b28  ock = mock.Mock(
+00006e90: 290a 2020 2020 2020 2020 6e61 6d65 645f  ).        named_
+00006ea0: 6d6f 636b 2e6e 616d 6520 3d20 276e 6769  mock.name = 'ngi
+00006eb0: 6e78 270a 0a20 2020 2020 2020 2073 656c  nx'..        sel
+00006ec0: 662e 6d6f 636b 735b 2770 6963 6b5f 696e  f.mocks['pick_in
+00006ed0: 7374 616c 6c65 7227 5d2e 7265 7475 726e  staller'].return
+00006ee0: 5f76 616c 7565 203d 206e 616d 6564 5f6d  _value = named_m
+00006ef0: 6f63 6b0a 2020 2020 2020 2020 7365 6c66  ock.        self
+00006f00: 2e6d 6f63 6b73 5b27 7069 636b 5f61 7574  .mocks['pick_aut
+00006f10: 6827 5d2e 7265 7475 726e 5f76 616c 7565  h'].return_value
+00006f20: 203d 206e 616d 6564 5f6d 6f63 6b0a 2020   = named_mock.  
+00006f30: 2020 2020 2020 7365 6c66 2e6d 6f63 6b73        self.mocks
+00006f40: 5b27 6669 6e64 5f69 6e69 7427 5d2e 7265  ['find_init'].re
+00006f50: 7475 726e 5f76 616c 7565 203d 206e 616d  turn_value = nam
+00006f60: 6564 5f6d 6f63 6b0a 2020 2020 2020 2020  ed_mock.        
+00006f70: 6d6f 636b 5f63 6572 745f 6d61 6e61 6765  mock_cert_manage
+00006f80: 722e 7265 7475 726e 5f76 616c 7565 203d  r.return_value =
+00006f90: 205b 2765 7861 6d70 6c65 2e63 6f6d 275d   ['example.com']
+00006fa0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00006fb0: 616c 6c28 272d 2d6e 6769 6e78 272e 7370  all('--nginx'.sp
+00006fc0: 6c69 7428 2929 0a20 2020 2020 2020 2061  lit()).        a
+00006fd0: 7373 6572 7420 6d6f 636b 5f63 6572 745f  ssert mock_cert_
+00006fe0: 6d61 6e61 6765 722e 6361 6c6c 5f63 6f75  manager.call_cou
+00006ff0: 6e74 203d 3d20 310a 0a20 2020 2064 6566  nt == 1..    def
+00007000: 2074 6573 745f 7570 6461 7465 5f63 6f6e   test_update_con
+00007010: 6669 6775 7261 746f 7228 7365 6c66 293a  figurator(self):
+00007020: 0a20 2020 2020 2020 206e 616d 6564 5f6d  .        named_m
+00007030: 6f63 6b20 3d20 6d6f 636b 2e4d 6f63 6b28  ock = mock.Mock(
+00007040: 290a 2020 2020 2020 2020 6e61 6d65 645f  ).        named_
+00007050: 6d6f 636b 2e6e 616d 6520 3d20 2761 7061  mock.name = 'apa
+00007060: 6368 6527 0a0a 2020 2020 2020 2020 7365  che'..        se
+00007070: 6c66 2e6d 6f63 6b73 5b27 7069 636b 5f69  lf.mocks['pick_i
+00007080: 6e73 7461 6c6c 6572 275d 2e72 6574 7572  nstaller'].retur
+00007090: 6e5f 7661 6c75 6520 3d20 6e61 6d65 645f  n_value = named_
+000070a0: 6d6f 636b 0a20 2020 2020 2020 2073 656c  mock.        sel
+000070b0: 662e 6d6f 636b 735b 2770 6963 6b5f 6175  f.mocks['pick_au
+000070c0: 7468 275d 2e72 6574 7572 6e5f 7661 6c75  th'].return_valu
+000070d0: 6520 3d20 6e61 6d65 645f 6d6f 636b 0a20  e = named_mock. 
+000070e0: 2020 2020 2020 2073 656c 662e 6d6f 636b         self.mock
+000070f0: 735b 2766 696e 645f 696e 6974 275d 2e72  s['find_init'].r
+00007100: 6574 7572 6e5f 7661 6c75 6520 3d20 6e61  eturn_value = na
+00007110: 6d65 645f 6d6f 636b 0a0a 2020 2020 2020  med_mock..      
+00007120: 2020 6e65 775f 636f 6e66 6967 203d 2073    new_config = s
+00007130: 656c 662e 5f63 616c 6c28 272d 2d63 6572  elf._call('--cer
+00007140: 742d 6e61 6d65 2065 7861 6d70 6c65 2e63  t-name example.c
+00007150: 6f6d 202d 2d61 7061 6368 6527 2e73 706c  om --apache'.spl
+00007160: 6974 2829 290a 2020 2020 2020 2020 6173  it()).        as
+00007170: 7365 7274 206e 6577 5f63 6f6e 6669 675b  sert new_config[
+00007180: 2772 656e 6577 616c 7061 7261 6d73 275d  'renewalparams']
+00007190: 5b27 6175 7468 656e 7469 6361 746f 7227  ['authenticator'
+000071a0: 5d20 3d3d 2027 6170 6163 6865 270a 0a20  ] == 'apache'.. 
+000071b0: 2020 2064 6566 2074 6573 745f 6f6e 6c79     def test_only
+000071c0: 5f69 6e74 656e 6465 645f 6368 616e 6765  _intended_change
+000071d0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000071e0: 2022 2222 2043 6865 636b 2074 6861 7420   """ Check that 
+000071f0: 7765 2064 6f6e 2774 2061 6363 6964 656e  we don't acciden
+00007200: 7461 6c6c 7920 6d6f 6469 6679 2061 6e79  tally modify any
+00007210: 7468 696e 6720 7468 6174 2077 6520 6469  thing that we di
+00007220: 646e 2774 206d 6561 6e20 746f 2022 2222  dn't mean to """
+00007230: 0a20 2020 2020 2020 206e 616d 6564 5f6d  .        named_m
+00007240: 6f63 6b20 3d20 6d6f 636b 2e4d 6f63 6b28  ock = mock.Mock(
+00007250: 290a 2020 2020 2020 2020 6e61 6d65 645f  ).        named_
+00007260: 6d6f 636b 2e6e 616d 6520 3d20 2761 7061  mock.name = 'apa
+00007270: 6368 6527 0a0a 2020 2020 2020 2020 7365  che'..        se
+00007280: 6c66 2e6d 6f63 6b73 5b27 7069 636b 5f69  lf.mocks['pick_i
+00007290: 6e73 7461 6c6c 6572 275d 2e72 6574 7572  nstaller'].retur
+000072a0: 6e5f 7661 6c75 6520 3d20 6e61 6d65 645f  n_value = named_
+000072b0: 6d6f 636b 0a20 2020 2020 2020 2073 656c  mock.        sel
+000072c0: 662e 6d6f 636b 735b 2770 6963 6b5f 6175  f.mocks['pick_au
+000072d0: 7468 275d 2e72 6574 7572 6e5f 7661 6c75  th'].return_valu
+000072e0: 6520 3d20 6e61 6d65 645f 6d6f 636b 0a20  e = named_mock. 
+000072f0: 2020 2020 2020 2073 656c 662e 6d6f 636b         self.mock
+00007300: 735b 2766 696e 645f 696e 6974 275d 2e72  s['find_init'].r
+00007310: 6574 7572 6e5f 7661 6c75 6520 3d20 6e61  eturn_value = na
+00007320: 6d65 645f 6d6f 636b 0a0a 2020 2020 2020  med_mock..      
 00007330: 2020 6e65 775f 636f 6e66 6967 203d 2073    new_config = s
 00007340: 656c 662e 5f63 616c 6c28 272d 2d63 6572  elf._call('--cer
 00007350: 742d 6e61 6d65 2065 7861 6d70 6c65 2e63  t-name example.c
-00007360: 6f6d 202d 2d70 7265 2d68 6f6f 6b27 2e73  om --pre-hook'.s
-00007370: 706c 6974 2829 202b 205b 2765 6368 6f20  plit() + ['echo 
-00007380: 7072 6532 275d 290a 2020 2020 2020 2020  pre2']).        
-00007390: 6173 7365 7274 206e 6577 5f63 6f6e 6669  assert new_confi
-000073a0: 675b 2772 656e 6577 616c 7061 7261 6d73  g['renewalparams
-000073b0: 275d 5b27 7072 655f 686f 6f6b 275d 203d  ']['pre_hook'] =
-000073c0: 3d20 2765 6368 6f20 7072 6532 270a 0a20  = 'echo pre2'.. 
-000073d0: 2020 2020 2020 2023 2074 6573 7420 6465         # test de
-000073e0: 706c 6f79 2068 6f6f 6b20 6973 2073 6574  ploy hook is set
-000073f0: 2065 7665 6e20 7468 6f75 6768 2077 6520   even though we 
-00007400: 6469 6420 6120 6472 7920 7275 6e0a 2020  did a dry run.  
-00007410: 2020 2020 2020 6173 7365 7274 2027 7265        assert 're
-00007420: 6e65 775f 686f 6f6b 2720 6e6f 7420 696e  new_hook' not in
-00007430: 2073 656c 662e 6f72 6967 696e 616c 5f63   self.original_c
-00007440: 6f6e 6669 670a 2020 2020 2020 2020 6e65  onfig.        ne
-00007450: 775f 636f 6e66 6967 203d 2073 656c 662e  w_config = self.
-00007460: 5f63 616c 6c28 272d 2d63 6572 742d 6e61  _call('--cert-na
-00007470: 6d65 2065 7861 6d70 6c65 2e63 6f6d 202d  me example.com -
-00007480: 2d64 6570 6c6f 792d 686f 6f6b 272e 7370  -deploy-hook'.sp
-00007490: 6c69 7428 2920 2b20 5b27 6563 686f 2064  lit() + ['echo d
-000074a0: 6570 6c6f 7927 5d29 0a20 2020 2020 2020  eploy']).       
-000074b0: 2061 7373 6572 7420 6e65 775f 636f 6e66   assert new_conf
-000074c0: 6967 5b27 7265 6e65 7761 6c70 6172 616d  ig['renewalparam
-000074d0: 7327 5d5b 2772 656e 6577 5f68 6f6f 6b27  s']['renew_hook'
-000074e0: 5d20 3d3d 2027 6563 686f 2064 6570 6c6f  ] == 'echo deplo
-000074f0: 7927 0a0a 2020 2020 6465 6620 7465 7374  y'..    def test
-00007500: 5f64 7279 5f72 756e 5f66 6169 6c73 2873  _dry_run_fails(s
-00007510: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-00007520: 7365 7420 7369 6465 2065 6666 6563 7420  set side effect 
-00007530: 6f66 2072 6169 7369 6e67 2065 7272 6f72  of raising error
-00007540: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00007550: 636b 735b 275f 6765 745f 616e 645f 7361  cks['_get_and_sa
-00007560: 7665 5f63 6572 7427 5d2e 7369 6465 5f65  ve_cert'].side_e
-00007570: 6666 6563 7420 3d20 6572 726f 7273 2e45  ffect = errors.E
-00007580: 7272 6f72 0a0a 2020 2020 2020 2020 7472  rror..        tr
-00007590: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-000075a0: 656c 662e 5f63 616c 6c28 272d 2d63 6572  elf._call('--cer
-000075b0: 742d 6e61 6d65 2065 7861 6d70 6c65 2e63  t-name example.c
-000075c0: 6f6d 202d 2d61 7061 6368 6527 2e73 706c  om --apache'.spl
-000075d0: 6974 2829 290a 2020 2020 2020 2020 6578  it()).        ex
-000075e0: 6365 7074 2065 7272 6f72 732e 4572 726f  cept errors.Erro
-000075f0: 723a 0a20 2020 2020 2020 2020 2020 2070  r:.            p
-00007600: 6173 730a 0a20 2020 2020 2020 2023 2063  ass..        # c
-00007610: 6865 636b 2074 6861 7420 636f 6e66 6967  heck that config
-00007620: 2069 736e 2774 206d 6f64 6966 6965 640a   isn't modified.
-00007630: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00007640: 6e28 7365 6c66 2e72 656e 6577 616c 5f66  n(self.renewal_f
-00007650: 696c 652c 2027 7227 2920 6173 2066 3a0a  ile, 'r') as f:.
-00007660: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00007670: 636f 6e66 6967 203d 2063 6f6e 6669 676f  config = configo
-00007680: 626a 2e43 6f6e 6669 674f 626a 2866 2c20  bj.ConfigObj(f, 
-00007690: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-000076a0: 2c20 6465 6661 756c 745f 656e 636f 6469  , default_encodi
-000076b0: 6e67 3d27 7574 662d 3827 290a 2020 2020  ng='utf-8').    
-000076c0: 2020 2020 6173 7365 7274 206e 6577 5f63      assert new_c
-000076d0: 6f6e 6669 675b 2772 656e 6577 616c 7061  onfig['renewalpa
-000076e0: 7261 6d73 275d 5b27 6175 7468 656e 7469  rams']['authenti
-000076f0: 6361 746f 7227 5d20 3d3d 2027 6e67 696e  cator'] == 'ngin
-00007700: 7827 0a0a 2020 2020 406d 6f63 6b2e 7061  x'..    @mock.pa
-00007710: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-00007720: 7465 726e 616c 2e6d 6169 6e2e 6469 7370  ternal.main.disp
-00007730: 6c61 795f 7574 696c 2e6e 6f74 6966 7927  lay_util.notify'
-00007740: 290a 2020 2020 6465 6620 7465 7374 5f72  ).    def test_r
-00007750: 6570 6f72 745f 7265 7375 6c74 7328 7365  eport_results(se
-00007760: 6c66 2c20 6d6f 636b 5f6e 6f74 6966 7929  lf, mock_notify)
-00007770: 3a0a 2020 2020 2020 2020 2320 6d61 6b65  :.        # make
-00007780: 2073 7572 6520 7265 706f 7274 2072 6573   sure report res
-00007790: 756c 7473 2077 6f72 6b73 2077 6865 6e20  ults works when 
-000077a0: 636f 6e66 6967 2068 6173 2061 2077 6562  config has a web
-000077b0: 726f 6f74 206d 6170 0a20 2020 2020 2020  root map.       
-000077c0: 206f 7269 6769 6e61 6c5f 636f 6e66 6967   original_config
-000077d0: 203d 2022 2222 0a20 2020 2020 2020 2020   = """.         
-000077e0: 2020 2076 6572 7369 6f6e 203d 2032 2e30     version = 2.0
-000077f0: 2e30 0a20 2020 2020 2020 2020 2020 2061  .0.            a
-00007800: 7263 6869 7665 5f64 6972 203d 202f 6574  rchive_dir = /et
-00007810: 632f 6c65 7473 656e 6372 7970 742f 6172  c/letsencrypt/ar
-00007820: 6368 6976 652f 6578 616d 706c 652e 636f  chive/example.co
-00007830: 6d0a 2020 2020 2020 2020 2020 2020 6365  m.            ce
-00007840: 7274 203d 202f 6574 632f 6c65 7473 656e  rt = /etc/letsen
-00007850: 6372 7970 742f 6c69 7665 2f65 7861 6d70  crypt/live/examp
-00007860: 6c65 2e63 6f6d 2f63 6572 742e 7065 6d0a  le.com/cert.pem.
-00007870: 2020 2020 2020 2020 2020 2020 7072 6976              priv
-00007880: 6b65 7920 3d20 2f65 7463 2f6c 6574 7365  key = /etc/letse
-00007890: 6e63 7279 7074 2f6c 6976 652f 6578 616d  ncrypt/live/exam
-000078a0: 706c 652e 636f 6d2f 7072 6976 6b65 792e  ple.com/privkey.
-000078b0: 7065 6d0a 2020 2020 2020 2020 2020 2020  pem.            
-000078c0: 6368 6169 6e20 3d20 2f65 7463 2f6c 6574  chain = /etc/let
-000078d0: 7365 6e63 7279 7074 2f6c 6976 652f 6578  sencrypt/live/ex
-000078e0: 616d 706c 652e 636f 6d2f 6368 6169 6e2e  ample.com/chain.
-000078f0: 7065 6d0a 2020 2020 2020 2020 2020 2020  pem.            
-00007900: 6675 6c6c 6368 6169 6e20 3d20 2f65 7463  fullchain = /etc
-00007910: 2f6c 6574 7365 6e63 7279 7074 2f6c 6976  /letsencrypt/liv
-00007920: 652f 6578 616d 706c 652e 636f 6d2f 6675  e/example.com/fu
-00007930: 6c6c 6368 6169 6e2e 7065 6d0a 0a20 2020  llchain.pem..   
-00007940: 2020 2020 2020 2020 2023 204f 7074 696f           # Optio
-00007950: 6e73 2075 7365 6420 696e 2074 6865 2072  ns used in the r
-00007960: 656e 6577 616c 2070 726f 6365 7373 0a20  enewal process. 
-00007970: 2020 2020 2020 2020 2020 205b 7265 6e65             [rene
-00007980: 7761 6c70 6172 616d 735d 0a20 2020 2020  walparams].     
-00007990: 2020 2020 2020 2061 6363 6f75 6e74 203d         account =
-000079a0: 2065 6534 3336 3334 6462 3061 6134 6536   ee43634db0aa4e6
-000079b0: 3830 3466 3135 3262 6533 3939 3930 6536  804f152be39990e6
-000079c0: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
-000079d0: 7276 6572 203d 2068 7474 7073 3a2f 2f61  rver = https://a
-000079e0: 636d 652d 7374 6167 696e 672d 7630 322e  cme-staging-v02.
-000079f0: 6170 692e 6c65 7473 656e 6372 7970 742e  api.letsencrypt.
-00007a00: 6f72 672f 6469 7265 6374 6f72 790a 2020  org/directory.  
-00007a10: 2020 2020 2020 2020 2020 6175 7468 656e            authen
-00007a20: 7469 6361 746f 7220 3d20 7765 6272 6f6f  ticator = webroo
-00007a30: 740a 2020 2020 2020 2020 2020 2020 696e  t.            in
-00007a40: 7374 616c 6c65 7220 3d20 6e67 696e 780a  staller = nginx.
-00007a50: 2020 2020 2020 2020 2020 2020 6b65 795f              key_
-00007a60: 7479 7065 203d 2065 6364 7361 0a20 2020  type = ecdsa.   
-00007a70: 2020 2020 2020 2020 2077 6562 726f 6f74           webroot
-00007a80: 5f70 6174 6820 3d20 2f76 6172 2f77 7777  _path = /var/www
-00007a90: 2f68 746d 6c2c 0a20 2020 2020 2020 2020  /html,.         
-00007aa0: 2020 205b 5b77 6562 726f 6f74 5f6d 6170     [[webroot_map
-00007ab0: 5d5d 0a20 2020 2020 2020 2020 2020 2065  ]].            e
-00007ac0: 7861 6d70 6c65 2e63 6f6d 203d 202f 7661  xample.com = /va
-00007ad0: 722f 7777 772f 6874 6d6c 0a20 2020 2020  r/www/html.     
-00007ae0: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
-00007af0: 6974 6820 6f70 656e 2873 656c 662e 7265  ith open(self.re
-00007b00: 6e65 7761 6c5f 6669 6c65 2c20 2777 2729  newal_file, 'w')
-00007b10: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00007b20: 2020 2066 2e77 7269 7465 286f 7269 6769     f.write(origi
-00007b30: 6e61 6c5f 636f 6e66 6967 290a 2020 2020  nal_config).    
-00007b40: 2020 2020 7769 7468 206f 7065 6e28 7365      with open(se
-00007b50: 6c66 2e72 656e 6577 616c 5f66 696c 652c  lf.renewal_file,
-00007b60: 2027 7227 2920 6173 2066 3a0a 2020 2020   'r') as f:.    
-00007b70: 2020 2020 2020 2020 7365 6c66 2e6f 7269          self.ori
-00007b80: 6769 6e61 6c5f 636f 6e66 6967 203d 2063  ginal_config = c
-00007b90: 6f6e 6669 676f 626a 2e43 6f6e 6669 674f  onfigobj.ConfigO
-00007ba0: 626a 2866 2c0a 2020 2020 2020 2020 2020  bj(f,.          
-00007bb0: 2020 2020 2020 656e 636f 6469 6e67 3d27        encoding='
-00007bc0: 7574 662d 3827 2c20 6465 6661 756c 745f  utf-8', default_
-00007bd0: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-00007be0: 290a 0a20 2020 2020 2020 206e 616d 6564  )..        named
-00007bf0: 5f6d 6f63 6b20 3d20 6d6f 636b 2e4d 6f63  _mock = mock.Moc
-00007c00: 6b28 290a 2020 2020 2020 2020 6e61 6d65  k().        name
-00007c10: 645f 6d6f 636b 2e6e 616d 6520 3d20 276e  d_mock.name = 'n
-00007c20: 6769 6e78 270a 0a20 2020 2020 2020 2073  ginx'..        s
-00007c30: 656c 662e 6d6f 636b 735b 2770 6963 6b5f  elf.mocks['pick_
-00007c40: 6175 7468 275d 2e72 6574 7572 6e5f 7661  auth'].return_va
-00007c50: 6c75 6520 3d20 6e61 6d65 645f 6d6f 636b  lue = named_mock
-00007c60: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00007c70: 636b 735b 2766 696e 645f 696e 6974 275d  cks['find_init']
-00007c80: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-00007c90: 6e61 6d65 645f 6d6f 636b 0a0a 2020 2020  named_mock..    
-00007ca0: 2020 2020 6e65 775f 636f 6e66 6967 203d      new_config =
-00007cb0: 2073 656c 662e 5f63 616c 6c28 272d 2d63   self._call('--c
-00007cc0: 6572 742d 6e61 6d65 2065 7861 6d70 6c65  ert-name example
-00007cd0: 2e63 6f6d 202d 2d6e 6769 6e78 272e 7370  .com --nginx'.sp
-00007ce0: 6c69 7428 2929 0a20 2020 2020 2020 2061  lit()).        a
-00007cf0: 7373 6572 7420 6e65 775f 636f 6e66 6967  ssert new_config
-00007d00: 5b27 7265 6e65 7761 6c70 6172 616d 7327  ['renewalparams'
-00007d10: 5d5b 2761 7574 6865 6e74 6963 6174 6f72  ]['authenticator
-00007d20: 275d 203d 3d20 276e 6769 6e78 270a 2020  '] == 'nginx'.  
-00007d30: 2020 2020 2020 6d6f 636b 5f6e 6f74 6966        mock_notif
-00007d40: 792e 6173 7365 7274 5f63 616c 6c65 645f  y.assert_called_
-00007d50: 7769 7468 280a 2020 2020 2020 2020 2020  with(.          
-00007d60: 2020 275c 6e53 7563 6365 7373 6675 6c6c    '\nSuccessfull
-00007d70: 7920 7570 6461 7465 6420 636f 6e66 6967  y updated config
-00007d80: 7572 6174 696f 6e2e 272b 0a20 2020 2020  uration.'+.     
-00007d90: 2020 2020 2020 2027 5c6e 4368 616e 6765         '\nChange
-00007da0: 7320 7769 6c6c 2061 7070 6c79 2077 6865  s will apply whe
-00007db0: 6e20 7468 6520 6365 7274 6966 6963 6174  n the certificat
-00007dc0: 6520 7265 6e65 7773 2e27 290a 0a0a 636c  e renews.')...cl
-00007dd0: 6173 7320 4465 6c65 7465 4966 4170 7072  ass DeleteIfAppr
-00007de0: 6f70 7269 6174 6554 6573 7428 7465 7374  opriateTest(test
-00007df0: 5f75 7469 6c2e 436f 6e66 6967 5465 7374  _util.ConfigTest
-00007e00: 4361 7365 293a 0a20 2020 2022 2222 5465  Case):.    """Te
-00007e10: 7374 7320 666f 7220 6365 7274 626f 742e  sts for certbot.
-00007e20: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e5f  _internal.main._
-00007e30: 6465 6c65 7465 5f69 665f 6170 7072 6f70  delete_if_approp
-00007e40: 7269 6174 6520 2222 220a 0a20 2020 2064  riate """..    d
-00007e50: 6566 205f 6361 6c6c 2873 656c 662c 206d  ef _call(self, m
-00007e60: 6f63 6b5f 636f 6e66 6967 293a 0a20 2020  ock_config):.   
-00007e70: 2020 2020 2066 726f 6d20 6365 7274 626f       from certbo
-00007e80: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-00007e90: 2069 6d70 6f72 7420 5f64 656c 6574 655f   import _delete_
-00007ea0: 6966 5f61 7070 726f 7072 6961 7465 0a20  if_appropriate. 
-00007eb0: 2020 2020 2020 205f 6465 6c65 7465 5f69         _delete_i
-00007ec0: 665f 6170 7072 6f70 7269 6174 6528 6d6f  f_appropriate(mo
-00007ed0: 636b 5f63 6f6e 6669 6729 0a0a 2020 2020  ck_config)..    
-00007ee0: 6465 6620 5f74 6573 745f 6465 6c65 7465  def _test_delete
-00007ef0: 5f6f 7074 5f6f 7574 5f63 6f6d 6d6f 6e28  _opt_out_common(
-00007f00: 7365 6c66 293a 0a20 2020 2020 2020 2077  self):.        w
-00007f10: 6974 6820 6d6f 636b 2e70 6174 6368 2827  ith mock.patch('
-00007f20: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00007f30: 6c2e 6365 7274 5f6d 616e 6167 6572 2e64  l.cert_manager.d
-00007f40: 656c 6574 6527 2920 6173 206d 6f63 6b5f  elete') as mock_
-00007f50: 6465 6c65 7465 3a0a 2020 2020 2020 2020  delete:.        
-00007f60: 2020 2020 7365 6c66 2e5f 6361 6c6c 2873      self._call(s
-00007f70: 656c 662e 636f 6e66 6967 290a 2020 2020  elf.config).    
-00007f80: 2020 2020 6d6f 636b 5f64 656c 6574 652e      mock_delete.
-00007f90: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
-00007fa0: 6428 290a 0a20 2020 2040 7465 7374 5f75  d()..    @test_u
-00007fb0: 7469 6c2e 7061 7463 685f 6469 7370 6c61  til.patch_displa
-00007fc0: 795f 7574 696c 2829 0a20 2020 2064 6566  y_util().    def
-00007fd0: 2074 6573 745f 6465 6c65 7465 5f66 6c61   test_delete_fla
-00007fe0: 675f 6f70 745f 6f75 7428 7365 6c66 2c20  g_opt_out(self, 
-00007ff0: 756e 7573 6564 5f6d 6f63 6b5f 6765 745f  unused_mock_get_
-00008000: 7574 696c 6974 7929 3a0a 2020 2020 2020  utility):.      
-00008010: 2020 7365 6c66 2e63 6f6e 6669 672e 6465    self.config.de
-00008020: 6c65 7465 5f61 6674 6572 5f72 6576 6f6b  lete_after_revok
-00008030: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-00008040: 2020 7365 6c66 2e5f 7465 7374 5f64 656c    self._test_del
-00008050: 6574 655f 6f70 745f 6f75 745f 636f 6d6d  ete_opt_out_comm
-00008060: 6f6e 2829 0a0a 2020 2020 4074 6573 745f  on()..    @test_
-00008070: 7574 696c 2e70 6174 6368 5f64 6973 706c  util.patch_displ
-00008080: 6179 5f75 7469 6c28 290a 2020 2020 6465  ay_util().    de
-00008090: 6620 7465 7374 5f64 656c 6574 655f 7072  f test_delete_pr
-000080a0: 6f6d 7074 5f6f 7074 5f6f 7574 2873 656c  ompt_opt_out(sel
-000080b0: 662c 206d 6f63 6b5f 6765 745f 7574 696c  f, mock_get_util
-000080c0: 6974 7929 3a0a 2020 2020 2020 2020 7574  ity):.        ut
-000080d0: 696c 5f6d 6f63 6b20 3d20 6d6f 636b 5f67  il_mock = mock_g
-000080e0: 6574 5f75 7469 6c69 7479 2829 0a20 2020  et_utility().   
-000080f0: 2020 2020 2075 7469 6c5f 6d6f 636b 2e79       util_mock.y
-00008100: 6573 6e6f 2e72 6574 7572 6e5f 7661 6c75  esno.return_valu
-00008110: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-00008120: 2020 7365 6c66 2e5f 7465 7374 5f64 656c    self._test_del
-00008130: 6574 655f 6f70 745f 6f75 745f 636f 6d6d  ete_opt_out_comm
-00008140: 6f6e 2829 0a0a 2020 2020 406d 6f63 6b2e  on()..    @mock.
-00008150: 7061 7463 6828 2263 6572 7462 6f74 2e5f  patch("certbot._
-00008160: 696e 7465 726e 616c 2e6d 6169 6e2e 6c6f  internal.main.lo
-00008170: 6767 6572 2e77 6172 6e69 6e67 2229 0a20  gger.warning"). 
-00008180: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00008190: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-000081a0: 6c2e 7374 6f72 6167 652e 7265 6e65 7761  l.storage.renewa
-000081b0: 6c5f 6669 6c65 5f66 6f72 5f63 6572 746e  l_file_for_certn
-000081c0: 616d 6527 290a 2020 2020 406d 6f63 6b2e  ame').    @mock.
-000081d0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-000081e0: 696e 7465 726e 616c 2e63 6572 745f 6d61  internal.cert_ma
-000081f0: 6e61 6765 722e 6465 6c65 7465 2729 0a20  nager.delete'). 
-00008200: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00008210: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00008220: 6c2e 6365 7274 5f6d 616e 6167 6572 2e6d  l.cert_manager.m
-00008230: 6174 6368 5f61 6e64 5f63 6865 636b 5f6f  atch_and_check_o
-00008240: 7665 726c 6170 7327 290a 2020 2020 406d  verlaps').    @m
-00008250: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00008260: 6f74 2e5f 696e 7465 726e 616c 2e73 746f  ot._internal.sto
-00008270: 7261 6765 2e66 756c 6c5f 6172 6368 6976  rage.full_archiv
-00008280: 655f 7061 7468 2729 0a20 2020 2040 6d6f  e_path').    @mo
-00008290: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-000082a0: 742e 5f69 6e74 6572 6e61 6c2e 6365 7274  t._internal.cert
-000082b0: 5f6d 616e 6167 6572 2e63 6572 745f 7061  _manager.cert_pa
-000082c0: 7468 5f74 6f5f 6c69 6e65 6167 6527 290a  th_to_lineage').
-000082d0: 2020 2020 4074 6573 745f 7574 696c 2e70      @test_util.p
-000082e0: 6174 6368 5f64 6973 706c 6179 5f75 7469  atch_display_uti
-000082f0: 6c28 290a 2020 2020 6465 6620 7465 7374  l().    def test
-00008300: 5f6f 7665 726c 6170 7069 6e67 5f61 7263  _overlapping_arc
-00008310: 6869 7665 5f64 6972 7328 7365 6c66 2c20  hive_dirs(self, 
-00008320: 6d6f 636b 5f67 6574 5f75 7469 6c69 7479  mock_get_utility
-00008330: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
-00008340: 636b 5f63 6572 745f 7061 7468 5f74 6f5f  ck_cert_path_to_
-00008350: 6c69 6e65 6167 652c 206d 6f63 6b5f 6172  lineage, mock_ar
-00008360: 6368 6976 652c 0a20 2020 2020 2020 2020  chive,.         
-00008370: 2020 206d 6f63 6b5f 6d61 7463 685f 616e     mock_match_an
-00008380: 645f 6368 6563 6b5f 6f76 6572 6c61 7073  d_check_overlaps
-00008390: 2c20 6d6f 636b 5f64 656c 6574 652c 0a20  , mock_delete,. 
-000083a0: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-000083b0: 7265 6e65 7761 6c5f 6669 6c65 5f66 6f72  renewal_file_for
-000083c0: 5f63 6572 746e 616d 652c 206d 6f63 6b5f  _certname, mock_
-000083d0: 7761 726e 696e 6729 3a0a 2020 2020 2020  warning):.      
-000083e0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
-000083f0: 626c 6520 3d20 756e 7573 6564 2d61 7267  ble = unused-arg
-00008400: 756d 656e 740a 2020 2020 2020 2020 636f  ument.        co
-00008410: 6e66 6967 203d 2073 656c 662e 636f 6e66  nfig = self.conf
-00008420: 6967 0a20 2020 2020 2020 2063 6f6e 6669  ig.        confi
-00008430: 672e 6365 7274 5f70 6174 6820 3d20 222f  g.cert_path = "/
-00008440: 736f 6d65 2f72 6561 736f 6e61 626c 652f  some/reasonable/
-00008450: 7061 7468 220a 2020 2020 2020 2020 636f  path".        co
-00008460: 6e66 6967 2e63 6572 746e 616d 6520 3d20  nfig.certname = 
-00008470: 2222 0a20 2020 2020 2020 206d 6f63 6b5f  "".        mock_
-00008480: 6365 7274 5f70 6174 685f 746f 5f6c 696e  cert_path_to_lin
-00008490: 6561 6765 2e72 6574 7572 6e5f 7661 6c75  eage.return_valu
-000084a0: 6520 3d20 2265 7861 6d70 6c65 2e63 6f6d  e = "example.com
-000084b0: 220a 2020 2020 2020 2020 6d6f 636b 5f6d  ".        mock_m
-000084c0: 6174 6368 5f61 6e64 5f63 6865 636b 5f6f  atch_and_check_o
-000084d0: 7665 726c 6170 732e 7369 6465 5f65 6666  verlaps.side_eff
-000084e0: 6563 7420 3d20 6572 726f 7273 2e4f 7665  ect = errors.Ove
-000084f0: 726c 6170 7069 6e67 4d61 7463 6846 6f75  rlappingMatchFou
-00008500: 6e64 2829 0a20 2020 2020 2020 2073 656c  nd().        sel
-00008510: 662e 5f63 616c 6c28 636f 6e66 6967 290a  f._call(config).
-00008520: 2020 2020 2020 2020 6d6f 636b 5f64 656c          mock_del
-00008530: 6574 652e 6173 7365 7274 5f6e 6f74 5f63  ete.assert_not_c
-00008540: 616c 6c65 6428 290a 2020 2020 2020 2020  alled().        
-00008550: 6173 7365 7274 206d 6f63 6b5f 7761 726e  assert mock_warn
-00008560: 696e 672e 6361 6c6c 5f63 6f75 6e74 203d  ing.call_count =
-00008570: 3d20 310a 0a20 2020 2040 6d6f 636b 2e70  = 1..    @mock.p
-00008580: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00008590: 6e74 6572 6e61 6c2e 7374 6f72 6167 652e  nternal.storage.
-000085a0: 7265 6e65 7761 6c5f 6669 6c65 5f66 6f72  renewal_file_for
-000085b0: 5f63 6572 746e 616d 6527 290a 2020 2020  _certname').    
-000085c0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-000085d0: 7462 6f74 2e5f 696e 7465 726e 616c 2e63  tbot._internal.c
-000085e0: 6572 745f 6d61 6e61 6765 722e 6d61 7463  ert_manager.matc
-000085f0: 685f 616e 645f 6368 6563 6b5f 6f76 6572  h_and_check_over
-00008600: 6c61 7073 2729 0a20 2020 2040 6d6f 636b  laps').    @mock
-00008610: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-00008620: 5f69 6e74 6572 6e61 6c2e 7374 6f72 6167  _internal.storag
-00008630: 652e 6675 6c6c 5f61 7263 6869 7665 5f70  e.full_archive_p
-00008640: 6174 6827 290a 2020 2020 406d 6f63 6b2e  ath').    @mock.
-00008650: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-00008660: 696e 7465 726e 616c 2e63 6572 745f 6d61  internal.cert_ma
-00008670: 6e61 6765 722e 6465 6c65 7465 2729 0a20  nager.delete'). 
-00008680: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00008690: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-000086a0: 6c2e 6365 7274 5f6d 616e 6167 6572 2e63  l.cert_manager.c
-000086b0: 6572 745f 7061 7468 5f74 6f5f 6c69 6e65  ert_path_to_line
-000086c0: 6167 6527 290a 2020 2020 4074 6573 745f  age').    @test_
-000086d0: 7574 696c 2e70 6174 6368 5f64 6973 706c  util.patch_displ
-000086e0: 6179 5f75 7469 6c28 290a 2020 2020 6465  ay_util().    de
-000086f0: 6620 7465 7374 5f63 6572 745f 7061 7468  f test_cert_path
-00008700: 5f6f 6e6c 7928 7365 6c66 2c20 6d6f 636b  _only(self, mock
-00008710: 5f67 6574 5f75 7469 6c69 7479 2c0a 2020  _get_utility,.  
-00008720: 2020 2020 2020 2020 2020 6d6f 636b 5f63            mock_c
-00008730: 6572 745f 7061 7468 5f74 6f5f 6c69 6e65  ert_path_to_line
-00008740: 6167 652c 206d 6f63 6b5f 6465 6c65 7465  age, mock_delete
-00008750: 2c20 6d6f 636b 5f61 7263 6869 7665 2c0a  , mock_archive,.
-00008760: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-00008770: 5f6f 7665 726c 6170 7069 6e67 5f61 7263  _overlapping_arc
-00008780: 6869 7665 5f64 6972 732c 206d 6f63 6b5f  hive_dirs, mock_
-00008790: 7265 6e65 7761 6c5f 6669 6c65 5f66 6f72  renewal_file_for
-000087a0: 5f63 6572 746e 616d 6529 3a0a 2020 2020  _certname):.    
-000087b0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-000087c0: 7361 626c 6520 3d20 756e 7573 6564 2d61  sable = unused-a
-000087d0: 7267 756d 656e 740a 2020 2020 2020 2020  rgument.        
-000087e0: 636f 6e66 6967 203d 2073 656c 662e 636f  config = self.co
-000087f0: 6e66 6967 0a20 2020 2020 2020 2063 6f6e  nfig.        con
-00008800: 6669 672e 6365 7274 5f70 6174 6820 3d20  fig.cert_path = 
-00008810: 222f 736f 6d65 2f72 6561 736f 6e61 626c  "/some/reasonabl
-00008820: 652f 7061 7468 220a 2020 2020 2020 2020  e/path".        
-00008830: 636f 6e66 6967 2e63 6572 746e 616d 6520  config.certname 
-00008840: 3d20 2222 0a20 2020 2020 2020 206d 6f63  = "".        moc
-00008850: 6b5f 6365 7274 5f70 6174 685f 746f 5f6c  k_cert_path_to_l
-00008860: 696e 6561 6765 2e72 6574 7572 6e5f 7661  ineage.return_va
-00008870: 6c75 6520 3d20 2265 7861 6d70 6c65 2e63  lue = "example.c
-00008880: 6f6d 220a 2020 2020 2020 2020 6d6f 636b  om".        mock
-00008890: 5f6f 7665 726c 6170 7069 6e67 5f61 7263  _overlapping_arc
-000088a0: 6869 7665 5f64 6972 732e 7265 7475 726e  hive_dirs.return
-000088b0: 5f76 616c 7565 203d 2046 616c 7365 0a20  _value = False. 
-000088c0: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-000088d0: 6c28 636f 6e66 6967 290a 2020 2020 2020  l(config).      
-000088e0: 2020 6173 7365 7274 206d 6f63 6b5f 6465    assert mock_de
-000088f0: 6c65 7465 2e63 616c 6c5f 636f 756e 7420  lete.call_count 
-00008900: 3d3d 2031 0a0a 2020 2020 406d 6f63 6b2e  == 1..    @mock.
-00008910: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-00008920: 696e 7465 726e 616c 2e73 746f 7261 6765  internal.storage
-00008930: 2e72 656e 6577 616c 5f66 696c 655f 666f  .renewal_file_fo
-00008940: 725f 6365 7274 6e61 6d65 2729 0a20 2020  r_certname').   
-00008950: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-00008960: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00008970: 6365 7274 5f6d 616e 6167 6572 2e6d 6174  cert_manager.mat
-00008980: 6368 5f61 6e64 5f63 6865 636b 5f6f 7665  ch_and_check_ove
-00008990: 726c 6170 7327 290a 2020 2020 406d 6f63  rlaps').    @moc
-000089a0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-000089b0: 2e5f 696e 7465 726e 616c 2e73 746f 7261  ._internal.stora
-000089c0: 6765 2e66 756c 6c5f 6172 6368 6976 655f  ge.full_archive_
-000089d0: 7061 7468 2729 0a20 2020 2040 6d6f 636b  path').    @mock
-000089e0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-000089f0: 5f69 6e74 6572 6e61 6c2e 6365 7274 5f6d  _internal.cert_m
-00008a00: 616e 6167 6572 2e63 6572 745f 7061 7468  anager.cert_path
-00008a10: 5f74 6f5f 6c69 6e65 6167 6527 290a 2020  _to_lineage').  
-00008a20: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-00008a30: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00008a40: 2e63 6572 745f 6d61 6e61 6765 722e 6465  .cert_manager.de
-00008a50: 6c65 7465 2729 0a20 2020 2040 7465 7374  lete').    @test
-00008a60: 5f75 7469 6c2e 7061 7463 685f 6469 7370  _util.patch_disp
-00008a70: 6c61 795f 7574 696c 2829 0a20 2020 2064  lay_util().    d
-00008a80: 6566 2074 6573 745f 6e6f 6e69 6e74 6572  ef test_noninter
-00008a90: 6163 7469 7665 5f64 656c 6574 696f 6e28  active_deletion(
-00008aa0: 7365 6c66 2c20 6d6f 636b 5f67 6574 5f75  self, mock_get_u
-00008ab0: 7469 6c69 7479 2c20 6d6f 636b 5f64 656c  tility, mock_del
-00008ac0: 6574 652c 0a20 2020 2020 2020 2020 2020  ete,.           
-00008ad0: 206d 6f63 6b5f 6365 7274 5f70 6174 685f   mock_cert_path_
-00008ae0: 746f 5f6c 696e 6561 6765 2c20 6d6f 636b  to_lineage, mock
-00008af0: 5f66 756c 6c5f 6172 6368 6976 655f 6469  _full_archive_di
-00008b00: 722c 0a20 2020 2020 2020 2020 2020 206d  r,.            m
-00008b10: 6f63 6b5f 6d61 7463 685f 616e 645f 6368  ock_match_and_ch
-00008b20: 6563 6b5f 6f76 6572 6c61 7073 2c20 6d6f  eck_overlaps, mo
-00008b30: 636b 5f72 656e 6577 616c 5f66 696c 655f  ck_renewal_file_
-00008b40: 666f 725f 6365 7274 6e61 6d65 293a 0a20  for_certname):. 
-00008b50: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
-00008b60: 2064 6973 6162 6c65 203d 2075 6e75 7365   disable = unuse
-00008b70: 642d 6172 6775 6d65 6e74 0a20 2020 2020  d-argument.     
-00008b80: 2020 2063 6f6e 6669 6720 3d20 7365 6c66     config = self
-00008b90: 2e63 6f6e 6669 670a 2020 2020 2020 2020  .config.        
-00008ba0: 636f 6e66 6967 2e6e 6f6e 696e 7465 7261  config.nonintera
-00008bb0: 6374 6976 655f 6d6f 6465 203d 2054 7275  ctive_mode = Tru
-00008bc0: 650a 2020 2020 2020 2020 636f 6e66 6967  e.        config
-00008bd0: 2e63 6572 745f 7061 7468 203d 2022 2f73  .cert_path = "/s
-00008be0: 6f6d 652f 7265 6173 6f6e 6162 6c65 2f70  ome/reasonable/p
-00008bf0: 6174 6822 0a20 2020 2020 2020 2063 6f6e  ath".        con
-00008c00: 6669 672e 6365 7274 6e61 6d65 203d 2022  fig.certname = "
-00008c10: 220a 2020 2020 2020 2020 6d6f 636b 5f63  ".        mock_c
-00008c20: 6572 745f 7061 7468 5f74 6f5f 6c69 6e65  ert_path_to_line
-00008c30: 6167 652e 7265 7475 726e 5f76 616c 7565  age.return_value
-00008c40: 203d 2022 6578 616d 706c 652e 636f 6d22   = "example.com"
-00008c50: 0a20 2020 2020 2020 206d 6f63 6b5f 6675  .        mock_fu
-00008c60: 6c6c 5f61 7263 6869 7665 5f64 6972 2e72  ll_archive_dir.r
-00008c70: 6574 7572 6e5f 7661 6c75 6520 3d20 2222  eturn_value = ""
-00008c80: 0a20 2020 2020 2020 206d 6f63 6b5f 6d61  .        mock_ma
-00008c90: 7463 685f 616e 645f 6368 6563 6b5f 6f76  tch_and_check_ov
-00008ca0: 6572 6c61 7073 2e72 6574 7572 6e5f 7661  erlaps.return_va
-00008cb0: 6c75 6520 3d20 2222 0a20 2020 2020 2020  lue = "".       
-00008cc0: 2073 656c 662e 5f63 616c 6c28 636f 6e66   self._call(conf
-00008cd0: 6967 290a 2020 2020 2020 2020 6173 7365  ig).        asse
-00008ce0: 7274 206d 6f63 6b5f 6465 6c65 7465 2e63  rt mock_delete.c
-00008cf0: 616c 6c5f 636f 756e 7420 3d3d 2031 0a0a  all_count == 1..
-00008d00: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-00008d10: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00008d20: 616c 2e73 746f 7261 6765 2e72 656e 6577  al.storage.renew
-00008d30: 616c 5f66 696c 655f 666f 725f 6365 7274  al_file_for_cert
-00008d40: 6e61 6d65 2729 0a20 2020 2040 6d6f 636b  name').    @mock
-00008d50: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-00008d60: 5f69 6e74 6572 6e61 6c2e 6365 7274 5f6d  _internal.cert_m
-00008d70: 616e 6167 6572 2e6d 6174 6368 5f61 6e64  anager.match_and
-00008d80: 5f63 6865 636b 5f6f 7665 726c 6170 7327  _check_overlaps'
-00008d90: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-00008da0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00008db0: 726e 616c 2e73 746f 7261 6765 2e66 756c  rnal.storage.ful
-00008dc0: 6c5f 6172 6368 6976 655f 7061 7468 2729  l_archive_path')
-00008dd0: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-00008de0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00008df0: 6e61 6c2e 6365 7274 5f6d 616e 6167 6572  nal.cert_manager
-00008e00: 2e63 6572 745f 7061 7468 5f74 6f5f 6c69  .cert_path_to_li
-00008e10: 6e65 6167 6527 290a 2020 2020 406d 6f63  neage').    @moc
-00008e20: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-00008e30: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
-00008e40: 6d61 6e61 6765 722e 6465 6c65 7465 2729  manager.delete')
-00008e50: 0a20 2020 2040 7465 7374 5f75 7469 6c2e  .    @test_util.
-00008e60: 7061 7463 685f 6469 7370 6c61 795f 7574  patch_display_ut
-00008e70: 696c 2829 0a20 2020 2064 6566 2074 6573  il().    def tes
-00008e80: 745f 6f70 745f 696e 5f64 656c 6574 696f  t_opt_in_deletio
-00008e90: 6e28 7365 6c66 2c20 6d6f 636b 5f67 6574  n(self, mock_get
-00008ea0: 5f75 7469 6c69 7479 2c20 6d6f 636b 5f64  _utility, mock_d
-00008eb0: 656c 6574 652c 0a20 2020 2020 2020 2020  elete,.         
-00008ec0: 2020 206d 6f63 6b5f 6365 7274 5f70 6174     mock_cert_pat
-00008ed0: 685f 746f 5f6c 696e 6561 6765 2c20 6d6f  h_to_lineage, mo
-00008ee0: 636b 5f66 756c 6c5f 6172 6368 6976 655f  ck_full_archive_
-00008ef0: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
-00008f00: 206d 6f63 6b5f 6d61 7463 685f 616e 645f   mock_match_and_
-00008f10: 6368 6563 6b5f 6f76 6572 6c61 7073 2c20  check_overlaps, 
-00008f20: 6d6f 636b 5f72 656e 6577 616c 5f66 696c  mock_renewal_fil
-00008f30: 655f 666f 725f 6365 7274 6e61 6d65 293a  e_for_certname):
-00008f40: 0a20 2020 2020 2020 2063 6f6e 6669 6720  .        config 
-00008f50: 3d20 7365 6c66 2e63 6f6e 6669 670a 2020  = self.config.  
-00008f60: 2020 2020 2020 636f 6e66 6967 2e64 656c        config.del
-00008f70: 6574 655f 6166 7465 725f 7265 766f 6b65  ete_after_revoke
-00008f80: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00008f90: 636f 6e66 6967 2e63 6572 745f 7061 7468  config.cert_path
-00008fa0: 203d 2022 2f73 6f6d 652f 7265 6173 6f6e   = "/some/reason
-00008fb0: 6162 6c65 2f70 6174 6822 0a20 2020 2020  able/path".     
-00008fc0: 2020 2063 6f6e 6669 672e 6365 7274 6e61     config.certna
-00008fd0: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
-00008fe0: 6d6f 636b 5f63 6572 745f 7061 7468 5f74  mock_cert_path_t
-00008ff0: 6f5f 6c69 6e65 6167 652e 7265 7475 726e  o_lineage.return
-00009000: 5f76 616c 7565 203d 2022 6578 616d 706c  _value = "exampl
-00009010: 652e 636f 6d22 0a20 2020 2020 2020 206d  e.com".        m
-00009020: 6f63 6b5f 6675 6c6c 5f61 7263 6869 7665  ock_full_archive
-00009030: 5f64 6972 2e72 6574 7572 6e5f 7661 6c75  _dir.return_valu
-00009040: 6520 3d20 2222 0a20 2020 2020 2020 206d  e = "".        m
-00009050: 6f63 6b5f 6d61 7463 685f 616e 645f 6368  ock_match_and_ch
-00009060: 6563 6b5f 6f76 6572 6c61 7073 2e72 6574  eck_overlaps.ret
-00009070: 7572 6e5f 7661 6c75 6520 3d20 2222 0a20  urn_value = "". 
-00009080: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-00009090: 6c28 636f 6e66 6967 290a 2020 2020 2020  l(config).      
-000090a0: 2020 6173 7365 7274 206d 6f63 6b5f 6465    assert mock_de
-000090b0: 6c65 7465 2e63 616c 6c5f 636f 756e 7420  lete.call_count 
-000090c0: 3d3d 2031 0a20 2020 2020 2020 2061 7373  == 1.        ass
-000090d0: 6572 7420 6e6f 7420 6d6f 636b 5f67 6574  ert not mock_get
-000090e0: 5f75 7469 6c69 7479 2829 2e79 6573 6e6f  _utility().yesno
-000090f0: 2e63 616c 6c65 640a 0a0a 636c 6173 7320  .called...class 
-00009100: 4465 7465 726d 696e 6541 6363 6f75 6e74  DetermineAccount
-00009110: 5465 7374 2874 6573 745f 7574 696c 2e43  Test(test_util.C
-00009120: 6f6e 6669 6754 6573 7443 6173 6529 3a0a  onfigTestCase):.
-00009130: 2020 2020 2222 2254 6573 7473 2066 6f72      """Tests for
-00009140: 2063 6572 7462 6f74 2e5f 696e 7465 726e   certbot._intern
-00009150: 616c 2e6d 6169 6e2e 5f64 6574 6572 6d69  al.main._determi
-00009160: 6e65 5f61 6363 6f75 6e74 2e22 2222 0a0a  ne_account."""..
-00009170: 2020 2020 6465 6620 7365 7455 7028 7365      def setUp(se
-00009180: 6c66 293a 0a20 2020 2020 2020 2073 7570  lf):.        sup
-00009190: 6572 2829 2e73 6574 5570 2829 0a20 2020  er().setUp().   
-000091a0: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-000091b0: 2e61 6363 6f75 6e74 203d 204e 6f6e 650a  .account = None.
-000091c0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000091d0: 6669 672e 656d 6169 6c20 3d20 4e6f 6e65  fig.email = None
-000091e0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-000091f0: 6e66 6967 2e72 6567 6973 7465 725f 756e  nfig.register_un
-00009200: 7361 6665 6c79 5f77 6974 686f 7574 5f65  safely_without_e
-00009210: 6d61 696c 203d 2046 616c 7365 0a20 2020  mail = False.   
-00009220: 2020 2020 2073 656c 662e 6163 6373 203d       self.accs =
-00009230: 205b 6d6f 636b 2e4d 6167 6963 4d6f 636b   [mock.MagicMock
-00009240: 2869 643d 2778 2729 2c20 6d6f 636b 2e4d  (id='x'), mock.M
-00009250: 6167 6963 4d6f 636b 2869 643d 2779 2729  agicMock(id='y')
-00009260: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
-00009270: 6363 6f75 6e74 5f73 746f 7261 6765 203d  ccount_storage =
-00009280: 2061 6363 6f75 6e74 2e41 6363 6f75 6e74   account.Account
-00009290: 4d65 6d6f 7279 5374 6f72 6167 6528 290a  MemoryStorage().
-000092a0: 2020 2020 2020 2020 2320 466f 7220 7573          # For us
-000092b0: 6520 696e 2073 6176 696e 6720 6163 636f  e in saving acco
-000092c0: 756e 7473 3a20 6661 6b65 206f 7574 2074  unts: fake out t
-000092d0: 6865 206e 6577 5f61 7574 687a 2055 524c  he new_authz URL
-000092e0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000092f0: 6f63 6b5f 636c 6965 6e74 203d 206d 6f63  ock_client = moc
-00009300: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
-00009310: 2020 2020 2020 7365 6c66 2e6d 6f63 6b5f        self.mock_
-00009320: 636c 6965 6e74 2e64 6972 6563 746f 7279  client.directory
-00009330: 2e6e 6577 5f61 7574 687a 203d 2022 6869  .new_authz = "hi
-00009340: 220a 0a0a 2020 2020 6465 6620 5f63 616c  "...    def _cal
-00009350: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-00009360: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00009370: 6c65 3d70 726f 7465 6374 6564 2d61 6363  le=protected-acc
-00009380: 6573 730a 2020 2020 2020 2020 6672 6f6d  ess.        from
-00009390: 2063 6572 7462 6f74 2e5f 696e 7465 726e   certbot._intern
-000093a0: 616c 2e6d 6169 6e20 696d 706f 7274 205f  al.main import _
-000093b0: 6465 7465 726d 696e 655f 6163 636f 756e  determine_accoun
-000093c0: 740a 2020 2020 2020 2020 7769 7468 206d  t.        with m
-000093d0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-000093e0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-000093f0: 6e2e 6163 636f 756e 742e 4163 636f 756e  n.account.Accoun
-00009400: 7446 696c 6553 746f 7261 6765 2729 2061  tFileStorage') a
-00009410: 7320 6d6f 636b 5f73 746f 7261 6765 2c20  s mock_storage, 
-00009420: 5c0a 2020 2020 2020 2020 2020 2020 2074  \.             t
-00009430: 6573 745f 7574 696c 2e70 6174 6368 5f64  est_util.patch_d
-00009440: 6973 706c 6179 5f75 7469 6c28 293a 0a20  isplay_util():. 
-00009450: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-00009460: 7374 6f72 6167 652e 7265 7475 726e 5f76  storage.return_v
-00009470: 616c 7565 203d 2073 656c 662e 6163 636f  alue = self.acco
-00009480: 756e 745f 7374 6f72 6167 650a 2020 2020  unt_storage.    
-00009490: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000094a0: 6465 7465 726d 696e 655f 6163 636f 756e  determine_accoun
-000094b0: 7428 7365 6c66 2e63 6f6e 6669 6729 0a0a  t(self.config)..
-000094c0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-000094d0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-000094e0: 616c 2e63 6c69 656e 742e 7265 6769 7374  al.client.regist
-000094f0: 6572 2729 0a20 2020 2040 6d6f 636b 2e70  er').    @mock.p
-00009500: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00009510: 6e74 6572 6e61 6c2e 636c 6965 6e74 2e64  nternal.client.d
-00009520: 6973 706c 6179 5f6f 7073 2e67 6574 5f65  isplay_ops.get_e
-00009530: 6d61 696c 2729 0a20 2020 2064 6566 205f  mail').    def _
-00009540: 7265 6769 7374 6572 5f65 7272 6f72 5f63  register_error_c
-00009550: 6f6d 6d6f 6e28 7365 6c66 2c20 6572 725f  ommon(self, err_
-00009560: 6d73 672c 2065 7863 6570 7469 6f6e 2c20  msg, exception, 
-00009570: 6d6f 636b 5f67 6574 5f65 6d61 696c 2c20  mock_get_email, 
-00009580: 6d6f 636b 5f72 6567 6973 7465 7229 3a0a  mock_register):.
-00009590: 2020 2020 2020 2020 6d6f 636b 5f67 6574          mock_get
-000095a0: 5f65 6d61 696c 2e72 6574 7572 6e5f 7661  _email.return_va
-000095b0: 6c75 6520 3d20 2766 6f6f 4062 6172 2e62  lue = 'foo@bar.b
-000095c0: 617a 270a 2020 2020 2020 2020 6d6f 636b  az'.        mock
-000095d0: 5f72 6567 6973 7465 722e 7369 6465 5f65  _register.side_e
-000095e0: 6666 6563 7420 3d20 6578 6365 7074 696f  ffect = exceptio
-000095f0: 6e0a 2020 2020 2020 2020 7472 793a 0a20  n.        try:. 
-00009600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009610: 5f63 616c 6c28 290a 2020 2020 2020 2020  _call().        
-00009620: 6578 6365 7074 2065 7272 6f72 732e 4572  except errors.Er
-00009630: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-00009640: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
-00009650: 2255 6e61 626c 6520 746f 2072 6567 6973  "Unable to regis
-00009660: 7465 7220 616e 2061 6363 6f75 6e74 2077  ter an account w
-00009670: 6974 6820 4143 4d45 2073 6572 7665 722e  ith ACME server.
-00009680: 207b 6572 725f 6d73 677d 2220 3d3d 205c   {err_msg}" == \
-00009690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096a0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-000096b0: 7228 6572 7229 0a0a 2020 2020 6465 6620  r(err)..    def 
-000096c0: 7465 7374 5f61 7267 735f 6163 636f 756e  test_args_accoun
-000096d0: 745f 7365 7428 7365 6c66 293a 0a20 2020  t_set(self):.   
-000096e0: 2020 2020 2073 656c 662e 6163 636f 756e       self.accoun
-000096f0: 745f 7374 6f72 6167 652e 7361 7665 2873  t_storage.save(s
-00009700: 656c 662e 6163 6373 5b31 5d2c 2073 656c  elf.accs[1], sel
-00009710: 662e 6d6f 636b 5f63 6c69 656e 7429 0a20  f.mock_client). 
-00009720: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-00009730: 6967 2e61 6363 6f75 6e74 203d 2073 656c  ig.account = sel
-00009740: 662e 6163 6373 5b31 5d2e 6964 0a20 2020  f.accs[1].id.   
-00009750: 2020 2020 2061 7373 6572 7420 2873 656c       assert (sel
-00009760: 662e 6163 6373 5b31 5d2c 204e 6f6e 6529  f.accs[1], None)
-00009770: 203d 3d20 7365 6c66 2e5f 6361 6c6c 2829   == self._call()
-00009780: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00009790: 7365 6c66 2e61 6363 735b 315d 2e69 6420  self.accs[1].id 
-000097a0: 3d3d 2073 656c 662e 636f 6e66 6967 2e61  == self.config.a
-000097b0: 6363 6f75 6e74 0a20 2020 2020 2020 2061  ccount.        a
-000097c0: 7373 6572 7420 7365 6c66 2e63 6f6e 6669  ssert self.confi
-000097d0: 672e 656d 6169 6c20 6973 204e 6f6e 650a  g.email is None.
-000097e0: 0a20 2020 2064 6566 2074 6573 745f 7369  .    def test_si
-000097f0: 6e67 6c65 5f61 6363 6f75 6e74 2873 656c  ngle_account(sel
-00009800: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00009810: 2e61 6363 6f75 6e74 5f73 746f 7261 6765  .account_storage
-00009820: 2e73 6176 6528 7365 6c66 2e61 6363 735b  .save(self.accs[
-00009830: 305d 2c20 7365 6c66 2e6d 6f63 6b5f 636c  0], self.mock_cl
-00009840: 6965 6e74 290a 2020 2020 2020 2020 6173  ient).        as
-00009850: 7365 7274 2028 7365 6c66 2e61 6363 735b  sert (self.accs[
-00009860: 305d 2c20 4e6f 6e65 2920 3d3d 2073 656c  0], None) == sel
-00009870: 662e 5f63 616c 6c28 290a 2020 2020 2020  f._call().      
-00009880: 2020 6173 7365 7274 2073 656c 662e 6163    assert self.ac
-00009890: 6373 5b30 5d2e 6964 203d 3d20 7365 6c66  cs[0].id == self
-000098a0: 2e63 6f6e 6669 672e 6163 636f 756e 740a  .config.account.
-000098b0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-000098c0: 656c 662e 636f 6e66 6967 2e65 6d61 696c  elf.config.email
-000098d0: 2069 7320 4e6f 6e65 0a0a 2020 2020 406d   is None..    @m
-000098e0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-000098f0: 6f74 2e5f 696e 7465 726e 616c 2e63 6c69  ot._internal.cli
-00009900: 656e 742e 6469 7370 6c61 795f 6f70 732e  ent.display_ops.
-00009910: 6368 6f6f 7365 5f61 6363 6f75 6e74 2729  choose_account')
-00009920: 0a20 2020 2064 6566 2074 6573 745f 6d75  .    def test_mu
-00009930: 6c74 6970 6c65 5f61 6363 6f75 6e74 7328  ltiple_accounts(
-00009940: 7365 6c66 2c20 6d6f 636b 5f63 686f 6f73  self, mock_choos
-00009950: 655f 6163 636f 756e 7473 293a 0a20 2020  e_accounts):.   
-00009960: 2020 2020 2066 6f72 2061 6363 2069 6e20       for acc in 
-00009970: 7365 6c66 2e61 6363 733a 0a20 2020 2020  self.accs:.     
-00009980: 2020 2020 2020 2073 656c 662e 6163 636f         self.acco
-00009990: 756e 745f 7374 6f72 6167 652e 7361 7665  unt_storage.save
-000099a0: 2861 6363 2c20 7365 6c66 2e6d 6f63 6b5f  (acc, self.mock_
-000099b0: 636c 6965 6e74 290a 2020 2020 2020 2020  client).        
-000099c0: 6d6f 636b 5f63 686f 6f73 655f 6163 636f  mock_choose_acco
-000099d0: 756e 7473 2e72 6574 7572 6e5f 7661 6c75  unts.return_valu
-000099e0: 6520 3d20 7365 6c66 2e61 6363 735b 315d  e = self.accs[1]
-000099f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00009a00: 2873 656c 662e 6163 6373 5b31 5d2c 204e  (self.accs[1], N
-00009a10: 6f6e 6529 203d 3d20 7365 6c66 2e5f 6361  one) == self._ca
-00009a20: 6c6c 2829 0a20 2020 2020 2020 2061 7373  ll().        ass
-00009a30: 6572 7420 7365 7428 6d6f 636b 5f63 686f  ert set(mock_cho
-00009a40: 6f73 655f 6163 636f 756e 7473 2e63 616c  ose_accounts.cal
-00009a50: 6c5f 6172 6773 5b30 5d5b 305d 2920 3d3d  l_args[0][0]) ==
-00009a60: 2073 6574 2873 656c 662e 6163 6373 290a   set(self.accs).
-00009a70: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00009a80: 656c 662e 6163 6373 5b31 5d2e 6964 203d  elf.accs[1].id =
-00009a90: 3d20 7365 6c66 2e63 6f6e 6669 672e 6163  = self.config.ac
-00009aa0: 636f 756e 740a 2020 2020 2020 2020 6173  count.        as
-00009ab0: 7365 7274 2073 656c 662e 636f 6e66 6967  sert self.config
-00009ac0: 2e65 6d61 696c 2069 7320 4e6f 6e65 0a0a  .email is None..
-00009ad0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-00009ae0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00009af0: 616c 2e63 6c69 656e 742e 6469 7370 6c61  al.client.displa
-00009b00: 795f 6f70 732e 6368 6f6f 7365 5f61 6363  y_ops.choose_acc
-00009b10: 6f75 6e74 2729 0a20 2020 2064 6566 2074  ount').    def t
-00009b20: 6573 745f 6d75 6c74 6970 6c65 5f61 6363  est_multiple_acc
-00009b30: 6f75 6e74 735f 6361 6e63 656c 6564 2873  ounts_canceled(s
-00009b40: 656c 662c 206d 6f63 6b5f 6368 6f6f 7365  elf, mock_choose
-00009b50: 5f61 6363 6f75 6e74 7329 3a0a 2020 2020  _accounts):.    
-00009b60: 2020 2020 666f 7220 6163 6320 696e 2073      for acc in s
-00009b70: 656c 662e 6163 6373 3a0a 2020 2020 2020  elf.accs:.      
-00009b80: 2020 2020 2020 7365 6c66 2e61 6363 6f75        self.accou
-00009b90: 6e74 5f73 746f 7261 6765 2e73 6176 6528  nt_storage.save(
-00009ba0: 6163 632c 2073 656c 662e 6d6f 636b 5f63  acc, self.mock_c
-00009bb0: 6c69 656e 7429 0a20 2020 2020 2020 206d  lient).        m
-00009bc0: 6f63 6b5f 6368 6f6f 7365 5f61 6363 6f75  ock_choose_accou
-00009bd0: 6e74 732e 7265 7475 726e 5f76 616c 7565  nts.return_value
-00009be0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00009bf0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00009c00: 2073 656c 662e 5f63 616c 6c28 290a 2020   self._call().  
-00009c10: 2020 2020 2020 6578 6365 7074 2065 7272        except err
-00009c20: 6f72 732e 4572 726f 7220 6173 2065 7272  ors.Error as err
-00009c30: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-00009c40: 7365 7274 2022 4e6f 2061 6363 6f75 6e74  sert "No account
-00009c50: 2068 6173 2062 6565 6e20 6368 6f73 656e   has been chosen
-00009c60: 2220 696e 2073 7472 2865 7272 290a 0a20  " in str(err).. 
-00009c70: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00009c80: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00009c90: 6c2e 636c 6965 6e74 2e64 6973 706c 6179  l.client.display
-00009ca0: 5f6f 7073 2e67 6574 5f65 6d61 696c 2729  _ops.get_email')
-00009cb0: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-00009cc0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00009cd0: 6e61 6c2e 6d61 696e 2e64 6973 706c 6179  nal.main.display
-00009ce0: 5f75 7469 6c2e 6e6f 7469 6679 2729 0a20  _util.notify'). 
-00009cf0: 2020 2064 6566 2074 6573 745f 6e6f 5f61     def test_no_a
-00009d00: 6363 6f75 6e74 735f 6e6f 5f65 6d61 696c  ccounts_no_email
-00009d10: 2873 656c 662c 206d 6f63 6b5f 6e6f 7469  (self, mock_noti
-00009d20: 6679 2c20 6d6f 636b 5f67 6574 5f65 6d61  fy, mock_get_ema
-00009d30: 696c 293a 0a20 2020 2020 2020 206d 6f63  il):.        moc
-00009d40: 6b5f 6765 745f 656d 6169 6c2e 7265 7475  k_get_email.retu
-00009d50: 726e 5f76 616c 7565 203d 2027 666f 6f40  rn_value = 'foo@
-00009d60: 6261 722e 6261 7a27 0a0a 2020 2020 2020  bar.baz'..      
-00009d70: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
-00009d80: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00009d90: 726e 616c 2e6d 6169 6e2e 636c 6965 6e74  rnal.main.client
-00009da0: 2729 2061 7320 636c 6965 6e74 3a0a 2020  ') as client:.  
-00009db0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00009dc0: 2e72 6567 6973 7465 722e 7265 7475 726e  .register.return
-00009dd0: 5f76 616c 7565 203d 2028 0a20 2020 2020  _value = (.     
-00009de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009df0: 6163 6373 5b30 5d2c 206d 6f63 6b2e 7365  accs[0], mock.se
-00009e00: 6e74 696e 656c 2e61 636d 6529 0a20 2020  ntinel.acme).   
-00009e10: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00009e20: 2873 656c 662e 6163 6373 5b30 5d2c 206d  (self.accs[0], m
-00009e30: 6f63 6b2e 7365 6e74 696e 656c 2e61 636d  ock.sentinel.acm
-00009e40: 6529 203d 3d20 7365 6c66 2e5f 6361 6c6c  e) == self._call
-00009e50: 2829 0a20 2020 2020 2020 2063 6c69 656e  ().        clien
-00009e60: 742e 7265 6769 7374 6572 2e61 7373 6572  t.register.asser
-00009e70: 745f 6361 6c6c 6564 5f6f 6e63 655f 7769  t_called_once_wi
-00009e80: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-00009e90: 7365 6c66 2e63 6f6e 6669 672c 2073 656c  self.config, sel
-00009ea0: 662e 6163 636f 756e 745f 7374 6f72 6167  f.account_storag
-00009eb0: 652c 2074 6f73 5f63 623d 6d6f 636b 2e41  e, tos_cb=mock.A
-00009ec0: 4e59 290a 0a20 2020 2020 2020 2061 7373  NY)..        ass
-00009ed0: 6572 7420 7365 6c66 2e61 6363 735b 305d  ert self.accs[0]
-00009ee0: 2e69 6420 3d3d 2073 656c 662e 636f 6e66  .id == self.conf
-00009ef0: 6967 2e61 6363 6f75 6e74 0a20 2020 2020  ig.account.     
-00009f00: 2020 2061 7373 6572 7420 2766 6f6f 4062     assert 'foo@b
-00009f10: 6172 2e62 617a 2720 3d3d 2073 656c 662e  ar.baz' == self.
-00009f20: 636f 6e66 6967 2e65 6d61 696c 0a20 2020  config.email.   
-00009f30: 2020 2020 206d 6f63 6b5f 6e6f 7469 6679       mock_notify
-00009f40: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
-00009f50: 6e63 655f 7769 7468 2827 4163 636f 756e  nce_with('Accoun
-00009f60: 7420 7265 6769 7374 6572 6564 2e27 290a  t registered.').
-00009f70: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
-00009f80: 5f61 6363 6f75 6e74 735f 656d 6169 6c28  _accounts_email(
-00009f90: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00009fa0: 656c 662e 636f 6e66 6967 2e65 6d61 696c  elf.config.email
-00009fb0: 203d 2027 6f74 6865 7220 656d 6169 6c27   = 'other email'
-00009fc0: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
-00009fd0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-00009fe0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-00009ff0: 2e63 6c69 656e 7427 2920 6173 2063 6c69  .client') as cli
-0000a000: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-0000a010: 2063 6c69 656e 742e 7265 6769 7374 6572   client.register
-0000a020: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-0000a030: 2873 656c 662e 6163 6373 5b31 5d2c 206d  (self.accs[1], m
-0000a040: 6f63 6b2e 7365 6e74 696e 656c 2e61 636d  ock.sentinel.acm
-0000a050: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-0000a060: 656c 662e 5f63 616c 6c28 290a 2020 2020  elf._call().    
-0000a070: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-0000a080: 6163 6373 5b31 5d2e 6964 203d 3d20 7365  accs[1].id == se
-0000a090: 6c66 2e63 6f6e 6669 672e 6163 636f 756e  lf.config.accoun
-0000a0a0: 740a 2020 2020 2020 2020 6173 7365 7274  t.        assert
-0000a0b0: 2027 6f74 6865 7220 656d 6169 6c27 203d   'other email' =
-0000a0c0: 3d20 7365 6c66 2e63 6f6e 6669 672e 656d  = self.config.em
-0000a0d0: 6169 6c0a 0a20 2020 2064 6566 2074 6573  ail..    def tes
-0000a0e0: 745f 7265 6769 7374 6572 5f65 7272 6f72  t_register_error
-0000a0f0: 5f63 6572 7462 6f74 2873 656c 6629 3a0a  _certbot(self):.
-0000a100: 2020 2020 2020 2020 6572 725f 6d73 6720          err_msg 
-0000a110: 3d20 2253 6f6d 6520 6572 726f 7220 6d65  = "Some error me
-0000a120: 7373 6167 6520 7261 6973 6564 2062 7920  ssage raised by 
-0000a130: 4365 7274 626f 7422 0a20 2020 2020 2020  Certbot".       
-0000a140: 2073 656c 662e 5f72 6567 6973 7465 725f   self._register_
-0000a150: 6572 726f 725f 636f 6d6d 6f6e 2865 7272  error_common(err
-0000a160: 5f6d 7367 2c20 6572 726f 7273 2e45 7272  _msg, errors.Err
-0000a170: 6f72 2865 7272 5f6d 7367 2929 0a0a 2020  or(err_msg))..  
-0000a180: 2020 6465 6620 7465 7374 5f72 6567 6973    def test_regis
-0000a190: 7465 725f 6572 726f 725f 6163 6d65 5f74  ter_error_acme_t
-0000a1a0: 7970 655f 616e 645f 6465 7461 696c 2873  ype_and_detail(s
-0000a1b0: 656c 6629 3a0a 2020 2020 2020 2020 6572  elf):.        er
-0000a1c0: 725f 6d73 6720 3d20 2822 4572 726f 7220  r_msg = ("Error 
-0000a1d0: 7265 7475 726e 6564 2062 7920 7468 6520  returned by the 
-0000a1e0: 4143 4d45 2073 6572 7665 723a 206d 7573  ACME server: mus
-0000a1f0: 7420 6167 7265 6520 746f 2074 6572 6d73  t agree to terms
-0000a200: 206f 6620 7365 7276 6963 6522 290a 2020   of service").  
-0000a210: 2020 2020 2020 6578 6365 7074 696f 6e20        exception 
-0000a220: 3d20 6163 6d65 5f65 7272 6f72 2874 7970  = acme_error(typ
-0000a230: 203d 2022 7572 6e3a 6965 7466 3a70 6172   = "urn:ietf:par
-0000a240: 616d 733a 6163 6d65 3a65 7272 6f72 3a6d  ams:acme:error:m
-0000a250: 616c 666f 726d 6564 222c 0a20 2020 2020  alformed",.     
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-0000a280: 203d 2022 6d75 7374 2061 6772 6565 2074   = "must agree t
-0000a290: 6f20 7465 726d 7320 6f66 2073 6572 7669  o terms of servi
-0000a2a0: 6365 2229 0a20 2020 2020 2020 2073 656c  ce").        sel
-0000a2b0: 662e 5f72 6567 6973 7465 725f 6572 726f  f._register_erro
-0000a2c0: 725f 636f 6d6d 6f6e 2865 7272 5f6d 7367  r_common(err_msg
-0000a2d0: 2c20 6578 6365 7074 696f 6e29 0a0a 2020  , exception)..  
-0000a2e0: 2020 6465 6620 7465 7374 5f72 6567 6973    def test_regis
-0000a2f0: 7465 725f 6572 726f 725f 6163 6d65 5f74  ter_error_acme_t
-0000a300: 7970 655f 6f6e 6c79 2873 656c 6629 3a0a  ype_only(self):.
-0000a310: 2020 2020 2020 2020 6572 725f 6d73 6720          err_msg 
-0000a320: 3d20 2822 4572 726f 7220 7265 7475 726e  = ("Error return
-0000a330: 6564 2062 7920 7468 6520 4143 4d45 2073  ed by the ACME s
-0000a340: 6572 7665 723a 2054 6865 2073 6572 7665  erver: The serve
-0000a350: 7220 6578 7065 7269 656e 6365 6420 616e  r experienced an
-0000a360: 2069 6e74 6572 6e61 6c20 6572 726f 7222   internal error"
-0000a370: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-0000a380: 696f 6e20 3d20 6163 6d65 5f65 7272 6f72  ion = acme_error
-0000a390: 2874 7970 203d 2022 7572 6e3a 6965 7466  (typ = "urn:ietf
-0000a3a0: 3a70 6172 616d 733a 6163 6d65 3a65 7272  :params:acme:err
-0000a3b0: 6f72 3a73 6572 7665 7249 6e74 6572 6e61  or:serverInterna
-0000a3c0: 6c22 290a 2020 2020 2020 2020 7365 6c66  l").        self
-0000a3d0: 2e5f 7265 6769 7374 6572 5f65 7272 6f72  ._register_error
-0000a3e0: 5f63 6f6d 6d6f 6e28 6572 725f 6d73 672c  _common(err_msg,
-0000a3f0: 2065 7863 6570 7469 6f6e 290a 0a0a 636c   exception)...cl
-0000a400: 6173 7320 4d61 696e 5465 7374 2874 6573  ass MainTest(tes
-0000a410: 745f 7574 696c 2e43 6f6e 6669 6754 6573  t_util.ConfigTes
-0000a420: 7443 6173 6529 3a0a 2020 2020 2222 2254  tCase):.    """T
-0000a430: 6573 7473 2066 6f72 2064 6966 6665 7265  ests for differe
-0000a440: 6e74 2063 6f6d 6d61 6e64 732e 2222 220a  nt commands.""".
-0000a450: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
-0000a460: 656c 6629 3a0a 2020 2020 2020 2020 7375  elf):.        su
-0000a470: 7065 7228 292e 7365 7455 7028 290a 0a20  per().setUp().. 
-0000a480: 2020 2020 2020 2066 696c 6573 7973 7465         filesyste
-0000a490: 6d2e 6d6b 6469 7228 7365 6c66 2e63 6f6e  m.mkdir(self.con
-0000a4a0: 6669 672e 6c6f 6773 5f64 6972 290a 2020  fig.logs_dir).  
-0000a4b0: 2020 2020 2020 7365 6c66 2e73 7461 6e64        self.stand
-0000a4c0: 6172 645f 6172 6773 203d 205b 272d 2d63  ard_args = ['--c
-0000a4d0: 6f6e 6669 672d 6469 7227 2c20 7365 6c66  onfig-dir', self
-0000a4e0: 2e63 6f6e 6669 672e 636f 6e66 6967 5f64  .config.config_d
-0000a4f0: 6972 2c0a 2020 2020 2020 2020 2020 2020  ir,.            
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 272d 2d77 6f72 6b2d 6469 7227 2c20    '--work-dir', 
-0000a520: 7365 6c66 2e63 6f6e 6669 672e 776f 726b  self.config.work
-0000a530: 5f64 6972 2c0a 2020 2020 2020 2020 2020  _dir,.          
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 272d 2d6c 6f67 732d 6469 7227      '--logs-dir'
-0000a560: 2c20 7365 6c66 2e63 6f6e 6669 672e 6c6f  , self.config.lo
-0000a570: 6773 5f64 6972 2c20 272d 2d74 6578 7427  gs_dir, '--text'
-0000a580: 5d0a 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-0000a590: 6d6f 636b 5f73 6c65 6570 203d 206d 6f63  mock_sleep = moc
-0000a5a0: 6b2e 7061 7463 6828 2774 696d 652e 736c  k.patch('time.sl
-0000a5b0: 6565 7027 292e 7374 6172 7428 290a 0a20  eep').start().. 
-0000a5c0: 2020 2064 6566 2074 6561 7244 6f77 6e28     def tearDown(
-0000a5d0: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
-0000a5e0: 2052 6573 6574 2067 6c6f 6261 6c73 2069   Reset globals i
-0000a5f0: 6e20 636c 690a 2020 2020 2020 2020 7265  n cli.        re
-0000a600: 6c6f 6164 5f6d 6f64 756c 6528 636c 6929  load_module(cli)
-0000a610: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-0000a620: 292e 7465 6172 446f 776e 2829 0a0a 2020  ).tearDown()..  
-0000a630: 2020 6465 6620 5f63 616c 6c28 7365 6c66    def _call(self
-0000a640: 2c20 6172 6773 2c20 7374 646f 7574 3d4e  , args, stdout=N
-0000a650: 6f6e 652c 206d 6f63 6b69 7366 696c 653d  one, mockisfile=
-0000a660: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
-0000a670: 2222 2252 756e 2074 6865 2063 6c69 2077  """Run the cli w
-0000a680: 6974 6820 6f75 7470 7574 2073 7472 6561  ith output strea
-0000a690: 6d73 2c20 6163 7475 616c 2063 6c69 656e  ms, actual clien
-0000a6a0: 7420 616e 6420 6f70 7469 6f6e 616c 6c79  t and optionally
-0000a6b0: 0a20 2020 2020 2020 206f 732e 7061 7468  .        os.path
-0000a6c0: 2e69 7366 696c 6528 2920 6d6f 636b 6564  .isfile() mocked
-0000a6d0: 206f 7574 2222 220a 0a20 2020 2020 2020   out"""..       
-0000a6e0: 2069 6620 6d6f 636b 6973 6669 6c65 3a0a   if mockisfile:.
-0000a6f0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000a700: 5f6f 7065 6e20 3d20 6f73 2e70 6174 682e  _open = os.path.
-0000a710: 6973 6669 6c65 0a0a 2020 2020 2020 2020  isfile..        
-0000a720: 2020 2020 6465 6620 6d6f 636b 5f69 7366      def mock_isf
-0000a730: 696c 6528 666e 2c20 2a61 7267 732c 202a  ile(fn, *args, *
-0000a740: 2a6b 7761 7267 7329 3a20 2023 2070 796c  *kwargs):  # pyl
-0000a750: 696e 743a 2064 6973 6162 6c65 3d75 6e75  int: disable=unu
-0000a760: 7365 642d 6172 6775 6d65 6e74 0a20 2020  sed-argument.   
-0000a770: 2020 2020 2020 2020 2020 2020 2022 2222               """
-0000a780: 4d6f 636b 206f 732e 7061 7468 2e69 7366  Mock os.path.isf
-0000a790: 696c 6528 2922 2222 0a20 2020 2020 2020  ile()""".       
-0000a7a0: 2020 2020 2020 2020 2069 6620 2866 6e2e           if (fn.
-0000a7b0: 656e 6473 7769 7468 2822 6365 7274 2229  endswith("cert")
-0000a7c0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-0000a7d0: 2020 2020 2020 2020 2020 2020 666e 2e65              fn.e
-0000a7e0: 6e64 7377 6974 6828 2263 6861 696e 2229  ndswith("chain")
-0000a7f0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-0000a800: 2020 2020 2020 2020 2020 2020 666e 2e65              fn.e
-0000a810: 6e64 7377 6974 6828 2270 7269 766b 6579  ndswith("privkey
-0000a820: 2229 293a 0a20 2020 2020 2020 2020 2020  ")):.           
-0000a830: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000a840: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000a850: 2020 2020 2072 6574 7572 6e20 6f72 6967       return orig
-0000a860: 5f6f 7065 6e28 666e 290a 0a20 2020 2020  _open(fn)..     
-0000a870: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
-0000a880: 2e70 6174 6368 2822 6365 7274 626f 742e  .patch("certbot.
-0000a890: 636f 6d70 6174 2e6f 732e 7061 7468 2e69  compat.os.path.i
-0000a8a0: 7366 696c 6522 2920 6173 206d 6f63 6b5f  sfile") as mock_
-0000a8b0: 6966 3a0a 2020 2020 2020 2020 2020 2020  if:.            
-0000a8c0: 2020 2020 6d6f 636b 5f69 662e 7369 6465      mock_if.side
-0000a8d0: 5f65 6666 6563 7420 3d20 6d6f 636b 5f69  _effect = mock_i
-0000a8e0: 7366 696c 650a 2020 2020 2020 2020 2020  sfile.          
-0000a8f0: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
-0000a900: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-0000a910: 696e 7465 726e 616c 2e6d 6169 6e2e 636c  internal.main.cl
-0000a920: 6965 6e74 2729 2061 7320 636c 6965 6e74  ient') as client
-0000a930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a940: 2020 2020 2020 7265 742c 2073 7464 6f75        ret, stdou
-0000a950: 742c 2073 7464 6572 7220 3d20 7365 6c66  t, stderr = self
-0000a960: 2e5f 6361 6c6c 5f6e 6f5f 636c 6965 6e74  ._call_no_client
-0000a970: 6d6f 636b 2861 7267 732c 2073 7464 6f75  mock(args, stdou
-0000a980: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-0000a990: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000a9a0: 742c 2073 7464 6f75 742c 2073 7464 6572  t, stdout, stder
-0000a9b0: 722c 2063 6c69 656e 740a 2020 2020 2020  r, client.      
-0000a9c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a9d0: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
-0000a9e0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0000a9f0: 7465 726e 616c 2e6d 6169 6e2e 636c 6965  ternal.main.clie
-0000aa00: 6e74 2729 2061 7320 636c 6965 6e74 3a0a  nt') as client:.
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 7265 742c 2073 7464 6f75 742c 2073 7464  ret, stdout, std
-0000aa30: 6572 7220 3d20 7365 6c66 2e5f 6361 6c6c  err = self._call
-0000aa40: 5f6e 6f5f 636c 6965 6e74 6d6f 636b 2861  _no_clientmock(a
-0000aa50: 7267 732c 2073 7464 6f75 7429 0a20 2020  rgs, stdout).   
-0000aa60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000aa70: 7572 6e20 7265 742c 2073 7464 6f75 742c  urn ret, stdout,
-0000aa80: 2073 7464 6572 722c 2063 6c69 656e 740a   stderr, client.
-0000aa90: 0a20 2020 2064 6566 205f 6361 6c6c 5f6e  .    def _call_n
-0000aaa0: 6f5f 636c 6965 6e74 6d6f 636b 2873 656c  o_clientmock(sel
-0000aab0: 662c 2061 7267 732c 2073 7464 6f75 743d  f, args, stdout=
-0000aac0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-0000aad0: 2222 5275 6e20 7468 6520 636c 6965 6e74  ""Run the client
-0000aae0: 2077 6974 6820 6f75 7470 7574 2073 7472   with output str
-0000aaf0: 6561 6d73 206d 6f63 6b65 6420 6f75 7422  eams mocked out"
-0000ab00: 2222 0a20 2020 2020 2020 2061 7267 7320  "".        args 
-0000ab10: 3d20 7365 6c66 2e73 7461 6e64 6172 645f  = self.standard_
-0000ab20: 6172 6773 202b 2061 7267 730a 0a20 2020  args + args..   
-0000ab30: 2020 2020 2074 6f79 5f73 7464 6f75 7420       toy_stdout 
-0000ab40: 3d20 7374 646f 7574 2069 6620 7374 646f  = stdout if stdo
-0000ab50: 7574 2065 6c73 6520 696f 2e53 7472 696e  ut else io.Strin
-0000ab60: 6749 4f28 290a 2020 2020 2020 2020 7769  gIO().        wi
-0000ab70: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-0000ab80: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-0000ab90: 2e6d 6169 6e2e 7379 732e 7374 646f 7574  .main.sys.stdout
-0000aba0: 272c 206e 6577 3d74 6f79 5f73 7464 6f75  ', new=toy_stdou
-0000abb0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000abc0: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
-0000abd0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0000abe0: 616c 2e6d 6169 6e2e 7379 732e 7374 6465  al.main.sys.stde
-0000abf0: 7272 2729 2061 7320 7374 6465 7272 3a0a  rr') as stderr:.
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
-0000ac20: 2263 6572 7462 6f74 2e75 7469 6c2e 6174  "certbot.util.at
-0000ac30: 6578 6974 2229 3a0a 2020 2020 2020 2020  exit"):.        
-0000ac40: 2020 2020 2020 2020 2020 2020 7265 7420              ret 
-0000ac50: 3d20 6d61 696e 2e6d 6169 6e28 6172 6773  = main.main(args
-0000ac60: 5b3a 5d29 2020 2320 4e4f 5445 3a20 7061  [:])  # NOTE: pa
-0000ac70: 7273 6572 2063 616e 2061 6c74 6572 2069  rser can alter i
-0000ac80: 7473 2061 7267 7321 0a20 2020 2020 2020  ts args!.       
-0000ac90: 2072 6574 7572 6e20 7265 742c 2074 6f79   return ret, toy
-0000aca0: 5f73 7464 6f75 742c 2073 7464 6572 720a  _stdout, stderr.
-0000acb0: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
-0000acc0: 5f66 6c61 6773 2873 656c 6629 3a0a 2020  _flags(self):.  
-0000acd0: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
-0000ace0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-0000acf0: 696e 7465 726e 616c 2e6d 6169 6e2e 7275  internal.main.ru
-0000ad00: 6e27 2920 6173 206d 6f63 6b5f 7275 6e3a  n') as mock_run:
-0000ad10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ad20: 662e 5f63 616c 6c28 5b5d 290a 2020 2020  f._call([]).    
-0000ad30: 2020 2020 2020 2020 6173 7365 7274 2031          assert 1
-0000ad40: 203d 3d20 6d6f 636b 5f72 756e 2e63 616c   == mock_run.cal
-0000ad50: 6c5f 636f 756e 740a 0a20 2020 2064 6566  l_count..    def
-0000ad60: 2074 6573 745f 7665 7273 696f 6e5f 7374   test_version_st
-0000ad70: 7269 6e67 5f70 726f 6772 616d 5f6e 616d  ring_program_nam
-0000ad80: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000ad90: 2074 6f79 5f6f 7574 203d 2069 6f2e 5374   toy_out = io.St
-0000ada0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-0000adb0: 2074 6f79 5f65 7272 203d 2069 6f2e 5374   toy_err = io.St
-0000adc0: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
-0000add0: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
-0000ade0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-0000adf0: 6e61 6c2e 6d61 696e 2e73 7973 2e73 7464  nal.main.sys.std
-0000ae00: 6f75 7427 2c20 6e65 773d 746f 795f 6f75  out', new=toy_ou
-0000ae10: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000ae20: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
-0000ae30: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0000ae40: 616c 2e6d 6169 6e2e 7379 732e 7374 6465  al.main.sys.stde
-0000ae50: 7272 272c 206e 6577 3d74 6f79 5f65 7272  rr', new=toy_err
-0000ae60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ae70: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000ae80: 2020 2020 2020 2020 2020 2020 6d61 696e              main
-0000ae90: 2e6d 6169 6e28 5b22 2d2d 7665 7273 696f  .main(["--versio
-0000aea0: 6e22 5d29 0a20 2020 2020 2020 2020 2020  n"]).           
-0000aeb0: 2020 2020 2065 7863 6570 7420 5379 7374       except Syst
-0000aec0: 656d 4578 6974 3a0a 2020 2020 2020 2020  emExit:.        
-0000aed0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0000aee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aef0: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-0000af00: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-0000af10: 7470 7574 203d 2074 6f79 5f6f 7574 2e67  tput = toy_out.g
-0000af20: 6574 7661 6c75 6528 2920 6f72 2074 6f79  etvalue() or toy
-0000af30: 5f65 7272 2e67 6574 7661 6c75 6528 290a  _err.getvalue().
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 6173 7365 7274 2022 6365 7274      assert "cert
-0000af60: 626f 7422 2069 6e20 6f75 7470 7574 2c20  bot" in output, 
-0000af70: 224f 7574 7075 7420 6973 207b 307d 222e  "Output is {0}".
-0000af80: 666f 726d 6174 286f 7574 7075 7429 0a0a  format(output)..
-0000af90: 2020 2020 6465 6620 5f63 6c69 5f6d 6973      def _cli_mis
-0000afa0: 7369 6e67 5f66 6c61 6728 7365 6c66 2c20  sing_flag(self, 
-0000afb0: 6172 6773 2c20 6d65 7373 6167 6529 3a0a  args, message):.
-0000afc0: 2020 2020 2020 2020 2245 6e73 7572 6520          "Ensure 
-0000afd0: 7468 6174 2061 2070 6172 7469 6375 6c61  that a particula
-0000afe0: 7220 6572 726f 7220 7261 6973 6573 2061  r error raises a
-0000aff0: 206d 6973 7369 6e67 2063 6c69 2066 6c61   missing cli fla
-0000b000: 6720 6572 726f 7220 636f 6e74 6169 6e69  g error containi
-0000b010: 6e67 206d 6573 7361 6765 220a 2020 2020  ng message".    
-0000b020: 2020 2020 6578 6320 3d20 4e6f 6e65 0a20      exc = None. 
-0000b030: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0000b040: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-0000b050: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-0000b060: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-0000b070: 7379 732e 7374 6465 7272 2729 3a0a 2020  sys.stderr'):.  
-0000b080: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0000b090: 696e 2e6d 6169 6e28 7365 6c66 2e73 7461  in.main(self.sta
-0000b0a0: 6e64 6172 645f 6172 6773 202b 2061 7267  ndard_args + arg
-0000b0b0: 735b 3a5d 2920 2023 204e 4f54 453a 2070  s[:])  # NOTE: p
-0000b0c0: 6172 7365 7220 6361 6e20 616c 7465 7220  arser can alter 
-0000b0d0: 6974 7320 6172 6773 210a 2020 2020 2020  its args!.      
-0000b0e0: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
-0000b0f0: 4d69 7373 696e 6743 6f6d 6d61 6e64 6c69  MissingCommandli
-0000b100: 6e65 466c 6167 2061 7320 6578 635f 3a0a  neFlag as exc_:.
-0000b110: 2020 2020 2020 2020 2020 2020 6578 6320              exc 
-0000b120: 3d20 6578 635f 0a20 2020 2020 2020 2020  = exc_.         
-0000b130: 2020 2061 7373 6572 7420 6d65 7373 6167     assert messag
-0000b140: 6520 696e 2073 7472 2865 7863 290a 2020  e in str(exc).  
-0000b150: 2020 2020 2020 6173 7365 7274 2065 7863        assert exc
-0000b160: 2069 7320 6e6f 7420 4e6f 6e65 0a0a 2020   is not None..  
-0000b170: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-0000b180: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-0000b190: 2e6c 6f67 2e70 6f73 745f 6172 675f 7061  .log.post_arg_pa
-0000b1a0: 7273 655f 7365 7475 7027 290a 2020 2020  rse_setup').    
-0000b1b0: 6465 6620 7465 7374 5f6e 6f6e 696e 7465  def test_noninte
-0000b1c0: 7261 6374 6976 6528 7365 6c66 2c20 5f29  ractive(self, _)
-0000b1d0: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
-0000b1e0: 205b 272d 6e27 2c20 2763 6572 746f 6e6c   ['-n', 'certonl
-0000b1f0: 7927 5d0a 2020 2020 2020 2020 7365 6c66  y'].        self
-0000b200: 2e5f 636c 695f 6d69 7373 696e 675f 666c  ._cli_missing_fl
-0000b210: 6167 2861 7267 732c 2022 7370 6563 6966  ag(args, "specif
-0000b220: 7920 6120 706c 7567 696e 2229 0a20 2020  y a plugin").   
-0000b230: 2020 2020 2061 7267 732e 6578 7465 6e64       args.extend
-0000b240: 285b 272d 2d73 7461 6e64 616c 6f6e 6527  (['--standalone'
-0000b250: 2c20 272d 6427 2c20 2765 672e 6973 275d  , '-d', 'eg.is']
-0000b260: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0000b270: 636c 695f 6d69 7373 696e 675f 666c 6167  cli_missing_flag
-0000b280: 2861 7267 732c 2022 7265 6769 7374 6572  (args, "register
-0000b290: 2062 6566 6f72 6520 7275 6e6e 696e 6722   before running"
-0000b2a0: 290a 0a20 2020 2040 6d6f 636b 2e70 6174  )..    @mock.pat
-0000b2b0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0000b2c0: 6572 6e61 6c2e 6566 662e 6861 6e64 6c65  ernal.eff.handle
-0000b2d0: 5f73 7562 7363 7269 7074 696f 6e27 290a  _subscription').
-0000b2e0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-0000b2f0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0000b300: 616c 2e6c 6f67 2e70 6f73 745f 6172 675f  al.log.post_arg_
-0000b310: 7061 7273 655f 7365 7475 7027 290a 2020  parse_setup').  
-0000b320: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-0000b330: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-0000b340: 2e6d 6169 6e2e 5f72 6570 6f72 745f 6e65  .main._report_ne
-0000b350: 775f 6365 7274 2729 0a20 2020 2040 6d6f  w_cert').    @mo
-0000b360: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-0000b370: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-0000b380: 2e5f 6465 7465 726d 696e 655f 6163 636f  ._determine_acco
-0000b390: 756e 7427 290a 2020 2020 406d 6f63 6b2e  unt').    @mock.
-0000b3a0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-0000b3b0: 696e 7465 726e 616c 2e6d 6169 6e2e 636c  internal.main.cl
-0000b3c0: 6965 6e74 2e43 6c69 656e 742e 6f62 7461  ient.Client.obta
-0000b3d0: 696e 5f61 6e64 5f65 6e72 6f6c 6c5f 6365  in_and_enroll_ce
-0000b3e0: 7274 6966 6963 6174 6527 290a 2020 2020  rtificate').    
-0000b3f0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-0000b400: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-0000b410: 6169 6e2e 5f67 6574 5f61 6e64 5f73 6176  ain._get_and_sav
-0000b420: 655f 6365 7274 2729 0a20 2020 2064 6566  e_cert').    def
-0000b430: 2074 6573 745f 7573 6572 5f61 6765 6e74   test_user_agent
-0000b440: 2873 656c 662c 2067 7363 2c20 5f6f 6274  (self, gsc, _obt
-0000b450: 2c20 6465 742c 205f 2c20 5f5f 2c20 5f5f  , det, _, __, __
-0000b460: 5f29 3a0a 2020 2020 2020 2020 2320 4e6f  _):.        # No
-0000b470: 726d 616c 6c79 2074 6865 2063 6c69 656e  rmally the clien
-0000b480: 7420 6973 2074 6f74 616c 6c79 206d 6f63  t is totally moc
-0000b490: 6b65 6420 6f75 742c 2062 7574 2068 6572  ked out, but her
-0000b4a0: 6520 7765 206e 6565 6420 6d6f 7265 0a20  e we need more. 
-0000b4b0: 2020 2020 2020 2023 2061 7267 756d 656e         # argumen
-0000b4c0: 7473 2074 6f20 6175 746f 6d61 7465 2069  ts to automate i
-0000b4d0: 742e 2e2e 0a20 2020 2020 2020 2061 7267  t....        arg
-0000b4e0: 7320 3d20 5b22 2d2d 7374 616e 6461 6c6f  s = ["--standalo
-0000b4f0: 6e65 222c 2022 6365 7274 6f6e 6c79 222c  ne", "certonly",
-0000b500: 2022 2d6d 222c 2022 6e6f 6e65 406e 6f6e   "-m", "none@non
-0000b510: 652e 636f 6d22 2c0a 2020 2020 2020 2020  e.com",.        
-0000b520: 2020 2020 2020 2020 222d 6422 2c20 2265          "-d", "e
-0000b530: 7861 6d70 6c65 2e63 6f6d 222c 2027 2d2d  xample.com", '--
-0000b540: 6167 7265 652d 746f 7327 5d20 2b20 7365  agree-tos'] + se
-0000b550: 6c66 2e73 7461 6e64 6172 645f 6172 6773  lf.standard_args
-0000b560: 0a20 2020 2020 2020 2064 6574 2e72 6574  .        det.ret
-0000b570: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
-0000b580: 2e4d 6167 6963 4d6f 636b 2829 2c20 4e6f  .MagicMock(), No
-0000b590: 6e65 0a20 2020 2020 2020 2067 7363 2e72  ne.        gsc.r
-0000b5a0: 6574 7572 6e5f 7661 6c75 6520 3d20 6d6f  eturn_value = mo
-0000b5b0: 636b 2e4d 6167 6963 4d6f 636b 2829 0a0a  ck.MagicMock()..
-0000b5c0: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-0000b5d0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-0000b5e0: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-0000b5f0: 636c 6965 6e74 2e61 636d 655f 636c 6965  client.acme_clie
-0000b600: 6e74 2729 2061 7320 6163 6d65 5f63 6c69  nt') as acme_cli
-0000b610: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-0000b620: 2061 636d 655f 6e65 7420 3d20 6163 6d65   acme_net = acme
-0000b630: 5f63 6c69 656e 742e 436c 6965 6e74 4e65  _client.ClientNe
-0000b640: 7477 6f72 6b0a 2020 2020 2020 2020 2020  twork.          
-0000b650: 2020 7365 6c66 2e5f 6361 6c6c 5f6e 6f5f    self._call_no_
-0000b660: 636c 6965 6e74 6d6f 636b 2861 7267 7329  clientmock(args)
-0000b670: 0a20 2020 2020 2020 2020 2020 206f 735f  .            os_
-0000b680: 7665 7220 3d20 7574 696c 2e67 6574 5f6f  ver = util.get_o
-0000b690: 735f 696e 666f 5f75 6128 290a 2020 2020  s_info_ua().    
-0000b6a0: 2020 2020 2020 2020 7561 203d 2061 636d          ua = acm
-0000b6b0: 655f 6e65 742e 6361 6c6c 5f61 7267 735b  e_net.call_args[
-0000b6c0: 315d 5b22 7573 6572 5f61 6765 6e74 225d  1]["user_agent"]
-0000b6d0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000b6e0: 6572 7420 6f73 5f76 6572 2069 6e20 7561  ert os_ver in ua
-0000b6f0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-0000b700: 6f72 7420 706c 6174 666f 726d 0a20 2020  ort platform.   
-0000b710: 2020 2020 2020 2020 2070 6c61 7420 3d20           plat = 
-0000b720: 706c 6174 666f 726d 2e70 6c61 7466 6f72  platform.platfor
-0000b730: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-0000b740: 6966 2022 6c69 6e75 7822 2069 6e20 706c  if "linux" in pl
-0000b750: 6174 2e6c 6f77 6572 2829 3a0a 2020 2020  at.lower():.    
-0000b760: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000b770: 7274 2075 7469 6c2e 6765 745f 6f73 5f69  rt util.get_os_i
-0000b780: 6e66 6f5f 7561 2829 2069 6e20 7561 0a0a  nfo_ua() in ua..
-0000b790: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-0000b7a0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-0000b7b0: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-0000b7c0: 636c 6965 6e74 2e61 636d 655f 636c 6965  client.acme_clie
-0000b7d0: 6e74 2729 2061 7320 6163 6d65 5f63 6c69  nt') as acme_cli
-0000b7e0: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-0000b7f0: 2061 636d 655f 6e65 7420 3d20 6163 6d65   acme_net = acme
-0000b800: 5f63 6c69 656e 742e 436c 6965 6e74 4e65  _client.ClientNe
-0000b810: 7477 6f72 6b0a 2020 2020 2020 2020 2020  twork.          
-0000b820: 2020 7561 203d 2022 6261 6e64 6572 736e    ua = "bandersn
-0000b830: 6174 6368 220a 2020 2020 2020 2020 2020  atch".          
-0000b840: 2020 6172 6773 202b 3d20 5b22 2d2d 7573    args += ["--us
-0000b850: 6572 2d61 6765 6e74 222c 2075 615d 0a20  er-agent", ua]. 
-0000b860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b870: 5f63 616c 6c5f 6e6f 5f63 6c69 656e 746d  _call_no_clientm
-0000b880: 6f63 6b28 6172 6773 290a 2020 2020 2020  ock(args).      
-0000b890: 2020 2020 2020 6163 6d65 5f6e 6574 2e61        acme_net.a
-0000b8a0: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
-0000b8b0: 655f 7769 7468 286d 6f63 6b2e 414e 592c  e_with(mock.ANY,
-0000b8c0: 2061 6363 6f75 6e74 3d6d 6f63 6b2e 414e   account=mock.AN
-0000b8d0: 592c 2076 6572 6966 795f 7373 6c3d 5472  Y, verify_ssl=Tr
-0000b8e0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000b8f0: 2020 2020 7573 6572 5f61 6765 6e74 3d75      user_agent=u
-0000b900: 612c 2061 6c67 3d6a 6f73 652e 5253 3235  a, alg=jose.RS25
-0000b910: 3629 0a0a 2020 2020 406d 6f63 6b2e 7061  6)..    @mock.pa
-0000b920: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0000b930: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
-0000b940: 5f73 656c 2e72 6563 6f72 645f 6368 6f73  _sel.record_chos
-0000b950: 656e 5f70 6c75 6769 6e73 2729 0a20 2020  en_plugins').   
-0000b960: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000b970: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000b980: 6d61 696e 2e70 6c75 675f 7365 6c2e 7069  main.plug_sel.pi
-0000b990: 636b 5f69 6e73 7461 6c6c 6572 2729 0a20  ck_installer'). 
-0000b9a0: 2020 2064 6566 2074 6573 745f 696e 7374     def test_inst
-0000b9b0: 616c 6c65 725f 7365 6c65 6374 696f 6e28  aller_selection(
-0000b9c0: 7365 6c66 2c20 6d6f 636b 5f70 6963 6b5f  self, mock_pick_
-0000b9d0: 696e 7374 616c 6c65 722c 205f 7265 6329  installer, _rec)
-0000b9e0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0000b9f0: 6361 6c6c 285b 2769 6e73 7461 6c6c 272c  call(['install',
-0000ba00: 2027 2d2d 646f 6d61 696e 7327 2c20 2766   '--domains', 'f
-0000ba10: 6f6f 2e62 6172 272c 2027 2d2d 6365 7274  oo.bar', '--cert
-0000ba20: 2d70 6174 6827 2c20 2763 6572 7427 2c0a  -path', 'cert',.
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 2020 2020 272d 2d6b 6579 2d70 6174 6827      '--key-path'
-0000ba50: 2c20 2770 7269 766b 6579 272c 2027 2d2d  , 'privkey', '--
-0000ba60: 6368 6169 6e2d 7061 7468 272c 2027 6368  chain-path', 'ch
-0000ba70: 6169 6e27 5d2c 206d 6f63 6b69 7366 696c  ain'], mockisfil
-0000ba80: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-0000ba90: 6173 7365 7274 206d 6f63 6b5f 7069 636b  assert mock_pick
-0000baa0: 5f69 6e73 7461 6c6c 6572 2e63 616c 6c5f  _installer.call_
-0000bab0: 636f 756e 7420 3d3d 2031 0a0a 2020 2020  count == 1..    
-0000bac0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-0000bad0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-0000bae0: 6169 6e2e 5f69 6e73 7461 6c6c 5f63 6572  ain._install_cer
-0000baf0: 7427 290a 2020 2020 406d 6f63 6b2e 7061  t').    @mock.pa
-0000bb00: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0000bb10: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
-0000bb20: 5f73 656c 2e72 6563 6f72 645f 6368 6f73  _sel.record_chos
-0000bb30: 656e 5f70 6c75 6769 6e73 2729 0a20 2020  en_plugins').   
-0000bb40: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000bb50: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000bb60: 6d61 696e 2e70 6c75 675f 7365 6c2e 7069  main.plug_sel.pi
-0000bb70: 636b 5f69 6e73 7461 6c6c 6572 2729 0a20  ck_installer'). 
-0000bb80: 2020 2064 6566 2074 6573 745f 696e 7374     def test_inst
-0000bb90: 616c 6c65 725f 6365 7274 6e61 6d65 2873  aller_certname(s
-0000bba0: 656c 662c 205f 696e 7374 2c20 5f72 6563  elf, _inst, _rec
-0000bbb0: 2c20 6d6f 636b 5f69 6e73 7461 6c6c 293a  , mock_install):
-0000bbc0: 0a20 2020 2020 2020 206d 6f63 6b5f 6c69  .        mock_li
-0000bbd0: 6e65 6167 6520 3d20 6d6f 636b 2e4d 6167  neage = mock.Mag
-0000bbe0: 6963 4d6f 636b 2863 6572 745f 7061 7468  icMock(cert_path
-0000bbf0: 3d74 6573 745f 7574 696c 2e74 656d 705f  =test_util.temp_
-0000bc00: 6a6f 696e 2827 6365 7274 2729 2c0a 2020  join('cert'),.  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 6368 6169 6e5f 7061 7468 3d74      chain_path=t
-0000bc40: 6573 745f 7574 696c 2e74 656d 705f 6a6f  est_util.temp_jo
-0000bc50: 696e 2827 6368 6169 6e27 292c 0a20 2020  in('chain'),.   
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2066 756c 6c63 6861 696e 5f70 6174     fullchain_pat
-0000bc90: 683d 7465 7374 5f75 7469 6c2e 7465 6d70  h=test_util.temp
-0000bca0: 5f6a 6f69 6e28 2763 6861 696e 2729 2c0a  _join('chain'),.
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2020 2020 2020 6b65 795f 7061 7468 3d74        key_path=t
-0000bce0: 6573 745f 7574 696c 2e74 656d 705f 6a6f  est_util.temp_jo
-0000bcf0: 696e 2827 7072 6976 6b65 7927 2929 0a0a  in('privkey'))..
-0000bd00: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-0000bd10: 6b2e 7061 7463 6828 2263 6572 7462 6f74  k.patch("certbot
-0000bd20: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
-0000bd30: 6d61 6e61 6765 722e 6c69 6e65 6167 655f  manager.lineage_
-0000bd40: 666f 725f 6365 7274 6e61 6d65 2229 2061  for_certname") a
-0000bd50: 7320 6d6f 636b 5f67 6574 6c69 6e3a 0a20  s mock_getlin:. 
-0000bd60: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-0000bd70: 6765 746c 696e 2e72 6574 7572 6e5f 7661  getlin.return_va
-0000bd80: 6c75 6520 3d20 6d6f 636b 5f6c 696e 6561  lue = mock_linea
-0000bd90: 6765 0a20 2020 2020 2020 2020 2020 2073  ge.            s
-0000bda0: 656c 662e 5f63 616c 6c28 5b27 696e 7374  elf._call(['inst
-0000bdb0: 616c 6c27 2c20 272d 2d63 6572 742d 6e61  all', '--cert-na
-0000bdc0: 6d65 272c 2027 7768 6174 6576 6572 275d  me', 'whatever']
-0000bdd0: 2c20 6d6f 636b 6973 6669 6c65 3d54 7275  , mockisfile=Tru
-0000bde0: 6529 0a20 2020 2020 2020 2020 2020 2063  e).            c
-0000bdf0: 616c 6c5f 636f 6e66 6967 203d 206d 6f63  all_config = moc
-0000be00: 6b5f 696e 7374 616c 6c2e 6361 6c6c 5f61  k_install.call_a
-0000be10: 7267 735b 305d 5b30 5d0a 2020 2020 2020  rgs[0][0].      
-0000be20: 2020 2020 2020 6173 7365 7274 2063 616c        assert cal
-0000be30: 6c5f 636f 6e66 6967 2e63 6572 745f 7061  l_config.cert_pa
-0000be40: 7468 203d 3d20 7465 7374 5f75 7469 6c2e  th == test_util.
-0000be50: 7465 6d70 5f6a 6f69 6e28 2763 6572 7427  temp_join('cert'
-0000be60: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-0000be70: 7365 7274 2063 616c 6c5f 636f 6e66 6967  sert call_config
-0000be80: 2e66 756c 6c63 6861 696e 5f70 6174 6820  .fullchain_path 
-0000be90: 3d3d 2074 6573 745f 7574 696c 2e74 656d  == test_util.tem
-0000bea0: 705f 6a6f 696e 2827 6368 6169 6e27 290a  p_join('chain').
-0000beb0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000bec0: 7274 2063 616c 6c5f 636f 6e66 6967 2e6b  rt call_config.k
-0000bed0: 6579 5f70 6174 6820 3d3d 2074 6573 745f  ey_path == test_
-0000bee0: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
-0000bef0: 7072 6976 6b65 7927 290a 0a20 2020 2040  privkey')..    @
-0000bf00: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-0000bf10: 626f 742e 5f69 6e74 6572 6e61 6c2e 6c6f  bot._internal.lo
-0000bf20: 672e 706f 7374 5f61 7267 5f70 6172 7365  g.post_arg_parse
-0000bf30: 5f73 6574 7570 2729 0a20 2020 2040 6d6f  _setup').    @mo
-0000bf40: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-0000bf50: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-0000bf60: 2e5f 696e 7374 616c 6c5f 6365 7274 2729  ._install_cert')
-0000bf70: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-0000bf80: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-0000bf90: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
-0000bfa0: 6c2e 7265 636f 7264 5f63 686f 7365 6e5f  l.record_chosen_
-0000bfb0: 706c 7567 696e 7327 290a 2020 2020 406d  plugins').    @m
-0000bfc0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000bfd0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-0000bfe0: 6e2e 706c 7567 5f73 656c 2e70 6963 6b5f  n.plug_sel.pick_
-0000bff0: 696e 7374 616c 6c65 7227 290a 2020 2020  installer').    
-0000c000: 6465 6620 7465 7374 5f69 6e73 7461 6c6c  def test_install
-0000c010: 6572 5f70 6172 616d 5f6f 7665 7272 6964  er_param_overrid
-0000c020: 6528 7365 6c66 2c20 5f69 6e73 742c 205f  e(self, _inst, _
-0000c030: 7265 632c 206d 6f63 6b5f 696e 7374 616c  rec, mock_instal
-0000c040: 6c2c 205f 293a 0a20 2020 2020 2020 206d  l, _):.        m
-0000c050: 6f63 6b5f 6c69 6e65 6167 6520 3d20 6d6f  ock_lineage = mo
-0000c060: 636b 2e4d 6167 6963 4d6f 636b 2863 6572  ck.MagicMock(cer
-0000c070: 745f 7061 7468 3d74 6573 745f 7574 696c  t_path=test_util
-0000c080: 2e74 656d 705f 6a6f 696e 2827 6365 7274  .temp_join('cert
-0000c090: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 6368 6169 6e5f            chain_
-0000c0c0: 7061 7468 3d74 6573 745f 7574 696c 2e74  path=test_util.t
-0000c0d0: 656d 705f 6a6f 696e 2827 6368 6169 6e27  emp_join('chain'
-0000c0e0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2020 2020 2020 2066 756c 6c63 6861           fullcha
-0000c110: 696e 5f70 6174 683d 7465 7374 5f75 7469  in_path=test_uti
-0000c120: 6c2e 7465 6d70 5f6a 6f69 6e28 2763 6861  l.temp_join('cha
-0000c130: 696e 2729 2c0a 2020 2020 2020 2020 2020  in'),.          
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2020 2020 2020 2020 6b65 795f              key_
-0000c160: 7061 7468 3d74 6573 745f 7574 696c 2e74  path=test_util.t
-0000c170: 656d 705f 6a6f 696e 2827 7072 6976 6b65  emp_join('privke
-0000c180: 7927 2929 0a20 2020 2020 2020 2077 6974  y')).        wit
-0000c190: 6820 6d6f 636b 2e70 6174 6368 2822 6365  h mock.patch("ce
-0000c1a0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000c1b0: 6365 7274 5f6d 616e 6167 6572 2e6c 696e  cert_manager.lin
-0000c1c0: 6561 6765 5f66 6f72 5f63 6572 746e 616d  eage_for_certnam
-0000c1d0: 6522 2920 6173 206d 6f63 6b5f 6765 746c  e") as mock_getl
-0000c1e0: 696e 3a0a 2020 2020 2020 2020 2020 2020  in:.            
-0000c1f0: 6d6f 636b 5f67 6574 6c69 6e2e 7265 7475  mock_getlin.retu
-0000c200: 726e 5f76 616c 7565 203d 206d 6f63 6b5f  rn_value = mock_
-0000c210: 6c69 6e65 6167 650a 2020 2020 2020 2020  lineage.        
-0000c220: 2020 2020 7365 6c66 2e5f 6361 6c6c 285b      self._call([
-0000c230: 2769 6e73 7461 6c6c 272c 2027 2d2d 6365  'install', '--ce
-0000c240: 7274 2d6e 616d 6527 2c20 2777 6861 7465  rt-name', 'whate
-0000c250: 7665 7227 2c0a 2020 2020 2020 2020 2020  ver',.          
-0000c260: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-0000c270: 2d6b 6579 2d70 6174 6827 2c20 7465 7374  -key-path', test
-0000c280: 5f75 7469 6c2e 7465 6d70 5f6a 6f69 6e28  _util.temp_join(
-0000c290: 276f 7665 7272 6964 696e 675f 7072 6976  'overriding_priv
-0000c2a0: 6b65 7927 295d 2c20 6d6f 636b 6973 6669  key')], mockisfi
-0000c2b0: 6c65 3d54 7275 6529 0a20 2020 2020 2020  le=True).       
-0000c2c0: 2020 2020 2063 616c 6c5f 636f 6e66 6967       call_config
-0000c2d0: 203d 206d 6f63 6b5f 696e 7374 616c 6c2e   = mock_install.
-0000c2e0: 6361 6c6c 5f61 7267 735b 305d 5b30 5d0a  call_args[0][0].
-0000c2f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000c300: 7274 2063 616c 6c5f 636f 6e66 6967 2e63  rt call_config.c
-0000c310: 6572 745f 7061 7468 203d 3d20 7465 7374  ert_path == test
-0000c320: 5f75 7469 6c2e 7465 6d70 5f6a 6f69 6e28  _util.temp_join(
-0000c330: 2763 6572 7427 290a 2020 2020 2020 2020  'cert').        
-0000c340: 2020 2020 6173 7365 7274 2063 616c 6c5f      assert call_
-0000c350: 636f 6e66 6967 2e66 756c 6c63 6861 696e  config.fullchain
-0000c360: 5f70 6174 6820 3d3d 2074 6573 745f 7574  _path == test_ut
-0000c370: 696c 2e74 656d 705f 6a6f 696e 2827 6368  il.temp_join('ch
-0000c380: 6169 6e27 290a 2020 2020 2020 2020 2020  ain').          
-0000c390: 2020 6173 7365 7274 2063 616c 6c5f 636f    assert call_co
-0000c3a0: 6e66 6967 2e63 6861 696e 5f70 6174 6820  nfig.chain_path 
-0000c3b0: 3d3d 2074 6573 745f 7574 696c 2e74 656d  == test_util.tem
-0000c3c0: 705f 6a6f 696e 2827 6368 6169 6e27 290a  p_join('chain').
-0000c3d0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000c3e0: 7274 2063 616c 6c5f 636f 6e66 6967 2e6b  rt call_config.k
-0000c3f0: 6579 5f70 6174 6820 3d3d 2074 6573 745f  ey_path == test_
-0000c400: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
-0000c410: 6f76 6572 7269 6469 6e67 5f70 7269 766b  overriding_privk
-0000c420: 6579 2729 0a0a 2020 2020 2020 2020 2020  ey')..          
-0000c430: 2020 6d6f 636b 5f69 6e73 7461 6c6c 2e72    mock_install.r
-0000c440: 6573 6574 2829 0a0a 2020 2020 2020 2020  eset()..        
-0000c450: 2020 2020 7365 6c66 2e5f 6361 6c6c 285b      self._call([
-0000c460: 2769 6e73 7461 6c6c 272c 2027 2d2d 6365  'install', '--ce
-0000c470: 7274 2d6e 616d 6527 2c20 2777 6861 7465  rt-name', 'whate
-0000c480: 7665 7227 2c0a 2020 2020 2020 2020 2020  ver',.          
-0000c490: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-0000c4a0: 2d63 6572 742d 7061 7468 272c 2074 6573  -cert-path', tes
-0000c4b0: 745f 7574 696c 2e74 656d 705f 6a6f 696e  t_util.temp_join
-0000c4c0: 2827 6f76 6572 7269 6469 6e67 5f63 6572  ('overriding_cer
-0000c4d0: 7427 295d 2c20 6d6f 636b 6973 6669 6c65  t')], mockisfile
-0000c4e0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0000c4f0: 2020 2063 616c 6c5f 636f 6e66 6967 203d     call_config =
-0000c500: 206d 6f63 6b5f 696e 7374 616c 6c2e 6361   mock_install.ca
-0000c510: 6c6c 5f61 7267 735b 305d 5b30 5d0a 2020  ll_args[0][0].  
-0000c520: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000c530: 2063 616c 6c5f 636f 6e66 6967 2e63 6572   call_config.cer
-0000c540: 745f 7061 7468 203d 3d20 7465 7374 5f75  t_path == test_u
-0000c550: 7469 6c2e 7465 6d70 5f6a 6f69 6e28 276f  til.temp_join('o
-0000c560: 7665 7272 6964 696e 675f 6365 7274 2729  verriding_cert')
-0000c570: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000c580: 6572 7420 6361 6c6c 5f63 6f6e 6669 672e  ert call_config.
-0000c590: 6675 6c6c 6368 6169 6e5f 7061 7468 203d  fullchain_path =
-0000c5a0: 3d20 7465 7374 5f75 7469 6c2e 7465 6d70  = test_util.temp
-0000c5b0: 5f6a 6f69 6e28 2763 6861 696e 2729 0a20  _join('chain'). 
-0000c5c0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000c5d0: 7420 6361 6c6c 5f63 6f6e 6669 672e 6b65  t call_config.ke
-0000c5e0: 795f 7061 7468 203d 3d20 7465 7374 5f75  y_path == test_u
-0000c5f0: 7469 6c2e 7465 6d70 5f6a 6f69 6e28 2770  til.temp_join('p
-0000c600: 7269 766b 6579 2729 0a0a 2020 2020 406d  rivkey')..    @m
-0000c610: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000c620: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-0000c630: 6e2e 706c 7567 5f73 656c 2e72 6563 6f72  n.plug_sel.recor
-0000c640: 645f 6368 6f73 656e 5f70 6c75 6769 6e73  d_chosen_plugins
-0000c650: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
-0000c660: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0000c670: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
-0000c680: 7365 6c2e 7069 636b 5f69 6e73 7461 6c6c  sel.pick_install
-0000c690: 6572 2729 0a20 2020 2064 6566 2074 6573  er').    def tes
-0000c6a0: 745f 696e 7374 616c 6c65 725f 7061 7261  t_installer_para
-0000c6b0: 6d5f 6572 726f 7228 7365 6c66 2c20 5f69  m_error(self, _i
-0000c6c0: 6e73 742c 205f 7265 6329 3a0a 2020 2020  nst, _rec):.    
-0000c6d0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-0000c6e0: 7261 6973 6573 2865 7272 6f72 732e 436f  raises(errors.Co
-0000c6f0: 6e66 6967 7572 6174 696f 6e45 7272 6f72  nfigurationError
-0000c700: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000c710: 656c 662e 5f63 616c 6c28 5b27 696e 7374  elf._call(['inst
-0000c720: 616c 6c27 2c20 272d 2d63 6572 742d 6e61  all', '--cert-na
-0000c730: 6d65 272c 2027 6e6f 7466 6f75 6e64 272c  me', 'notfound',
-0000c740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c750: 2020 2020 2020 2020 2020 2020 272d 2d6b              '--k
-0000c760: 6579 2d70 6174 6827 2c20 2769 6e76 616c  ey-path', 'inval
-0000c770: 6964 275d 290a 0a20 2020 2040 6d6f 636b  id'])..    @mock
-0000c780: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-0000c790: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e70  _internal.main.p
-0000c7a0: 6c75 675f 7365 6c2e 7265 636f 7264 5f63  lug_sel.record_c
-0000c7b0: 686f 7365 6e5f 706c 7567 696e 7327 290a  hosen_plugins').
-0000c7c0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-0000c7d0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0000c7e0: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
-0000c7f0: 2e70 6963 6b5f 696e 7374 616c 6c65 7227  .pick_installer'
-0000c800: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-0000c810: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-0000c820: 726e 616c 2e63 6572 745f 6d61 6e61 6765  rnal.cert_manage
-0000c830: 722e 6765 745f 6365 7274 6e61 6d65 7327  r.get_certnames'
-0000c840: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-0000c850: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-0000c860: 726e 616c 2e6d 6169 6e2e 5f69 6e73 7461  rnal.main._insta
-0000c870: 6c6c 5f63 6572 7427 290a 2020 2020 6465  ll_cert').    de
-0000c880: 6620 7465 7374 5f69 6e73 7461 6c6c 6572  f test_installer
-0000c890: 5f73 656c 6563 745f 6365 7274 2873 656c  _select_cert(sel
-0000c8a0: 662c 206d 6f63 6b5f 696e 7374 2c20 6d6f  f, mock_inst, mo
-0000c8b0: 636b 5f67 6574 6365 7274 2c20 5f69 6e73  ck_getcert, _ins
-0000c8c0: 742c 205f 7265 6329 3a0a 2020 2020 2020  t, _rec):.      
-0000c8d0: 2020 6d6f 636b 5f6c 696e 6561 6765 203d    mock_lineage =
-0000c8e0: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
-0000c8f0: 6365 7274 5f70 6174 683d 7465 7374 5f75  cert_path=test_u
-0000c900: 7469 6c2e 7465 6d70 5f6a 6f69 6e28 2763  til.temp_join('c
-0000c910: 6572 7427 292c 0a20 2020 2020 2020 2020  ert'),.         
-0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c930: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0000c940: 696e 5f70 6174 683d 7465 7374 5f75 7469  in_path=test_uti
-0000c950: 6c2e 7465 6d70 5f6a 6f69 6e28 2763 6861  l.temp_join('cha
-0000c960: 696e 2729 2c0a 2020 2020 2020 2020 2020  in'),.          
-0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c980: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
-0000c990: 6368 6169 6e5f 7061 7468 3d74 6573 745f  chain_path=test_
-0000c9a0: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
-0000c9b0: 6368 6169 6e27 292c 0a20 2020 2020 2020  chain'),.       
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-0000c9e0: 6579 5f70 6174 683d 7465 7374 5f75 7469  ey_path=test_uti
-0000c9f0: 6c2e 7465 6d70 5f6a 6f69 6e28 2770 7269  l.temp_join('pri
-0000ca00: 766b 6579 2729 290a 2020 2020 2020 2020  vkey')).        
-0000ca10: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
-0000ca20: 2263 6572 7462 6f74 2e5f 696e 7465 726e  "certbot._intern
-0000ca30: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
-0000ca40: 6c69 6e65 6167 655f 666f 725f 6365 7274  lineage_for_cert
-0000ca50: 6e61 6d65 2229 2061 7320 6d6f 636b 5f67  name") as mock_g
-0000ca60: 6574 6c69 6e3a 0a20 2020 2020 2020 2020  etlin:.         
-0000ca70: 2020 206d 6f63 6b5f 6765 746c 696e 2e72     mock_getlin.r
-0000ca80: 6574 7572 6e5f 7661 6c75 6520 3d20 6d6f  eturn_value = mo
-0000ca90: 636b 5f6c 696e 6561 6765 0a20 2020 2020  ck_lineage.     
-0000caa0: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-0000cab0: 6c28 5b27 696e 7374 616c 6c27 5d2c 206d  l(['install'], m
-0000cac0: 6f63 6b69 7366 696c 653d 5472 7565 290a  ockisfile=True).
-0000cad0: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-0000cae0: 6f63 6b5f 6765 7463 6572 742e 6361 6c6c  ock_getcert.call
-0000caf0: 6564 0a20 2020 2020 2020 2061 7373 6572  ed.        asser
-0000cb00: 7420 6d6f 636b 5f69 6e73 742e 6361 6c6c  t mock_inst.call
-0000cb10: 6564 0a0a 2020 2020 406d 6f63 6b2e 7061  ed..    @mock.pa
-0000cb20: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0000cb30: 7465 726e 616c 2e65 6666 2e68 616e 646c  ternal.eff.handl
-0000cb40: 655f 7375 6273 6372 6970 7469 6f6e 2729  e_subscription')
-0000cb50: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-0000cb60: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-0000cb70: 6e61 6c2e 6c6f 672e 706f 7374 5f61 7267  nal.log.post_arg
-0000cb80: 5f70 6172 7365 5f73 6574 7570 2729 0a20  _parse_setup'). 
-0000cb90: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-0000cba0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-0000cbb0: 6c2e 6d61 696e 2e5f 7265 706f 7274 5f6e  l.main._report_n
-0000cbc0: 6577 5f63 6572 7427 290a 2020 2020 406d  ew_cert').    @m
-0000cbd0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000cbe0: 6f74 2e75 7469 6c2e 6578 655f 6578 6973  ot.util.exe_exis
-0000cbf0: 7473 2729 0a20 2020 2064 6566 2074 6573  ts').    def tes
-0000cc00: 745f 636f 6e66 6967 7572 6174 6f72 5f73  t_configurator_s
-0000cc10: 656c 6563 7469 6f6e 2873 656c 662c 206d  election(self, m
-0000cc20: 6f63 6b5f 6578 655f 6578 6973 7473 2c20  ock_exe_exists, 
-0000cc30: 5f2c 205f 5f2c 205f 5f5f 293a 0a20 2020  _, __, ___):.   
-0000cc40: 2020 2020 206d 6f63 6b5f 6578 655f 6578       mock_exe_ex
-0000cc50: 6973 7473 2e72 6574 7572 6e5f 7661 6c75  ists.return_valu
-0000cc60: 6520 3d20 5472 7565 0a20 2020 2020 2020  e = True.       
-0000cc70: 2072 6561 6c5f 706c 7567 696e 7320 3d20   real_plugins = 
-0000cc80: 6469 7363 6f2e 506c 7567 696e 7352 6567  disco.PluginsReg
-0000cc90: 6973 7472 792e 6669 6e64 5f61 6c6c 2829  istry.find_all()
-0000cca0: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-0000ccb0: 5b27 2d2d 6170 6163 6865 272c 2027 2d2d  ['--apache', '--
-0000ccc0: 6175 7468 656e 7469 6361 746f 7227 2c20  authenticator', 
-0000ccd0: 2773 7461 6e64 616c 6f6e 6527 5d0a 0a20  'standalone'].. 
-0000cce0: 2020 2020 2020 2023 2054 6869 7320 6e65         # This ne
-0000ccf0: 6564 6564 2074 776f 2063 616c 6c73 2074  eded two calls t
-0000cd00: 6f20 6669 6e64 5f61 6c6c 2829 2c20 7768  o find_all(), wh
-0000cd10: 6963 6820 7765 2772 6520 6176 6f69 6469  ich we're avoidi
-0000cd20: 6e67 2066 6f72 206e 6f77 0a20 2020 2020  ng for now.     
-0000cd30: 2020 2023 2062 6563 6175 7365 206f 6620     # because of 
-0000cd40: 706f 7373 6962 6c65 2073 6964 6520 6566  possible side ef
-0000cd50: 6665 6374 733a 0a20 2020 2020 2020 2023  fects:.        #
-0000cd60: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-0000cd70: 636f 6d2f 6365 7274 626f 742f 6365 7274  com/certbot/cert
-0000cd80: 626f 742f 636f 6d6d 6974 2f35 3165 6432  bot/commit/51ed2
-0000cd90: 6236 3831 6638 3762 3165 6232 3930 3838  b681f87b1eb29088
-0000cda0: 6464 3438 3731 3861 3534 6634 3031 6534  dd48718a54f401e4
-0000cdb0: 3835 350a 2020 2020 2020 2020 2320 7769  855.        # wi
-0000cdc0: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-0000cdd0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-0000cde0: 2e63 6c69 2e70 6c75 6769 6e73 5f74 6573  .cli.plugins_tes
-0000cdf0: 7461 626c 6527 2920 6173 2070 6c75 6769  table') as plugi
-0000ce00: 6e73 3a0a 2020 2020 2020 2020 2320 2020  ns:.        #   
-0000ce10: 2070 6c75 6769 6e73 2e72 6574 7572 6e5f   plugins.return_
-0000ce20: 7661 6c75 6520 3d20 7b22 6170 6163 6865  value = {"apache
-0000ce30: 223a 2054 7275 652c 2022 6e67 696e 7822  ": True, "nginx"
-0000ce40: 3a20 5472 7565 7d0a 2020 2020 2020 2020  : True}.        
-0000ce50: 2320 2020 2072 6574 2c20 5f2c 205f 2c20  #    ret, _, _, 
-0000ce60: 5f20 3d20 7365 6c66 2e5f 6361 6c6c 2861  _ = self._call(a
-0000ce70: 7267 7329 0a20 2020 2020 2020 2023 2020  rgs).        #  
-0000ce80: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-0000ce90: 6528 2254 6f6f 206d 616e 7920 666c 6167  e("Too many flag
-0000cea0: 7320 7365 7474 696e 6722 2069 6e20 7265  s setting" in re
-0000ceb0: 7429 0a0a 2020 2020 2020 2020 6172 6773  t)..        args
-0000cec0: 203d 205b 2269 6e73 7461 6c6c 222c 2022   = ["install", "
-0000ced0: 2d2d 6e67 696e 7822 2c20 222d 2d63 6572  --nginx", "--cer
-0000cee0: 742d 7061 7468 222c 0a20 2020 2020 2020  t-path",.       
-0000cef0: 2020 2020 2020 2020 2074 6573 745f 7574           test_ut
-0000cf00: 696c 2e74 656d 705f 6a6f 696e 2827 626c  il.temp_join('bl
-0000cf10: 6168 2729 2c20 222d 2d6b 6579 2d70 6174  ah'), "--key-pat
-0000cf20: 6822 2c20 7465 7374 5f75 7469 6c2e 7465  h", test_util.te
-0000cf30: 6d70 5f6a 6f69 6e28 2762 6c61 6827 292c  mp_join('blah'),
-0000cf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf50: 2022 2d2d 6e67 696e 782d 7365 7276 6572   "--nginx-server
-0000cf60: 2d72 6f6f 7422 2c20 222f 6e6f 6e65 7869  -root", "/nonexi
-0000cf70: 7374 656e 742f 7468 696e 6722 2c20 222d  stent/thing", "-
-0000cf80: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-0000cf90: 2020 2020 2265 7861 6d70 6c65 2e63 6f6d      "example.com
-0000cfa0: 222c 2022 2d2d 6465 6275 6722 5d0a 2020  ", "--debug"].  
-0000cfb0: 2020 2020 2020 6966 2022 6e67 696e 7822        if "nginx"
-0000cfc0: 2069 6e20 7265 616c 5f70 6c75 6769 6e73   in real_plugins
-0000cfd0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000cfe0: 5365 6e64 696e 6720 6e67 696e 7820 6120  Sending nginx a 
-0000cff0: 6e6f 6e2d 6578 6973 7465 6e74 2063 6f6e  non-existent con
-0000d000: 6620 6469 7220 7769 6c6c 2073 696d 756c  f dir will simul
-0000d010: 6174 6520 6d69 7363 6f6e 6669 6775 7261  ate misconfigura
-0000d020: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0000d030: 2023 2028 7765 2063 616e 206f 6e6c 7920   # (we can only 
-0000d040: 646f 2074 6861 7420 6966 2063 6572 7462  do that if certb
-0000d050: 6f74 2d6e 6769 6e78 2069 7320 6163 7475  ot-nginx is actu
-0000d060: 616c 6c79 2070 7265 7365 6e74 290a 2020  ally present).  
-0000d070: 2020 2020 2020 2020 2020 7265 742c 205f            ret, _
-0000d080: 2c20 5f2c 205f 203d 2073 656c 662e 5f63  , _, _ = self._c
-0000d090: 616c 6c28 6172 6773 290a 2020 2020 2020  all(args).      
-0000d0a0: 2020 2020 2020 6173 7365 7274 2022 5468        assert "Th
-0000d0b0: 6520 6e67 696e 7820 706c 7567 696e 2069  e nginx plugin i
-0000d0c0: 7320 6e6f 7420 776f 726b 696e 6722 2069  s not working" i
-0000d0d0: 6e20 7265 740a 2020 2020 2020 2020 2020  n ret.          
-0000d0e0: 2020 6173 7365 7274 2022 4d69 7363 6f6e    assert "Miscon
-0000d0f0: 6669 6775 7261 7469 6f6e 4572 726f 7222  figurationError"
-0000d100: 2069 6e20 7265 740a 0a20 2020 2020 2020   in ret..       
-0000d110: 2073 656c 662e 5f63 6c69 5f6d 6973 7369   self._cli_missi
-0000d120: 6e67 5f66 6c61 6728 5b22 2d2d 7374 616e  ng_flag(["--stan
-0000d130: 6461 6c6f 6e65 225d 2c20 2257 6974 6820  dalone"], "With 
-0000d140: 7468 6520 7374 616e 6461 6c6f 6e65 2070  the standalone p
-0000d150: 6c75 6769 6e2c 2079 6f75 2070 726f 6261  lugin, you proba
-0000d160: 626c 7922 290a 0a20 2020 2020 2020 2077  bly")..        w
-0000d170: 6974 6820 6d6f 636b 2e70 6174 6368 2822  ith mock.patch("
-0000d180: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-0000d190: 6c2e 6d61 696e 2e5f 696e 6974 5f6c 655f  l.main._init_le_
-0000d1a0: 636c 6965 6e74 2229 2061 7320 6d6f 636b  client") as mock
-0000d1b0: 5f69 6e69 743a 0a20 2020 2020 2020 2020  _init:.         
-0000d1c0: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
-0000d1d0: 6368 2822 6365 7274 626f 742e 5f69 6e74  ch("certbot._int
-0000d1e0: 6572 6e61 6c2e 6d61 696e 2e5f 6765 745f  ernal.main._get_
-0000d1f0: 616e 645f 7361 7665 5f63 6572 7422 2920  and_save_cert") 
-0000d200: 6173 206d 6f63 6b5f 6773 633a 0a20 2020  as mock_gsc:.   
-0000d210: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
-0000d220: 6b5f 6773 632e 7265 7475 726e 5f76 616c  k_gsc.return_val
-0000d230: 7565 203d 206d 6f63 6b2e 4d61 6769 634d  ue = mock.MagicM
-0000d240: 6f63 6b28 290a 2020 2020 2020 2020 2020  ock().          
-0000d250: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
-0000d260: 285b 2263 6572 746f 6e6c 7922 2c20 222d  (["certonly", "-
-0000d270: 2d6d 616e 7561 6c22 2c20 222d 6422 2c20  -manual", "-d", 
-0000d280: 2266 6f6f 2e62 6172 225d 290a 2020 2020  "foo.bar"]).    
-0000d290: 2020 2020 2020 2020 2020 2020 756e 7573              unus
-0000d2a0: 6564 5f63 6f6e 6669 672c 2061 7574 682c  ed_config, auth,
-0000d2b0: 2075 6e75 7365 645f 696e 7374 616c 6c65   unused_installe
-0000d2c0: 7220 3d20 6d6f 636b 5f69 6e69 742e 6361  r = mock_init.ca
-0000d2d0: 6c6c 5f61 7267 735b 305d 0a20 2020 2020  ll_args[0].     
-0000d2e0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000d2f0: 7420 6973 696e 7374 616e 6365 2861 7574  t isinstance(aut
-0000d300: 682c 206d 616e 7561 6c2e 4175 7468 656e  h, manual.Authen
-0000d310: 7469 6361 746f 7229 0a0a 2020 2020 2020  ticator)..      
-0000d320: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
-0000d330: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-0000d340: 726e 616c 2e6d 6169 6e2e 6365 7274 6f6e  rnal.main.certon
-0000d350: 6c79 2729 2061 7320 6d6f 636b 5f63 6572  ly') as mock_cer
-0000d360: 746f 6e6c 793a 0a20 2020 2020 2020 2020  tonly:.         
-0000d370: 2020 2073 656c 662e 5f63 616c 6c28 5b22     self._call(["
-0000d380: 6175 7468 222c 2022 2d2d 7374 616e 6461  auth", "--standa
-0000d390: 6c6f 6e65 225d 290a 2020 2020 2020 2020  lone"]).        
-0000d3a0: 2020 2020 6173 7365 7274 2031 203d 3d20      assert 1 == 
-0000d3b0: 6d6f 636b 5f63 6572 746f 6e6c 792e 6361  mock_certonly.ca
-0000d3c0: 6c6c 5f63 6f75 6e74 0a0a 2020 2020 406d  ll_count..    @m
-0000d3d0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000d3e0: 6f74 2e5f 696e 7465 726e 616c 2e6c 6f67  ot._internal.log
-0000d3f0: 2e70 6f73 745f 6172 675f 7061 7273 655f  .post_arg_parse_
-0000d400: 7365 7475 7027 290a 2020 2020 6465 6620  setup').    def 
-0000d410: 7465 7374 5f72 6f6c 6c62 6163 6b28 7365  test_rollback(se
-0000d420: 6c66 2c20 5f29 3a0a 2020 2020 2020 2020  lf, _):.        
-0000d430: 5f2c 205f 2c20 5f2c 2063 6c69 656e 7420  _, _, _, client 
-0000d440: 3d20 7365 6c66 2e5f 6361 6c6c 285b 2772  = self._call(['r
-0000d450: 6f6c 6c62 6163 6b27 5d29 0a20 2020 2020  ollback']).     
-0000d460: 2020 2061 7373 6572 7420 3120 3d3d 2063     assert 1 == c
-0000d470: 6c69 656e 742e 726f 6c6c 6261 636b 2e63  lient.rollback.c
-0000d480: 616c 6c5f 636f 756e 740a 0a20 2020 2020  all_count..     
-0000d490: 2020 205f 2c20 5f2c 205f 2c20 636c 6965     _, _, _, clie
-0000d4a0: 6e74 203d 2073 656c 662e 5f63 616c 6c28  nt = self._call(
-0000d4b0: 5b27 726f 6c6c 6261 636b 272c 2027 2d2d  ['rollback', '--
-0000d4c0: 6368 6563 6b70 6f69 6e74 7327 2c20 2731  checkpoints', '1
-0000d4d0: 3233 275d 290a 2020 2020 2020 2020 636c  23']).        cl
-0000d4e0: 6965 6e74 2e72 6f6c 6c62 6163 6b2e 6173  ient.rollback.as
-0000d4f0: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
-0000d500: 5f77 6974 6828 0a20 2020 2020 2020 2020  _with(.         
-0000d510: 2020 206d 6f63 6b2e 414e 592c 2031 3233     mock.ANY, 123
-0000d520: 2c20 6d6f 636b 2e41 4e59 2c20 6d6f 636b  , mock.ANY, mock
-0000d530: 2e41 4e59 290a 0a20 2020 2040 6d6f 636b  .ANY)..    @mock
-0000d540: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-0000d550: 5f69 6e74 6572 6e61 6c2e 6365 7274 5f6d  _internal.cert_m
-0000d560: 616e 6167 6572 2e75 7064 6174 655f 6c69  anager.update_li
-0000d570: 7665 5f73 796d 6c69 6e6b 7327 290a 2020  ve_symlinks').  
-0000d580: 2020 6465 6620 7465 7374 5f75 7064 6174    def test_updat
-0000d590: 655f 7379 6d6c 696e 6b73 2873 656c 662c  e_symlinks(self,
-0000d5a0: 206d 6f63 6b5f 6365 7274 5f6d 616e 6167   mock_cert_manag
-0000d5b0: 6572 293a 0a20 2020 2020 2020 2073 656c  er):.        sel
-0000d5c0: 662e 5f63 616c 6c5f 6e6f 5f63 6c69 656e  f._call_no_clien
-0000d5d0: 746d 6f63 6b28 5b27 7570 6461 7465 5f73  tmock(['update_s
-0000d5e0: 796d 6c69 6e6b 7327 5d29 0a20 2020 2020  ymlinks']).     
-0000d5f0: 2020 2061 7373 6572 7420 3120 3d3d 206d     assert 1 == m
-0000d600: 6f63 6b5f 6365 7274 5f6d 616e 6167 6572  ock_cert_manager
-0000d610: 2e63 616c 6c5f 636f 756e 740a 0a20 2020  .call_count..   
-0000d620: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000d630: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000d640: 6365 7274 5f6d 616e 6167 6572 2e63 6572  cert_manager.cer
-0000d650: 7469 6669 6361 7465 7327 290a 2020 2020  tificates').    
-0000d660: 6465 6620 7465 7374 5f63 6572 7469 6669  def test_certifi
-0000d670: 6361 7465 7328 7365 6c66 2c20 6d6f 636b  cates(self, mock
-0000d680: 5f63 6572 745f 6d61 6e61 6765 7229 3a0a  _cert_manager):.
-0000d690: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-0000d6a0: 6c6c 5f6e 6f5f 636c 6965 6e74 6d6f 636b  ll_no_clientmock
-0000d6b0: 285b 2763 6572 7469 6669 6361 7465 7327  (['certificates'
-0000d6c0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0000d6d0: 7420 3120 3d3d 206d 6f63 6b5f 6365 7274  t 1 == mock_cert
-0000d6e0: 5f6d 616e 6167 6572 2e63 616c 6c5f 636f  _manager.call_co
-0000d6f0: 756e 740a 0a20 2020 2040 6d6f 636b 2e70  unt..    @mock.p
-0000d700: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-0000d710: 6e74 6572 6e61 6c2e 6365 7274 5f6d 616e  nternal.cert_man
-0000d720: 6167 6572 2e64 656c 6574 6527 290a 2020  ager.delete').  
-0000d730: 2020 6465 6620 7465 7374 5f64 656c 6574    def test_delet
-0000d740: 6528 7365 6c66 2c20 6d6f 636b 5f63 6572  e(self, mock_cer
-0000d750: 745f 6d61 6e61 6765 7229 3a0a 2020 2020  t_manager):.    
-0000d760: 2020 2020 7365 6c66 2e5f 6361 6c6c 5f6e      self._call_n
-0000d770: 6f5f 636c 6965 6e74 6d6f 636b 285b 2764  o_clientmock(['d
-0000d780: 656c 6574 6527 5d29 0a20 2020 2020 2020  elete']).       
-0000d790: 2061 7373 6572 7420 3120 3d3d 206d 6f63   assert 1 == moc
-0000d7a0: 6b5f 6365 7274 5f6d 616e 6167 6572 2e63  k_cert_manager.c
-0000d7b0: 616c 6c5f 636f 756e 740a 0a20 2020 2040  all_count..    @
-0000d7c0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-0000d7d0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-0000d7e0: 696e 2e70 6c75 6769 6e73 5f64 6973 636f  in.plugins_disco
-0000d7f0: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
-0000d800: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0000d810: 6572 6e61 6c2e 6d61 696e 2e63 6c69 2e48  ernal.main.cli.H
-0000d820: 656c 7066 756c 4172 6775 6d65 6e74 5061  elpfulArgumentPa
-0000d830: 7273 6572 2e64 6574 6572 6d69 6e65 5f68  rser.determine_h
-0000d840: 656c 705f 746f 7069 6373 2729 0a20 2020  elp_topics').   
-0000d850: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000d860: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000d870: 6c6f 672e 706f 7374 5f61 7267 5f70 6172  log.post_arg_par
-0000d880: 7365 5f73 6574 7570 2729 0a20 2020 2064  se_setup').    d
-0000d890: 6566 2074 6573 745f 706c 7567 696e 7328  ef test_plugins(
-0000d8a0: 7365 6c66 2c20 5f2c 205f 6465 742c 206d  self, _, _det, m
-0000d8b0: 6f63 6b5f 6469 7363 6f29 3a0a 2020 2020  ock_disco):.    
-0000d8c0: 2020 2020 666c 6167 7320 3d20 5b27 2d2d      flags = ['--
-0000d8d0: 696e 6974 272c 2027 2d2d 7072 6570 6172  init', '--prepar
-0000d8e0: 6527 2c20 272d 2d61 7574 6865 6e74 6963  e', '--authentic
-0000d8f0: 6174 6f72 7327 2c20 272d 2d69 6e73 7461  ators', '--insta
-0000d900: 6c6c 6572 7327 5d0a 2020 2020 2020 2020  llers'].        
-0000d910: 666f 7220 6172 6773 2069 6e20 6974 6572  for args in iter
-0000d920: 746f 6f6c 732e 6368 6169 6e28 0a20 2020  tools.chain(.   
-0000d930: 2020 2020 2020 2020 2020 2020 202a 2869               *(i
-0000d940: 7465 7274 6f6f 6c73 2e63 6f6d 6269 6e61  tertools.combina
-0000d950: 7469 6f6e 7328 666c 6167 732c 2072 290a  tions(flags, r).
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 2020 666f 7220 7220 696e 2072 616e 6765    for r in range
-0000d980: 286c 656e 2866 6c61 6773 2929 2929 3a0a  (len(flags)))):.
-0000d990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d9a0: 2e5f 6361 6c6c 285b 2770 6c75 6769 6e73  ._call(['plugins
-0000d9b0: 275d 202b 206c 6973 7428 6172 6773 2929  '] + list(args))
-0000d9c0: 0a0a 2020 2020 406d 6f63 6b2e 7061 7463  ..    @mock.patc
-0000d9d0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-0000d9e0: 726e 616c 2e6d 6169 6e2e 706c 7567 696e  rnal.main.plugin
-0000d9f0: 735f 6469 7363 6f27 290a 2020 2020 406d  s_disco').    @m
-0000da00: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000da10: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-0000da20: 6e2e 636c 692e 4865 6c70 6675 6c41 7267  n.cli.HelpfulArg
-0000da30: 756d 656e 7450 6172 7365 722e 6465 7465  umentParser.dete
-0000da40: 726d 696e 655f 6865 6c70 5f74 6f70 6963  rmine_help_topic
-0000da50: 7327 290a 2020 2020 6465 6620 7465 7374  s').    def test
-0000da60: 5f70 6c75 6769 6e73 5f6e 6f5f 6172 6773  _plugins_no_args
-0000da70: 2873 656c 662c 205f 6465 742c 206d 6f63  (self, _det, moc
-0000da80: 6b5f 6469 7363 6f29 3a0a 2020 2020 2020  k_disco):.      
-0000da90: 2020 6966 6163 6573 3a20 4c69 7374 5b69    ifaces: List[i
-0000daa0: 6e74 6572 6661 6365 732e 506c 7567 696e  nterfaces.Plugin
-0000dab0: 5d20 3d20 5b5d 0a20 2020 2020 2020 2070  ] = [].        p
-0000dac0: 6c75 6769 6e73 203d 206d 6f63 6b5f 6469  lugins = mock_di
-0000dad0: 7363 6f2e 506c 7567 696e 7352 6567 6973  sco.PluginsRegis
-0000dae0: 7472 792e 6669 6e64 5f61 6c6c 2829 0a0a  try.find_all()..
-0000daf0: 2020 2020 2020 2020 7374 646f 7574 203d          stdout =
-0000db00: 2069 6f2e 5374 7269 6e67 494f 2829 0a20   io.StringIO(). 
-0000db10: 2020 2020 2020 2077 6974 6820 7465 7374         with test
-0000db20: 5f75 7469 6c2e 7061 7463 685f 6469 7370  _util.patch_disp
-0000db30: 6c61 795f 7574 696c 5f77 6974 685f 7374  lay_util_with_st
-0000db40: 646f 7574 2873 7464 6f75 743d 7374 646f  dout(stdout=stdo
-0000db50: 7574 293a 0a20 2020 2020 2020 2020 2020  ut):.           
-0000db60: 205f 2c20 7374 646f 7574 2c20 5f2c 205f   _, stdout, _, _
-0000db70: 203d 2073 656c 662e 5f63 616c 6c28 5b27   = self._call(['
-0000db80: 706c 7567 696e 7327 5d2c 2073 7464 6f75  plugins'], stdou
-0000db90: 7429 0a0a 2020 2020 2020 2020 706c 7567  t)..        plug
-0000dba0: 696e 732e 7669 7369 626c 652e 6173 7365  ins.visible.asse
-0000dbb0: 7274 5f63 616c 6c65 645f 6f6e 6365 5f77  rt_called_once_w
-0000dbc0: 6974 6828 290a 2020 2020 2020 2020 706c  ith().        pl
-0000dbd0: 7567 696e 732e 7669 7369 626c 6528 292e  ugins.visible().
-0000dbe0: 6966 6163 6573 2e61 7373 6572 745f 6361  ifaces.assert_ca
-0000dbf0: 6c6c 6564 5f6f 6e63 655f 7769 7468 2869  lled_once_with(i
-0000dc00: 6661 6365 7329 0a20 2020 2020 2020 2066  faces).        f
-0000dc10: 696c 7465 7265 6420 3d20 706c 7567 696e  iltered = plugin
-0000dc20: 732e 7669 7369 626c 6528 292e 6966 6163  s.visible().ifac
-0000dc30: 6573 2829 0a20 2020 2020 2020 2061 7373  es().        ass
-0000dc40: 6572 7420 7374 646f 7574 2e67 6574 7661  ert stdout.getva
-0000dc50: 6c75 6528 292e 7374 7269 7028 2920 3d3d  lue().strip() ==
-0000dc60: 2073 7472 2866 696c 7465 7265 6429 0a0a   str(filtered)..
-0000dc70: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-0000dc80: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0000dc90: 616c 2e6d 6169 6e2e 706c 7567 696e 735f  al.main.plugins_
-0000dca0: 6469 7363 6f27 290a 2020 2020 406d 6f63  disco').    @moc
-0000dcb0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-0000dcc0: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-0000dcd0: 636c 692e 4865 6c70 6675 6c41 7267 756d  cli.HelpfulArgum
-0000dce0: 656e 7450 6172 7365 722e 6465 7465 726d  entParser.determ
-0000dcf0: 696e 655f 6865 6c70 5f74 6f70 6963 7327  ine_help_topics'
-0000dd00: 290a 2020 2020 6465 6620 7465 7374 5f70  ).    def test_p
-0000dd10: 6c75 6769 6e73 5f6e 6f5f 6172 6773 5f75  lugins_no_args_u
-0000dd20: 6e70 7269 7669 6c65 6765 6428 7365 6c66  nprivileged(self
-0000dd30: 2c20 5f64 6574 2c20 6d6f 636b 5f64 6973  , _det, mock_dis
-0000dd40: 636f 293a 0a20 2020 2020 2020 2069 6661  co):.        ifa
-0000dd50: 6365 733a 204c 6973 745b 696e 7465 7266  ces: List[interf
-0000dd60: 6163 6573 2e50 6c75 6769 6e5d 203d 205b  aces.Plugin] = [
-0000dd70: 5d0a 2020 2020 2020 2020 706c 7567 696e  ].        plugin
-0000dd80: 7320 3d20 6d6f 636b 5f64 6973 636f 2e50  s = mock_disco.P
-0000dd90: 6c75 6769 6e73 5265 6769 7374 7279 2e66  luginsRegistry.f
-0000dda0: 696e 645f 616c 6c28 290a 0a20 2020 2020  ind_all()..     
-0000ddb0: 2020 2064 6566 2074 6872 6f77 5f65 7272     def throw_err
-0000ddc0: 6f72 2864 6972 6563 746f 7279 2c20 6d6f  or(directory, mo
-0000ddd0: 6465 2c20 7374 7269 6374 293a 0a20 2020  de, strict):.   
-0000dde0: 2020 2020 2020 2020 2022 2222 5261 6973           """Rais
-0000ddf0: 6573 2065 7272 6f72 2e45 7272 6f72 2e22  es error.Error."
-0000de00: 2222 0a20 2020 2020 2020 2020 2020 205f  "".            _
-0000de10: 2c20 5f2c 205f 203d 2064 6972 6563 746f  , _, _ = directo
-0000de20: 7279 2c20 6d6f 6465 2c20 7374 7269 6374  ry, mode, strict
-0000de30: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000de40: 7365 2065 7272 6f72 732e 4572 726f 7228  se errors.Error(
-0000de50: 290a 0a20 2020 2020 2020 2073 7464 6f75  )..        stdou
-0000de60: 7420 3d20 696f 2e53 7472 696e 6749 4f28  t = io.StringIO(
-0000de70: 290a 2020 2020 2020 2020 7769 7468 206d  ).        with m
-0000de80: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000de90: 6f74 2e75 7469 6c2e 7365 745f 7570 5f63  ot.util.set_up_c
-0000dea0: 6f72 655f 6469 7227 2920 6173 206d 6f63  ore_dir') as moc
-0000deb0: 6b5f 7365 745f 7570 5f63 6f72 655f 6469  k_set_up_core_di
-0000dec0: 723a 0a20 2020 2020 2020 2020 2020 2077  r:.            w
-0000ded0: 6974 6820 7465 7374 5f75 7469 6c2e 7061  ith test_util.pa
-0000dee0: 7463 685f 6469 7370 6c61 795f 7574 696c  tch_display_util
-0000def0: 5f77 6974 685f 7374 646f 7574 2873 7464  _with_stdout(std
-0000df00: 6f75 743d 7374 646f 7574 293a 0a20 2020  out=stdout):.   
-0000df10: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
-0000df20: 6b5f 7365 745f 7570 5f63 6f72 655f 6469  k_set_up_core_di
-0000df30: 722e 7369 6465 5f65 6666 6563 7420 3d20  r.side_effect = 
-0000df40: 7468 726f 775f 6572 726f 720a 2020 2020  throw_error.    
-0000df50: 2020 2020 2020 2020 2020 2020 5f2c 2073              _, s
-0000df60: 7464 6f75 742c 205f 2c20 5f20 3d20 7365  tdout, _, _ = se
-0000df70: 6c66 2e5f 6361 6c6c 285b 2770 6c75 6769  lf._call(['plugi
-0000df80: 6e73 275d 2c20 7374 646f 7574 290a 0a20  ns'], stdout).. 
-0000df90: 2020 2020 2020 2070 6c75 6769 6e73 2e76         plugins.v
-0000dfa0: 6973 6962 6c65 2e61 7373 6572 745f 6361  isible.assert_ca
-0000dfb0: 6c6c 6564 5f6f 6e63 655f 7769 7468 2829  lled_once_with()
-0000dfc0: 0a20 2020 2020 2020 2070 6c75 6769 6e73  .        plugins
-0000dfd0: 2e76 6973 6962 6c65 2829 2e69 6661 6365  .visible().iface
-0000dfe0: 732e 6173 7365 7274 5f63 616c 6c65 645f  s.assert_called_
-0000dff0: 6f6e 6365 5f77 6974 6828 6966 6163 6573  once_with(ifaces
-0000e000: 290a 2020 2020 2020 2020 6669 6c74 6572  ).        filter
-0000e010: 6564 203d 2070 6c75 6769 6e73 2e76 6973  ed = plugins.vis
-0000e020: 6962 6c65 2829 2e69 6661 6365 7328 290a  ible().ifaces().
-0000e030: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-0000e040: 7464 6f75 742e 6765 7476 616c 7565 2829  tdout.getvalue()
-0000e050: 2e73 7472 6970 2829 203d 3d20 7374 7228  .strip() == str(
-0000e060: 6669 6c74 6572 6564 290a 0a20 2020 2040  filtered)..    @
-0000e070: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-0000e080: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-0000e090: 696e 2e70 6c75 6769 6e73 5f64 6973 636f  in.plugins_disco
-0000e0a0: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
-0000e0b0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0000e0c0: 6572 6e61 6c2e 6d61 696e 2e63 6c69 2e48  ernal.main.cli.H
-0000e0d0: 656c 7066 756c 4172 6775 6d65 6e74 5061  elpfulArgumentPa
-0000e0e0: 7273 6572 2e64 6574 6572 6d69 6e65 5f68  rser.determine_h
-0000e0f0: 656c 705f 746f 7069 6373 2729 0a20 2020  elp_topics').   
-0000e100: 2064 6566 2074 6573 745f 706c 7567 696e   def test_plugin
-0000e110: 735f 696e 6974 2873 656c 662c 205f 6465  s_init(self, _de
-0000e120: 742c 206d 6f63 6b5f 6469 7363 6f29 3a0a  t, mock_disco):.
-0000e130: 2020 2020 2020 2020 6966 6163 6573 3a20          ifaces: 
-0000e140: 4c69 7374 5b69 6e74 6572 6661 6365 732e  List[interfaces.
-0000e150: 506c 7567 696e 5d20 3d20 5b5d 0a20 2020  Plugin] = [].   
-0000e160: 2020 2020 2070 6c75 6769 6e73 203d 206d       plugins = m
-0000e170: 6f63 6b5f 6469 7363 6f2e 506c 7567 696e  ock_disco.Plugin
-0000e180: 7352 6567 6973 7472 792e 6669 6e64 5f61  sRegistry.find_a
-0000e190: 6c6c 2829 0a0a 2020 2020 2020 2020 7374  ll()..        st
-0000e1a0: 646f 7574 203d 2069 6f2e 5374 7269 6e67  dout = io.String
-0000e1b0: 494f 2829 0a20 2020 2020 2020 2077 6974  IO().        wit
-0000e1c0: 6820 7465 7374 5f75 7469 6c2e 7061 7463  h test_util.patc
-0000e1d0: 685f 6469 7370 6c61 795f 7574 696c 5f77  h_display_util_w
-0000e1e0: 6974 685f 7374 646f 7574 2873 7464 6f75  ith_stdout(stdou
-0000e1f0: 743d 7374 646f 7574 293a 0a20 2020 2020  t=stdout):.     
-0000e200: 2020 2020 2020 205f 2c20 7374 646f 7574         _, stdout
-0000e210: 2c20 5f2c 205f 203d 2073 656c 662e 5f63  , _, _ = self._c
-0000e220: 616c 6c28 5b27 706c 7567 696e 7327 2c20  all(['plugins', 
-0000e230: 272d 2d69 6e69 7427 5d2c 2073 7464 6f75  '--init'], stdou
-0000e240: 7429 0a0a 2020 2020 2020 2020 706c 7567  t)..        plug
-0000e250: 696e 732e 7669 7369 626c 652e 6173 7365  ins.visible.asse
-0000e260: 7274 5f63 616c 6c65 645f 6f6e 6365 5f77  rt_called_once_w
-0000e270: 6974 6828 290a 2020 2020 2020 2020 706c  ith().        pl
-0000e280: 7567 696e 732e 7669 7369 626c 6528 292e  ugins.visible().
-0000e290: 6966 6163 6573 2e61 7373 6572 745f 6361  ifaces.assert_ca
-0000e2a0: 6c6c 6564 5f6f 6e63 655f 7769 7468 2869  lled_once_with(i
-0000e2b0: 6661 6365 7329 0a20 2020 2020 2020 2066  faces).        f
-0000e2c0: 696c 7465 7265 6420 3d20 706c 7567 696e  iltered = plugin
-0000e2d0: 732e 7669 7369 626c 6528 292e 6966 6163  s.visible().ifac
-0000e2e0: 6573 2829 0a20 2020 2020 2020 2061 7373  es().        ass
-0000e2f0: 6572 7420 6669 6c74 6572 6564 2e69 6e69  ert filtered.ini
-0000e300: 742e 6361 6c6c 5f63 6f75 6e74 203d 3d20  t.call_count == 
-0000e310: 310a 2020 2020 2020 2020 6173 7365 7274  1.        assert
-0000e320: 2073 7464 6f75 742e 6765 7476 616c 7565   stdout.getvalue
-0000e330: 2829 2e73 7472 6970 2829 203d 3d20 7374  ().strip() == st
-0000e340: 7228 6669 6c74 6572 6564 290a 0a20 2020  r(filtered)..   
-0000e350: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000e360: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000e370: 6d61 696e 2e70 6c75 6769 6e73 5f64 6973  main.plugins_dis
-0000e380: 636f 2729 0a20 2020 2040 6d6f 636b 2e70  co').    @mock.p
-0000e390: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-0000e3a0: 6e74 6572 6e61 6c2e 6d61 696e 2e63 6c69  nternal.main.cli
-0000e3b0: 2e48 656c 7066 756c 4172 6775 6d65 6e74  .HelpfulArgument
-0000e3c0: 5061 7273 6572 2e64 6574 6572 6d69 6e65  Parser.determine
-0000e3d0: 5f68 656c 705f 746f 7069 6373 2729 0a20  _help_topics'). 
-0000e3e0: 2020 2064 6566 2074 6573 745f 706c 7567     def test_plug
-0000e3f0: 696e 735f 7072 6570 6172 6528 7365 6c66  ins_prepare(self
-0000e400: 2c20 5f64 6574 2c20 6d6f 636b 5f64 6973  , _det, mock_dis
-0000e410: 636f 293a 0a20 2020 2020 2020 2069 6661  co):.        ifa
-0000e420: 6365 733a 204c 6973 745b 696e 7465 7266  ces: List[interf
-0000e430: 6163 6573 2e50 6c75 6769 6e5d 203d 205b  aces.Plugin] = [
-0000e440: 5d0a 2020 2020 2020 2020 706c 7567 696e  ].        plugin
-0000e450: 7320 3d20 6d6f 636b 5f64 6973 636f 2e50  s = mock_disco.P
-0000e460: 6c75 6769 6e73 5265 6769 7374 7279 2e66  luginsRegistry.f
-0000e470: 696e 645f 616c 6c28 290a 0a20 2020 2020  ind_all()..     
-0000e480: 2020 2073 7464 6f75 7420 3d20 696f 2e53     stdout = io.S
-0000e490: 7472 696e 6749 4f28 290a 2020 2020 2020  tringIO().      
-0000e4a0: 2020 7769 7468 2074 6573 745f 7574 696c    with test_util
-0000e4b0: 2e70 6174 6368 5f64 6973 706c 6179 5f75  .patch_display_u
-0000e4c0: 7469 6c5f 7769 7468 5f73 7464 6f75 7428  til_with_stdout(
-0000e4d0: 7374 646f 7574 3d73 7464 6f75 7429 3a0a  stdout=stdout):.
-0000e4e0: 2020 2020 2020 2020 2020 2020 5f2c 2073              _, s
-0000e4f0: 7464 6f75 742c 205f 2c20 5f20 3d20 7365  tdout, _, _ = se
-0000e500: 6c66 2e5f 6361 6c6c 285b 2770 6c75 6769  lf._call(['plugi
-0000e510: 6e73 272c 2027 2d2d 696e 6974 272c 2027  ns', '--init', '
-0000e520: 2d2d 7072 6570 6172 6527 5d2c 2073 7464  --prepare'], std
-0000e530: 6f75 7429 0a0a 2020 2020 2020 2020 706c  out)..        pl
-0000e540: 7567 696e 732e 7669 7369 626c 652e 6173  ugins.visible.as
-0000e550: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
-0000e560: 5f77 6974 6828 290a 2020 2020 2020 2020  _with().        
-0000e570: 706c 7567 696e 732e 7669 7369 626c 6528  plugins.visible(
-0000e580: 292e 6966 6163 6573 2e61 7373 6572 745f  ).ifaces.assert_
-0000e590: 6361 6c6c 6564 5f6f 6e63 655f 7769 7468  called_once_with
-0000e5a0: 2869 6661 6365 7329 0a20 2020 2020 2020  (ifaces).       
-0000e5b0: 2066 696c 7465 7265 6420 3d20 706c 7567   filtered = plug
-0000e5c0: 696e 732e 7669 7369 626c 6528 292e 6966  ins.visible().if
-0000e5d0: 6163 6573 2829 0a20 2020 2020 2020 2061  aces().        a
-0000e5e0: 7373 6572 7420 6669 6c74 6572 6564 2e69  ssert filtered.i
-0000e5f0: 6e69 742e 6361 6c6c 5f63 6f75 6e74 203d  nit.call_count =
-0000e600: 3d20 310a 2020 2020 2020 2020 6669 6c74  = 1.        filt
-0000e610: 6572 6564 2e70 7265 7061 7265 2e61 7373  ered.prepare.ass
-0000e620: 6572 745f 6361 6c6c 6564 5f6f 6e63 655f  ert_called_once_
-0000e630: 7769 7468 2829 0a20 2020 2020 2020 2066  with().        f
-0000e640: 696c 7465 7265 642e 6176 6169 6c61 626c  iltered.availabl
-0000e650: 652e 6173 7365 7274 5f63 616c 6c65 645f  e.assert_called_
-0000e660: 6f6e 6365 5f77 6974 6828 290a 2020 2020  once_with().    
-0000e670: 2020 2020 6176 6169 6c61 626c 6520 3d20      available = 
-0000e680: 6669 6c74 6572 6564 2e61 7661 696c 6162  filtered.availab
-0000e690: 6c65 2829 0a20 2020 2020 2020 2061 7373  le().        ass
-0000e6a0: 6572 7420 7374 646f 7574 2e67 6574 7661  ert stdout.getva
-0000e6b0: 6c75 6528 292e 7374 7269 7028 2920 3d3d  lue().strip() ==
-0000e6c0: 2073 7472 2861 7661 696c 6162 6c65 290a   str(available).
-0000e6d0: 0a20 2020 2064 6566 2074 6573 745f 6365  .    def test_ce
-0000e6e0: 7274 6f6e 6c79 5f61 6273 7061 7468 2873  rtonly_abspath(s
-0000e6f0: 656c 6629 3a0a 2020 2020 2020 2020 6365  elf):.        ce
-0000e700: 7274 203d 2027 6365 7274 270a 2020 2020  rt = 'cert'.    
-0000e710: 2020 2020 6b65 7920 3d20 276b 6579 270a      key = 'key'.
-0000e720: 2020 2020 2020 2020 6368 6169 6e20 3d20          chain = 
-0000e730: 2763 6861 696e 270a 2020 2020 2020 2020  'chain'.        
-0000e740: 6675 6c6c 6368 6169 6e20 3d20 2766 756c  fullchain = 'ful
-0000e750: 6c63 6861 696e 270a 0a20 2020 2020 2020  lchain'..       
-0000e760: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
-0000e770: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-0000e780: 6e61 6c2e 6d61 696e 2e63 6572 746f 6e6c  nal.main.certonl
-0000e790: 7927 2920 6173 206d 6f63 6b5f 6365 7274  y') as mock_cert
-0000e7a0: 6f6e 6c79 3a0a 2020 2020 2020 2020 2020  only:.          
-0000e7b0: 2020 7365 6c66 2e5f 6361 6c6c 285b 2763    self._call(['c
-0000e7c0: 6572 746f 6e6c 7927 2c20 272d 2d63 6572  ertonly', '--cer
-0000e7d0: 742d 7061 7468 272c 2063 6572 742c 2027  t-path', cert, '
-0000e7e0: 2d2d 6b65 792d 7061 7468 272c 2027 6b65  --key-path', 'ke
-0000e7f0: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
-0000e800: 2020 2020 2020 2020 2020 2020 272d 2d63              '--c
-0000e810: 6861 696e 2d70 6174 6827 2c20 2763 6861  hain-path', 'cha
-0000e820: 696e 272c 0a20 2020 2020 2020 2020 2020  in',.           
-0000e830: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
-0000e840: 6675 6c6c 6368 6169 6e2d 7061 7468 272c  fullchain-path',
-0000e850: 2027 6675 6c6c 6368 6169 6e27 5d29 0a0a   'fullchain'])..
-0000e860: 2020 2020 2020 2020 636f 6e66 6967 2c20          config, 
-0000e870: 756e 7573 6564 5f70 6c75 6769 6e73 203d  unused_plugins =
-0000e880: 206d 6f63 6b5f 6365 7274 6f6e 6c79 2e63   mock_certonly.c
-0000e890: 616c 6c5f 6172 6773 5b30 5d0a 2020 2020  all_args[0].    
-0000e8a0: 2020 2020 6173 7365 7274 2063 6f6e 6669      assert confi
-0000e8b0: 672e 6365 7274 5f70 6174 6820 3d3d 206f  g.cert_path == o
-0000e8c0: 732e 7061 7468 2e61 6273 7061 7468 2863  s.path.abspath(c
-0000e8d0: 6572 7429 0a20 2020 2020 2020 2061 7373  ert).        ass
-0000e8e0: 6572 7420 636f 6e66 6967 2e6b 6579 5f70  ert config.key_p
-0000e8f0: 6174 6820 3d3d 206f 732e 7061 7468 2e61  ath == os.path.a
-0000e900: 6273 7061 7468 286b 6579 290a 2020 2020  bspath(key).    
-0000e910: 2020 2020 6173 7365 7274 2063 6f6e 6669      assert confi
-0000e920: 672e 6368 6169 6e5f 7061 7468 203d 3d20  g.chain_path == 
-0000e930: 6f73 2e70 6174 682e 6162 7370 6174 6828  os.path.abspath(
-0000e940: 6368 6169 6e29 0a20 2020 2020 2020 2061  chain).        a
-0000e950: 7373 6572 7420 636f 6e66 6967 2e66 756c  ssert config.ful
-0000e960: 6c63 6861 696e 5f70 6174 6820 3d3d 206f  lchain_path == o
-0000e970: 732e 7061 7468 2e61 6273 7061 7468 2866  s.path.abspath(f
-0000e980: 756c 6c63 6861 696e 290a 0a20 2020 2064  ullchain)..    d
-0000e990: 6566 2074 6573 745f 6365 7274 6f6e 6c79  ef test_certonly
-0000e9a0: 5f62 6164 5f61 7267 7328 7365 6c66 293a  _bad_args(self):
-0000e9b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000e9c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e9d0: 6361 6c6c 285b 272d 6127 2c20 2762 6164  call(['-a', 'bad
-0000e9e0: 5f61 7574 6827 2c20 2763 6572 746f 6e6c  _auth', 'certonl
-0000e9f0: 7927 5d29 0a20 2020 2020 2020 2020 2020  y']).           
-0000ea00: 2061 7373 6572 7420 4661 6c73 652c 2022   assert False, "
-0000ea10: 4578 6365 7074 696f 6e20 7368 6f75 6c64  Exception should
-0000ea20: 2068 6176 6520 6265 656e 2072 6169 7365   have been raise
-0000ea30: 6422 0a20 2020 2020 2020 2065 7863 6570  d".        excep
-0000ea40: 7420 6572 726f 7273 2e50 6c75 6769 6e53  t errors.PluginS
-0000ea50: 656c 6563 7469 6f6e 4572 726f 7220 6173  electionError as
-0000ea60: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-0000ea70: 6173 7365 7274 2027 5468 6520 7265 7175  assert 'The requ
-0000ea80: 6573 7465 6420 6261 645f 6175 7468 2070  ested bad_auth p
-0000ea90: 6c75 6769 6e20 646f 6573 206e 6f74 2061  lugin does not a
-0000eaa0: 7070 6561 7227 2069 6e20 7374 7228 6529  ppear' in str(e)
-0000eab0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
-0000eac0: 6865 636b 5f63 6f6e 6669 675f 7361 6e69  heck_config_sani
-0000ead0: 7479 5f64 6f6d 6169 6e28 7365 6c66 293a  ty_domain(self):
-0000eae0: 0a20 2020 2020 2020 2023 2046 5144 4e0a  .        # FQDN.
-0000eaf0: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0000eb00: 6573 742e 7261 6973 6573 2865 7272 6f72  est.raises(error
-0000eb10: 732e 436f 6e66 6967 7572 6174 696f 6e45  s.ConfigurationE
-0000eb20: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
-0000eb30: 2020 2073 656c 662e 5f63 616c 6c28 5b27     self._call(['
-0000eb40: 2d64 272c 2027 6127 202a 2036 345d 290a  -d', 'a' * 64]).
-0000eb50: 2020 2020 2020 2020 2320 4651 444e 2032          # FQDN 2
-0000eb60: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
-0000eb70: 7465 7374 2e72 6169 7365 7328 6572 726f  test.raises(erro
-0000eb80: 7273 2e43 6f6e 6669 6775 7261 7469 6f6e  rs.Configuration
-0000eb90: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-0000eba0: 2020 2020 7365 6c66 2e5f 6361 6c6c 285b      self._call([
-0000ebb0: 272d 6427 2c20 2828 2761 2720 2a20 3530  '-d', (('a' * 50
-0000ebc0: 2920 2b20 272e 2729 202a 2031 305d 290a  ) + '.') * 10]).
-0000ebd0: 2020 2020 2020 2020 2320 4261 7265 2049          # Bare I
-0000ebe0: 5020 6164 6472 6573 7320 2874 6869 7320  P address (this 
-0000ebf0: 6973 2061 6374 7561 6c6c 7920 6120 6469  is actually a di
-0000ec00: 6666 6572 656e 7420 6572 726f 7220 6d65  fferent error me
-0000ec10: 7373 6167 6520 6e6f 7729 0a20 2020 2020  ssage now).     
-0000ec20: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-0000ec30: 6169 7365 7328 6572 726f 7273 2e43 6f6e  aises(errors.Con
-0000ec40: 6669 6775 7261 7469 6f6e 4572 726f 7229  figurationError)
-0000ec50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ec60: 6c66 2e5f 6361 6c6c 285b 272d 6427 2c20  lf._call(['-d', 
-0000ec70: 2732 3034 2e31 312e 3233 312e 3335 275d  '204.11.231.35']
-0000ec80: 290a 2020 2020 2020 2020 2320 4261 7265  ).        # Bare
-0000ec90: 2049 5076 3620 6164 6472 6573 730a 2020   IPv6 address.  
-0000eca0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-0000ecb0: 742e 7261 6973 6573 2865 7272 6f72 732e  t.raises(errors.
-0000ecc0: 436f 6e66 6967 7572 6174 696f 6e45 7272  ConfigurationErr
-0000ecd0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0000ece0: 2073 656c 662e 5f63 616c 6c28 5b27 2d64   self._call(['-d
-0000ecf0: 272c 2027 3230 3031 3a64 6238 3a61 6336  ', '2001:db8:ac6
-0000ed00: 393a 3366 663a 6231 6362 3a63 3863 363a  9:3ff:b1cb:c8c6:
-0000ed10: 3561 3834 3a61 3331 6227 5d29 0a0a 2020  5a84:a31b'])..  
-0000ed20: 2020 6465 6620 7465 7374 5f63 7372 5f77    def test_csr_w
-0000ed30: 6974 685f 6265 7374 6566 666f 7274 2873  ith_besteffort(s
-0000ed40: 656c 6629 3a0a 2020 2020 2020 2020 7769  elf):.        wi
-0000ed50: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-0000ed60: 2865 7272 6f72 732e 4572 726f 7229 3a0a  (errors.Error):.
-0000ed70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ed80: 2e5f 6361 6c6c 2827 6365 7274 6f6e 6c79  ._call('certonly
-0000ed90: 202d 2d63 7372 207b 307d 202d 2d61 6c6c   --csr {0} --all
-0000eda0: 6f77 2d73 7562 7365 742d 6f66 2d6e 616d  ow-subset-of-nam
-0000edb0: 6573 272e 666f 726d 6174 2843 5352 292e  es'.format(CSR).
-0000edc0: 7370 6c69 7428 2929 0a0a 2020 2020 6465  split())..    de
-0000edd0: 6620 7465 7374 5f72 756e 5f77 6974 685f  f test_run_with_
-0000ede0: 6373 7228 7365 6c66 293a 0a20 2020 2020  csr(self):.     
-0000edf0: 2020 2023 2054 6869 7320 6973 2061 6e20     # This is an 
-0000ee00: 6572 726f 7220 6265 6361 7573 6520 796f  error because yo
-0000ee10: 7520 6361 6e20 6f6e 6c79 2075 7365 202d  u can only use -
-0000ee20: 2d63 7372 2077 6974 6820 6365 7274 6f6e  -csr with certon
-0000ee30: 6c79 0a20 2020 2020 2020 2074 7279 3a0a  ly.        try:.
-0000ee40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ee50: 2e5f 6361 6c6c 285b 272d 2d63 7372 272c  ._call(['--csr',
-0000ee60: 2043 5352 5d29 0a20 2020 2020 2020 2065   CSR]).        e
-0000ee70: 7863 6570 7420 6572 726f 7273 2e45 7272  xcept errors.Err
-0000ee80: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-0000ee90: 2020 2020 2061 7373 6572 7420 2250 6c65       assert "Ple
-0000eea0: 6173 6520 7472 7920 7468 6520 6365 7274  ase try the cert
-0000eeb0: 6f6e 6c79 2220 696e 2072 6570 7228 6529  only" in repr(e)
-0000eec0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000eed0: 7572 6e0a 2020 2020 2020 2020 6173 7365  urn.        asse
-0000eee0: 7274 2046 616c 7365 2c20 2245 7870 6563  rt False, "Expec
-0000eef0: 7465 6420 7375 7070 6c79 696e 6720 2d2d  ted supplying --
-0000ef00: 6373 7220 746f 2066 6169 6c20 7769 7468  csr to fail with
-0000ef10: 2064 6566 6175 6c74 2076 6572 6222 0a0a   default verb"..
-0000ef20: 2020 2020 6465 6620 7465 7374 5f63 7372      def test_csr
-0000ef30: 5f77 6974 685f 6e6f 5f64 6f6d 6169 6e73  _with_no_domains
-0000ef40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ef50: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-0000ef60: 6573 2865 7272 6f72 732e 4572 726f 7229  es(errors.Error)
-0000ef70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ef80: 6c66 2e5f 6361 6c6c 2827 6365 7274 6f6e  lf._call('certon
-0000ef90: 6c79 202d 2d63 7372 207b 307d 272e 666f  ly --csr {0}'.fo
-0000efa0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-0000efb0: 2020 2020 2020 7465 7374 5f75 7469 6c2e        test_util.
-0000efc0: 7665 6374 6f72 5f70 6174 6828 2763 7372  vector_path('csr
-0000efd0: 2d6e 6f6e 616d 6573 5f35 3132 2e70 656d  -nonames_512.pem
-0000efe0: 2729 292e 7370 6c69 7428 2929 0a0a 2020  ')).split())..  
-0000eff0: 2020 6465 6620 7465 7374 5f63 7372 5f77    def test_csr_w
-0000f000: 6974 685f 696e 636f 6e73 6973 7465 6e74  ith_inconsistent
-0000f010: 5f64 6f6d 6169 6e73 2873 656c 6629 3a0a  _domains(self):.
-0000f020: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-0000f030: 6573 742e 7261 6973 6573 2865 7272 6f72  est.raises(error
-0000f040: 732e 4572 726f 7229 3a0a 2020 2020 2020  s.Error):.      
-0000f050: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
-0000f060: 2827 6365 7274 6f6e 6c79 202d 6420 6578  ('certonly -d ex
-0000f070: 616d 706c 652e 6f72 6720 2d2d 6373 7220  ample.org --csr 
-0000f080: 7b30 7d27 2e66 6f72 6d61 7428 4353 5229  {0}'.format(CSR)
-0000f090: 2e73 706c 6974 2829 290a 0a20 2020 2064  .split())..    d
-0000f0a0: 6566 205f 6365 7274 6f6e 6c79 5f6e 6577  ef _certonly_new
-0000f0b0: 5f72 6571 7565 7374 5f63 6f6d 6d6f 6e28  _request_common(
-0000f0c0: 7365 6c66 2c20 6d6f 636b 5f63 6c69 656e  self, mock_clien
-0000f0d0: 742c 2061 7267 733d 4e6f 6e65 293a 0a20  t, args=None):. 
-0000f0e0: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
-0000f0f0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-0000f100: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e5f  _internal.main._
-0000f110: 6669 6e64 5f6c 696e 6561 6765 5f66 6f72  find_lineage_for
-0000f120: 5f64 6f6d 6169 6e73 5f61 6e64 5f63 6572  _domains_and_cer
-0000f130: 746e 616d 6527 2920 5c0a 2020 2020 2020  tname') \.      
-0000f140: 2020 2020 2020 6173 206d 6f63 6b5f 7265        as mock_re
-0000f150: 6e65 7761 6c3a 0a20 2020 2020 2020 2020  newal:.         
-0000f160: 2020 206d 6f63 6b5f 7265 6e65 7761 6c2e     mock_renewal.
-0000f170: 7265 7475 726e 5f76 616c 7565 203d 2028  return_value = (
-0000f180: 226e 6577 6365 7274 222c 204e 6f6e 6529  "newcert", None)
-0000f190: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0000f1a0: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
-0000f1b0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000f1c0: 6d61 696e 2e5f 696e 6974 5f6c 655f 636c  main._init_le_cl
-0000f1d0: 6965 6e74 2729 2061 7320 6d6f 636b 5f69  ient') as mock_i
-0000f1e0: 6e69 743a 0a20 2020 2020 2020 2020 2020  nit:.           
-0000f1f0: 2020 2020 206d 6f63 6b5f 696e 6974 2e72       mock_init.r
-0000f200: 6574 7572 6e5f 7661 6c75 6520 3d20 6d6f  eturn_value = mo
-0000f210: 636b 5f63 6c69 656e 740a 2020 2020 2020  ck_client.      
-0000f220: 2020 2020 2020 2020 2020 6966 2061 7267            if arg
-0000f230: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0000f240: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000f250: 7267 7320 3d20 5b5d 0a20 2020 2020 2020  rgs = [].       
-0000f260: 2020 2020 2020 2020 2061 7267 7320 2b3d           args +=
-0000f270: 2027 2d64 2066 6f6f 2e62 6172 202d 6120   '-d foo.bar -a 
-0000f280: 7374 616e 6461 6c6f 6e65 2063 6572 746f  standalone certo
-0000f290: 6e6c 7927 2e73 706c 6974 2829 0a20 2020  nly'.split().   
-0000f2a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f2b0: 662e 5f63 616c 6c28 6172 6773 290a 0a20  f._call(args).. 
-0000f2c0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-0000f2d0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-0000f2e0: 6c2e 6d61 696e 2e5f 7265 706f 7274 5f6e  l.main._report_n
-0000f2f0: 6577 5f63 6572 7427 290a 2020 2020 6465  ew_cert').    de
-0000f300: 6620 7465 7374 5f63 6572 746f 6e6c 795f  f test_certonly_
-0000f310: 6472 795f 7275 6e5f 6e65 775f 7265 7175  dry_run_new_requ
-0000f320: 6573 745f 7375 6363 6573 7328 7365 6c66  est_success(self
-0000f330: 2c20 6d6f 636b 5f72 6570 6f72 7429 3a0a  , mock_report):.
-0000f340: 2020 2020 2020 2020 6d6f 636b 5f63 6c69          mock_cli
-0000f350: 656e 7420 3d20 6d6f 636b 2e4d 6167 6963  ent = mock.Magic
-0000f360: 4d6f 636b 2829 0a20 2020 2020 2020 206d  Mock().        m
-0000f370: 6f63 6b5f 636c 6965 6e74 2e6f 6274 6169  ock_client.obtai
-0000f380: 6e5f 616e 645f 656e 726f 6c6c 5f63 6572  n_and_enroll_cer
-0000f390: 7469 6669 6361 7465 2e72 6574 7572 6e5f  tificate.return_
-0000f3a0: 7661 6c75 6520 3d20 4e6f 6e65 0a20 2020  value = None.   
-0000f3b0: 2020 2020 2073 656c 662e 5f63 6572 746f       self._certo
-0000f3c0: 6e6c 795f 6e65 775f 7265 7175 6573 745f  nly_new_request_
-0000f3d0: 636f 6d6d 6f6e 286d 6f63 6b5f 636c 6965  common(mock_clie
-0000f3e0: 6e74 2c20 5b27 2d2d 6472 792d 7275 6e27  nt, ['--dry-run'
-0000f3f0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0000f400: 7420 6d6f 636b 5f63 6c69 656e 742e 6f62  t mock_client.ob
-0000f410: 7461 696e 5f61 6e64 5f65 6e72 6f6c 6c5f  tain_and_enroll_
-0000f420: 6365 7274 6966 6963 6174 652e 6361 6c6c  certificate.call
-0000f430: 5f63 6f75 6e74 203d 3d20 310a 2020 2020  _count == 1.    
-0000f440: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
-0000f450: 7265 706f 7274 2e63 616c 6c5f 636f 756e  report.call_coun
-0000f460: 7420 3d3d 2031 0a20 2020 2020 2020 2061  t == 1.        a
-0000f470: 7373 6572 7420 6d6f 636b 5f72 6570 6f72  ssert mock_repor
-0000f480: 742e 6361 6c6c 5f61 7267 735b 305d 5b30  t.call_args[0][0
-0000f490: 5d2e 6472 795f 7275 6e20 6973 2054 7275  ].dry_run is Tru
-0000f4a0: 650a 0a20 2020 2040 6d6f 636b 2e70 6174  e..    @mock.pat
-0000f4b0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0000f4c0: 6572 6e61 6c2e 6d61 696e 2e5f 7265 706f  ernal.main._repo
-0000f4d0: 7274 5f6e 6577 5f63 6572 7427 290a 2020  rt_new_cert').  
-0000f4e0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-0000f4f0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-0000f500: 2e6d 6169 6e2e 7574 696c 2e61 7465 7869  .main.util.atexi
-0000f510: 745f 7265 6769 7374 6572 2729 0a20 2020  t_register').   
-0000f520: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000f530: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000f540: 6566 662e 6861 6e64 6c65 5f73 7562 7363  eff.handle_subsc
-0000f550: 7269 7074 696f 6e27 290a 2020 2020 406d  ription').    @m
-0000f560: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0000f570: 6f74 2e63 7279 7074 6f5f 7574 696c 2e6e  ot.crypto_util.n
-0000f580: 6f74 4166 7465 7227 290a 2020 2020 6465  otAfter').    de
-0000f590: 6620 7465 7374 5f63 6572 746f 6e6c 795f  f test_certonly_
-0000f5a0: 6e65 775f 7265 7175 6573 745f 7375 6363  new_request_succ
-0000f5b0: 6573 7328 7365 6c66 2c20 6d6f 636b 5f6e  ess(self, mock_n
-0000f5c0: 6f74 4166 7465 722c 0a20 2020 2020 2020  otAfter,.       
-0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5f0: 2020 206d 6f63 6b5f 7375 6273 6372 6970     mock_subscrip
-0000f600: 7469 6f6e 2c20 6d6f 636b 5f72 6567 6973  tion, mock_regis
-0000f610: 7465 722c 206d 6f63 6b5f 7265 706f 7274  ter, mock_report
-0000f620: 293a 0a20 2020 2020 2020 2063 6572 745f  ):.        cert_
-0000f630: 7061 7468 203d 206f 732e 7061 7468 2e6e  path = os.path.n
-0000f640: 6f72 6d70 6174 6828 6f73 2e70 6174 682e  ormpath(os.path.
-0000f650: 6a6f 696e 2873 656c 662e 636f 6e66 6967  join(self.config
-0000f660: 2e63 6f6e 6669 675f 6469 722c 2027 6c69  .config_dir, 'li
-0000f670: 7665 2f66 6f6f 2e62 6172 2729 290a 2020  ve/foo.bar')).  
-0000f680: 2020 2020 2020 6b65 795f 7061 7468 203d        key_path =
-0000f690: 206f 732e 7061 7468 2e6e 6f72 6d70 6174   os.path.normpat
-0000f6a0: 6828 6f73 2e70 6174 682e 6a6f 696e 2873  h(os.path.join(s
-0000f6b0: 656c 662e 636f 6e66 6967 2e63 6f6e 6669  elf.config.confi
-0000f6c0: 675f 6469 722c 2027 6c69 7665 2f62 617a  g_dir, 'live/baz
-0000f6d0: 2e71 7578 2729 290a 2020 2020 2020 2020  .qux')).        
-0000f6e0: 6461 7465 203d 2027 3139 3730 2d30 312d  date = '1970-01-
-0000f6f0: 3031 270a 2020 2020 2020 2020 6d6f 636b  01'.        mock
-0000f700: 5f6e 6f74 4166 7465 7228 292e 6461 7465  _notAfter().date
-0000f710: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-0000f720: 6461 7465 0a0a 2020 2020 2020 2020 6d6f  date..        mo
-0000f730: 636b 5f6c 696e 6561 6765 203d 206d 6f63  ck_lineage = moc
-0000f740: 6b2e 4d61 6769 634d 6f63 6b28 6365 7274  k.MagicMock(cert
-0000f750: 3d63 6572 745f 7061 7468 2c20 6675 6c6c  =cert_path, full
-0000f760: 6368 6169 6e3d 6365 7274 5f70 6174 682c  chain=cert_path,
-0000f770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f790: 2020 2020 2020 2066 756c 6c63 6861 696e         fullchain
-0000f7a0: 5f70 6174 683d 6365 7274 5f70 6174 682c  _path=cert_path,
-0000f7b0: 206b 6579 5f70 6174 683d 6b65 795f 7061   key_path=key_pa
-0000f7c0: 7468 290a 2020 2020 2020 2020 6d6f 636b  th).        mock
-0000f7d0: 5f63 6c69 656e 7420 3d20 6d6f 636b 2e4d  _client = mock.M
-0000f7e0: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-0000f7f0: 2020 206d 6f63 6b5f 636c 6965 6e74 2e6f     mock_client.o
-0000f800: 6274 6169 6e5f 616e 645f 656e 726f 6c6c  btain_and_enroll
-0000f810: 5f63 6572 7469 6669 6361 7465 2e72 6574  _certificate.ret
-0000f820: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
-0000f830: 5f6c 696e 6561 6765 0a20 2020 2020 2020  _lineage.       
-0000f840: 2073 656c 662e 5f63 6572 746f 6e6c 795f   self._certonly_
-0000f850: 6e65 775f 7265 7175 6573 745f 636f 6d6d  new_request_comm
-0000f860: 6f6e 286d 6f63 6b5f 636c 6965 6e74 290a  on(mock_client).
-0000f870: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-0000f880: 6f63 6b5f 636c 6965 6e74 2e6f 6274 6169  ock_client.obtai
-0000f890: 6e5f 616e 645f 656e 726f 6c6c 5f63 6572  n_and_enroll_cer
-0000f8a0: 7469 6669 6361 7465 2e63 616c 6c5f 636f  tificate.call_co
-0000f8b0: 756e 7420 3d3d 2031 0a20 2020 2020 2020  unt == 1.       
-0000f8c0: 2061 7373 6572 7420 6d6f 636b 5f72 6570   assert mock_rep
-0000f8d0: 6f72 742e 6361 6c6c 5f63 6f75 6e74 203d  ort.call_count =
-0000f8e0: 3d20 310a 2020 2020 2020 2020 6173 7365  = 1.        asse
-0000f8f0: 7274 2063 6572 745f 7061 7468 2069 6e20  rt cert_path in 
-0000f900: 6d6f 636b 5f72 6570 6f72 742e 6361 6c6c  mock_report.call
-0000f910: 5f61 7267 735b 305d 5b32 5d0a 2020 2020  _args[0][2].    
-0000f920: 2020 2020 6173 7365 7274 206b 6579 5f70      assert key_p
-0000f930: 6174 6820 696e 206d 6f63 6b5f 7265 706f  ath in mock_repo
-0000f940: 7274 2e63 616c 6c5f 6172 6773 5b30 5d5b  rt.call_args[0][
-0000f950: 335d 0a20 2020 2020 2020 2061 7373 6572  3].        asser
-0000f960: 7420 2764 6f6e 6174 6527 2069 6e20 6d6f  t 'donate' in mo
-0000f970: 636b 5f72 6567 6973 7465 722e 6361 6c6c  ck_register.call
-0000f980: 5f61 7267 735b 305d 5b31 5d0a 2020 2020  _args[0][1].    
-0000f990: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
-0000f9a0: 7375 6273 6372 6970 7469 6f6e 2e63 616c  subscription.cal
-0000f9b0: 6c65 6420 6973 2054 7275 650a 0a20 2020  led is True..   
-0000f9c0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-0000f9d0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0000f9e0: 6566 662e 6861 6e64 6c65 5f73 7562 7363  eff.handle_subsc
-0000f9f0: 7269 7074 696f 6e27 290a 2020 2020 6465  ription').    de
-0000fa00: 6620 7465 7374 5f63 6572 746f 6e6c 795f  f test_certonly_
-0000fa10: 6e65 775f 7265 7175 6573 745f 6661 696c  new_request_fail
-0000fa20: 7572 6528 7365 6c66 2c20 6d6f 636b 5f73  ure(self, mock_s
-0000fa30: 7562 7363 7269 7074 696f 6e29 3a0a 2020  ubscription):.  
-0000fa40: 2020 2020 2020 6d6f 636b 5f63 6c69 656e        mock_clien
-0000fa50: 7420 3d20 6d6f 636b 2e4d 6167 6963 4d6f  t = mock.MagicMo
-0000fa60: 636b 2829 0a20 2020 2020 2020 206d 6f63  ck().        moc
-0000fa70: 6b5f 636c 6965 6e74 2e6f 6274 6169 6e5f  k_client.obtain_
-0000fa80: 616e 645f 656e 726f 6c6c 5f63 6572 7469  and_enroll_certi
-0000fa90: 6669 6361 7465 2e72 6574 7572 6e5f 7661  ficate.return_va
-0000faa0: 6c75 6520 3d20 4661 6c73 650a 2020 2020  lue = False.    
-0000fab0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-0000fac0: 7261 6973 6573 2865 7272 6f72 732e 4572  raises(errors.Er
-0000fad0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0000fae0: 2020 7365 6c66 2e5f 6365 7274 6f6e 6c79    self._certonly
-0000faf0: 5f6e 6577 5f72 6571 7565 7374 5f63 6f6d  _new_request_com
-0000fb00: 6d6f 6e28 6d6f 636b 5f63 6c69 656e 7429  mon(mock_client)
-0000fb10: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000fb20: 6d6f 636b 5f73 7562 7363 7269 7074 696f  mock_subscriptio
-0000fb30: 6e2e 6361 6c6c 6564 2069 7320 4661 6c73  n.called is Fals
-0000fb40: 650a 0a20 2020 2064 6566 205f 7465 7374  e..    def _test
-0000fb50: 5f72 656e 6577 616c 5f63 6f6d 6d6f 6e28  _renewal_common(
-0000fb60: 7365 6c66 2c20 6475 655f 666f 725f 7265  self, due_for_re
-0000fb70: 6e65 7761 6c2c 2065 7874 7261 5f61 7267  newal, extra_arg
-0000fb80: 732c 206c 6f67 5f6f 7574 3d4e 6f6e 652c  s, log_out=None,
-0000fb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-0000fbb0: 6773 3d4e 6f6e 652c 2073 686f 756c 645f  gs=None, should_
-0000fbc0: 7265 6e65 773d 5472 7565 2c20 6572 726f  renew=True, erro
-0000fbd0: 725f 6578 7065 6374 6564 3d46 616c 7365  r_expected=False
-0000fbe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-0000fc00: 7569 6574 5f6d 6f64 653d 4661 6c73 652c  uiet_mode=False,
-0000fc10: 2065 7870 6972 795f 6461 7465 3d64 6174   expiry_date=dat
-0000fc20: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
-0000fc30: 6f77 2829 2c0a 2020 2020 2020 2020 2020  ow(),.          
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc50: 2020 2072 6575 7365 5f6b 6579 3d46 616c     reuse_key=Fal
-0000fc60: 7365 2c20 6e65 775f 6b65 793d 4661 6c73  se, new_key=Fals
-0000fc70: 6529 3a0a 2020 2020 2020 2020 6365 7274  e):.        cert
-0000fc80: 5f70 6174 6820 3d20 7465 7374 5f75 7469  _path = test_uti
-0000fc90: 6c2e 7665 6374 6f72 5f70 6174 6828 2763  l.vector_path('c
-0000fca0: 6572 745f 3531 322e 7065 6d27 290a 2020  ert_512.pem').  
-0000fcb0: 2020 2020 2020 6368 6169 6e5f 7061 7468        chain_path
-0000fcc0: 203d 206f 732e 7061 7468 2e6e 6f72 6d70   = os.path.normp
-0000fcd0: 6174 6828 6f73 2e70 6174 682e 6a6f 696e  ath(os.path.join
-0000fce0: 2873 656c 662e 636f 6e66 6967 2e63 6f6e  (self.config.con
-0000fcf0: 6669 675f 6469 722c 0a20 2020 2020 2020  fig_dir,.       
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd20: 2020 2020 2020 2020 2020 2020 276c 6976              'liv
-0000fd30: 652f 666f 6f2e 6261 722f 6675 6c6c 6368  e/foo.bar/fullch
-0000fd40: 6169 6e2e 7065 6d27 2929 0a20 2020 2020  ain.pem')).     
-0000fd50: 2020 206d 6f63 6b5f 6c69 6e65 6167 6520     mock_lineage 
-0000fd60: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
-0000fd70: 2863 6572 743d 6365 7274 5f70 6174 682c  (cert=cert_path,
-0000fd80: 2066 756c 6c63 6861 696e 3d63 6861 696e   fullchain=chain
-0000fd90: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdb0: 2020 2020 2020 2020 2020 2020 2063 6572               cer
-0000fdc0: 745f 7061 7468 3d63 6572 745f 7061 7468  t_path=cert_path
-0000fdd0: 2c20 6675 6c6c 6368 6169 6e5f 7061 7468  , fullchain_path
-0000fde0: 3d63 6861 696e 5f70 6174 6829 0a20 2020  =chain_path).   
-0000fdf0: 2020 2020 206d 6f63 6b5f 6c69 6e65 6167       mock_lineag
-0000fe00: 652e 7368 6f75 6c64 5f61 7574 6f72 656e  e.should_autoren
-0000fe10: 6577 2e72 6574 7572 6e5f 7661 6c75 6520  ew.return_value 
-0000fe20: 3d20 6475 655f 666f 725f 7265 6e65 7761  = due_for_renewa
-0000fe30: 6c0a 2020 2020 2020 2020 6d6f 636b 5f6c  l.        mock_l
-0000fe40: 696e 6561 6765 2e68 6173 5f70 656e 6469  ineage.has_pendi
-0000fe50: 6e67 5f64 6570 6c6f 796d 656e 742e 7265  ng_deployment.re
-0000fe60: 7475 726e 5f76 616c 7565 203d 2046 616c  turn_value = Fal
-0000fe70: 7365 0a20 2020 2020 2020 206d 6f63 6b5f  se.        mock_
-0000fe80: 6c69 6e65 6167 652e 6e61 6d65 732e 7265  lineage.names.re
-0000fe90: 7475 726e 5f76 616c 7565 203d 205b 2769  turn_value = ['i
-0000fea0: 736e 6f74 2e6f 7267 275d 0a20 2020 2020  snot.org'].     
-0000feb0: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
-0000fec0: 7072 6976 6174 655f 6b65 795f 7479 7065  private_key_type
-0000fed0: 203d 2027 6563 6473 6127 0a20 2020 2020   = 'ecdsa'.     
-0000fee0: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
-0000fef0: 656c 6c69 7074 6963 5f63 7572 7665 203d  elliptic_curve =
-0000ff00: 2027 7365 6370 3235 3672 3127 0a20 2020   'secp256r1'.   
-0000ff10: 2020 2020 206d 6f63 6b5f 6c69 6e65 6167       mock_lineag
-0000ff20: 652e 7265 7573 655f 6b65 7920 3d20 7265  e.reuse_key = re
-0000ff30: 7573 655f 6b65 790a 2020 2020 2020 2020  use_key.        
-0000ff40: 6d6f 636b 5f63 6572 7472 203d 206d 6f63  mock_certr = moc
-0000ff50: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
-0000ff60: 2020 2020 2020 6d6f 636b 5f6b 6579 203d        mock_key =
-0000ff70: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
-0000ff80: 7065 6d3d 2770 656d 5f6b 6579 2729 0a20  pem='pem_key'). 
-0000ff90: 2020 2020 2020 206d 6f63 6b5f 636c 6965         mock_clie
-0000ffa0: 6e74 203d 206d 6f63 6b2e 4d61 6769 634d  nt = mock.MagicM
-0000ffb0: 6f63 6b28 290a 2020 2020 2020 2020 7374  ock().        st
-0000ffc0: 646f 7574 203d 2069 6f2e 5374 7269 6e67  dout = io.String
-0000ffd0: 494f 2829 0a20 2020 2020 2020 206d 6f63  IO().        moc
-0000ffe0: 6b5f 636c 6965 6e74 2e6f 6274 6169 6e5f  k_client.obtain_
-0000fff0: 6365 7274 6966 6963 6174 652e 7265 7475  certificate.retu
-00010000: 726e 5f76 616c 7565 203d 2028 6d6f 636b  rn_value = (mock
-00010010: 5f63 6572 7472 2c20 2763 6861 696e 272c  _certr, 'chain',
-00010020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010050: 2020 2020 2020 2020 6d6f 636b 5f6b 6579          mock_key
-00010060: 2c20 2763 7372 2729 0a0a 2020 2020 2020  , 'csr')..      
-00010070: 2020 6465 6620 7772 6974 655f 6d73 6728    def write_msg(
-00010080: 6d65 7373 6167 652c 202a 6172 6773 2c20  message, *args, 
-00010090: 2a2a 6b77 6172 6773 293a 2020 2320 7079  **kwargs):  # py
-000100a0: 6c69 6e74 3a20 6469 7361 626c 653d 756e  lint: disable=un
-000100b0: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
-000100c0: 2020 2020 2020 2020 2020 2222 2257 7269            """Wri
-000100d0: 7465 206d 6573 7361 6765 2074 6f20 7374  te message to st
-000100e0: 646f 7574 2e22 2222 0a20 2020 2020 2020  dout.""".       
-000100f0: 2020 2020 2073 7464 6f75 742e 7772 6974       stdout.writ
-00010100: 6528 6d65 7373 6167 6529 0a0a 2020 2020  e(message)..    
-00010110: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00010120: 2020 2020 2077 6974 6820 6d6f 636b 2e70       with mock.p
-00010130: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00010140: 6e74 6572 6e61 6c2e 6365 7274 5f6d 616e  nternal.cert_man
-00010150: 6167 6572 2e66 696e 645f 6475 706c 6963  ager.find_duplic
-00010160: 6174 6976 655f 6365 7274 7327 2920 6173  ative_certs') as
-00010170: 206d 6f63 6b5f 6664 633a 0a20 2020 2020   mock_fdc:.     
-00010180: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-00010190: 6664 632e 7265 7475 726e 5f76 616c 7565  fdc.return_value
-000101a0: 203d 2028 6d6f 636b 5f6c 696e 6561 6765   = (mock_lineage
-000101b0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-000101c0: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-000101d0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-000101e0: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-000101f0: 5f69 6e69 745f 6c65 5f63 6c69 656e 7427  _init_le_client'
-00010200: 2920 6173 206d 6f63 6b5f 696e 6974 3a0a  ) as mock_init:.
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2020 2020 6d6f 636b 5f69 6e69 742e 7265      mock_init.re
-00010230: 7475 726e 5f76 616c 7565 203d 206d 6f63  turn_value = moc
-00010240: 6b5f 636c 6965 6e74 0a20 2020 2020 2020  k_client.       
-00010250: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00010260: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
-00010270: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00010280: 6469 7370 6c61 792e 6f62 6a2e 6765 745f  display.obj.get_
-00010290: 6469 7370 6c61 7927 2920 6173 206d 6f63  display') as moc
-000102a0: 6b5f 6469 7370 6c61 793a 0a20 2020 2020  k_display:.     
-000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2020 2069 6620 6e6f 7420 7175 6965 745f     if not quiet_
-000102d0: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
-000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 6d6f 636b 5f64 6973 706c 6179 2829    mock_display()
-00010300: 2e6e 6f74 6966 6963 6174 696f 6e2e 7369  .notification.si
-00010310: 6465 5f65 6666 6563 7420 3d20 7772 6974  de_effect = writ
-00010320: 655f 6d73 670a 2020 2020 2020 2020 2020  e_msg.          
-00010330: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00010340: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-00010350: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00010360: 2e6d 6169 6e2e 7265 6e65 7761 6c2e 6372  .main.renewal.cr
-00010370: 7970 746f 5f75 7469 6c27 2920 5c0a 2020  ypto_util') \.  
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 2020 2020 6173 206d 6f63            as moc
-000103a0: 6b5f 6372 7970 746f 5f75 7469 6c3a 0a20  k_crypto_util:. 
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-000103d0: 6372 7970 746f 5f75 7469 6c2e 6e6f 7441  crypto_util.notA
-000103e0: 6674 6572 2e72 6574 7572 6e5f 7661 6c75  fter.return_valu
-000103f0: 6520 3d20 6578 7069 7279 5f64 6174 650a  e = expiry_date.
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00010420: 206d 6f63 6b2e 7061 7463 6828 2763 6572   mock.patch('cer
-00010430: 7462 6f74 2e5f 696e 7465 726e 616c 2e65  tbot._internal.e
-00010440: 6666 2e68 616e 646c 655f 7375 6273 6372  ff.handle_subscr
-00010450: 6970 7469 6f6e 2729 3a0a 2020 2020 2020  iption'):.      
-00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010470: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00010480: 2061 7267 733a 0a20 2020 2020 2020 2020   args:.         
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2020 2020 2020 2020 2020 2061 7267 7320             args 
-000104b0: 3d20 5b27 2d64 272c 2027 6973 6e6f 742e  = ['-d', 'isnot.
-000104c0: 6f72 6727 2c20 272d 6127 2c20 2773 7461  org', '-a', 'sta
-000104d0: 6e64 616c 6f6e 6527 2c20 2763 6572 746f  ndalone', 'certo
-000104e0: 6e6c 7927 5d0a 2020 2020 2020 2020 2020  nly'].          
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2020 2020 6966 2065 7874 7261 5f61        if extra_a
-00010510: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010530: 2020 2020 2020 2020 2061 7267 7320 2b3d           args +=
-00010540: 2065 7874 7261 5f61 7267 730a 2020 2020   extra_args.    
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00010570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2020 2020 2072 6574 2c20 7374 646f 7574       ret, stdout
-000105a0: 2c20 5f2c 205f 203d 2073 656c 662e 5f63  , _, _ = self._c
-000105b0: 616c 6c28 6172 6773 2c20 7374 646f 7574  all(args, stdout
-000105c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 2020 2020 6966 2072 6574 3a0a 2020        if ret:.  
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010610: 2020 2020 2020 7072 696e 7428 2252 6574        print("Ret
-00010620: 7572 6e65 6422 2c20 7265 7429 0a20 2020  urned", ret).   
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010650: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
-00010660: 7469 6f6e 4572 726f 7228 7265 7429 0a20  tionError(ret). 
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2061 7373 6572 7420 6e6f 7420 6572     assert not er
-000106a0: 726f 725f 6578 7065 6374 6564 2c20 2272  ror_expected, "r
-000106b0: 656e 6577 616c 2073 686f 756c 6420 6861  enewal should ha
-000106c0: 7665 2065 7272 6f72 6564 220a 2020 2020  ve errored".    
-000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000106f0: 7074 3a20 2320 7079 6c69 6e74 3a20 6469  pt: # pylint: di
-00010700: 7361 626c 653d 6261 7265 2d65 7863 6570  sable=bare-excep
-00010710: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 2020 2020 2020 6966 206e 6f74 2065 7272        if not err
-00010740: 6f72 5f65 7870 6563 7465 643a 0a20 2020  or_expected:.   
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2020 2072 6169 7365 2041 7373 6572       raise Asser
-00010780: 7469 6f6e 4572 726f 7228 0a20 2020 2020  tionError(.     
+00007360: 6f6d 202d 2d61 7061 6368 6527 2e73 706c  om --apache'.spl
+00007370: 6974 2829 290a 2020 2020 2020 2020 2320  it()).        # 
+00007380: 556e 646f 2074 6865 2063 6861 6e67 6573  Undo the changes
+00007390: 2077 6520 6d61 6465 2069 6e20 6361 6c6c   we made in call
+000073a0: 696e 6720 616e 6420 696e 2074 6573 7469  ing and in testi
+000073b0: 6e67 0a20 2020 2020 2020 206e 6577 5f63  ng.        new_c
+000073c0: 6f6e 6669 675b 2772 656e 6577 616c 7061  onfig['renewalpa
+000073d0: 7261 6d73 275d 5b27 6175 7468 656e 7469  rams']['authenti
+000073e0: 6361 746f 7227 5d20 3d20 276e 6769 6e78  cator'] = 'nginx
+000073f0: 270a 2020 2020 2020 2020 6e65 775f 636f  '.        new_co
+00007400: 6e66 6967 5b27 7265 6e65 7761 6c70 6172  nfig['renewalpar
+00007410: 616d 7327 5d5b 2769 6e73 7461 6c6c 6572  ams']['installer
+00007420: 275d 203d 2027 6e67 696e 7827 0a20 2020  '] = 'nginx'.   
+00007430: 2020 2020 2064 656c 206e 6577 5f63 6f6e       del new_con
+00007440: 6669 675b 2772 656e 6577 616c 7061 7261  fig['renewalpara
+00007450: 6d73 275d 5b27 636f 6e66 6967 5f64 6972  ms']['config_dir
+00007460: 275d 0a20 2020 2020 2020 206e 6577 5f63  '].        new_c
+00007470: 6f6e 6669 675b 2776 6572 7369 6f6e 275d  onfig['version']
+00007480: 203d 2073 656c 662e 6f72 6967 696e 616c   = self.original
+00007490: 5f63 6f6e 6669 675b 2776 6572 7369 6f6e  _config['version
+000074a0: 275d 0a0a 2020 2020 2020 2020 6173 7365  ']..        asse
+000074b0: 7274 206e 6577 5f63 6f6e 6669 6720 3d3d  rt new_config ==
+000074c0: 2073 656c 662e 6f72 6967 696e 616c 5f63   self.original_c
+000074d0: 6f6e 6669 670a 0a20 2020 2040 6d6f 636b  onfig..    @mock
+000074e0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+000074f0: 5f69 6e74 6572 6e61 6c2e 686f 6f6b 732e  _internal.hooks.
+00007500: 7661 6c69 6461 7465 5f68 6f6f 6b73 2729  validate_hooks')
+00007510: 0a20 2020 2064 6566 2074 6573 745f 7374  .    def test_st
+00007520: 6167 696e 675f 7573 6564 2873 656c 662c  aging_used(self,
+00007530: 2075 6e75 7365 645f 7661 6c69 6461 7465   unused_validate
+00007540: 5f68 6f6f 6b73 293a 0a20 2020 2020 2020  _hooks):.       
+00007550: 2022 2222 2043 6865 636b 2074 6861 7420   """ Check that 
+00007560: 7765 2075 7365 2074 6865 2073 7461 6769  we use the stagi
+00007570: 6e67 2073 6572 7665 7220 666f 7220 7468  ng server for th
+00007580: 6520 6472 7920 7275 6e20 2222 220a 2020  e dry run """.  
+00007590: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+000075a0: 662e 6f72 6967 696e 616c 5f63 6f6e 6669  f.original_confi
+000075b0: 675b 2772 656e 6577 616c 7061 7261 6d73  g['renewalparams
+000075c0: 275d 5b27 7365 7276 6572 275d 203d 3d20  ']['server'] == 
+000075d0: 5c0a 2020 2020 2020 2020 2020 2020 2768  \.            'h
+000075e0: 7474 7073 3a2f 2f61 636d 652d 7630 322e  ttps://acme-v02.
+000075f0: 6170 692e 6c65 7473 656e 6372 7970 742e  api.letsencrypt.
+00007600: 6f72 672f 6469 7265 6374 6f72 7927 0a0a  org/directory'..
+00007610: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+00007620: 6c6c 2827 2d2d 6365 7274 2d6e 616d 6520  ll('--cert-name 
+00007630: 6578 616d 706c 652e 636f 6d20 2d2d 7072  example.com --pr
+00007640: 652d 686f 6f6b 272e 7370 6c69 7428 2920  e-hook'.split() 
+00007650: 2b20 5b27 6563 686f 2070 7265 275d 290a  + ['echo pre']).
+00007660: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00007670: 2773 7461 6769 6e67 2720 696e 2073 656c  'staging' in sel
+00007680: 662e 6d6f 636b 735b 275f 696e 6974 5f6c  f.mocks['_init_l
+00007690: 655f 636c 6965 6e74 275d 2e63 616c 6c5f  e_client'].call_
+000076a0: 6172 6773 2e61 7267 735b 305d 2e73 6572  args.args[0].ser
+000076b0: 7665 720a 2020 2020 2020 2020 6173 7365  ver.        asse
+000076c0: 7274 2027 7374 6167 696e 6727 2069 6e20  rt 'staging' in 
+000076d0: 7365 6c66 2e6d 6f63 6b73 5b27 5f67 6574  self.mocks['_get
+000076e0: 5f61 6e64 5f73 6176 655f 6365 7274 275d  _and_save_cert']
+000076f0: 2e63 616c 6c5f 6172 6773 2e61 7267 735b  .call_args.args[
+00007700: 315d 2e73 6572 7665 720a 0a20 2020 2064  1].server..    d
+00007710: 6566 2074 6573 745f 6e65 775f 6163 636f  ef test_new_acco
+00007720: 756e 745f 6f72 5f73 6572 7665 725f 6572  unt_or_server_er
+00007730: 726f 7273 2873 656c 6629 3a0a 2020 2020  rors(self):.    
+00007740: 2020 2020 2222 2220 4368 6563 6b20 7468      """ Check th
+00007750: 6174 2077 6520 6572 726f 7220 7768 656e  at we error when
+00007760: 2061 7474 656d 7074 696e 6720 746f 2063   attempting to c
+00007770: 6861 6e67 6520 7468 6520 6163 636f 756e  hange the accoun
+00007780: 7420 6964 206f 7220 7365 7276 6572 2c0a  t id or server,.
+00007790: 2020 2020 2020 2020 2020 2020 6275 7420              but 
+000077a0: 6e6f 7420 7768 656e 2069 7427 7320 7468  not when it's th
+000077b0: 6520 7361 6d65 0a20 2020 2020 2020 2022  e same.        "
+000077c0: 2222 0a20 2020 2020 2020 206f 7269 675f  "".        orig_
+000077d0: 6163 636f 756e 745f 6964 203d 2073 656c  account_id = sel
+000077e0: 662e 6f72 6967 696e 616c 5f63 6f6e 6669  f.original_confi
+000077f0: 675b 2772 656e 6577 616c 7061 7261 6d73  g['renewalparams
+00007800: 275d 5b27 6163 636f 756e 7427 5d0a 2020  ']['account'].  
+00007810: 2020 2020 2020 6f72 6967 5f73 6572 7665        orig_serve
+00007820: 7220 3d20 7365 6c66 2e6f 7269 6769 6e61  r = self.origina
+00007830: 6c5f 636f 6e66 6967 5b27 7265 6e65 7761  l_config['renewa
+00007840: 6c70 6172 616d 7327 5d5b 2773 6572 7665  lparams']['serve
+00007850: 7227 5d0a 0a20 2020 2020 2020 2023 206e  r']..        # n
+00007860: 6577 2061 6363 6f75 6e74 0a20 2020 2020  ew account.     
+00007870: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00007880: 2020 2020 7365 6c66 2e5f 6361 6c6c 2866      self._call(f
+00007890: 272d 2d63 6572 742d 6e61 6d65 2065 7861  '--cert-name exa
+000078a0: 6d70 6c65 2e63 6f6d 202d 2d61 6363 6f75  mple.com --accou
+000078b0: 6e74 206e 6577 6163 636f 756e 7469 6427  nt newaccountid'
+000078c0: 2e73 706c 6974 2829 290a 2020 2020 2020  .split()).      
+000078d0: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
+000078e0: 436f 6e66 6967 7572 6174 696f 6e45 7272  ConfigurationErr
+000078f0: 6f72 2061 7320 6572 723a 0a20 2020 2020  or as err:.     
+00007900: 2020 2020 2020 2061 7373 6572 7420 2255         assert "U
+00007910: 7369 6e67 2072 6563 6f6e 6669 6775 7265  sing reconfigure
+00007920: 2074 6f20 6368 616e 6765 2074 6865 2041   to change the A
+00007930: 434d 4520 6163 636f 756e 7422 2069 6e20  CME account" in 
+00007940: 7374 7228 6572 7229 0a0a 2020 2020 2020  str(err)..      
+00007950: 2020 2320 6368 6563 6b20 7468 6174 2063    # check that c
+00007960: 6f6e 6669 6720 6973 6e27 7420 6d6f 6469  onfig isn't modi
+00007970: 6669 6564 0a20 2020 2020 2020 2077 6974  fied.        wit
+00007980: 6820 6f70 656e 2873 656c 662e 7265 6e65  h open(self.rene
+00007990: 7761 6c5f 6669 6c65 2c20 2772 2729 2061  wal_file, 'r') a
+000079a0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+000079b0: 206e 6577 5f63 6f6e 6669 6720 3d20 636f   new_config = co
+000079c0: 6e66 6967 6f62 6a2e 436f 6e66 6967 4f62  nfigobj.ConfigOb
+000079d0: 6a28 662c 2065 6e63 6f64 696e 673d 2775  j(f, encoding='u
+000079e0: 7466 2d38 272c 2064 6566 6175 6c74 5f65  tf-8', default_e
+000079f0: 6e63 6f64 696e 673d 2775 7466 2d38 2729  ncoding='utf-8')
+00007a00: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00007a10: 6e65 775f 636f 6e66 6967 5b27 7265 6e65  new_config['rene
+00007a20: 7761 6c70 6172 616d 7327 5d5b 2761 6363  walparams']['acc
+00007a30: 6f75 6e74 275d 203d 3d20 6f72 6967 5f61  ount'] == orig_a
+00007a40: 6363 6f75 6e74 5f69 640a 0a20 2020 2020  ccount_id..     
+00007a50: 2020 2023 2073 616d 6520 6163 636f 756e     # same accoun
+00007a60: 740a 2020 2020 2020 2020 6e65 775f 636f  t.        new_co
+00007a70: 6e66 6967 203d 2073 656c 662e 5f63 616c  nfig = self._cal
+00007a80: 6c28 6627 2d2d 6365 7274 2d6e 616d 6520  l(f'--cert-name 
+00007a90: 6578 616d 706c 652e 636f 6d20 2d2d 6163  example.com --ac
+00007aa0: 636f 756e 7420 7b6f 7269 675f 6163 636f  count {orig_acco
+00007ab0: 756e 745f 6964 7d27 2e73 706c 6974 2829  unt_id}'.split()
+00007ac0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00007ad0: 206e 6577 5f63 6f6e 6669 675b 2772 656e   new_config['ren
+00007ae0: 6577 616c 7061 7261 6d73 275d 5b27 6163  ewalparams']['ac
+00007af0: 636f 756e 7427 5d20 3d3d 206f 7269 675f  count'] == orig_
+00007b00: 6163 636f 756e 745f 6964 0a0a 2020 2020  account_id..    
+00007b10: 2020 2020 2320 6e65 7720 7365 7276 6572      # new server
+00007b20: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00007b30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007b40: 6361 6c6c 2866 272d 2d63 6572 742d 6e61  call(f'--cert-na
+00007b50: 6d65 2065 7861 6d70 6c65 2e63 6f6d 202d  me example.com -
+00007b60: 2d73 6572 7665 7220 782e 636f 6d27 2e73  -server x.com'.s
+00007b70: 706c 6974 2829 290a 2020 2020 2020 2020  plit()).        
+00007b80: 6578 6365 7074 2065 7272 6f72 732e 436f  except errors.Co
+00007b90: 6e66 6967 7572 6174 696f 6e45 7272 6f72  nfigurationError
+00007ba0: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+00007bb0: 2020 2020 2061 7373 6572 7420 2255 7369       assert "Usi
+00007bc0: 6e67 2072 6563 6f6e 6669 6775 7265 2074  ng reconfigure t
+00007bd0: 6f20 6368 616e 6765 2074 6865 2041 434d  o change the ACM
+00007be0: 4520 6163 636f 756e 7422 2069 6e20 7374  E account" in st
+00007bf0: 7228 6572 7229 0a0a 2020 2020 2020 2020  r(err)..        
+00007c00: 2320 6368 6563 6b20 7468 6174 2063 6f6e  # check that con
+00007c10: 6669 6720 6973 6e27 7420 6d6f 6469 6669  fig isn't modifi
+00007c20: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
+00007c30: 6f70 656e 2873 656c 662e 7265 6e65 7761  open(self.renewa
+00007c40: 6c5f 6669 6c65 2c20 2772 2729 2061 7320  l_file, 'r') as 
+00007c50: 663a 0a20 2020 2020 2020 2020 2020 206e  f:.            n
+00007c60: 6577 5f63 6f6e 6669 6720 3d20 636f 6e66  ew_config = conf
+00007c70: 6967 6f62 6a2e 436f 6e66 6967 4f62 6a28  igobj.ConfigObj(
+00007c80: 662c 2065 6e63 6f64 696e 673d 2775 7466  f, encoding='utf
+00007c90: 2d38 272c 2064 6566 6175 6c74 5f65 6e63  -8', default_enc
+00007ca0: 6f64 696e 673d 2775 7466 2d38 2729 0a20  oding='utf-8'). 
+00007cb0: 2020 2020 2020 2061 7373 6572 7420 6e65         assert ne
+00007cc0: 775f 636f 6e66 6967 5b27 7265 6e65 7761  w_config['renewa
+00007cd0: 6c70 6172 616d 7327 5d5b 2773 6572 7665  lparams']['serve
+00007ce0: 7227 5d20 3d3d 206f 7269 675f 7365 7276  r'] == orig_serv
+00007cf0: 6572 0a0a 2020 2020 2020 2020 2320 7361  er..        # sa
+00007d00: 6d65 2073 6572 7665 720a 2020 2020 2020  me server.      
+00007d10: 2020 6e65 775f 636f 6e66 6967 203d 2073    new_config = s
+00007d20: 656c 662e 5f63 616c 6c28 6627 2d2d 6365  elf._call(f'--ce
+00007d30: 7274 2d6e 616d 6520 6578 616d 706c 652e  rt-name example.
+00007d40: 636f 6d20 2d2d 7365 7276 6572 207b 6f72  com --server {or
+00007d50: 6967 5f73 6572 7665 727d 272e 7370 6c69  ig_server}'.spli
+00007d60: 7428 2929 0a20 2020 2020 2020 2061 7373  t()).        ass
+00007d70: 6572 7420 6e65 775f 636f 6e66 6967 5b27  ert new_config['
+00007d80: 7265 6e65 7761 6c70 6172 616d 7327 5d5b  renewalparams'][
+00007d90: 2773 6572 7665 7227 5d20 3d3d 206f 7269  'server'] == ori
+00007da0: 675f 7365 7276 6572 0a0a 2020 2020 406d  g_server..    @m
+00007db0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00007dc0: 6f74 2e5f 696e 7465 726e 616c 2e68 6f6f  ot._internal.hoo
+00007dd0: 6b73 2e76 616c 6964 6174 655f 686f 6f6b  ks.validate_hook
+00007de0: 7327 290a 2020 2020 6465 6620 7465 7374  s').    def test
+00007df0: 5f75 7064 6174 655f 686f 6f6b 7328 7365  _update_hooks(se
+00007e00: 6c66 2c20 756e 7573 6564 5f76 616c 6964  lf, unused_valid
+00007e10: 6174 655f 686f 6f6b 7329 3a0a 2020 2020  ate_hooks):.    
+00007e20: 2020 2020 6173 7365 7274 2027 7072 655f      assert 'pre_
+00007e30: 686f 6f6b 2720 6e6f 7420 696e 2073 656c  hook' not in sel
+00007e40: 662e 6f72 6967 696e 616c 5f63 6f6e 6669  f.original_confi
+00007e50: 670a 2020 2020 2020 2020 2320 7465 7374  g.        # test
+00007e60: 2073 6574 0a20 2020 2020 2020 206e 6577   set.        new
+00007e70: 5f63 6f6e 6669 6720 3d20 7365 6c66 2e5f  _config = self._
+00007e80: 6361 6c6c 2827 2d2d 6365 7274 2d6e 616d  call('--cert-nam
+00007e90: 6520 6578 616d 706c 652e 636f 6d20 2d2d  e example.com --
+00007ea0: 7072 652d 686f 6f6b 272e 7370 6c69 7428  pre-hook'.split(
+00007eb0: 2920 2b20 5b27 6563 686f 2070 7265 275d  ) + ['echo pre']
+00007ec0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00007ed0: 206e 6577 5f63 6f6e 6669 675b 2772 656e   new_config['ren
+00007ee0: 6577 616c 7061 7261 6d73 275d 5b27 7072  ewalparams']['pr
+00007ef0: 655f 686f 6f6b 275d 203d 3d20 2765 6368  e_hook'] == 'ech
+00007f00: 6f20 7072 6527 0a20 2020 2020 2020 2023  o pre'.        #
+00007f10: 2074 6573 7420 7570 6461 7465 0a20 2020   test update.   
+00007f20: 2020 2020 206e 6577 5f63 6f6e 6669 6720       new_config 
+00007f30: 3d20 7365 6c66 2e5f 6361 6c6c 2827 2d2d  = self._call('--
+00007f40: 6365 7274 2d6e 616d 6520 6578 616d 706c  cert-name exampl
+00007f50: 652e 636f 6d20 2d2d 7072 652d 686f 6f6b  e.com --pre-hook
+00007f60: 272e 7370 6c69 7428 2920 2b20 5b27 6563  '.split() + ['ec
+00007f70: 686f 2070 7265 3227 5d29 0a20 2020 2020  ho pre2']).     
+00007f80: 2020 2061 7373 6572 7420 6e65 775f 636f     assert new_co
+00007f90: 6e66 6967 5b27 7265 6e65 7761 6c70 6172  nfig['renewalpar
+00007fa0: 616d 7327 5d5b 2770 7265 5f68 6f6f 6b27  ams']['pre_hook'
+00007fb0: 5d20 3d3d 2027 6563 686f 2070 7265 3227  ] == 'echo pre2'
+00007fc0: 0a0a 2020 2020 2020 2020 2320 7465 7374  ..        # test
+00007fd0: 2064 6570 6c6f 7920 686f 6f6b 2069 7320   deploy hook is 
+00007fe0: 7365 7420 6576 656e 2074 686f 7567 6820  set even though 
+00007ff0: 7765 2064 6964 2061 2064 7279 2072 756e  we did a dry run
+00008000: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00008010: 2772 656e 6577 5f68 6f6f 6b27 206e 6f74  'renew_hook' not
+00008020: 2069 6e20 7365 6c66 2e6f 7269 6769 6e61   in self.origina
+00008030: 6c5f 636f 6e66 6967 0a20 2020 2020 2020  l_config.       
+00008040: 206e 6577 5f63 6f6e 6669 6720 3d20 7365   new_config = se
+00008050: 6c66 2e5f 6361 6c6c 2827 2d2d 6365 7274  lf._call('--cert
+00008060: 2d6e 616d 6520 6578 616d 706c 652e 636f  -name example.co
+00008070: 6d20 2d2d 6465 706c 6f79 2d68 6f6f 6b27  m --deploy-hook'
+00008080: 2e73 706c 6974 2829 202b 205b 2765 6368  .split() + ['ech
+00008090: 6f20 6465 706c 6f79 275d 290a 2020 2020  o deploy']).    
+000080a0: 2020 2020 6173 7365 7274 206e 6577 5f63      assert new_c
+000080b0: 6f6e 6669 675b 2772 656e 6577 616c 7061  onfig['renewalpa
+000080c0: 7261 6d73 275d 5b27 7265 6e65 775f 686f  rams']['renew_ho
+000080d0: 6f6b 275d 203d 3d20 2765 6368 6f20 6465  ok'] == 'echo de
+000080e0: 706c 6f79 270a 0a20 2020 2064 6566 2074  ploy'..    def t
+000080f0: 6573 745f 6472 795f 7275 6e5f 6661 696c  est_dry_run_fail
+00008100: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00008110: 2023 2073 6574 2073 6964 6520 6566 6665   # set side effe
+00008120: 6374 206f 6620 7261 6973 696e 6720 6572  ct of raising er
+00008130: 726f 720a 2020 2020 2020 2020 7365 6c66  ror.        self
+00008140: 2e6d 6f63 6b73 5b27 5f67 6574 5f61 6e64  .mocks['_get_and
+00008150: 5f73 6176 655f 6365 7274 275d 2e73 6964  _save_cert'].sid
+00008160: 655f 6566 6665 6374 203d 2065 7272 6f72  e_effect = error
+00008170: 732e 4572 726f 720a 0a20 2020 2020 2020  s.Error..       
+00008180: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00008190: 2020 7365 6c66 2e5f 6361 6c6c 2827 2d2d    self._call('--
+000081a0: 6365 7274 2d6e 616d 6520 6578 616d 706c  cert-name exampl
+000081b0: 652e 636f 6d20 2d2d 6170 6163 6865 272e  e.com --apache'.
+000081c0: 7370 6c69 7428 2929 0a20 2020 2020 2020  split()).       
+000081d0: 2065 7863 6570 7420 6572 726f 7273 2e45   except errors.E
+000081e0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+000081f0: 2020 7061 7373 0a0a 2020 2020 2020 2020    pass..        
+00008200: 2320 6368 6563 6b20 7468 6174 2063 6f6e  # check that con
+00008210: 6669 6720 6973 6e27 7420 6d6f 6469 6669  fig isn't modifi
+00008220: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
+00008230: 6f70 656e 2873 656c 662e 7265 6e65 7761  open(self.renewa
+00008240: 6c5f 6669 6c65 2c20 2772 2729 2061 7320  l_file, 'r') as 
+00008250: 663a 0a20 2020 2020 2020 2020 2020 206e  f:.            n
+00008260: 6577 5f63 6f6e 6669 6720 3d20 636f 6e66  ew_config = conf
+00008270: 6967 6f62 6a2e 436f 6e66 6967 4f62 6a28  igobj.ConfigObj(
+00008280: 662c 2065 6e63 6f64 696e 673d 2775 7466  f, encoding='utf
+00008290: 2d38 272c 2064 6566 6175 6c74 5f65 6e63  -8', default_enc
+000082a0: 6f64 696e 673d 2775 7466 2d38 2729 0a20  oding='utf-8'). 
+000082b0: 2020 2020 2020 2061 7373 6572 7420 6e65         assert ne
+000082c0: 775f 636f 6e66 6967 5b27 7265 6e65 7761  w_config['renewa
+000082d0: 6c70 6172 616d 7327 5d5b 2761 7574 6865  lparams']['authe
+000082e0: 6e74 6963 6174 6f72 275d 203d 3d20 276e  nticator'] == 'n
+000082f0: 6769 6e78 270a 0a20 2020 2040 6d6f 636b  ginx'..    @mock
+00008300: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+00008310: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e64  _internal.main.d
+00008320: 6973 706c 6179 5f75 7469 6c2e 6e6f 7469  isplay_util.noti
+00008330: 6679 2729 0a20 2020 2064 6566 2074 6573  fy').    def tes
+00008340: 745f 7265 706f 7274 5f72 6573 756c 7473  t_report_results
+00008350: 2873 656c 662c 206d 6f63 6b5f 6e6f 7469  (self, mock_noti
+00008360: 6679 293a 0a20 2020 2020 2020 2023 206d  fy):.        # m
+00008370: 616b 6520 7375 7265 2072 6570 6f72 7420  ake sure report 
+00008380: 7265 7375 6c74 7320 776f 726b 7320 7768  results works wh
+00008390: 656e 2063 6f6e 6669 6720 6861 7320 6120  en config has a 
+000083a0: 7765 6272 6f6f 7420 6d61 700a 2020 2020  webroot map.    
+000083b0: 2020 2020 6f72 6967 696e 616c 5f63 6f6e      original_con
+000083c0: 6669 6720 3d20 2222 220a 2020 2020 2020  fig = """.      
+000083d0: 2020 2020 2020 7665 7273 696f 6e20 3d20        version = 
+000083e0: 322e 302e 300a 2020 2020 2020 2020 2020  2.0.0.          
+000083f0: 2020 6172 6368 6976 655f 6469 7220 3d20    archive_dir = 
+00008400: 2f65 7463 2f6c 6574 7365 6e63 7279 7074  /etc/letsencrypt
+00008410: 2f61 7263 6869 7665 2f65 7861 6d70 6c65  /archive/example
+00008420: 2e63 6f6d 0a20 2020 2020 2020 2020 2020  .com.           
+00008430: 2063 6572 7420 3d20 2f65 7463 2f6c 6574   cert = /etc/let
+00008440: 7365 6e63 7279 7074 2f6c 6976 652f 6578  sencrypt/live/ex
+00008450: 616d 706c 652e 636f 6d2f 6365 7274 2e70  ample.com/cert.p
+00008460: 656d 0a20 2020 2020 2020 2020 2020 2070  em.            p
+00008470: 7269 766b 6579 203d 202f 6574 632f 6c65  rivkey = /etc/le
+00008480: 7473 656e 6372 7970 742f 6c69 7665 2f65  tsencrypt/live/e
+00008490: 7861 6d70 6c65 2e63 6f6d 2f70 7269 766b  xample.com/privk
+000084a0: 6579 2e70 656d 0a20 2020 2020 2020 2020  ey.pem.         
+000084b0: 2020 2063 6861 696e 203d 202f 6574 632f     chain = /etc/
+000084c0: 6c65 7473 656e 6372 7970 742f 6c69 7665  letsencrypt/live
+000084d0: 2f65 7861 6d70 6c65 2e63 6f6d 2f63 6861  /example.com/cha
+000084e0: 696e 2e70 656d 0a20 2020 2020 2020 2020  in.pem.         
+000084f0: 2020 2066 756c 6c63 6861 696e 203d 202f     fullchain = /
+00008500: 6574 632f 6c65 7473 656e 6372 7970 742f  etc/letsencrypt/
+00008510: 6c69 7665 2f65 7861 6d70 6c65 2e63 6f6d  live/example.com
+00008520: 2f66 756c 6c63 6861 696e 2e70 656d 0a0a  /fullchain.pem..
+00008530: 2020 2020 2020 2020 2020 2020 2320 4f70              # Op
+00008540: 7469 6f6e 7320 7573 6564 2069 6e20 7468  tions used in th
+00008550: 6520 7265 6e65 7761 6c20 7072 6f63 6573  e renewal proces
+00008560: 730a 2020 2020 2020 2020 2020 2020 5b72  s.            [r
+00008570: 656e 6577 616c 7061 7261 6d73 5d0a 2020  enewalparams].  
+00008580: 2020 2020 2020 2020 2020 6163 636f 756e            accoun
+00008590: 7420 3d20 6565 3433 3633 3464 6230 6161  t = ee43634db0aa
+000085a0: 3465 3638 3034 6631 3532 6265 3339 3939  4e6804f152be3999
+000085b0: 3065 3661 0a20 2020 2020 2020 2020 2020  0e6a.           
+000085c0: 2073 6572 7665 7220 3d20 6874 7470 733a   server = https:
+000085d0: 2f2f 6163 6d65 2d73 7461 6769 6e67 2d76  //acme-staging-v
+000085e0: 3032 2e61 7069 2e6c 6574 7365 6e63 7279  02.api.letsencry
+000085f0: 7074 2e6f 7267 2f64 6972 6563 746f 7279  pt.org/directory
+00008600: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
+00008610: 6865 6e74 6963 6174 6f72 203d 2077 6562  henticator = web
+00008620: 726f 6f74 0a20 2020 2020 2020 2020 2020  root.           
+00008630: 2069 6e73 7461 6c6c 6572 203d 206e 6769   installer = ngi
+00008640: 6e78 0a20 2020 2020 2020 2020 2020 206b  nx.            k
+00008650: 6579 5f74 7970 6520 3d20 6563 6473 610a  ey_type = ecdsa.
+00008660: 2020 2020 2020 2020 2020 2020 7765 6272              webr
+00008670: 6f6f 745f 7061 7468 203d 202f 7661 722f  oot_path = /var/
+00008680: 7777 772f 6874 6d6c 2c0a 2020 2020 2020  www/html,.      
+00008690: 2020 2020 2020 5b5b 7765 6272 6f6f 745f        [[webroot_
+000086a0: 6d61 705d 5d0a 2020 2020 2020 2020 2020  map]].          
+000086b0: 2020 6578 616d 706c 652e 636f 6d20 3d20    example.com = 
+000086c0: 2f76 6172 2f77 7777 2f68 746d 6c0a 2020  /var/www/html.  
+000086d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000086e0: 2020 7769 7468 206f 7065 6e28 7365 6c66    with open(self
+000086f0: 2e72 656e 6577 616c 5f66 696c 652c 2027  .renewal_file, '
+00008700: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
+00008710: 2020 2020 2020 662e 7772 6974 6528 6f72        f.write(or
+00008720: 6967 696e 616c 5f63 6f6e 6669 6729 0a20  iginal_config). 
+00008730: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00008740: 2873 656c 662e 7265 6e65 7761 6c5f 6669  (self.renewal_fi
+00008750: 6c65 2c20 2772 2729 2061 7320 663a 0a20  le, 'r') as f:. 
+00008760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008770: 6f72 6967 696e 616c 5f63 6f6e 6669 6720  original_config 
+00008780: 3d20 636f 6e66 6967 6f62 6a2e 436f 6e66  = configobj.Conf
+00008790: 6967 4f62 6a28 662c 0a20 2020 2020 2020  igObj(f,.       
+000087a0: 2020 2020 2020 2020 2065 6e63 6f64 696e           encodin
+000087b0: 673d 2775 7466 2d38 272c 2064 6566 6175  g='utf-8', defau
+000087c0: 6c74 5f65 6e63 6f64 696e 673d 2775 7466  lt_encoding='utf
+000087d0: 2d38 2729 0a0a 2020 2020 2020 2020 6e61  -8')..        na
+000087e0: 6d65 645f 6d6f 636b 203d 206d 6f63 6b2e  med_mock = mock.
+000087f0: 4d6f 636b 2829 0a20 2020 2020 2020 206e  Mock().        n
+00008800: 616d 6564 5f6d 6f63 6b2e 6e61 6d65 203d  amed_mock.name =
+00008810: 2027 6e67 696e 7827 0a0a 2020 2020 2020   'nginx'..      
+00008820: 2020 7365 6c66 2e6d 6f63 6b73 5b27 7069    self.mocks['pi
+00008830: 636b 5f61 7574 6827 5d2e 7265 7475 726e  ck_auth'].return
+00008840: 5f76 616c 7565 203d 206e 616d 6564 5f6d  _value = named_m
+00008850: 6f63 6b0a 2020 2020 2020 2020 7365 6c66  ock.        self
+00008860: 2e6d 6f63 6b73 5b27 6669 6e64 5f69 6e69  .mocks['find_ini
+00008870: 7427 5d2e 7265 7475 726e 5f76 616c 7565  t'].return_value
+00008880: 203d 206e 616d 6564 5f6d 6f63 6b0a 0a20   = named_mock.. 
+00008890: 2020 2020 2020 206e 6577 5f63 6f6e 6669         new_confi
+000088a0: 6720 3d20 7365 6c66 2e5f 6361 6c6c 2827  g = self._call('
+000088b0: 2d2d 6365 7274 2d6e 616d 6520 6578 616d  --cert-name exam
+000088c0: 706c 652e 636f 6d20 2d2d 6e67 696e 7827  ple.com --nginx'
+000088d0: 2e73 706c 6974 2829 290a 2020 2020 2020  .split()).      
+000088e0: 2020 6173 7365 7274 206e 6577 5f63 6f6e    assert new_con
+000088f0: 6669 675b 2772 656e 6577 616c 7061 7261  fig['renewalpara
+00008900: 6d73 275d 5b27 6175 7468 656e 7469 6361  ms']['authentica
+00008910: 746f 7227 5d20 3d3d 2027 6e67 696e 7827  tor'] == 'nginx'
+00008920: 0a20 2020 2020 2020 206d 6f63 6b5f 6e6f  .        mock_no
+00008930: 7469 6679 2e61 7373 6572 745f 6361 6c6c  tify.assert_call
+00008940: 6564 5f77 6974 6828 0a20 2020 2020 2020  ed_with(.       
+00008950: 2020 2020 2027 5c6e 5375 6363 6573 7366       '\nSuccessf
+00008960: 756c 6c79 2075 7064 6174 6564 2063 6f6e  ully updated con
+00008970: 6669 6775 7261 7469 6f6e 2e27 2b0a 2020  figuration.'+.  
+00008980: 2020 2020 2020 2020 2020 275c 6e43 6861            '\nCha
+00008990: 6e67 6573 2077 696c 6c20 6170 706c 7920  nges will apply 
+000089a0: 7768 656e 2074 6865 2063 6572 7469 6669  when the certifi
+000089b0: 6361 7465 2072 656e 6577 732e 2729 0a0a  cate renews.')..
+000089c0: 0a63 6c61 7373 2044 656c 6574 6549 6641  .class DeleteIfA
+000089d0: 7070 726f 7072 6961 7465 5465 7374 2874  ppropriateTest(t
+000089e0: 6573 745f 7574 696c 2e43 6f6e 6669 6754  est_util.ConfigT
+000089f0: 6573 7443 6173 6529 3a0a 2020 2020 2222  estCase):.    ""
+00008a00: 2254 6573 7473 2066 6f72 2063 6572 7462  "Tests for certb
+00008a10: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+00008a20: 6e2e 5f64 656c 6574 655f 6966 5f61 7070  n._delete_if_app
+00008a30: 726f 7072 6961 7465 2022 2222 0a0a 2020  ropriate """..  
+00008a40: 2020 6465 6620 5f63 616c 6c28 7365 6c66    def _call(self
+00008a50: 2c20 6d6f 636b 5f63 6f6e 6669 6729 3a0a  , mock_config):.
+00008a60: 2020 2020 2020 2020 6672 6f6d 2063 6572          from cer
+00008a70: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+00008a80: 6169 6e20 696d 706f 7274 205f 6465 6c65  ain import _dele
+00008a90: 7465 5f69 665f 6170 7072 6f70 7269 6174  te_if_appropriat
+00008aa0: 650a 2020 2020 2020 2020 5f64 656c 6574  e.        _delet
+00008ab0: 655f 6966 5f61 7070 726f 7072 6961 7465  e_if_appropriate
+00008ac0: 286d 6f63 6b5f 636f 6e66 6967 290a 0a20  (mock_config).. 
+00008ad0: 2020 2064 6566 205f 7465 7374 5f64 656c     def _test_del
+00008ae0: 6574 655f 6f70 745f 6f75 745f 636f 6d6d  ete_opt_out_comm
+00008af0: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+00008b00: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+00008b10: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00008b20: 726e 616c 2e63 6572 745f 6d61 6e61 6765  rnal.cert_manage
+00008b30: 722e 6465 6c65 7465 2729 2061 7320 6d6f  r.delete') as mo
+00008b40: 636b 5f64 656c 6574 653a 0a20 2020 2020  ck_delete:.     
+00008b50: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+00008b60: 6c28 7365 6c66 2e63 6f6e 6669 6729 0a20  l(self.config). 
+00008b70: 2020 2020 2020 206d 6f63 6b5f 6465 6c65         mock_dele
+00008b80: 7465 2e61 7373 6572 745f 6e6f 745f 6361  te.assert_not_ca
+00008b90: 6c6c 6564 2829 0a0a 2020 2020 4074 6573  lled()..    @tes
+00008ba0: 745f 7574 696c 2e70 6174 6368 5f64 6973  t_util.patch_dis
+00008bb0: 706c 6179 5f75 7469 6c28 290a 2020 2020  play_util().    
+00008bc0: 6465 6620 7465 7374 5f64 656c 6574 655f  def test_delete_
+00008bd0: 666c 6167 5f6f 7074 5f6f 7574 2873 656c  flag_opt_out(sel
+00008be0: 662c 2075 6e75 7365 645f 6d6f 636b 5f67  f, unused_mock_g
+00008bf0: 6574 5f75 7469 6c69 7479 293a 0a20 2020  et_utility):.   
+00008c00: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
+00008c10: 2e64 656c 6574 655f 6166 7465 725f 7265  .delete_after_re
+00008c20: 766f 6b65 203d 2046 616c 7365 0a20 2020  voke = False.   
+00008c30: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
+00008c40: 6465 6c65 7465 5f6f 7074 5f6f 7574 5f63  delete_opt_out_c
+00008c50: 6f6d 6d6f 6e28 290a 0a20 2020 2040 7465  ommon()..    @te
+00008c60: 7374 5f75 7469 6c2e 7061 7463 685f 6469  st_util.patch_di
+00008c70: 7370 6c61 795f 7574 696c 2829 0a20 2020  splay_util().   
+00008c80: 2064 6566 2074 6573 745f 6465 6c65 7465   def test_delete
+00008c90: 5f70 726f 6d70 745f 6f70 745f 6f75 7428  _prompt_opt_out(
+00008ca0: 7365 6c66 2c20 6d6f 636b 5f67 6574 5f75  self, mock_get_u
+00008cb0: 7469 6c69 7479 293a 0a20 2020 2020 2020  tility):.       
+00008cc0: 2075 7469 6c5f 6d6f 636b 203d 206d 6f63   util_mock = moc
+00008cd0: 6b5f 6765 745f 7574 696c 6974 7928 290a  k_get_utility().
+00008ce0: 2020 2020 2020 2020 7574 696c 5f6d 6f63          util_moc
+00008cf0: 6b2e 7965 736e 6f2e 7265 7475 726e 5f76  k.yesno.return_v
+00008d00: 616c 7565 203d 2046 616c 7365 0a20 2020  alue = False.   
+00008d10: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
+00008d20: 6465 6c65 7465 5f6f 7074 5f6f 7574 5f63  delete_opt_out_c
+00008d30: 6f6d 6d6f 6e28 290a 0a20 2020 2040 6d6f  ommon()..    @mo
+00008d40: 636b 2e70 6174 6368 2822 6365 7274 626f  ck.patch("certbo
+00008d50: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+00008d60: 2e6c 6f67 6765 722e 7761 726e 696e 6722  .logger.warning"
+00008d70: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00008d80: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00008d90: 726e 616c 2e73 746f 7261 6765 2e72 656e  rnal.storage.ren
+00008da0: 6577 616c 5f66 696c 655f 666f 725f 6365  ewal_file_for_ce
+00008db0: 7274 6e61 6d65 2729 0a20 2020 2040 6d6f  rtname').    @mo
+00008dc0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+00008dd0: 742e 5f69 6e74 6572 6e61 6c2e 6365 7274  t._internal.cert
+00008de0: 5f6d 616e 6167 6572 2e64 656c 6574 6527  _manager.delete'
+00008df0: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00008e00: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00008e10: 726e 616c 2e63 6572 745f 6d61 6e61 6765  rnal.cert_manage
+00008e20: 722e 6d61 7463 685f 616e 645f 6368 6563  r.match_and_chec
+00008e30: 6b5f 6f76 6572 6c61 7073 2729 0a20 2020  k_overlaps').   
+00008e40: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+00008e50: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00008e60: 7374 6f72 6167 652e 6675 6c6c 5f61 7263  storage.full_arc
+00008e70: 6869 7665 5f70 6174 6827 290a 2020 2020  hive_path').    
+00008e80: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
+00008e90: 7462 6f74 2e5f 696e 7465 726e 616c 2e63  tbot._internal.c
+00008ea0: 6572 745f 6d61 6e61 6765 722e 6365 7274  ert_manager.cert
+00008eb0: 5f70 6174 685f 746f 5f6c 696e 6561 6765  _path_to_lineage
+00008ec0: 2729 0a20 2020 2040 7465 7374 5f75 7469  ').    @test_uti
+00008ed0: 6c2e 7061 7463 685f 6469 7370 6c61 795f  l.patch_display_
+00008ee0: 7574 696c 2829 0a20 2020 2064 6566 2074  util().    def t
+00008ef0: 6573 745f 6f76 6572 6c61 7070 696e 675f  est_overlapping_
+00008f00: 6172 6368 6976 655f 6469 7273 2873 656c  archive_dirs(sel
+00008f10: 662c 206d 6f63 6b5f 6765 745f 7574 696c  f, mock_get_util
+00008f20: 6974 792c 0a20 2020 2020 2020 2020 2020  ity,.           
+00008f30: 206d 6f63 6b5f 6365 7274 5f70 6174 685f   mock_cert_path_
+00008f40: 746f 5f6c 696e 6561 6765 2c20 6d6f 636b  to_lineage, mock
+00008f50: 5f61 7263 6869 7665 2c0a 2020 2020 2020  _archive,.      
+00008f60: 2020 2020 2020 6d6f 636b 5f6d 6174 6368        mock_match
+00008f70: 5f61 6e64 5f63 6865 636b 5f6f 7665 726c  _and_check_overl
+00008f80: 6170 732c 206d 6f63 6b5f 6465 6c65 7465  aps, mock_delete
+00008f90: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+00008fa0: 636b 5f72 656e 6577 616c 5f66 696c 655f  ck_renewal_file_
+00008fb0: 666f 725f 6365 7274 6e61 6d65 2c20 6d6f  for_certname, mo
+00008fc0: 636b 5f77 6172 6e69 6e67 293a 0a20 2020  ck_warning):.   
+00008fd0: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
+00008fe0: 6973 6162 6c65 203d 2075 6e75 7365 642d  isable = unused-
+00008ff0: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
+00009000: 2063 6f6e 6669 6720 3d20 7365 6c66 2e63   config = self.c
+00009010: 6f6e 6669 670a 2020 2020 2020 2020 636f  onfig.        co
+00009020: 6e66 6967 2e63 6572 745f 7061 7468 203d  nfig.cert_path =
+00009030: 2022 2f73 6f6d 652f 7265 6173 6f6e 6162   "/some/reasonab
+00009040: 6c65 2f70 6174 6822 0a20 2020 2020 2020  le/path".       
+00009050: 2063 6f6e 6669 672e 6365 7274 6e61 6d65   config.certname
+00009060: 203d 2022 220a 2020 2020 2020 2020 6d6f   = "".        mo
+00009070: 636b 5f63 6572 745f 7061 7468 5f74 6f5f  ck_cert_path_to_
+00009080: 6c69 6e65 6167 652e 7265 7475 726e 5f76  lineage.return_v
+00009090: 616c 7565 203d 2022 6578 616d 706c 652e  alue = "example.
+000090a0: 636f 6d22 0a20 2020 2020 2020 206d 6f63  com".        moc
+000090b0: 6b5f 6d61 7463 685f 616e 645f 6368 6563  k_match_and_chec
+000090c0: 6b5f 6f76 6572 6c61 7073 2e73 6964 655f  k_overlaps.side_
+000090d0: 6566 6665 6374 203d 2065 7272 6f72 732e  effect = errors.
+000090e0: 4f76 6572 6c61 7070 696e 674d 6174 6368  OverlappingMatch
+000090f0: 466f 756e 6428 290a 2020 2020 2020 2020  Found().        
+00009100: 7365 6c66 2e5f 6361 6c6c 2863 6f6e 6669  self._call(confi
+00009110: 6729 0a20 2020 2020 2020 206d 6f63 6b5f  g).        mock_
+00009120: 6465 6c65 7465 2e61 7373 6572 745f 6e6f  delete.assert_no
+00009130: 745f 6361 6c6c 6564 2829 0a20 2020 2020  t_called().     
+00009140: 2020 2061 7373 6572 7420 6d6f 636b 5f77     assert mock_w
+00009150: 6172 6e69 6e67 2e63 616c 6c5f 636f 756e  arning.call_coun
+00009160: 7420 3d3d 2031 0a0a 2020 2020 406d 6f63  t == 1..    @moc
+00009170: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00009180: 2e5f 696e 7465 726e 616c 2e73 746f 7261  ._internal.stora
+00009190: 6765 2e72 656e 6577 616c 5f66 696c 655f  ge.renewal_file_
+000091a0: 666f 725f 6365 7274 6e61 6d65 2729 0a20  for_certname'). 
+000091b0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+000091c0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+000091d0: 6c2e 6365 7274 5f6d 616e 6167 6572 2e6d  l.cert_manager.m
+000091e0: 6174 6368 5f61 6e64 5f63 6865 636b 5f6f  atch_and_check_o
+000091f0: 7665 726c 6170 7327 290a 2020 2020 406d  verlaps').    @m
+00009200: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00009210: 6f74 2e5f 696e 7465 726e 616c 2e73 746f  ot._internal.sto
+00009220: 7261 6765 2e66 756c 6c5f 6172 6368 6976  rage.full_archiv
+00009230: 655f 7061 7468 2729 0a20 2020 2040 6d6f  e_path').    @mo
+00009240: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+00009250: 742e 5f69 6e74 6572 6e61 6c2e 6365 7274  t._internal.cert
+00009260: 5f6d 616e 6167 6572 2e64 656c 6574 6527  _manager.delete'
+00009270: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00009280: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00009290: 726e 616c 2e63 6572 745f 6d61 6e61 6765  rnal.cert_manage
+000092a0: 722e 6365 7274 5f70 6174 685f 746f 5f6c  r.cert_path_to_l
+000092b0: 696e 6561 6765 2729 0a20 2020 2040 7465  ineage').    @te
+000092c0: 7374 5f75 7469 6c2e 7061 7463 685f 6469  st_util.patch_di
+000092d0: 7370 6c61 795f 7574 696c 2829 0a20 2020  splay_util().   
+000092e0: 2064 6566 2074 6573 745f 6365 7274 5f70   def test_cert_p
+000092f0: 6174 685f 6f6e 6c79 2873 656c 662c 206d  ath_only(self, m
+00009300: 6f63 6b5f 6765 745f 7574 696c 6974 792c  ock_get_utility,
+00009310: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
+00009320: 6b5f 6365 7274 5f70 6174 685f 746f 5f6c  k_cert_path_to_l
+00009330: 696e 6561 6765 2c20 6d6f 636b 5f64 656c  ineage, mock_del
+00009340: 6574 652c 206d 6f63 6b5f 6172 6368 6976  ete, mock_archiv
+00009350: 652c 0a20 2020 2020 2020 2020 2020 206d  e,.            m
+00009360: 6f63 6b5f 6f76 6572 6c61 7070 696e 675f  ock_overlapping_
+00009370: 6172 6368 6976 655f 6469 7273 2c20 6d6f  archive_dirs, mo
+00009380: 636b 5f72 656e 6577 616c 5f66 696c 655f  ck_renewal_file_
+00009390: 666f 725f 6365 7274 6e61 6d65 293a 0a20  for_certname):. 
+000093a0: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
+000093b0: 2064 6973 6162 6c65 203d 2075 6e75 7365   disable = unuse
+000093c0: 642d 6172 6775 6d65 6e74 0a20 2020 2020  d-argument.     
+000093d0: 2020 2063 6f6e 6669 6720 3d20 7365 6c66     config = self
+000093e0: 2e63 6f6e 6669 670a 2020 2020 2020 2020  .config.        
+000093f0: 636f 6e66 6967 2e63 6572 745f 7061 7468  config.cert_path
+00009400: 203d 2022 2f73 6f6d 652f 7265 6173 6f6e   = "/some/reason
+00009410: 6162 6c65 2f70 6174 6822 0a20 2020 2020  able/path".     
+00009420: 2020 2063 6f6e 6669 672e 6365 7274 6e61     config.certna
+00009430: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
+00009440: 6d6f 636b 5f63 6572 745f 7061 7468 5f74  mock_cert_path_t
+00009450: 6f5f 6c69 6e65 6167 652e 7265 7475 726e  o_lineage.return
+00009460: 5f76 616c 7565 203d 2022 6578 616d 706c  _value = "exampl
+00009470: 652e 636f 6d22 0a20 2020 2020 2020 206d  e.com".        m
+00009480: 6f63 6b5f 6f76 6572 6c61 7070 696e 675f  ock_overlapping_
+00009490: 6172 6368 6976 655f 6469 7273 2e72 6574  archive_dirs.ret
+000094a0: 7572 6e5f 7661 6c75 6520 3d20 4661 6c73  urn_value = Fals
+000094b0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+000094c0: 6361 6c6c 2863 6f6e 6669 6729 0a20 2020  call(config).   
+000094d0: 2020 2020 2061 7373 6572 7420 6d6f 636b       assert mock
+000094e0: 5f64 656c 6574 652e 6361 6c6c 5f63 6f75  _delete.call_cou
+000094f0: 6e74 203d 3d20 310a 0a20 2020 2040 6d6f  nt == 1..    @mo
+00009500: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+00009510: 742e 5f69 6e74 6572 6e61 6c2e 7374 6f72  t._internal.stor
+00009520: 6167 652e 7265 6e65 7761 6c5f 6669 6c65  age.renewal_file
+00009530: 5f66 6f72 5f63 6572 746e 616d 6527 290a  _for_certname').
+00009540: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+00009550: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00009560: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
+00009570: 6d61 7463 685f 616e 645f 6368 6563 6b5f  match_and_check_
+00009580: 6f76 6572 6c61 7073 2729 0a20 2020 2040  overlaps').    @
+00009590: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+000095a0: 626f 742e 5f69 6e74 6572 6e61 6c2e 7374  bot._internal.st
+000095b0: 6f72 6167 652e 6675 6c6c 5f61 7263 6869  orage.full_archi
+000095c0: 7665 5f70 6174 6827 290a 2020 2020 406d  ve_path').    @m
+000095d0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+000095e0: 6f74 2e5f 696e 7465 726e 616c 2e63 6572  ot._internal.cer
+000095f0: 745f 6d61 6e61 6765 722e 6365 7274 5f70  t_manager.cert_p
+00009600: 6174 685f 746f 5f6c 696e 6561 6765 2729  ath_to_lineage')
+00009610: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+00009620: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00009630: 6e61 6c2e 6365 7274 5f6d 616e 6167 6572  nal.cert_manager
+00009640: 2e64 656c 6574 6527 290a 2020 2020 4074  .delete').    @t
+00009650: 6573 745f 7574 696c 2e70 6174 6368 5f64  est_util.patch_d
+00009660: 6973 706c 6179 5f75 7469 6c28 290a 2020  isplay_util().  
+00009670: 2020 6465 6620 7465 7374 5f6e 6f6e 696e    def test_nonin
+00009680: 7465 7261 6374 6976 655f 6465 6c65 7469  teractive_deleti
+00009690: 6f6e 2873 656c 662c 206d 6f63 6b5f 6765  on(self, mock_ge
+000096a0: 745f 7574 696c 6974 792c 206d 6f63 6b5f  t_utility, mock_
+000096b0: 6465 6c65 7465 2c0a 2020 2020 2020 2020  delete,.        
+000096c0: 2020 2020 6d6f 636b 5f63 6572 745f 7061      mock_cert_pa
+000096d0: 7468 5f74 6f5f 6c69 6e65 6167 652c 206d  th_to_lineage, m
+000096e0: 6f63 6b5f 6675 6c6c 5f61 7263 6869 7665  ock_full_archive
+000096f0: 5f64 6972 2c0a 2020 2020 2020 2020 2020  _dir,.          
+00009700: 2020 6d6f 636b 5f6d 6174 6368 5f61 6e64    mock_match_and
+00009710: 5f63 6865 636b 5f6f 7665 726c 6170 732c  _check_overlaps,
+00009720: 206d 6f63 6b5f 7265 6e65 7761 6c5f 6669   mock_renewal_fi
+00009730: 6c65 5f66 6f72 5f63 6572 746e 616d 6529  le_for_certname)
+00009740: 3a0a 2020 2020 2020 2020 2320 7079 6c69  :.        # pyli
+00009750: 6e74 3a20 6469 7361 626c 6520 3d20 756e  nt: disable = un
+00009760: 7573 6564 2d61 7267 756d 656e 740a 2020  used-argument.  
+00009770: 2020 2020 2020 636f 6e66 6967 203d 2073        config = s
+00009780: 656c 662e 636f 6e66 6967 0a20 2020 2020  elf.config.     
+00009790: 2020 2063 6f6e 6669 672e 6e6f 6e69 6e74     config.nonint
+000097a0: 6572 6163 7469 7665 5f6d 6f64 6520 3d20  eractive_mode = 
+000097b0: 5472 7565 0a20 2020 2020 2020 2063 6f6e  True.        con
+000097c0: 6669 672e 6365 7274 5f70 6174 6820 3d20  fig.cert_path = 
+000097d0: 222f 736f 6d65 2f72 6561 736f 6e61 626c  "/some/reasonabl
+000097e0: 652f 7061 7468 220a 2020 2020 2020 2020  e/path".        
+000097f0: 636f 6e66 6967 2e63 6572 746e 616d 6520  config.certname 
+00009800: 3d20 2222 0a20 2020 2020 2020 206d 6f63  = "".        moc
+00009810: 6b5f 6365 7274 5f70 6174 685f 746f 5f6c  k_cert_path_to_l
+00009820: 696e 6561 6765 2e72 6574 7572 6e5f 7661  ineage.return_va
+00009830: 6c75 6520 3d20 2265 7861 6d70 6c65 2e63  lue = "example.c
+00009840: 6f6d 220a 2020 2020 2020 2020 6d6f 636b  om".        mock
+00009850: 5f66 756c 6c5f 6172 6368 6976 655f 6469  _full_archive_di
+00009860: 722e 7265 7475 726e 5f76 616c 7565 203d  r.return_value =
+00009870: 2022 220a 2020 2020 2020 2020 6d6f 636b   "".        mock
+00009880: 5f6d 6174 6368 5f61 6e64 5f63 6865 636b  _match_and_check
+00009890: 5f6f 7665 726c 6170 732e 7265 7475 726e  _overlaps.return
+000098a0: 5f76 616c 7565 203d 2022 220a 2020 2020  _value = "".    
+000098b0: 2020 2020 7365 6c66 2e5f 6361 6c6c 2863      self._call(c
+000098c0: 6f6e 6669 6729 0a20 2020 2020 2020 2061  onfig).        a
+000098d0: 7373 6572 7420 6d6f 636b 5f64 656c 6574  ssert mock_delet
+000098e0: 652e 6361 6c6c 5f63 6f75 6e74 203d 3d20  e.call_count == 
+000098f0: 310a 0a20 2020 2040 6d6f 636b 2e70 6174  1..    @mock.pat
+00009900: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+00009910: 6572 6e61 6c2e 7374 6f72 6167 652e 7265  ernal.storage.re
+00009920: 6e65 7761 6c5f 6669 6c65 5f66 6f72 5f63  newal_file_for_c
+00009930: 6572 746e 616d 6527 290a 2020 2020 406d  ertname').    @m
+00009940: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00009950: 6f74 2e5f 696e 7465 726e 616c 2e63 6572  ot._internal.cer
+00009960: 745f 6d61 6e61 6765 722e 6d61 7463 685f  t_manager.match_
+00009970: 616e 645f 6368 6563 6b5f 6f76 6572 6c61  and_check_overla
+00009980: 7073 2729 0a20 2020 2040 6d6f 636b 2e70  ps').    @mock.p
+00009990: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+000099a0: 6e74 6572 6e61 6c2e 7374 6f72 6167 652e  nternal.storage.
+000099b0: 6675 6c6c 5f61 7263 6869 7665 5f70 6174  full_archive_pat
+000099c0: 6827 290a 2020 2020 406d 6f63 6b2e 7061  h').    @mock.pa
+000099d0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+000099e0: 7465 726e 616c 2e63 6572 745f 6d61 6e61  ternal.cert_mana
+000099f0: 6765 722e 6365 7274 5f70 6174 685f 746f  ger.cert_path_to
+00009a00: 5f6c 696e 6561 6765 2729 0a20 2020 2040  _lineage').    @
+00009a10: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+00009a20: 626f 742e 5f69 6e74 6572 6e61 6c2e 6365  bot._internal.ce
+00009a30: 7274 5f6d 616e 6167 6572 2e64 656c 6574  rt_manager.delet
+00009a40: 6527 290a 2020 2020 4074 6573 745f 7574  e').    @test_ut
+00009a50: 696c 2e70 6174 6368 5f64 6973 706c 6179  il.patch_display
+00009a60: 5f75 7469 6c28 290a 2020 2020 6465 6620  _util().    def 
+00009a70: 7465 7374 5f6f 7074 5f69 6e5f 6465 6c65  test_opt_in_dele
+00009a80: 7469 6f6e 2873 656c 662c 206d 6f63 6b5f  tion(self, mock_
+00009a90: 6765 745f 7574 696c 6974 792c 206d 6f63  get_utility, moc
+00009aa0: 6b5f 6465 6c65 7465 2c0a 2020 2020 2020  k_delete,.      
+00009ab0: 2020 2020 2020 6d6f 636b 5f63 6572 745f        mock_cert_
+00009ac0: 7061 7468 5f74 6f5f 6c69 6e65 6167 652c  path_to_lineage,
+00009ad0: 206d 6f63 6b5f 6675 6c6c 5f61 7263 6869   mock_full_archi
+00009ae0: 7665 5f64 6972 2c0a 2020 2020 2020 2020  ve_dir,.        
+00009af0: 2020 2020 6d6f 636b 5f6d 6174 6368 5f61      mock_match_a
+00009b00: 6e64 5f63 6865 636b 5f6f 7665 726c 6170  nd_check_overlap
+00009b10: 732c 206d 6f63 6b5f 7265 6e65 7761 6c5f  s, mock_renewal_
+00009b20: 6669 6c65 5f66 6f72 5f63 6572 746e 616d  file_for_certnam
+00009b30: 6529 3a0a 2020 2020 2020 2020 636f 6e66  e):.        conf
+00009b40: 6967 203d 2073 656c 662e 636f 6e66 6967  ig = self.config
+00009b50: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00009b60: 6465 6c65 7465 5f61 6674 6572 5f72 6576  delete_after_rev
+00009b70: 6f6b 6520 3d20 5472 7565 0a20 2020 2020  oke = True.     
+00009b80: 2020 2063 6f6e 6669 672e 6365 7274 5f70     config.cert_p
+00009b90: 6174 6820 3d20 222f 736f 6d65 2f72 6561  ath = "/some/rea
+00009ba0: 736f 6e61 626c 652f 7061 7468 220a 2020  sonable/path".  
+00009bb0: 2020 2020 2020 636f 6e66 6967 2e63 6572        config.cer
+00009bc0: 746e 616d 6520 3d20 2222 0a20 2020 2020  tname = "".     
+00009bd0: 2020 206d 6f63 6b5f 6365 7274 5f70 6174     mock_cert_pat
+00009be0: 685f 746f 5f6c 696e 6561 6765 2e72 6574  h_to_lineage.ret
+00009bf0: 7572 6e5f 7661 6c75 6520 3d20 2265 7861  urn_value = "exa
+00009c00: 6d70 6c65 2e63 6f6d 220a 2020 2020 2020  mple.com".      
+00009c10: 2020 6d6f 636b 5f66 756c 6c5f 6172 6368    mock_full_arch
+00009c20: 6976 655f 6469 722e 7265 7475 726e 5f76  ive_dir.return_v
+00009c30: 616c 7565 203d 2022 220a 2020 2020 2020  alue = "".      
+00009c40: 2020 6d6f 636b 5f6d 6174 6368 5f61 6e64    mock_match_and
+00009c50: 5f63 6865 636b 5f6f 7665 726c 6170 732e  _check_overlaps.
+00009c60: 7265 7475 726e 5f76 616c 7565 203d 2022  return_value = "
+00009c70: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+00009c80: 6361 6c6c 2863 6f6e 6669 6729 0a20 2020  call(config).   
+00009c90: 2020 2020 2061 7373 6572 7420 6d6f 636b       assert mock
+00009ca0: 5f64 656c 6574 652e 6361 6c6c 5f63 6f75  _delete.call_cou
+00009cb0: 6e74 203d 3d20 310a 2020 2020 2020 2020  nt == 1.        
+00009cc0: 6173 7365 7274 206e 6f74 206d 6f63 6b5f  assert not mock_
+00009cd0: 6765 745f 7574 696c 6974 7928 292e 7965  get_utility().ye
+00009ce0: 736e 6f2e 6361 6c6c 6564 0a0a 0a63 6c61  sno.called...cla
+00009cf0: 7373 2044 6574 6572 6d69 6e65 4163 636f  ss DetermineAcco
+00009d00: 756e 7454 6573 7428 7465 7374 5f75 7469  untTest(test_uti
+00009d10: 6c2e 436f 6e66 6967 5465 7374 4361 7365  l.ConfigTestCase
+00009d20: 293a 0a20 2020 2022 2222 5465 7374 7320  ):.    """Tests 
+00009d30: 666f 7220 6365 7274 626f 742e 5f69 6e74  for certbot._int
+00009d40: 6572 6e61 6c2e 6d61 696e 2e5f 6465 7465  ernal.main._dete
+00009d50: 726d 696e 655f 6163 636f 756e 742e 2222  rmine_account.""
+00009d60: 220a 0a20 2020 2064 6566 2073 6574 5570  "..    def setUp
+00009d70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00009d80: 7375 7065 7228 292e 7365 7455 7028 290a  super().setUp().
+00009d90: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009da0: 6669 672e 6163 636f 756e 7420 3d20 4e6f  fig.account = No
+00009db0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00009dc0: 636f 6e66 6967 2e65 6d61 696c 203d 204e  config.email = N
+00009dd0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00009de0: 2e63 6f6e 6669 672e 7265 6769 7374 6572  .config.register
+00009df0: 5f75 6e73 6166 656c 795f 7769 7468 6f75  _unsafely_withou
+00009e00: 745f 656d 6169 6c20 3d20 4661 6c73 650a  t_email = False.
+00009e10: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
+00009e20: 7320 3d20 5b6d 6f63 6b2e 4d61 6769 634d  s = [mock.MagicM
+00009e30: 6f63 6b28 6964 3d27 7827 292c 206d 6f63  ock(id='x'), moc
+00009e40: 6b2e 4d61 6769 634d 6f63 6b28 6964 3d27  k.MagicMock(id='
+00009e50: 7927 295d 0a20 2020 2020 2020 2073 656c  y')].        sel
+00009e60: 662e 6163 636f 756e 745f 7374 6f72 6167  f.account_storag
+00009e70: 6520 3d20 6163 636f 756e 742e 4163 636f  e = account.Acco
+00009e80: 756e 744d 656d 6f72 7953 746f 7261 6765  untMemoryStorage
+00009e90: 2829 0a20 2020 2020 2020 2023 2046 6f72  ().        # For
+00009ea0: 2075 7365 2069 6e20 7361 7669 6e67 2061   use in saving a
+00009eb0: 6363 6f75 6e74 733a 2066 616b 6520 6f75  ccounts: fake ou
+00009ec0: 7420 7468 6520 6e65 775f 6175 7468 7a20  t the new_authz 
+00009ed0: 5552 4c2e 0a20 2020 2020 2020 2073 656c  URL..        sel
+00009ee0: 662e 6d6f 636b 5f63 6c69 656e 7420 3d20  f.mock_client = 
+00009ef0: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
+00009f00: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+00009f10: 636b 5f63 6c69 656e 742e 6469 7265 6374  ck_client.direct
+00009f20: 6f72 792e 6e65 775f 6175 7468 7a20 3d20  ory.new_authz = 
+00009f30: 2268 6922 0a0a 0a20 2020 2064 6566 205f  "hi"...    def _
+00009f40: 6361 6c6c 2873 656c 6629 3a0a 2020 2020  call(self):.    
+00009f50: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
+00009f60: 7361 626c 653d 7072 6f74 6563 7465 642d  sable=protected-
+00009f70: 6163 6365 7373 0a20 2020 2020 2020 2066  access.        f
+00009f80: 726f 6d20 6365 7274 626f 742e 5f69 6e74  rom certbot._int
+00009f90: 6572 6e61 6c2e 6d61 696e 2069 6d70 6f72  ernal.main impor
+00009fa0: 7420 5f64 6574 6572 6d69 6e65 5f61 6363  t _determine_acc
+00009fb0: 6f75 6e74 0a20 2020 2020 2020 2077 6974  ount.        wit
+00009fc0: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
+00009fd0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00009fe0: 6d61 696e 2e61 6363 6f75 6e74 2e41 6363  main.account.Acc
+00009ff0: 6f75 6e74 4669 6c65 5374 6f72 6167 6527  ountFileStorage'
+0000a000: 2920 6173 206d 6f63 6b5f 7374 6f72 6167  ) as mock_storag
+0000a010: 652c 205c 0a20 2020 2020 2020 2020 2020  e, \.           
+0000a020: 2020 7465 7374 5f75 7469 6c2e 7061 7463    test_util.patc
+0000a030: 685f 6469 7370 6c61 795f 7574 696c 2829  h_display_util()
+0000a040: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+0000a050: 636b 5f73 746f 7261 6765 2e72 6574 7572  ck_storage.retur
+0000a060: 6e5f 7661 6c75 6520 3d20 7365 6c66 2e61  n_value = self.a
+0000a070: 6363 6f75 6e74 5f73 746f 7261 6765 0a20  ccount_storage. 
+0000a080: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a090: 6e20 5f64 6574 6572 6d69 6e65 5f61 6363  n _determine_acc
+0000a0a0: 6f75 6e74 2873 656c 662e 636f 6e66 6967  ount(self.config
+0000a0b0: 290a 0a20 2020 2040 6d6f 636b 2e70 6174  )..    @mock.pat
+0000a0c0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000a0d0: 6572 6e61 6c2e 636c 6965 6e74 2e72 6567  ernal.client.reg
+0000a0e0: 6973 7465 7227 290a 2020 2020 406d 6f63  ister').    @moc
+0000a0f0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+0000a100: 2e5f 696e 7465 726e 616c 2e63 6c69 656e  ._internal.clien
+0000a110: 742e 6469 7370 6c61 795f 6f70 732e 6765  t.display_ops.ge
+0000a120: 745f 656d 6169 6c27 290a 2020 2020 6465  t_email').    de
+0000a130: 6620 5f72 6567 6973 7465 725f 6572 726f  f _register_erro
+0000a140: 725f 636f 6d6d 6f6e 2873 656c 662c 2065  r_common(self, e
+0000a150: 7272 5f6d 7367 2c20 6578 6365 7074 696f  rr_msg, exceptio
+0000a160: 6e2c 206d 6f63 6b5f 6765 745f 656d 6169  n, mock_get_emai
+0000a170: 6c2c 206d 6f63 6b5f 7265 6769 7374 6572  l, mock_register
+0000a180: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
+0000a190: 6765 745f 656d 6169 6c2e 7265 7475 726e  get_email.return
+0000a1a0: 5f76 616c 7565 203d 2027 666f 6f40 6261  _value = 'foo@ba
+0000a1b0: 722e 6261 7a27 0a20 2020 2020 2020 206d  r.baz'.        m
+0000a1c0: 6f63 6b5f 7265 6769 7374 6572 2e73 6964  ock_register.sid
+0000a1d0: 655f 6566 6665 6374 203d 2065 7863 6570  e_effect = excep
+0000a1e0: 7469 6f6e 0a20 2020 2020 2020 2074 7279  tion.        try
+0000a1f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a200: 6c66 2e5f 6361 6c6c 2829 0a20 2020 2020  lf._call().     
+0000a210: 2020 2065 7863 6570 7420 6572 726f 7273     except errors
+0000a220: 2e45 7272 6f72 2061 7320 6572 723a 0a20  .Error as err:. 
+0000a230: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000a240: 7420 6622 556e 6162 6c65 2074 6f20 7265  t f"Unable to re
+0000a250: 6769 7374 6572 2061 6e20 6163 636f 756e  gister an accoun
+0000a260: 7420 7769 7468 2041 434d 4520 7365 7276  t with ACME serv
+0000a270: 6572 2e20 7b65 7272 5f6d 7367 7d22 203d  er. {err_msg}" =
+0000a280: 3d20 5c0a 2020 2020 2020 2020 2020 2020  = \.            
+0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2a0: 2073 7472 2865 7272 290a 0a20 2020 2064   str(err)..    d
+0000a2b0: 6566 2074 6573 745f 6172 6773 5f61 6363  ef test_args_acc
+0000a2c0: 6f75 6e74 5f73 6574 2873 656c 6629 3a0a  ount_set(self):.
+0000a2d0: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
+0000a2e0: 6f75 6e74 5f73 746f 7261 6765 2e73 6176  ount_storage.sav
+0000a2f0: 6528 7365 6c66 2e61 6363 735b 315d 2c20  e(self.accs[1], 
+0000a300: 7365 6c66 2e6d 6f63 6b5f 636c 6965 6e74  self.mock_client
+0000a310: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000a320: 6f6e 6669 672e 6163 636f 756e 7420 3d20  onfig.account = 
+0000a330: 7365 6c66 2e61 6363 735b 315d 2e69 640a  self.accs[1].id.
+0000a340: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+0000a350: 7365 6c66 2e61 6363 735b 315d 2c20 4e6f  self.accs[1], No
+0000a360: 6e65 2920 3d3d 2073 656c 662e 5f63 616c  ne) == self._cal
+0000a370: 6c28 290a 2020 2020 2020 2020 6173 7365  l().        asse
+0000a380: 7274 2073 656c 662e 6163 6373 5b31 5d2e  rt self.accs[1].
+0000a390: 6964 203d 3d20 7365 6c66 2e63 6f6e 6669  id == self.confi
+0000a3a0: 672e 6163 636f 756e 740a 2020 2020 2020  g.account.      
+0000a3b0: 2020 6173 7365 7274 2073 656c 662e 636f    assert self.co
+0000a3c0: 6e66 6967 2e65 6d61 696c 2069 7320 4e6f  nfig.email is No
+0000a3d0: 6e65 0a0a 2020 2020 6465 6620 7465 7374  ne..    def test
+0000a3e0: 5f73 696e 676c 655f 6163 636f 756e 7428  _single_account(
+0000a3f0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0000a400: 656c 662e 6163 636f 756e 745f 7374 6f72  elf.account_stor
+0000a410: 6167 652e 7361 7665 2873 656c 662e 6163  age.save(self.ac
+0000a420: 6373 5b30 5d2c 2073 656c 662e 6d6f 636b  cs[0], self.mock
+0000a430: 5f63 6c69 656e 7429 0a20 2020 2020 2020  _client).       
+0000a440: 2061 7373 6572 7420 2873 656c 662e 6163   assert (self.ac
+0000a450: 6373 5b30 5d2c 204e 6f6e 6529 203d 3d20  cs[0], None) == 
+0000a460: 7365 6c66 2e5f 6361 6c6c 2829 0a20 2020  self._call().   
+0000a470: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+0000a480: 2e61 6363 735b 305d 2e69 6420 3d3d 2073  .accs[0].id == s
+0000a490: 656c 662e 636f 6e66 6967 2e61 6363 6f75  elf.config.accou
+0000a4a0: 6e74 0a20 2020 2020 2020 2061 7373 6572  nt.        asser
+0000a4b0: 7420 7365 6c66 2e63 6f6e 6669 672e 656d  t self.config.em
+0000a4c0: 6169 6c20 6973 204e 6f6e 650a 0a20 2020  ail is None..   
+0000a4d0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000a4e0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0000a4f0: 636c 6965 6e74 2e64 6973 706c 6179 5f6f  client.display_o
+0000a500: 7073 2e63 686f 6f73 655f 6163 636f 756e  ps.choose_accoun
+0000a510: 7427 290a 2020 2020 6465 6620 7465 7374  t').    def test
+0000a520: 5f6d 756c 7469 706c 655f 6163 636f 756e  _multiple_accoun
+0000a530: 7473 2873 656c 662c 206d 6f63 6b5f 6368  ts(self, mock_ch
+0000a540: 6f6f 7365 5f61 6363 6f75 6e74 7329 3a0a  oose_accounts):.
+0000a550: 2020 2020 2020 2020 666f 7220 6163 6320          for acc 
+0000a560: 696e 2073 656c 662e 6163 6373 3a0a 2020  in self.accs:.  
+0000a570: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000a580: 6363 6f75 6e74 5f73 746f 7261 6765 2e73  ccount_storage.s
+0000a590: 6176 6528 6163 632c 2073 656c 662e 6d6f  ave(acc, self.mo
+0000a5a0: 636b 5f63 6c69 656e 7429 0a20 2020 2020  ck_client).     
+0000a5b0: 2020 206d 6f63 6b5f 6368 6f6f 7365 5f61     mock_choose_a
+0000a5c0: 6363 6f75 6e74 732e 7265 7475 726e 5f76  ccounts.return_v
+0000a5d0: 616c 7565 203d 2073 656c 662e 6163 6373  alue = self.accs
+0000a5e0: 5b31 5d0a 2020 2020 2020 2020 6173 7365  [1].        asse
+0000a5f0: 7274 2028 7365 6c66 2e61 6363 735b 315d  rt (self.accs[1]
+0000a600: 2c20 4e6f 6e65 2920 3d3d 2073 656c 662e  , None) == self.
+0000a610: 5f63 616c 6c28 290a 2020 2020 2020 2020  _call().        
+0000a620: 6173 7365 7274 2073 6574 286d 6f63 6b5f  assert set(mock_
+0000a630: 6368 6f6f 7365 5f61 6363 6f75 6e74 732e  choose_accounts.
+0000a640: 6361 6c6c 5f61 7267 735b 305d 5b30 5d29  call_args[0][0])
+0000a650: 203d 3d20 7365 7428 7365 6c66 2e61 6363   == set(self.acc
+0000a660: 7329 0a20 2020 2020 2020 2061 7373 6572  s).        asser
+0000a670: 7420 7365 6c66 2e61 6363 735b 315d 2e69  t self.accs[1].i
+0000a680: 6420 3d3d 2073 656c 662e 636f 6e66 6967  d == self.config
+0000a690: 2e61 6363 6f75 6e74 0a20 2020 2020 2020  .account.       
+0000a6a0: 2061 7373 6572 7420 7365 6c66 2e63 6f6e   assert self.con
+0000a6b0: 6669 672e 656d 6169 6c20 6973 204e 6f6e  fig.email is Non
+0000a6c0: 650a 0a20 2020 2040 6d6f 636b 2e70 6174  e..    @mock.pat
+0000a6d0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000a6e0: 6572 6e61 6c2e 636c 6965 6e74 2e64 6973  ernal.client.dis
+0000a6f0: 706c 6179 5f6f 7073 2e63 686f 6f73 655f  play_ops.choose_
+0000a700: 6163 636f 756e 7427 290a 2020 2020 6465  account').    de
+0000a710: 6620 7465 7374 5f6d 756c 7469 706c 655f  f test_multiple_
+0000a720: 6163 636f 756e 7473 5f63 616e 6365 6c65  accounts_cancele
+0000a730: 6428 7365 6c66 2c20 6d6f 636b 5f63 686f  d(self, mock_cho
+0000a740: 6f73 655f 6163 636f 756e 7473 293a 0a20  ose_accounts):. 
+0000a750: 2020 2020 2020 2066 6f72 2061 6363 2069         for acc i
+0000a760: 6e20 7365 6c66 2e61 6363 733a 0a20 2020  n self.accs:.   
+0000a770: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+0000a780: 636f 756e 745f 7374 6f72 6167 652e 7361  count_storage.sa
+0000a790: 7665 2861 6363 2c20 7365 6c66 2e6d 6f63  ve(acc, self.moc
+0000a7a0: 6b5f 636c 6965 6e74 290a 2020 2020 2020  k_client).      
+0000a7b0: 2020 6d6f 636b 5f63 686f 6f73 655f 6163    mock_choose_ac
+0000a7c0: 636f 756e 7473 2e72 6574 7572 6e5f 7661  counts.return_va
+0000a7d0: 6c75 6520 3d20 4e6f 6e65 0a20 2020 2020  lue = None.     
+0000a7e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000a7f0: 2020 2020 7365 6c66 2e5f 6361 6c6c 2829      self._call()
+0000a800: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000a810: 6572 726f 7273 2e45 7272 6f72 2061 7320  errors.Error as 
+0000a820: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+0000a830: 2061 7373 6572 7420 224e 6f20 6163 636f   assert "No acco
+0000a840: 756e 7420 6861 7320 6265 656e 2063 686f  unt has been cho
+0000a850: 7365 6e22 2069 6e20 7374 7228 6572 7229  sen" in str(err)
+0000a860: 0a0a 2020 2020 406d 6f63 6b2e 7061 7463  ..    @mock.patc
+0000a870: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+0000a880: 726e 616c 2e63 6c69 656e 742e 6469 7370  rnal.client.disp
+0000a890: 6c61 795f 6f70 732e 6765 745f 656d 6169  lay_ops.get_emai
+0000a8a0: 6c27 290a 2020 2020 406d 6f63 6b2e 7061  l').    @mock.pa
+0000a8b0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+0000a8c0: 7465 726e 616c 2e6d 6169 6e2e 6469 7370  ternal.main.disp
+0000a8d0: 6c61 795f 7574 696c 2e6e 6f74 6966 7927  lay_util.notify'
+0000a8e0: 290a 2020 2020 6465 6620 7465 7374 5f6e  ).    def test_n
+0000a8f0: 6f5f 6163 636f 756e 7473 5f6e 6f5f 656d  o_accounts_no_em
+0000a900: 6169 6c28 7365 6c66 2c20 6d6f 636b 5f6e  ail(self, mock_n
+0000a910: 6f74 6966 792c 206d 6f63 6b5f 6765 745f  otify, mock_get_
+0000a920: 656d 6169 6c29 3a0a 2020 2020 2020 2020  email):.        
+0000a930: 6d6f 636b 5f67 6574 5f65 6d61 696c 2e72  mock_get_email.r
+0000a940: 6574 7572 6e5f 7661 6c75 6520 3d20 2766  eturn_value = 'f
+0000a950: 6f6f 4062 6172 2e62 617a 270a 0a20 2020  oo@bar.baz'..   
+0000a960: 2020 2020 2077 6974 6820 6d6f 636b 2e70       with mock.p
+0000a970: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0000a980: 6e74 6572 6e61 6c2e 6d61 696e 2e63 6c69  nternal.main.cli
+0000a990: 656e 7427 2920 6173 2063 6c69 656e 743a  ent') as client:
+0000a9a0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+0000a9b0: 656e 742e 7265 6769 7374 6572 2e72 6574  ent.register.ret
+0000a9c0: 7572 6e5f 7661 6c75 6520 3d20 280a 2020  urn_value = (.  
+0000a9d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a9e0: 6c66 2e61 6363 735b 305d 2c20 6d6f 636b  lf.accs[0], mock
+0000a9f0: 2e73 656e 7469 6e65 6c2e 6163 6d65 290a  .sentinel.acme).
+0000aa00: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000aa10: 7274 2028 7365 6c66 2e61 6363 735b 305d  rt (self.accs[0]
+0000aa20: 2c20 6d6f 636b 2e73 656e 7469 6e65 6c2e  , mock.sentinel.
+0000aa30: 6163 6d65 2920 3d3d 2073 656c 662e 5f63  acme) == self._c
+0000aa40: 616c 6c28 290a 2020 2020 2020 2020 636c  all().        cl
+0000aa50: 6965 6e74 2e72 6567 6973 7465 722e 6173  ient.register.as
+0000aa60: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+0000aa70: 5f77 6974 6828 0a20 2020 2020 2020 2020  _with(.         
+0000aa80: 2020 2073 656c 662e 636f 6e66 6967 2c20     self.config, 
+0000aa90: 7365 6c66 2e61 6363 6f75 6e74 5f73 746f  self.account_sto
+0000aaa0: 7261 6765 2c20 746f 735f 6362 3d6d 6f63  rage, tos_cb=moc
+0000aab0: 6b2e 414e 5929 0a0a 2020 2020 2020 2020  k.ANY)..        
+0000aac0: 6173 7365 7274 2073 656c 662e 6163 6373  assert self.accs
+0000aad0: 5b30 5d2e 6964 203d 3d20 7365 6c66 2e63  [0].id == self.c
+0000aae0: 6f6e 6669 672e 6163 636f 756e 740a 2020  onfig.account.  
+0000aaf0: 2020 2020 2020 6173 7365 7274 2027 666f        assert 'fo
+0000ab00: 6f40 6261 722e 6261 7a27 203d 3d20 7365  o@bar.baz' == se
+0000ab10: 6c66 2e63 6f6e 6669 672e 656d 6169 6c0a  lf.config.email.
+0000ab20: 2020 2020 2020 2020 6d6f 636b 5f6e 6f74          mock_not
+0000ab30: 6966 792e 6173 7365 7274 5f63 616c 6c65  ify.assert_calle
+0000ab40: 645f 6f6e 6365 5f77 6974 6828 2741 6363  d_once_with('Acc
+0000ab50: 6f75 6e74 2072 6567 6973 7465 7265 642e  ount registered.
+0000ab60: 2729 0a0a 2020 2020 6465 6620 7465 7374  ')..    def test
+0000ab70: 5f6e 6f5f 6163 636f 756e 7473 5f65 6d61  _no_accounts_ema
+0000ab80: 696c 2873 656c 6629 3a0a 2020 2020 2020  il(self):.      
+0000ab90: 2020 7365 6c66 2e63 6f6e 6669 672e 656d    self.config.em
+0000aba0: 6169 6c20 3d20 276f 7468 6572 2065 6d61  ail = 'other ema
+0000abb0: 696c 270a 2020 2020 2020 2020 7769 7468  il'.        with
+0000abc0: 206d 6f63 6b2e 7061 7463 6828 2763 6572   mock.patch('cer
+0000abd0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+0000abe0: 6169 6e2e 636c 6965 6e74 2729 2061 7320  ain.client') as 
+0000abf0: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+0000ac00: 2020 2020 636c 6965 6e74 2e72 6567 6973      client.regis
+0000ac10: 7465 722e 7265 7475 726e 5f76 616c 7565  ter.return_value
+0000ac20: 203d 2028 7365 6c66 2e61 6363 735b 315d   = (self.accs[1]
+0000ac30: 2c20 6d6f 636b 2e73 656e 7469 6e65 6c2e  , mock.sentinel.
+0000ac40: 6163 6d65 290a 2020 2020 2020 2020 2020  acme).          
+0000ac50: 2020 7365 6c66 2e5f 6361 6c6c 2829 0a20    self._call(). 
+0000ac60: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000ac70: 6c66 2e61 6363 735b 315d 2e69 6420 3d3d  lf.accs[1].id ==
+0000ac80: 2073 656c 662e 636f 6e66 6967 2e61 6363   self.config.acc
+0000ac90: 6f75 6e74 0a20 2020 2020 2020 2061 7373  ount.        ass
+0000aca0: 6572 7420 276f 7468 6572 2065 6d61 696c  ert 'other email
+0000acb0: 2720 3d3d 2073 656c 662e 636f 6e66 6967  ' == self.config
+0000acc0: 2e65 6d61 696c 0a0a 2020 2020 6465 6620  .email..    def 
+0000acd0: 7465 7374 5f72 6567 6973 7465 725f 6572  test_register_er
+0000ace0: 726f 725f 6365 7274 626f 7428 7365 6c66  ror_certbot(self
+0000acf0: 293a 0a20 2020 2020 2020 2065 7272 5f6d  ):.        err_m
+0000ad00: 7367 203d 2022 536f 6d65 2065 7272 6f72  sg = "Some error
+0000ad10: 206d 6573 7361 6765 2072 6169 7365 6420   message raised 
+0000ad20: 6279 2043 6572 7462 6f74 220a 2020 2020  by Certbot".    
+0000ad30: 2020 2020 7365 6c66 2e5f 7265 6769 7374      self._regist
+0000ad40: 6572 5f65 7272 6f72 5f63 6f6d 6d6f 6e28  er_error_common(
+0000ad50: 6572 725f 6d73 672c 2065 7272 6f72 732e  err_msg, errors.
+0000ad60: 4572 726f 7228 6572 725f 6d73 6729 290a  Error(err_msg)).
+0000ad70: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+0000ad80: 6769 7374 6572 5f65 7272 6f72 5f61 636d  gister_error_acm
+0000ad90: 655f 7479 7065 5f61 6e64 5f64 6574 6169  e_type_and_detai
+0000ada0: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
+0000adb0: 2065 7272 5f6d 7367 203d 2028 2245 7272   err_msg = ("Err
+0000adc0: 6f72 2072 6574 7572 6e65 6420 6279 2074  or returned by t
+0000add0: 6865 2041 434d 4520 7365 7276 6572 3a20  he ACME server: 
+0000ade0: 6d75 7374 2061 6772 6565 2074 6f20 7465  must agree to te
+0000adf0: 726d 7320 6f66 2073 6572 7669 6365 2229  rms of service")
+0000ae00: 0a20 2020 2020 2020 2065 7863 6570 7469  .        excepti
+0000ae10: 6f6e 203d 2061 636d 655f 6572 726f 7228  on = acme_error(
+0000ae20: 7479 7020 3d20 2275 726e 3a69 6574 663a  typ = "urn:ietf:
+0000ae30: 7061 7261 6d73 3a61 636d 653a 6572 726f  params:acme:erro
+0000ae40: 723a 6d61 6c66 6f72 6d65 6422 2c0a 2020  r:malformed",.  
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2020 2020 2020 2020 2020 2064 6574               det
+0000ae70: 6169 6c20 3d20 226d 7573 7420 6167 7265  ail = "must agre
+0000ae80: 6520 746f 2074 6572 6d73 206f 6620 7365  e to terms of se
+0000ae90: 7276 6963 6522 290a 2020 2020 2020 2020  rvice").        
+0000aea0: 7365 6c66 2e5f 7265 6769 7374 6572 5f65  self._register_e
+0000aeb0: 7272 6f72 5f63 6f6d 6d6f 6e28 6572 725f  rror_common(err_
+0000aec0: 6d73 672c 2065 7863 6570 7469 6f6e 290a  msg, exception).
+0000aed0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+0000aee0: 6769 7374 6572 5f65 7272 6f72 5f61 636d  gister_error_acm
+0000aef0: 655f 7479 7065 5f6f 6e6c 7928 7365 6c66  e_type_only(self
+0000af00: 293a 0a20 2020 2020 2020 2065 7272 5f6d  ):.        err_m
+0000af10: 7367 203d 2028 2245 7272 6f72 2072 6574  sg = ("Error ret
+0000af20: 7572 6e65 6420 6279 2074 6865 2041 434d  urned by the ACM
+0000af30: 4520 7365 7276 6572 3a20 5468 6520 7365  E server: The se
+0000af40: 7276 6572 2065 7870 6572 6965 6e63 6564  rver experienced
+0000af50: 2061 6e20 696e 7465 726e 616c 2065 7272   an internal err
+0000af60: 6f72 2229 0a20 2020 2020 2020 2065 7863  or").        exc
+0000af70: 6570 7469 6f6e 203d 2061 636d 655f 6572  eption = acme_er
+0000af80: 726f 7228 7479 7020 3d20 2275 726e 3a69  ror(typ = "urn:i
+0000af90: 6574 663a 7061 7261 6d73 3a61 636d 653a  etf:params:acme:
+0000afa0: 6572 726f 723a 7365 7276 6572 496e 7465  error:serverInte
+0000afb0: 726e 616c 2229 0a20 2020 2020 2020 2073  rnal").        s
+0000afc0: 656c 662e 5f72 6567 6973 7465 725f 6572  elf._register_er
+0000afd0: 726f 725f 636f 6d6d 6f6e 2865 7272 5f6d  ror_common(err_m
+0000afe0: 7367 2c20 6578 6365 7074 696f 6e29 0a0a  sg, exception)..
+0000aff0: 0a63 6c61 7373 204d 6169 6e54 6573 7428  .class MainTest(
+0000b000: 7465 7374 5f75 7469 6c2e 436f 6e66 6967  test_util.Config
+0000b010: 5465 7374 4361 7365 293a 0a20 2020 2022  TestCase):.    "
+0000b020: 2222 5465 7374 7320 666f 7220 6469 6666  ""Tests for diff
+0000b030: 6572 656e 7420 636f 6d6d 616e 6473 2e22  erent commands."
+0000b040: 2222 0a0a 2020 2020 6465 6620 7365 7455  ""..    def setU
+0000b050: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0000b060: 2073 7570 6572 2829 2e73 6574 5570 2829   super().setUp()
+0000b070: 0a0a 2020 2020 2020 2020 6669 6c65 7379  ..        filesy
+0000b080: 7374 656d 2e6d 6b64 6972 2873 656c 662e  stem.mkdir(self.
+0000b090: 636f 6e66 6967 2e6c 6f67 735f 6469 7229  config.logs_dir)
+0000b0a0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0000b0b0: 616e 6461 7264 5f61 7267 7320 3d20 5b27  andard_args = ['
+0000b0c0: 2d2d 636f 6e66 6967 2d64 6972 272c 2073  --config-dir', s
+0000b0d0: 656c 662e 636f 6e66 6967 2e63 6f6e 6669  elf.config.confi
+0000b0e0: 675f 6469 722c 0a20 2020 2020 2020 2020  g_dir,.         
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b100: 2020 2020 2027 2d2d 776f 726b 2d64 6972       '--work-dir
+0000b110: 272c 2073 656c 662e 636f 6e66 6967 2e77  ', self.config.w
+0000b120: 6f72 6b5f 6469 722c 0a20 2020 2020 2020  ork_dir,.       
+0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b140: 2020 2020 2020 2027 2d2d 6c6f 6773 2d64         '--logs-d
+0000b150: 6972 272c 2073 656c 662e 636f 6e66 6967  ir', self.config
+0000b160: 2e6c 6f67 735f 6469 722c 2027 2d2d 7465  .logs_dir, '--te
+0000b170: 7874 275d 0a0a 2020 2020 2020 2020 7365  xt']..        se
+0000b180: 6c66 2e6d 6f63 6b5f 736c 6565 7020 3d20  lf.mock_sleep = 
+0000b190: 6d6f 636b 2e70 6174 6368 2827 7469 6d65  mock.patch('time
+0000b1a0: 2e73 6c65 6570 2729 2e73 7461 7274 2829  .sleep').start()
+0000b1b0: 0a0a 2020 2020 6465 6620 7465 6172 446f  ..    def tearDo
+0000b1c0: 776e 2873 656c 6629 3a0a 2020 2020 2020  wn(self):.      
+0000b1d0: 2020 2320 5265 7365 7420 676c 6f62 616c    # Reset global
+0000b1e0: 7320 696e 2063 6c69 0a20 2020 2020 2020  s in cli.       
+0000b1f0: 2072 656c 6f61 645f 6d6f 6475 6c65 2863   reload_module(c
+0000b200: 6c69 290a 0a20 2020 2020 2020 2073 7570  li)..        sup
+0000b210: 6572 2829 2e74 6561 7244 6f77 6e28 290a  er().tearDown().
+0000b220: 0a20 2020 2064 6566 205f 6361 6c6c 2873  .    def _call(s
+0000b230: 656c 662c 2061 7267 732c 2073 7464 6f75  elf, args, stdou
+0000b240: 743d 4e6f 6e65 2c20 6d6f 636b 6973 6669  t=None, mockisfi
+0000b250: 6c65 3d46 616c 7365 293a 0a20 2020 2020  le=False):.     
+0000b260: 2020 2022 2222 5275 6e20 7468 6520 636c     """Run the cl
+0000b270: 6920 7769 7468 206f 7574 7075 7420 7374  i with output st
+0000b280: 7265 616d 732c 2061 6374 7561 6c20 636c  reams, actual cl
+0000b290: 6965 6e74 2061 6e64 206f 7074 696f 6e61  ient and optiona
+0000b2a0: 6c6c 790a 2020 2020 2020 2020 6f73 2e70  lly.        os.p
+0000b2b0: 6174 682e 6973 6669 6c65 2829 206d 6f63  ath.isfile() moc
+0000b2c0: 6b65 6420 6f75 7422 2222 0a0a 2020 2020  ked out"""..    
+0000b2d0: 2020 2020 6966 206d 6f63 6b69 7366 696c      if mockisfil
+0000b2e0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+0000b2f0: 7269 675f 6f70 656e 203d 206f 732e 7061  rig_open = os.pa
+0000b300: 7468 2e69 7366 696c 650a 0a20 2020 2020  th.isfile..     
+0000b310: 2020 2020 2020 2064 6566 206d 6f63 6b5f         def mock_
+0000b320: 6973 6669 6c65 2866 6e2c 202a 6172 6773  isfile(fn, *args
+0000b330: 2c20 2a2a 6b77 6172 6773 293a 2020 2320  , **kwargs):  # 
+0000b340: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+0000b350: 756e 7573 6564 2d61 7267 756d 656e 740a  unused-argument.
+0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b370: 2222 224d 6f63 6b20 6f73 2e70 6174 682e  """Mock os.path.
+0000b380: 6973 6669 6c65 2829 2222 220a 2020 2020  isfile()""".    
+0000b390: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0000b3a0: 666e 2e65 6e64 7377 6974 6828 2263 6572  fn.endswith("cer
+0000b3b0: 7422 2920 6f72 0a20 2020 2020 2020 2020  t") or.         
+0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b3d0: 6e2e 656e 6473 7769 7468 2822 6368 6169  n.endswith("chai
+0000b3e0: 6e22 2920 6f72 0a20 2020 2020 2020 2020  n") or.         
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b400: 6e2e 656e 6473 7769 7468 2822 7072 6976  n.endswith("priv
+0000b410: 6b65 7922 2929 3a0a 2020 2020 2020 2020  key")):.        
+0000b420: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b430: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000b440: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0000b450: 7269 675f 6f70 656e 2866 6e29 0a0a 2020  rig_open(fn)..  
+0000b460: 2020 2020 2020 2020 2020 7769 7468 206d            with m
+0000b470: 6f63 6b2e 7061 7463 6828 2263 6572 7462  ock.patch("certb
+0000b480: 6f74 2e63 6f6d 7061 742e 6f73 2e70 6174  ot.compat.os.pat
+0000b490: 682e 6973 6669 6c65 2229 2061 7320 6d6f  h.isfile") as mo
+0000b4a0: 636b 5f69 663a 0a20 2020 2020 2020 2020  ck_if:.         
+0000b4b0: 2020 2020 2020 206d 6f63 6b5f 6966 2e73         mock_if.s
+0000b4c0: 6964 655f 6566 6665 6374 203d 206d 6f63  ide_effect = moc
+0000b4d0: 6b5f 6973 6669 6c65 0a20 2020 2020 2020  k_isfile.       
+0000b4e0: 2020 2020 2020 2020 2077 6974 6820 6d6f           with mo
+0000b4f0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+0000b500: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+0000b510: 2e63 6c69 656e 7427 2920 6173 2063 6c69  .client') as cli
+0000b520: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
+0000b530: 2020 2020 2020 2020 2072 6574 2c20 7374           ret, st
+0000b540: 646f 7574 2c20 7374 6465 7272 203d 2073  dout, stderr = s
+0000b550: 656c 662e 5f63 616c 6c5f 6e6f 5f63 6c69  elf._call_no_cli
+0000b560: 656e 746d 6f63 6b28 6172 6773 2c20 7374  entmock(args, st
+0000b570: 646f 7574 290a 2020 2020 2020 2020 2020  dout).          
+0000b580: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000b590: 2072 6574 2c20 7374 646f 7574 2c20 7374   ret, stdout, st
+0000b5a0: 6465 7272 2c20 636c 6965 6e74 0a20 2020  derr, client.   
+0000b5b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b5c0: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
+0000b5d0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0000b5e0: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e63  _internal.main.c
+0000b5f0: 6c69 656e 7427 2920 6173 2063 6c69 656e  lient') as clien
+0000b600: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000b610: 2020 2072 6574 2c20 7374 646f 7574 2c20     ret, stdout, 
+0000b620: 7374 6465 7272 203d 2073 656c 662e 5f63  stderr = self._c
+0000b630: 616c 6c5f 6e6f 5f63 6c69 656e 746d 6f63  all_no_clientmoc
+0000b640: 6b28 6172 6773 2c20 7374 646f 7574 290a  k(args, stdout).
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 7265 7475 726e 2072 6574 2c20 7374 646f  return ret, stdo
+0000b670: 7574 2c20 7374 6465 7272 2c20 636c 6965  ut, stderr, clie
+0000b680: 6e74 0a0a 2020 2020 6465 6620 5f63 616c  nt..    def _cal
+0000b690: 6c5f 6e6f 5f63 6c69 656e 746d 6f63 6b28  l_no_clientmock(
+0000b6a0: 7365 6c66 2c20 6172 6773 2c20 7374 646f  self, args, stdo
+0000b6b0: 7574 3d4e 6f6e 6529 3a0a 2020 2020 2020  ut=None):.      
+0000b6c0: 2020 2222 2252 756e 2074 6865 2063 6c69    """Run the cli
+0000b6d0: 656e 7420 7769 7468 206f 7574 7075 7420  ent with output 
+0000b6e0: 7374 7265 616d 7320 6d6f 636b 6564 206f  streams mocked o
+0000b6f0: 7574 2222 220a 2020 2020 2020 2020 6172  ut""".        ar
+0000b700: 6773 203d 2073 656c 662e 7374 616e 6461  gs = self.standa
+0000b710: 7264 5f61 7267 7320 2b20 6172 6773 0a0a  rd_args + args..
+0000b720: 2020 2020 2020 2020 746f 795f 7374 646f          toy_stdo
+0000b730: 7574 203d 2073 7464 6f75 7420 6966 2073  ut = stdout if s
+0000b740: 7464 6f75 7420 656c 7365 2069 6f2e 5374  tdout else io.St
+0000b750: 7269 6e67 494f 2829 0a20 2020 2020 2020  ringIO().       
+0000b760: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+0000b770: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+0000b780: 6e61 6c2e 6d61 696e 2e73 7973 2e73 7464  nal.main.sys.std
+0000b790: 6f75 7427 2c20 6e65 773d 746f 795f 7374  out', new=toy_st
+0000b7a0: 646f 7574 293a 0a20 2020 2020 2020 2020  dout):.         
+0000b7b0: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
+0000b7c0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000b7d0: 6572 6e61 6c2e 6d61 696e 2e73 7973 2e73  ernal.main.sys.s
+0000b7e0: 7464 6572 7227 2920 6173 2073 7464 6572  tderr') as stder
+0000b7f0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000b800: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
+0000b810: 6368 2822 6365 7274 626f 742e 7574 696c  ch("certbot.util
+0000b820: 2e61 7465 7869 7422 293a 0a20 2020 2020  .atexit"):.     
+0000b830: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b840: 6574 203d 206d 6169 6e2e 6d61 696e 2861  et = main.main(a
+0000b850: 7267 735b 3a5d 2920 2023 204e 4f54 453a  rgs[:])  # NOTE:
+0000b860: 2070 6172 7365 7220 6361 6e20 616c 7465   parser can alte
+0000b870: 7220 6974 7320 6172 6773 210a 2020 2020  r its args!.    
+0000b880: 2020 2020 7265 7475 726e 2072 6574 2c20      return ret, 
+0000b890: 746f 795f 7374 646f 7574 2c20 7374 6465  toy_stdout, stde
+0000b8a0: 7272 0a0a 2020 2020 6465 6620 7465 7374  rr..    def test
+0000b8b0: 5f6e 6f5f 666c 6167 7328 7365 6c66 293a  _no_flags(self):
+0000b8c0: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
+0000b8d0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+0000b8e0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+0000b8f0: 2e72 756e 2729 2061 7320 6d6f 636b 5f72  .run') as mock_r
+0000b900: 756e 3a0a 2020 2020 2020 2020 2020 2020  un:.            
+0000b910: 7365 6c66 2e5f 6361 6c6c 285b 5d29 0a20  self._call([]). 
+0000b920: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000b930: 7420 3120 3d3d 206d 6f63 6b5f 7275 6e2e  t 1 == mock_run.
+0000b940: 6361 6c6c 5f63 6f75 6e74 0a0a 2020 2020  call_count..    
+0000b950: 6465 6620 7465 7374 5f76 6572 7369 6f6e  def test_version
+0000b960: 5f73 7472 696e 675f 7072 6f67 7261 6d5f  _string_program_
+0000b970: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
+0000b980: 2020 2020 746f 795f 6f75 7420 3d20 696f      toy_out = io
+0000b990: 2e53 7472 696e 6749 4f28 290a 2020 2020  .StringIO().    
+0000b9a0: 2020 2020 746f 795f 6572 7220 3d20 696f      toy_err = io
+0000b9b0: 2e53 7472 696e 6749 4f28 290a 2020 2020  .StringIO().    
+0000b9c0: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
+0000b9d0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+0000b9e0: 7465 726e 616c 2e6d 6169 6e2e 7379 732e  ternal.main.sys.
+0000b9f0: 7374 646f 7574 272c 206e 6577 3d74 6f79  stdout', new=toy
+0000ba00: 5f6f 7574 293a 0a20 2020 2020 2020 2020  _out):.         
+0000ba10: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
+0000ba20: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000ba30: 6572 6e61 6c2e 6d61 696e 2e73 7973 2e73  ernal.main.sys.s
+0000ba40: 7464 6572 7227 2c20 6e65 773d 746f 795f  tderr', new=toy_
+0000ba50: 6572 7229 3a0a 2020 2020 2020 2020 2020  err):.          
+0000ba60: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000ba80: 6169 6e2e 6d61 696e 285b 222d 2d76 6572  ain.main(["--ver
+0000ba90: 7369 6f6e 225d 290a 2020 2020 2020 2020  sion"]).        
+0000baa0: 2020 2020 2020 2020 6578 6365 7074 2053          except S
+0000bab0: 7973 7465 6d45 7869 743a 0a20 2020 2020  ystemExit:.     
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000bad0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+0000bae0: 2020 2020 6669 6e61 6c6c 793a 0a20 2020      finally:.   
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 206f 7574 7075 7420 3d20 746f 795f 6f75   output = toy_ou
+0000bb10: 742e 6765 7476 616c 7565 2829 206f 7220  t.getvalue() or 
+0000bb20: 746f 795f 6572 722e 6765 7476 616c 7565  toy_err.getvalue
+0000bb30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000bb40: 2020 2020 2020 2061 7373 6572 7420 2263         assert "c
+0000bb50: 6572 7462 6f74 2220 696e 206f 7574 7075  ertbot" in outpu
+0000bb60: 742c 2022 4f75 7470 7574 2069 7320 7b30  t, "Output is {0
+0000bb70: 7d22 2e66 6f72 6d61 7428 6f75 7470 7574  }".format(output
+0000bb80: 290a 0a20 2020 2064 6566 205f 636c 695f  )..    def _cli_
+0000bb90: 6d69 7373 696e 675f 666c 6167 2873 656c  missing_flag(sel
+0000bba0: 662c 2061 7267 732c 206d 6573 7361 6765  f, args, message
+0000bbb0: 293a 0a20 2020 2020 2020 2022 456e 7375  ):.        "Ensu
+0000bbc0: 7265 2074 6861 7420 6120 7061 7274 6963  re that a partic
+0000bbd0: 756c 6172 2065 7272 6f72 2072 6169 7365  ular error raise
+0000bbe0: 7320 6120 6d69 7373 696e 6720 636c 6920  s a missing cli 
+0000bbf0: 666c 6167 2065 7272 6f72 2063 6f6e 7461  flag error conta
+0000bc00: 696e 696e 6720 6d65 7373 6167 6522 0a20  ining message". 
+0000bc10: 2020 2020 2020 2065 7863 203d 204e 6f6e         exc = Non
+0000bc20: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
+0000bc30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000bc40: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+0000bc50: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0000bc60: 696e 2e73 7973 2e73 7464 6572 7227 293a  in.sys.stderr'):
+0000bc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc80: 206d 6169 6e2e 6d61 696e 2873 656c 662e   main.main(self.
+0000bc90: 7374 616e 6461 7264 5f61 7267 7320 2b20  standard_args + 
+0000bca0: 6172 6773 5b3a 5d29 2020 2320 4e4f 5445  args[:])  # NOTE
+0000bcb0: 3a20 7061 7273 6572 2063 616e 2061 6c74  : parser can alt
+0000bcc0: 6572 2069 7473 2061 7267 7321 0a20 2020  er its args!.   
+0000bcd0: 2020 2020 2065 7863 6570 7420 6572 726f       except erro
+0000bce0: 7273 2e4d 6973 7369 6e67 436f 6d6d 616e  rs.MissingComman
+0000bcf0: 646c 696e 6546 6c61 6720 6173 2065 7863  dlineFlag as exc
+0000bd00: 5f3a 0a20 2020 2020 2020 2020 2020 2065  _:.            e
+0000bd10: 7863 203d 2065 7863 5f0a 2020 2020 2020  xc = exc_.      
+0000bd20: 2020 2020 2020 6173 7365 7274 206d 6573        assert mes
+0000bd30: 7361 6765 2069 6e20 7374 7228 6578 6329  sage in str(exc)
+0000bd40: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000bd50: 6578 6320 6973 206e 6f74 204e 6f6e 650a  exc is not None.
+0000bd60: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+0000bd70: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+0000bd80: 6e61 6c2e 6c6f 672e 706f 7374 5f61 7267  nal.log.post_arg
+0000bd90: 5f70 6172 7365 5f73 6574 7570 2729 0a20  _parse_setup'). 
+0000bda0: 2020 2064 6566 2074 6573 745f 6e6f 6e69     def test_noni
+0000bdb0: 6e74 6572 6163 7469 7665 2873 656c 662c  nteractive(self,
+0000bdc0: 205f 293a 0a20 2020 2020 2020 2061 7267   _):.        arg
+0000bdd0: 7320 3d20 5b27 2d6e 272c 2027 6365 7274  s = ['-n', 'cert
+0000bde0: 6f6e 6c79 275d 0a20 2020 2020 2020 2073  only'].        s
+0000bdf0: 656c 662e 5f63 6c69 5f6d 6973 7369 6e67  elf._cli_missing
+0000be00: 5f66 6c61 6728 6172 6773 2c20 2273 7065  _flag(args, "spe
+0000be10: 6369 6679 2061 2070 6c75 6769 6e22 290a  cify a plugin").
+0000be20: 2020 2020 2020 2020 6172 6773 2e65 7874          args.ext
+0000be30: 656e 6428 5b27 2d2d 7374 616e 6461 6c6f  end(['--standalo
+0000be40: 6e65 272c 2027 2d64 272c 2027 6567 2e69  ne', '-d', 'eg.i
+0000be50: 7327 5d29 0a20 2020 2020 2020 2073 656c  s']).        sel
+0000be60: 662e 5f63 6c69 5f6d 6973 7369 6e67 5f66  f._cli_missing_f
+0000be70: 6c61 6728 6172 6773 2c20 2272 6567 6973  lag(args, "regis
+0000be80: 7465 7220 6265 666f 7265 2072 756e 6e69  ter before runni
+0000be90: 6e67 2229 0a0a 2020 2020 406d 6f63 6b2e  ng")..    @mock.
+0000bea0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0000beb0: 696e 7465 726e 616c 2e65 6666 2e68 616e  internal.eff.han
+0000bec0: 646c 655f 7375 6273 6372 6970 7469 6f6e  dle_subscription
+0000bed0: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
+0000bee0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000bef0: 6572 6e61 6c2e 6c6f 672e 706f 7374 5f61  ernal.log.post_a
+0000bf00: 7267 5f70 6172 7365 5f73 6574 7570 2729  rg_parse_setup')
+0000bf10: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+0000bf20: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+0000bf30: 6e61 6c2e 6d61 696e 2e5f 7265 706f 7274  nal.main._report
+0000bf40: 5f6e 6577 5f63 6572 7427 290a 2020 2020  _new_cert').    
+0000bf50: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
+0000bf60: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+0000bf70: 6169 6e2e 5f64 6574 6572 6d69 6e65 5f61  ain._determine_a
+0000bf80: 6363 6f75 6e74 2729 0a20 2020 2040 6d6f  ccount').    @mo
+0000bf90: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+0000bfa0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+0000bfb0: 2e63 6c69 656e 742e 436c 6965 6e74 2e6f  .client.Client.o
+0000bfc0: 6274 6169 6e5f 616e 645f 656e 726f 6c6c  btain_and_enroll
+0000bfd0: 5f63 6572 7469 6669 6361 7465 2729 0a20  _certificate'). 
+0000bfe0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+0000bff0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+0000c000: 6c2e 6d61 696e 2e5f 6765 745f 616e 645f  l.main._get_and_
+0000c010: 7361 7665 5f63 6572 7427 290a 2020 2020  save_cert').    
+0000c020: 6465 6620 7465 7374 5f75 7365 725f 6167  def test_user_ag
+0000c030: 656e 7428 7365 6c66 2c20 6773 632c 205f  ent(self, gsc, _
+0000c040: 6f62 742c 2064 6574 2c20 5f2c 205f 5f2c  obt, det, _, __,
+0000c050: 205f 5f5f 293a 0a20 2020 2020 2020 2023   ___):.        #
+0000c060: 204e 6f72 6d61 6c6c 7920 7468 6520 636c   Normally the cl
+0000c070: 6965 6e74 2069 7320 746f 7461 6c6c 7920  ient is totally 
+0000c080: 6d6f 636b 6564 206f 7574 2c20 6275 7420  mocked out, but 
+0000c090: 6865 7265 2077 6520 6e65 6564 206d 6f72  here we need mor
+0000c0a0: 650a 2020 2020 2020 2020 2320 6172 6775  e.        # argu
+0000c0b0: 6d65 6e74 7320 746f 2061 7574 6f6d 6174  ments to automat
+0000c0c0: 6520 6974 2e2e 2e0a 2020 2020 2020 2020  e it....        
+0000c0d0: 6172 6773 203d 205b 222d 2d73 7461 6e64  args = ["--stand
+0000c0e0: 616c 6f6e 6522 2c20 2263 6572 746f 6e6c  alone", "certonl
+0000c0f0: 7922 2c20 222d 6d22 2c20 226e 6f6e 6540  y", "-m", "none@
+0000c100: 6e6f 6e65 2e63 6f6d 222c 0a20 2020 2020  none.com",.     
+0000c110: 2020 2020 2020 2020 2020 2022 2d64 222c             "-d",
+0000c120: 2022 6578 616d 706c 652e 636f 6d22 2c20   "example.com", 
+0000c130: 272d 2d61 6772 6565 2d74 6f73 275d 202b  '--agree-tos'] +
+0000c140: 2073 656c 662e 7374 616e 6461 7264 5f61   self.standard_a
+0000c150: 7267 730a 2020 2020 2020 2020 6465 742e  rgs.        det.
+0000c160: 7265 7475 726e 5f76 616c 7565 203d 206d  return_value = m
+0000c170: 6f63 6b2e 4d61 6769 634d 6f63 6b28 292c  ock.MagicMock(),
+0000c180: 204e 6f6e 650a 2020 2020 2020 2020 6773   None.        gs
+0000c190: 632e 7265 7475 726e 5f76 616c 7565 203d  c.return_value =
+0000c1a0: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
+0000c1b0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+0000c1c0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+0000c1d0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0000c1e0: 696e 2e63 6c69 656e 742e 6163 6d65 5f63  in.client.acme_c
+0000c1f0: 6c69 656e 7427 2920 6173 2061 636d 655f  lient') as acme_
+0000c200: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+0000c210: 2020 2020 6163 6d65 5f6e 6574 203d 2061      acme_net = a
+0000c220: 636d 655f 636c 6965 6e74 2e43 6c69 656e  cme_client.Clien
+0000c230: 744e 6574 776f 726b 0a20 2020 2020 2020  tNetwork.       
+0000c240: 2020 2020 2073 656c 662e 5f63 616c 6c5f       self._call_
+0000c250: 6e6f 5f63 6c69 656e 746d 6f63 6b28 6172  no_clientmock(ar
+0000c260: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
+0000c270: 6f73 5f76 6572 203d 2075 7469 6c2e 6765  os_ver = util.ge
+0000c280: 745f 6f73 5f69 6e66 6f5f 7561 2829 0a20  t_os_info_ua(). 
+0000c290: 2020 2020 2020 2020 2020 2075 6120 3d20             ua = 
+0000c2a0: 6163 6d65 5f6e 6574 2e63 616c 6c5f 6172  acme_net.call_ar
+0000c2b0: 6773 5b31 5d5b 2275 7365 725f 6167 656e  gs[1]["user_agen
+0000c2c0: 7422 5d0a 2020 2020 2020 2020 2020 2020  t"].            
+0000c2d0: 6173 7365 7274 206f 735f 7665 7220 696e  assert os_ver in
+0000c2e0: 2075 610a 2020 2020 2020 2020 2020 2020   ua.            
+0000c2f0: 696d 706f 7274 2070 6c61 7466 6f72 6d0a  import platform.
+0000c300: 2020 2020 2020 2020 2020 2020 706c 6174              plat
+0000c310: 203d 2070 6c61 7466 6f72 6d2e 706c 6174   = platform.plat
+0000c320: 666f 726d 2829 0a20 2020 2020 2020 2020  form().         
+0000c330: 2020 2069 6620 226c 696e 7578 2220 696e     if "linux" in
+0000c340: 2070 6c61 742e 6c6f 7765 7228 293a 0a20   plat.lower():. 
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000c360: 7373 6572 7420 7574 696c 2e67 6574 5f6f  ssert util.get_o
+0000c370: 735f 696e 666f 5f75 6128 2920 696e 2075  s_info_ua() in u
+0000c380: 610a 0a20 2020 2020 2020 2077 6974 6820  a..        with 
+0000c390: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+0000c3a0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0000c3b0: 696e 2e63 6c69 656e 742e 6163 6d65 5f63  in.client.acme_c
+0000c3c0: 6c69 656e 7427 2920 6173 2061 636d 655f  lient') as acme_
+0000c3d0: 636c 6965 6e74 3a0a 2020 2020 2020 2020  client:.        
+0000c3e0: 2020 2020 6163 6d65 5f6e 6574 203d 2061      acme_net = a
+0000c3f0: 636d 655f 636c 6965 6e74 2e43 6c69 656e  cme_client.Clien
+0000c400: 744e 6574 776f 726b 0a20 2020 2020 2020  tNetwork.       
+0000c410: 2020 2020 2075 6120 3d20 2262 616e 6465       ua = "bande
+0000c420: 7273 6e61 7463 6822 0a20 2020 2020 2020  rsnatch".       
+0000c430: 2020 2020 2061 7267 7320 2b3d 205b 222d       args += ["-
+0000c440: 2d75 7365 722d 6167 656e 7422 2c20 7561  -user-agent", ua
+0000c450: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+0000c460: 6c66 2e5f 6361 6c6c 5f6e 6f5f 636c 6965  lf._call_no_clie
+0000c470: 6e74 6d6f 636b 2861 7267 7329 0a20 2020  ntmock(args).   
+0000c480: 2020 2020 2020 2020 2061 636d 655f 6e65           acme_ne
+0000c490: 742e 6173 7365 7274 5f63 616c 6c65 645f  t.assert_called_
+0000c4a0: 6f6e 6365 5f77 6974 6828 6d6f 636b 2e41  once_with(mock.A
+0000c4b0: 4e59 2c20 6163 636f 756e 743d 6d6f 636b  NY, account=mock
+0000c4c0: 2e41 4e59 2c20 7665 7269 6679 5f73 736c  .ANY, verify_ssl
+0000c4d0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+0000c4e0: 2020 2020 2020 2075 7365 725f 6167 656e         user_agen
+0000c4f0: 743d 7561 2c20 616c 673d 6a6f 7365 2e52  t=ua, alg=jose.R
+0000c500: 5332 3536 290a 0a20 2020 2040 6d6f 636b  S256)..    @mock
+0000c510: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0000c520: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e70  _internal.main.p
+0000c530: 6c75 675f 7365 6c2e 7265 636f 7264 5f63  lug_sel.record_c
+0000c540: 686f 7365 6e5f 706c 7567 696e 7327 290a  hosen_plugins').
+0000c550: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+0000c560: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000c570: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
+0000c580: 2e70 6963 6b5f 696e 7374 616c 6c65 7227  .pick_installer'
+0000c590: 290a 2020 2020 6465 6620 7465 7374 5f69  ).    def test_i
+0000c5a0: 6e73 7461 6c6c 6572 5f73 656c 6563 7469  nstaller_selecti
+0000c5b0: 6f6e 2873 656c 662c 206d 6f63 6b5f 7069  on(self, mock_pi
+0000c5c0: 636b 5f69 6e73 7461 6c6c 6572 2c20 5f72  ck_installer, _r
+0000c5d0: 6563 293a 0a20 2020 2020 2020 2073 656c  ec):.        sel
+0000c5e0: 662e 5f63 616c 6c28 5b27 696e 7374 616c  f._call(['instal
+0000c5f0: 6c27 2c20 272d 2d64 6f6d 6169 6e73 272c  l', '--domains',
+0000c600: 2027 666f 6f2e 6261 7227 2c20 272d 2d63   'foo.bar', '--c
+0000c610: 6572 742d 7061 7468 272c 2027 6365 7274  ert-path', 'cert
+0000c620: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000c630: 2020 2020 2020 2027 2d2d 6b65 792d 7061         '--key-pa
+0000c640: 7468 272c 2027 7072 6976 6b65 7927 2c20  th', 'privkey', 
+0000c650: 272d 2d63 6861 696e 2d70 6174 6827 2c20  '--chain-path', 
+0000c660: 2763 6861 696e 275d 2c20 6d6f 636b 6973  'chain'], mockis
+0000c670: 6669 6c65 3d54 7275 6529 0a20 2020 2020  file=True).     
+0000c680: 2020 2061 7373 6572 7420 6d6f 636b 5f70     assert mock_p
+0000c690: 6963 6b5f 696e 7374 616c 6c65 722e 6361  ick_installer.ca
+0000c6a0: 6c6c 5f63 6f75 6e74 203d 3d20 310a 0a20  ll_count == 1.. 
+0000c6b0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+0000c6c0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+0000c6d0: 6c2e 6d61 696e 2e5f 696e 7374 616c 6c5f  l.main._install_
+0000c6e0: 6365 7274 2729 0a20 2020 2040 6d6f 636b  cert').    @mock
+0000c6f0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0000c700: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e70  _internal.main.p
+0000c710: 6c75 675f 7365 6c2e 7265 636f 7264 5f63  lug_sel.record_c
+0000c720: 686f 7365 6e5f 706c 7567 696e 7327 290a  hosen_plugins').
+0000c730: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+0000c740: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000c750: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
+0000c760: 2e70 6963 6b5f 696e 7374 616c 6c65 7227  .pick_installer'
+0000c770: 290a 2020 2020 6465 6620 7465 7374 5f69  ).    def test_i
+0000c780: 6e73 7461 6c6c 6572 5f63 6572 746e 616d  nstaller_certnam
+0000c790: 6528 7365 6c66 2c20 5f69 6e73 742c 205f  e(self, _inst, _
+0000c7a0: 7265 632c 206d 6f63 6b5f 696e 7374 616c  rec, mock_instal
+0000c7b0: 6c29 3a0a 2020 2020 2020 2020 6d6f 636b  l):.        mock
+0000c7c0: 5f6c 696e 6561 6765 203d 206d 6f63 6b2e  _lineage = mock.
+0000c7d0: 4d61 6769 634d 6f63 6b28 6365 7274 5f70  MagicMock(cert_p
+0000c7e0: 6174 683d 7465 7374 5f75 7469 6c2e 7465  ath=test_util.te
+0000c7f0: 6d70 5f6a 6f69 6e28 2763 6572 7427 292c  mp_join('cert'),
+0000c800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 2020 2020 2020 2063 6861 696e 5f70 6174         chain_pat
+0000c830: 683d 7465 7374 5f75 7469 6c2e 7465 6d70  h=test_util.temp
+0000c840: 5f6a 6f69 6e28 2763 6861 696e 2729 2c0a  _join('chain'),.
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2020 2020 2020 6675 6c6c 6368 6169 6e5f        fullchain_
+0000c880: 7061 7468 3d74 6573 745f 7574 696c 2e74  path=test_util.t
+0000c890: 656d 705f 6a6f 696e 2827 6368 6169 6e27  emp_join('chain'
+0000c8a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 206b 6579 5f70 6174           key_pat
+0000c8d0: 683d 7465 7374 5f75 7469 6c2e 7465 6d70  h=test_util.temp
+0000c8e0: 5f6a 6f69 6e28 2770 7269 766b 6579 2729  _join('privkey')
+0000c8f0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+0000c900: 6d6f 636b 2e70 6174 6368 2822 6365 7274  mock.patch("cert
+0000c910: 626f 742e 5f69 6e74 6572 6e61 6c2e 6365  bot._internal.ce
+0000c920: 7274 5f6d 616e 6167 6572 2e6c 696e 6561  rt_manager.linea
+0000c930: 6765 5f66 6f72 5f63 6572 746e 616d 6522  ge_for_certname"
+0000c940: 2920 6173 206d 6f63 6b5f 6765 746c 696e  ) as mock_getlin
+0000c950: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+0000c960: 636b 5f67 6574 6c69 6e2e 7265 7475 726e  ck_getlin.return
+0000c970: 5f76 616c 7565 203d 206d 6f63 6b5f 6c69  _value = mock_li
+0000c980: 6e65 6167 650a 2020 2020 2020 2020 2020  neage.          
+0000c990: 2020 7365 6c66 2e5f 6361 6c6c 285b 2769    self._call(['i
+0000c9a0: 6e73 7461 6c6c 272c 2027 2d2d 6365 7274  nstall', '--cert
+0000c9b0: 2d6e 616d 6527 2c20 2777 6861 7465 7665  -name', 'whateve
+0000c9c0: 7227 5d2c 206d 6f63 6b69 7366 696c 653d  r'], mockisfile=
+0000c9d0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0000c9e0: 2020 6361 6c6c 5f63 6f6e 6669 6720 3d20    call_config = 
+0000c9f0: 6d6f 636b 5f69 6e73 7461 6c6c 2e63 616c  mock_install.cal
+0000ca00: 6c5f 6172 6773 5b30 5d5b 305d 0a20 2020  l_args[0][0].   
+0000ca10: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000ca20: 6361 6c6c 5f63 6f6e 6669 672e 6365 7274  call_config.cert
+0000ca30: 5f70 6174 6820 3d3d 2074 6573 745f 7574  _path == test_ut
+0000ca40: 696c 2e74 656d 705f 6a6f 696e 2827 6365  il.temp_join('ce
+0000ca50: 7274 2729 0a20 2020 2020 2020 2020 2020  rt').           
+0000ca60: 2061 7373 6572 7420 6361 6c6c 5f63 6f6e   assert call_con
+0000ca70: 6669 672e 6675 6c6c 6368 6169 6e5f 7061  fig.fullchain_pa
+0000ca80: 7468 203d 3d20 7465 7374 5f75 7469 6c2e  th == test_util.
+0000ca90: 7465 6d70 5f6a 6f69 6e28 2763 6861 696e  temp_join('chain
+0000caa0: 2729 0a20 2020 2020 2020 2020 2020 2061  ').            a
+0000cab0: 7373 6572 7420 6361 6c6c 5f63 6f6e 6669  ssert call_confi
+0000cac0: 672e 6b65 795f 7061 7468 203d 3d20 7465  g.key_path == te
+0000cad0: 7374 5f75 7469 6c2e 7465 6d70 5f6a 6f69  st_util.temp_joi
+0000cae0: 6e28 2770 7269 766b 6579 2729 0a0a 2020  n('privkey')..  
+0000caf0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+0000cb00: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+0000cb10: 2e6c 6f67 2e70 6f73 745f 6172 675f 7061  .log.post_arg_pa
+0000cb20: 7273 655f 7365 7475 7027 290a 2020 2020  rse_setup').    
+0000cb30: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
+0000cb40: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+0000cb50: 6169 6e2e 5f69 6e73 7461 6c6c 5f63 6572  ain._install_cer
+0000cb60: 7427 290a 2020 2020 406d 6f63 6b2e 7061  t').    @mock.pa
+0000cb70: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+0000cb80: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
+0000cb90: 5f73 656c 2e72 6563 6f72 645f 6368 6f73  _sel.record_chos
+0000cba0: 656e 5f70 6c75 6769 6e73 2729 0a20 2020  en_plugins').   
+0000cbb0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000cbc0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0000cbd0: 6d61 696e 2e70 6c75 675f 7365 6c2e 7069  main.plug_sel.pi
+0000cbe0: 636b 5f69 6e73 7461 6c6c 6572 2729 0a20  ck_installer'). 
+0000cbf0: 2020 2064 6566 2074 6573 745f 696e 7374     def test_inst
+0000cc00: 616c 6c65 725f 7061 7261 6d5f 6f76 6572  aller_param_over
+0000cc10: 7269 6465 2873 656c 662c 205f 696e 7374  ride(self, _inst
+0000cc20: 2c20 5f72 6563 2c20 6d6f 636b 5f69 6e73  , _rec, mock_ins
+0000cc30: 7461 6c6c 2c20 5f29 3a0a 2020 2020 2020  tall, _):.      
+0000cc40: 2020 6d6f 636b 5f6c 696e 6561 6765 203d    mock_lineage =
+0000cc50: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
+0000cc60: 6365 7274 5f70 6174 683d 7465 7374 5f75  cert_path=test_u
+0000cc70: 7469 6c2e 7465 6d70 5f6a 6f69 6e28 2763  til.temp_join('c
+0000cc80: 6572 7427 292c 0a20 2020 2020 2020 2020  ert'),.         
+0000cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cca0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0000ccb0: 696e 5f70 6174 683d 7465 7374 5f75 7469  in_path=test_uti
+0000ccc0: 6c2e 7465 6d70 5f6a 6f69 6e28 2763 6861  l.temp_join('cha
+0000ccd0: 696e 2729 2c0a 2020 2020 2020 2020 2020  in'),.          
+0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccf0: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
+0000cd00: 6368 6169 6e5f 7061 7468 3d74 6573 745f  chain_path=test_
+0000cd10: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
+0000cd20: 6368 6169 6e27 292c 0a20 2020 2020 2020  chain'),.       
+0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+0000cd50: 6579 5f70 6174 683d 7465 7374 5f75 7469  ey_path=test_uti
+0000cd60: 6c2e 7465 6d70 5f6a 6f69 6e28 2770 7269  l.temp_join('pri
+0000cd70: 766b 6579 2729 290a 2020 2020 2020 2020  vkey')).        
+0000cd80: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
+0000cd90: 2263 6572 7462 6f74 2e5f 696e 7465 726e  "certbot._intern
+0000cda0: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
+0000cdb0: 6c69 6e65 6167 655f 666f 725f 6365 7274  lineage_for_cert
+0000cdc0: 6e61 6d65 2229 2061 7320 6d6f 636b 5f67  name") as mock_g
+0000cdd0: 6574 6c69 6e3a 0a20 2020 2020 2020 2020  etlin:.         
+0000cde0: 2020 206d 6f63 6b5f 6765 746c 696e 2e72     mock_getlin.r
+0000cdf0: 6574 7572 6e5f 7661 6c75 6520 3d20 6d6f  eturn_value = mo
+0000ce00: 636b 5f6c 696e 6561 6765 0a20 2020 2020  ck_lineage.     
+0000ce10: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+0000ce20: 6c28 5b27 696e 7374 616c 6c27 2c20 272d  l(['install', '-
+0000ce30: 2d63 6572 742d 6e61 6d65 272c 2027 7768  -cert-name', 'wh
+0000ce40: 6174 6576 6572 272c 0a20 2020 2020 2020  atever',.       
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2027 2d2d 6b65 792d 7061 7468 272c 2074   '--key-path', t
+0000ce70: 6573 745f 7574 696c 2e74 656d 705f 6a6f  est_util.temp_jo
+0000ce80: 696e 2827 6f76 6572 7269 6469 6e67 5f70  in('overriding_p
+0000ce90: 7269 766b 6579 2729 5d2c 206d 6f63 6b69  rivkey')], mocki
+0000cea0: 7366 696c 653d 5472 7565 290a 2020 2020  sfile=True).    
+0000ceb0: 2020 2020 2020 2020 6361 6c6c 5f63 6f6e          call_con
+0000cec0: 6669 6720 3d20 6d6f 636b 5f69 6e73 7461  fig = mock_insta
+0000ced0: 6c6c 2e63 616c 6c5f 6172 6773 5b30 5d5b  ll.call_args[0][
+0000cee0: 305d 0a20 2020 2020 2020 2020 2020 2061  0].            a
+0000cef0: 7373 6572 7420 6361 6c6c 5f63 6f6e 6669  ssert call_confi
+0000cf00: 672e 6365 7274 5f70 6174 6820 3d3d 2074  g.cert_path == t
+0000cf10: 6573 745f 7574 696c 2e74 656d 705f 6a6f  est_util.temp_jo
+0000cf20: 696e 2827 6365 7274 2729 0a20 2020 2020  in('cert').     
+0000cf30: 2020 2020 2020 2061 7373 6572 7420 6361         assert ca
+0000cf40: 6c6c 5f63 6f6e 6669 672e 6675 6c6c 6368  ll_config.fullch
+0000cf50: 6169 6e5f 7061 7468 203d 3d20 7465 7374  ain_path == test
+0000cf60: 5f75 7469 6c2e 7465 6d70 5f6a 6f69 6e28  _util.temp_join(
+0000cf70: 2763 6861 696e 2729 0a20 2020 2020 2020  'chain').       
+0000cf80: 2020 2020 2061 7373 6572 7420 6361 6c6c       assert call
+0000cf90: 5f63 6f6e 6669 672e 6368 6169 6e5f 7061  _config.chain_pa
+0000cfa0: 7468 203d 3d20 7465 7374 5f75 7469 6c2e  th == test_util.
+0000cfb0: 7465 6d70 5f6a 6f69 6e28 2763 6861 696e  temp_join('chain
+0000cfc0: 2729 0a20 2020 2020 2020 2020 2020 2061  ').            a
+0000cfd0: 7373 6572 7420 6361 6c6c 5f63 6f6e 6669  ssert call_confi
+0000cfe0: 672e 6b65 795f 7061 7468 203d 3d20 7465  g.key_path == te
+0000cff0: 7374 5f75 7469 6c2e 7465 6d70 5f6a 6f69  st_util.temp_joi
+0000d000: 6e28 276f 7665 7272 6964 696e 675f 7072  n('overriding_pr
+0000d010: 6976 6b65 7927 290a 0a20 2020 2020 2020  ivkey')..       
+0000d020: 2020 2020 206d 6f63 6b5f 696e 7374 616c       mock_instal
+0000d030: 6c2e 7265 7365 7428 290a 0a20 2020 2020  l.reset()..     
+0000d040: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+0000d050: 6c28 5b27 696e 7374 616c 6c27 2c20 272d  l(['install', '-
+0000d060: 2d63 6572 742d 6e61 6d65 272c 2027 7768  -cert-name', 'wh
+0000d070: 6174 6576 6572 272c 0a20 2020 2020 2020  atever',.       
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2027 2d2d 6365 7274 2d70 6174 6827 2c20   '--cert-path', 
+0000d0a0: 7465 7374 5f75 7469 6c2e 7465 6d70 5f6a  test_util.temp_j
+0000d0b0: 6f69 6e28 276f 7665 7272 6964 696e 675f  oin('overriding_
+0000d0c0: 6365 7274 2729 5d2c 206d 6f63 6b69 7366  cert')], mockisf
+0000d0d0: 696c 653d 5472 7565 290a 2020 2020 2020  ile=True).      
+0000d0e0: 2020 2020 2020 6361 6c6c 5f63 6f6e 6669        call_confi
+0000d0f0: 6720 3d20 6d6f 636b 5f69 6e73 7461 6c6c  g = mock_install
+0000d100: 2e63 616c 6c5f 6172 6773 5b30 5d5b 305d  .call_args[0][0]
+0000d110: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+0000d120: 6572 7420 6361 6c6c 5f63 6f6e 6669 672e  ert call_config.
+0000d130: 6365 7274 5f70 6174 6820 3d3d 2074 6573  cert_path == tes
+0000d140: 745f 7574 696c 2e74 656d 705f 6a6f 696e  t_util.temp_join
+0000d150: 2827 6f76 6572 7269 6469 6e67 5f63 6572  ('overriding_cer
+0000d160: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
+0000d170: 6173 7365 7274 2063 616c 6c5f 636f 6e66  assert call_conf
+0000d180: 6967 2e66 756c 6c63 6861 696e 5f70 6174  ig.fullchain_pat
+0000d190: 6820 3d3d 2074 6573 745f 7574 696c 2e74  h == test_util.t
+0000d1a0: 656d 705f 6a6f 696e 2827 6368 6169 6e27  emp_join('chain'
+0000d1b0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
+0000d1c0: 7365 7274 2063 616c 6c5f 636f 6e66 6967  sert call_config
+0000d1d0: 2e6b 6579 5f70 6174 6820 3d3d 2074 6573  .key_path == tes
+0000d1e0: 745f 7574 696c 2e74 656d 705f 6a6f 696e  t_util.temp_join
+0000d1f0: 2827 7072 6976 6b65 7927 290a 0a20 2020  ('privkey')..   
+0000d200: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000d210: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0000d220: 6d61 696e 2e70 6c75 675f 7365 6c2e 7265  main.plug_sel.re
+0000d230: 636f 7264 5f63 686f 7365 6e5f 706c 7567  cord_chosen_plug
+0000d240: 696e 7327 290a 2020 2020 406d 6f63 6b2e  ins').    @mock.
+0000d250: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0000d260: 696e 7465 726e 616c 2e6d 6169 6e2e 706c  internal.main.pl
+0000d270: 7567 5f73 656c 2e70 6963 6b5f 696e 7374  ug_sel.pick_inst
+0000d280: 616c 6c65 7227 290a 2020 2020 6465 6620  aller').    def 
+0000d290: 7465 7374 5f69 6e73 7461 6c6c 6572 5f70  test_installer_p
+0000d2a0: 6172 616d 5f65 7272 6f72 2873 656c 662c  aram_error(self,
+0000d2b0: 205f 696e 7374 2c20 5f72 6563 293a 0a20   _inst, _rec):. 
+0000d2c0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+0000d2d0: 7374 2e72 6169 7365 7328 6572 726f 7273  st.raises(errors
+0000d2e0: 2e43 6f6e 6669 6775 7261 7469 6f6e 4572  .ConfigurationEr
+0000d2f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+0000d300: 2020 7365 6c66 2e5f 6361 6c6c 285b 2769    self._call(['i
+0000d310: 6e73 7461 6c6c 272c 2027 2d2d 6365 7274  nstall', '--cert
+0000d320: 2d6e 616d 6527 2c20 276e 6f74 666f 756e  -name', 'notfoun
+0000d330: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000d350: 2d2d 6b65 792d 7061 7468 272c 2027 696e  --key-path', 'in
+0000d360: 7661 6c69 6427 5d29 0a0a 2020 2020 406d  valid'])..    @m
+0000d370: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+0000d380: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+0000d390: 6e2e 706c 7567 5f73 656c 2e72 6563 6f72  n.plug_sel.recor
+0000d3a0: 645f 6368 6f73 656e 5f70 6c75 6769 6e73  d_chosen_plugins
+0000d3b0: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
+0000d3c0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000d3d0: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
+0000d3e0: 7365 6c2e 7069 636b 5f69 6e73 7461 6c6c  sel.pick_install
+0000d3f0: 6572 2729 0a20 2020 2040 6d6f 636b 2e70  er').    @mock.p
+0000d400: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0000d410: 6e74 6572 6e61 6c2e 6365 7274 5f6d 616e  nternal.cert_man
+0000d420: 6167 6572 2e67 6574 5f63 6572 746e 616d  ager.get_certnam
+0000d430: 6573 2729 0a20 2020 2040 6d6f 636b 2e70  es').    @mock.p
+0000d440: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0000d450: 6e74 6572 6e61 6c2e 6d61 696e 2e5f 696e  nternal.main._in
+0000d460: 7374 616c 6c5f 6365 7274 2729 0a20 2020  stall_cert').   
+0000d470: 2064 6566 2074 6573 745f 696e 7374 616c   def test_instal
+0000d480: 6c65 725f 7365 6c65 6374 5f63 6572 7428  ler_select_cert(
+0000d490: 7365 6c66 2c20 6d6f 636b 5f69 6e73 742c  self, mock_inst,
+0000d4a0: 206d 6f63 6b5f 6765 7463 6572 742c 205f   mock_getcert, _
+0000d4b0: 696e 7374 2c20 5f72 6563 293a 0a20 2020  inst, _rec):.   
+0000d4c0: 2020 2020 206d 6f63 6b5f 6c69 6e65 6167       mock_lineag
+0000d4d0: 6520 3d20 6d6f 636b 2e4d 6167 6963 4d6f  e = mock.MagicMo
+0000d4e0: 636b 2863 6572 745f 7061 7468 3d74 6573  ck(cert_path=tes
+0000d4f0: 745f 7574 696c 2e74 656d 705f 6a6f 696e  t_util.temp_join
+0000d500: 2827 6365 7274 2729 2c0a 2020 2020 2020  ('cert'),.      
+0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 6368 6169 6e5f 7061 7468 3d74 6573 745f  chain_path=test_
+0000d540: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
+0000d550: 6368 6169 6e27 292c 0a20 2020 2020 2020  chain'),.       
+0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d570: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000d580: 756c 6c63 6861 696e 5f70 6174 683d 7465  ullchain_path=te
+0000d590: 7374 5f75 7469 6c2e 7465 6d70 5f6a 6f69  st_util.temp_joi
+0000d5a0: 6e28 2763 6861 696e 2729 2c0a 2020 2020  n('chain'),.    
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5d0: 2020 6b65 795f 7061 7468 3d74 6573 745f    key_path=test_
+0000d5e0: 7574 696c 2e74 656d 705f 6a6f 696e 2827  util.temp_join('
+0000d5f0: 7072 6976 6b65 7927 2929 0a20 2020 2020  privkey')).     
+0000d600: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
+0000d610: 6368 2822 6365 7274 626f 742e 5f69 6e74  ch("certbot._int
+0000d620: 6572 6e61 6c2e 6365 7274 5f6d 616e 6167  ernal.cert_manag
+0000d630: 6572 2e6c 696e 6561 6765 5f66 6f72 5f63  er.lineage_for_c
+0000d640: 6572 746e 616d 6522 2920 6173 206d 6f63  ertname") as moc
+0000d650: 6b5f 6765 746c 696e 3a0a 2020 2020 2020  k_getlin:.      
+0000d660: 2020 2020 2020 6d6f 636b 5f67 6574 6c69        mock_getli
+0000d670: 6e2e 7265 7475 726e 5f76 616c 7565 203d  n.return_value =
+0000d680: 206d 6f63 6b5f 6c69 6e65 6167 650a 2020   mock_lineage.  
+0000d690: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000d6a0: 6361 6c6c 285b 2769 6e73 7461 6c6c 275d  call(['install']
+0000d6b0: 2c20 6d6f 636b 6973 6669 6c65 3d54 7275  , mockisfile=Tru
+0000d6c0: 6529 0a20 2020 2020 2020 2061 7373 6572  e).        asser
+0000d6d0: 7420 6d6f 636b 5f67 6574 6365 7274 2e63  t mock_getcert.c
+0000d6e0: 616c 6c65 640a 2020 2020 2020 2020 6173  alled.        as
+0000d6f0: 7365 7274 206d 6f63 6b5f 696e 7374 2e63  sert mock_inst.c
+0000d700: 616c 6c65 640a 0a20 2020 2040 6d6f 636b  alled..    @mock
+0000d710: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0000d720: 5f69 6e74 6572 6e61 6c2e 6566 662e 6861  _internal.eff.ha
+0000d730: 6e64 6c65 5f73 7562 7363 7269 7074 696f  ndle_subscriptio
+0000d740: 6e27 290a 2020 2020 406d 6f63 6b2e 7061  n').    @mock.pa
+0000d750: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+0000d760: 7465 726e 616c 2e6c 6f67 2e70 6f73 745f  ternal.log.post_
+0000d770: 6172 675f 7061 7273 655f 7365 7475 7027  arg_parse_setup'
+0000d780: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+0000d790: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+0000d7a0: 726e 616c 2e6d 6169 6e2e 5f72 6570 6f72  rnal.main._repor
+0000d7b0: 745f 6e65 775f 6365 7274 2729 0a20 2020  t_new_cert').   
+0000d7c0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000d7d0: 7274 626f 742e 7574 696c 2e65 7865 5f65  rtbot.util.exe_e
+0000d7e0: 7869 7374 7327 290a 2020 2020 6465 6620  xists').    def 
+0000d7f0: 7465 7374 5f63 6f6e 6669 6775 7261 746f  test_configurato
+0000d800: 725f 7365 6c65 6374 696f 6e28 7365 6c66  r_selection(self
+0000d810: 2c20 6d6f 636b 5f65 7865 5f65 7869 7374  , mock_exe_exist
+0000d820: 732c 205f 2c20 5f5f 2c20 5f5f 5f29 3a0a  s, _, __, ___):.
+0000d830: 2020 2020 2020 2020 6d6f 636b 5f65 7865          mock_exe
+0000d840: 5f65 7869 7374 732e 7265 7475 726e 5f76  _exists.return_v
+0000d850: 616c 7565 203d 2054 7275 650a 2020 2020  alue = True.    
+0000d860: 2020 2020 7265 616c 5f70 6c75 6769 6e73      real_plugins
+0000d870: 203d 2064 6973 636f 2e50 6c75 6769 6e73   = disco.Plugins
+0000d880: 5265 6769 7374 7279 2e66 696e 645f 616c  Registry.find_al
+0000d890: 6c28 290a 2020 2020 2020 2020 6172 6773  l().        args
+0000d8a0: 203d 205b 272d 2d61 7061 6368 6527 2c20   = ['--apache', 
+0000d8b0: 272d 2d61 7574 6865 6e74 6963 6174 6f72  '--authenticator
+0000d8c0: 272c 2027 7374 616e 6461 6c6f 6e65 275d  ', 'standalone']
+0000d8d0: 0a0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
+0000d8e0: 206e 6565 6465 6420 7477 6f20 6361 6c6c   needed two call
+0000d8f0: 7320 746f 2066 696e 645f 616c 6c28 292c  s to find_all(),
+0000d900: 2077 6869 6368 2077 6527 7265 2061 766f   which we're avo
+0000d910: 6964 696e 6720 666f 7220 6e6f 770a 2020  iding for now.  
+0000d920: 2020 2020 2020 2320 6265 6361 7573 6520        # because 
+0000d930: 6f66 2070 6f73 7369 626c 6520 7369 6465  of possible side
+0000d940: 2065 6666 6563 7473 3a0a 2020 2020 2020   effects:.      
+0000d950: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
+0000d960: 7562 2e63 6f6d 2f63 6572 7462 6f74 2f63  ub.com/certbot/c
+0000d970: 6572 7462 6f74 2f63 6f6d 6d69 742f 3531  ertbot/commit/51
+0000d980: 6564 3262 3638 3166 3837 6231 6562 3239  ed2b681f87b1eb29
+0000d990: 3038 3864 6434 3837 3138 6135 3466 3430  088dd48718a54f40
+0000d9a0: 3165 3438 3535 0a20 2020 2020 2020 2023  1e4855.        #
+0000d9b0: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+0000d9c0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+0000d9d0: 6e61 6c2e 636c 692e 706c 7567 696e 735f  nal.cli.plugins_
+0000d9e0: 7465 7374 6162 6c65 2729 2061 7320 706c  testable') as pl
+0000d9f0: 7567 696e 733a 0a20 2020 2020 2020 2023  ugins:.        #
+0000da00: 2020 2020 706c 7567 696e 732e 7265 7475      plugins.retu
+0000da10: 726e 5f76 616c 7565 203d 207b 2261 7061  rn_value = {"apa
+0000da20: 6368 6522 3a20 5472 7565 2c20 226e 6769  che": True, "ngi
+0000da30: 6e78 223a 2054 7275 657d 0a20 2020 2020  nx": True}.     
+0000da40: 2020 2023 2020 2020 7265 742c 205f 2c20     #    ret, _, 
+0000da50: 5f2c 205f 203d 2073 656c 662e 5f63 616c  _, _ = self._cal
+0000da60: 6c28 6172 6773 290a 2020 2020 2020 2020  l(args).        
+0000da70: 2320 2020 2073 656c 662e 6173 7365 7274  #    self.assert
+0000da80: 5472 7565 2822 546f 6f20 6d61 6e79 2066  True("Too many f
+0000da90: 6c61 6773 2073 6574 7469 6e67 2220 696e  lags setting" in
+0000daa0: 2072 6574 290a 0a20 2020 2020 2020 2061   ret)..        a
+0000dab0: 7267 7320 3d20 5b22 696e 7374 616c 6c22  rgs = ["install"
+0000dac0: 2c20 222d 2d6e 6769 6e78 222c 2022 2d2d  , "--nginx", "--
+0000dad0: 6365 7274 2d70 6174 6822 2c0a 2020 2020  cert-path",.    
+0000dae0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+0000daf0: 5f75 7469 6c2e 7465 6d70 5f6a 6f69 6e28  _util.temp_join(
+0000db00: 2762 6c61 6827 292c 2022 2d2d 6b65 792d  'blah'), "--key-
+0000db10: 7061 7468 222c 2074 6573 745f 7574 696c  path", test_util
+0000db20: 2e74 656d 705f 6a6f 696e 2827 626c 6168  .temp_join('blah
+0000db30: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000db40: 2020 2020 222d 2d6e 6769 6e78 2d73 6572      "--nginx-ser
+0000db50: 7665 722d 726f 6f74 222c 2022 2f6e 6f6e  ver-root", "/non
+0000db60: 6578 6973 7465 6e74 2f74 6869 6e67 222c  existent/thing",
+0000db70: 2022 2d64 222c 0a20 2020 2020 2020 2020   "-d",.         
+0000db80: 2020 2020 2020 2022 6578 616d 706c 652e         "example.
+0000db90: 636f 6d22 2c20 222d 2d64 6562 7567 225d  com", "--debug"]
+0000dba0: 0a20 2020 2020 2020 2069 6620 226e 6769  .        if "ngi
+0000dbb0: 6e78 2220 696e 2072 6561 6c5f 706c 7567  nx" in real_plug
+0000dbc0: 696e 733a 0a20 2020 2020 2020 2020 2020  ins:.           
+0000dbd0: 2023 2053 656e 6469 6e67 206e 6769 6e78   # Sending nginx
+0000dbe0: 2061 206e 6f6e 2d65 7869 7374 656e 7420   a non-existent 
+0000dbf0: 636f 6e66 2064 6972 2077 696c 6c20 7369  conf dir will si
+0000dc00: 6d75 6c61 7465 206d 6973 636f 6e66 6967  mulate misconfig
+0000dc10: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+0000dc20: 2020 2020 2320 2877 6520 6361 6e20 6f6e      # (we can on
+0000dc30: 6c79 2064 6f20 7468 6174 2069 6620 6365  ly do that if ce
+0000dc40: 7274 626f 742d 6e67 696e 7820 6973 2061  rtbot-nginx is a
+0000dc50: 6374 7561 6c6c 7920 7072 6573 656e 7429  ctually present)
+0000dc60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000dc70: 2c20 5f2c 205f 2c20 5f20 3d20 7365 6c66  , _, _, _ = self
+0000dc80: 2e5f 6361 6c6c 2861 7267 7329 0a20 2020  ._call(args).   
+0000dc90: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000dca0: 2254 6865 206e 6769 6e78 2070 6c75 6769  "The nginx plugi
+0000dcb0: 6e20 6973 206e 6f74 2077 6f72 6b69 6e67  n is not working
+0000dcc0: 2220 696e 2072 6574 0a20 2020 2020 2020  " in ret.       
+0000dcd0: 2020 2020 2061 7373 6572 7420 224d 6973       assert "Mis
+0000dce0: 636f 6e66 6967 7572 6174 696f 6e45 7272  configurationErr
+0000dcf0: 6f72 2220 696e 2072 6574 0a0a 2020 2020  or" in ret..    
+0000dd00: 2020 2020 7365 6c66 2e5f 636c 695f 6d69      self._cli_mi
+0000dd10: 7373 696e 675f 666c 6167 285b 222d 2d73  ssing_flag(["--s
+0000dd20: 7461 6e64 616c 6f6e 6522 5d2c 2022 5769  tandalone"], "Wi
+0000dd30: 7468 2074 6865 2073 7461 6e64 616c 6f6e  th the standalon
+0000dd40: 6520 706c 7567 696e 2c20 796f 7520 7072  e plugin, you pr
+0000dd50: 6f62 6162 6c79 2229 0a0a 2020 2020 2020  obably")..      
+0000dd60: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+0000dd70: 6828 2263 6572 7462 6f74 2e5f 696e 7465  h("certbot._inte
+0000dd80: 726e 616c 2e6d 6169 6e2e 5f69 6e69 745f  rnal.main._init_
+0000dd90: 6c65 5f63 6c69 656e 7422 2920 6173 206d  le_client") as m
+0000dda0: 6f63 6b5f 696e 6974 3a0a 2020 2020 2020  ock_init:.      
+0000ddb0: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
+0000ddc0: 7061 7463 6828 2263 6572 7462 6f74 2e5f  patch("certbot._
+0000ddd0: 696e 7465 726e 616c 2e6d 6169 6e2e 5f67  internal.main._g
+0000dde0: 6574 5f61 6e64 5f73 6176 655f 6365 7274  et_and_save_cert
+0000ddf0: 2229 2061 7320 6d6f 636b 5f67 7363 3a0a  ") as mock_gsc:.
+0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de10: 6d6f 636b 5f67 7363 2e72 6574 7572 6e5f  mock_gsc.return_
+0000de20: 7661 6c75 6520 3d20 6d6f 636b 2e4d 6167  value = mock.Mag
+0000de30: 6963 4d6f 636b 2829 0a20 2020 2020 2020  icMock().       
+0000de40: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0000de50: 616c 6c28 5b22 6365 7274 6f6e 6c79 222c  all(["certonly",
+0000de60: 2022 2d2d 6d61 6e75 616c 222c 2022 2d64   "--manual", "-d
+0000de70: 222c 2022 666f 6f2e 6261 7222 5d29 0a20  ", "foo.bar"]). 
+0000de80: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0000de90: 6e75 7365 645f 636f 6e66 6967 2c20 6175  nused_config, au
+0000dea0: 7468 2c20 756e 7573 6564 5f69 6e73 7461  th, unused_insta
+0000deb0: 6c6c 6572 203d 206d 6f63 6b5f 696e 6974  ller = mock_init
+0000dec0: 2e63 616c 6c5f 6172 6773 5b30 5d0a 2020  .call_args[0].  
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 6173                as
+0000dee0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+0000def0: 6175 7468 2c20 6d61 6e75 616c 2e41 7574  auth, manual.Aut
+0000df00: 6865 6e74 6963 6174 6f72 290a 0a20 2020  henticator)..   
+0000df10: 2020 2020 2077 6974 6820 6d6f 636b 2e70       with mock.p
+0000df20: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0000df30: 6e74 6572 6e61 6c2e 6d61 696e 2e63 6572  nternal.main.cer
+0000df40: 746f 6e6c 7927 2920 6173 206d 6f63 6b5f  tonly') as mock_
+0000df50: 6365 7274 6f6e 6c79 3a0a 2020 2020 2020  certonly:.      
+0000df60: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
+0000df70: 285b 2261 7574 6822 2c20 222d 2d73 7461  (["auth", "--sta
+0000df80: 6e64 616c 6f6e 6522 5d29 0a20 2020 2020  ndalone"]).     
+0000df90: 2020 2020 2020 2061 7373 6572 7420 3120         assert 1 
+0000dfa0: 3d3d 206d 6f63 6b5f 6365 7274 6f6e 6c79  == mock_certonly
+0000dfb0: 2e63 616c 6c5f 636f 756e 740a 0a20 2020  .call_count..   
+0000dfc0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000dfd0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0000dfe0: 6c6f 672e 706f 7374 5f61 7267 5f70 6172  log.post_arg_par
+0000dff0: 7365 5f73 6574 7570 2729 0a20 2020 2064  se_setup').    d
+0000e000: 6566 2074 6573 745f 726f 6c6c 6261 636b  ef test_rollback
+0000e010: 2873 656c 662c 205f 293a 0a20 2020 2020  (self, _):.     
+0000e020: 2020 205f 2c20 5f2c 205f 2c20 636c 6965     _, _, _, clie
+0000e030: 6e74 203d 2073 656c 662e 5f63 616c 6c28  nt = self._call(
+0000e040: 5b27 726f 6c6c 6261 636b 275d 290a 2020  ['rollback']).  
+0000e050: 2020 2020 2020 6173 7365 7274 2031 203d        assert 1 =
+0000e060: 3d20 636c 6965 6e74 2e72 6f6c 6c62 6163  = client.rollbac
+0000e070: 6b2e 6361 6c6c 5f63 6f75 6e74 0a0a 2020  k.call_count..  
+0000e080: 2020 2020 2020 5f2c 205f 2c20 5f2c 2063        _, _, _, c
+0000e090: 6c69 656e 7420 3d20 7365 6c66 2e5f 6361  lient = self._ca
+0000e0a0: 6c6c 285b 2772 6f6c 6c62 6163 6b27 2c20  ll(['rollback', 
+0000e0b0: 272d 2d63 6865 636b 706f 696e 7473 272c  '--checkpoints',
+0000e0c0: 2027 3132 3327 5d29 0a20 2020 2020 2020   '123']).       
+0000e0d0: 2063 6c69 656e 742e 726f 6c6c 6261 636b   client.rollback
+0000e0e0: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
+0000e0f0: 6e63 655f 7769 7468 280a 2020 2020 2020  nce_with(.      
+0000e100: 2020 2020 2020 6d6f 636b 2e41 4e59 2c20        mock.ANY, 
+0000e110: 3132 332c 206d 6f63 6b2e 414e 592c 206d  123, mock.ANY, m
+0000e120: 6f63 6b2e 414e 5929 0a0a 2020 2020 406d  ock.ANY)..    @m
+0000e130: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+0000e140: 6f74 2e5f 696e 7465 726e 616c 2e63 6572  ot._internal.cer
+0000e150: 745f 6d61 6e61 6765 722e 7570 6461 7465  t_manager.update
+0000e160: 5f6c 6976 655f 7379 6d6c 696e 6b73 2729  _live_symlinks')
+0000e170: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
+0000e180: 6461 7465 5f73 796d 6c69 6e6b 7328 7365  date_symlinks(se
+0000e190: 6c66 2c20 6d6f 636b 5f63 6572 745f 6d61  lf, mock_cert_ma
+0000e1a0: 6e61 6765 7229 3a0a 2020 2020 2020 2020  nager):.        
+0000e1b0: 7365 6c66 2e5f 6361 6c6c 5f6e 6f5f 636c  self._call_no_cl
+0000e1c0: 6965 6e74 6d6f 636b 285b 2775 7064 6174  ientmock(['updat
+0000e1d0: 655f 7379 6d6c 696e 6b73 275d 290a 2020  e_symlinks']).  
+0000e1e0: 2020 2020 2020 6173 7365 7274 2031 203d        assert 1 =
+0000e1f0: 3d20 6d6f 636b 5f63 6572 745f 6d61 6e61  = mock_cert_mana
+0000e200: 6765 722e 6361 6c6c 5f63 6f75 6e74 0a0a  ger.call_count..
+0000e210: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+0000e220: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000e230: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
+0000e240: 6365 7274 6966 6963 6174 6573 2729 0a20  certificates'). 
+0000e250: 2020 2064 6566 2074 6573 745f 6365 7274     def test_cert
+0000e260: 6966 6963 6174 6573 2873 656c 662c 206d  ificates(self, m
+0000e270: 6f63 6b5f 6365 7274 5f6d 616e 6167 6572  ock_cert_manager
+0000e280: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000e290: 5f63 616c 6c5f 6e6f 5f63 6c69 656e 746d  _call_no_clientm
+0000e2a0: 6f63 6b28 5b27 6365 7274 6966 6963 6174  ock(['certificat
+0000e2b0: 6573 275d 290a 2020 2020 2020 2020 6173  es']).        as
+0000e2c0: 7365 7274 2031 203d 3d20 6d6f 636b 5f63  sert 1 == mock_c
+0000e2d0: 6572 745f 6d61 6e61 6765 722e 6361 6c6c  ert_manager.call
+0000e2e0: 5f63 6f75 6e74 0a0a 2020 2020 406d 6f63  _count..    @moc
+0000e2f0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+0000e300: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
+0000e310: 6d61 6e61 6765 722e 6465 6c65 7465 2729  manager.delete')
+0000e320: 0a20 2020 2064 6566 2074 6573 745f 6465  .    def test_de
+0000e330: 6c65 7465 2873 656c 662c 206d 6f63 6b5f  lete(self, mock_
+0000e340: 6365 7274 5f6d 616e 6167 6572 293a 0a20  cert_manager):. 
+0000e350: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+0000e360: 6c5f 6e6f 5f63 6c69 656e 746d 6f63 6b28  l_no_clientmock(
+0000e370: 5b27 6465 6c65 7465 275d 290a 2020 2020  ['delete']).    
+0000e380: 2020 2020 6173 7365 7274 2031 203d 3d20      assert 1 == 
+0000e390: 6d6f 636b 5f63 6572 745f 6d61 6e61 6765  mock_cert_manage
+0000e3a0: 722e 6361 6c6c 5f63 6f75 6e74 0a0a 2020  r.call_count..  
+0000e3b0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+0000e3c0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+0000e3d0: 2e6d 6169 6e2e 706c 7567 696e 735f 6469  .main.plugins_di
+0000e3e0: 7363 6f27 290a 2020 2020 406d 6f63 6b2e  sco').    @mock.
+0000e3f0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0000e400: 696e 7465 726e 616c 2e6d 6169 6e2e 636c  internal.main.cl
+0000e410: 692e 4865 6c70 6675 6c41 7267 756d 656e  i.HelpfulArgumen
+0000e420: 7450 6172 7365 722e 6465 7465 726d 696e  tParser.determin
+0000e430: 655f 6865 6c70 5f74 6f70 6963 7327 290a  e_help_topics').
+0000e440: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+0000e450: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000e460: 616c 2e6c 6f67 2e70 6f73 745f 6172 675f  al.log.post_arg_
+0000e470: 7061 7273 655f 7365 7475 7027 290a 2020  parse_setup').  
+0000e480: 2020 6465 6620 7465 7374 5f70 6c75 6769    def test_plugi
+0000e490: 6e73 2873 656c 662c 205f 2c20 5f64 6574  ns(self, _, _det
+0000e4a0: 2c20 6d6f 636b 5f64 6973 636f 293a 0a20  , mock_disco):. 
+0000e4b0: 2020 2020 2020 2066 6c61 6773 203d 205b         flags = [
+0000e4c0: 272d 2d69 6e69 7427 2c20 272d 2d70 7265  '--init', '--pre
+0000e4d0: 7061 7265 272c 2027 2d2d 6175 7468 656e  pare', '--authen
+0000e4e0: 7469 6361 746f 7273 272c 2027 2d2d 696e  ticators', '--in
+0000e4f0: 7374 616c 6c65 7273 275d 0a20 2020 2020  stallers'].     
+0000e500: 2020 2066 6f72 2061 7267 7320 696e 2069     for args in i
+0000e510: 7465 7274 6f6f 6c73 2e63 6861 696e 280a  tertools.chain(.
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2a28 6974 6572 746f 6f6c 732e 636f 6d62  *(itertools.comb
+0000e540: 696e 6174 696f 6e73 2866 6c61 6773 2c20  inations(flags, 
+0000e550: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0000e560: 2020 2020 2066 6f72 2072 2069 6e20 7261       for r in ra
+0000e570: 6e67 6528 6c65 6e28 666c 6167 7329 2929  nge(len(flags)))
+0000e580: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000e590: 656c 662e 5f63 616c 6c28 5b27 706c 7567  elf._call(['plug
+0000e5a0: 696e 7327 5d20 2b20 6c69 7374 2861 7267  ins'] + list(arg
+0000e5b0: 7329 290a 0a20 2020 2040 6d6f 636b 2e70  s))..    @mock.p
+0000e5c0: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0000e5d0: 6e74 6572 6e61 6c2e 6d61 696e 2e70 6c75  nternal.main.plu
+0000e5e0: 6769 6e73 5f64 6973 636f 2729 0a20 2020  gins_disco').   
+0000e5f0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+0000e600: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0000e610: 6d61 696e 2e63 6c69 2e48 656c 7066 756c  main.cli.Helpful
+0000e620: 4172 6775 6d65 6e74 5061 7273 6572 2e64  ArgumentParser.d
+0000e630: 6574 6572 6d69 6e65 5f68 656c 705f 746f  etermine_help_to
+0000e640: 7069 6373 2729 0a20 2020 2064 6566 2074  pics').    def t
+0000e650: 6573 745f 706c 7567 696e 735f 6e6f 5f61  est_plugins_no_a
+0000e660: 7267 7328 7365 6c66 2c20 5f64 6574 2c20  rgs(self, _det, 
+0000e670: 6d6f 636b 5f64 6973 636f 293a 0a20 2020  mock_disco):.   
+0000e680: 2020 2020 2069 6661 6365 733a 204c 6973       ifaces: Lis
+0000e690: 745b 696e 7465 7266 6163 6573 2e50 6c75  t[interfaces.Plu
+0000e6a0: 6769 6e5d 203d 205b 5d0a 2020 2020 2020  gin] = [].      
+0000e6b0: 2020 706c 7567 696e 7320 3d20 6d6f 636b    plugins = mock
+0000e6c0: 5f64 6973 636f 2e50 6c75 6769 6e73 5265  _disco.PluginsRe
+0000e6d0: 6769 7374 7279 2e66 696e 645f 616c 6c28  gistry.find_all(
+0000e6e0: 290a 0a20 2020 2020 2020 2073 7464 6f75  )..        stdou
+0000e6f0: 7420 3d20 696f 2e53 7472 696e 6749 4f28  t = io.StringIO(
+0000e700: 290a 2020 2020 2020 2020 7769 7468 2074  ).        with t
+0000e710: 6573 745f 7574 696c 2e70 6174 6368 5f64  est_util.patch_d
+0000e720: 6973 706c 6179 5f75 7469 6c5f 7769 7468  isplay_util_with
+0000e730: 5f73 7464 6f75 7428 7374 646f 7574 3d73  _stdout(stdout=s
+0000e740: 7464 6f75 7429 3a0a 2020 2020 2020 2020  tdout):.        
+0000e750: 2020 2020 5f2c 2073 7464 6f75 742c 205f      _, stdout, _
+0000e760: 2c20 5f20 3d20 7365 6c66 2e5f 6361 6c6c  , _ = self._call
+0000e770: 285b 2770 6c75 6769 6e73 275d 2c20 7374  (['plugins'], st
+0000e780: 646f 7574 290a 0a20 2020 2020 2020 2070  dout)..        p
+0000e790: 6c75 6769 6e73 2e76 6973 6962 6c65 2e61  lugins.visible.a
+0000e7a0: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
+0000e7b0: 655f 7769 7468 2829 0a20 2020 2020 2020  e_with().       
+0000e7c0: 2070 6c75 6769 6e73 2e76 6973 6962 6c65   plugins.visible
+0000e7d0: 2829 2e69 6661 6365 732e 6173 7365 7274  ().ifaces.assert
+0000e7e0: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+0000e7f0: 6828 6966 6163 6573 290a 2020 2020 2020  h(ifaces).      
+0000e800: 2020 6669 6c74 6572 6564 203d 2070 6c75    filtered = plu
+0000e810: 6769 6e73 2e76 6973 6962 6c65 2829 2e69  gins.visible().i
+0000e820: 6661 6365 7328 290a 2020 2020 2020 2020  faces().        
+0000e830: 6173 7365 7274 2073 7464 6f75 742e 6765  assert stdout.ge
+0000e840: 7476 616c 7565 2829 2e73 7472 6970 2829  tvalue().strip()
+0000e850: 203d 3d20 7374 7228 6669 6c74 6572 6564   == str(filtered
+0000e860: 290a 0a20 2020 2040 6d6f 636b 2e70 6174  )..    @mock.pat
+0000e870: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0000e880: 6572 6e61 6c2e 6d61 696e 2e70 6c75 6769  ernal.main.plugi
+0000e890: 6e73 5f64 6973 636f 2729 0a20 2020 2040  ns_disco').    @
+0000e8a0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+0000e8b0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0000e8c0: 696e 2e63 6c69 2e48 656c 7066 756c 4172  in.cli.HelpfulAr
+0000e8d0: 6775 6d65 6e74 5061 7273 6572 2e64 6574  gumentParser.det
+0000e8e0: 6572 6d69 6e65 5f68 656c 705f 746f 7069  ermine_help_topi
+0000e8f0: 6373 2729 0a20 2020 2064 6566 2074 6573  cs').    def tes
+0000e900: 745f 706c 7567 696e 735f 6e6f 5f61 7267  t_plugins_no_arg
+0000e910: 735f 756e 7072 6976 696c 6567 6564 2873  s_unprivileged(s
+0000e920: 656c 662c 205f 6465 742c 206d 6f63 6b5f  elf, _det, mock_
+0000e930: 6469 7363 6f29 3a0a 2020 2020 2020 2020  disco):.        
+0000e940: 6966 6163 6573 3a20 4c69 7374 5b69 6e74  ifaces: List[int
+0000e950: 6572 6661 6365 732e 506c 7567 696e 5d20  erfaces.Plugin] 
+0000e960: 3d20 5b5d 0a20 2020 2020 2020 2070 6c75  = [].        plu
+0000e970: 6769 6e73 203d 206d 6f63 6b5f 6469 7363  gins = mock_disc
+0000e980: 6f2e 506c 7567 696e 7352 6567 6973 7472  o.PluginsRegistr
+0000e990: 792e 6669 6e64 5f61 6c6c 2829 0a0a 2020  y.find_all()..  
+0000e9a0: 2020 2020 2020 6465 6620 7468 726f 775f        def throw_
+0000e9b0: 6572 726f 7228 6469 7265 6374 6f72 792c  error(directory,
+0000e9c0: 206d 6f64 652c 2073 7472 6963 7429 3a0a   mode, strict):.
+0000e9d0: 2020 2020 2020 2020 2020 2020 2222 2252              """R
+0000e9e0: 6169 7365 7320 6572 726f 722e 4572 726f  aises error.Erro
+0000e9f0: 722e 2222 220a 2020 2020 2020 2020 2020  r.""".          
+0000ea00: 2020 5f2c 205f 2c20 5f20 3d20 6469 7265    _, _, _ = dire
+0000ea10: 6374 6f72 792c 206d 6f64 652c 2073 7472  ctory, mode, str
+0000ea20: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+0000ea30: 7261 6973 6520 6572 726f 7273 2e45 7272  raise errors.Err
+0000ea40: 6f72 2829 0a0a 2020 2020 2020 2020 7374  or()..        st
+0000ea50: 646f 7574 203d 2069 6f2e 5374 7269 6e67  dout = io.String
+0000ea60: 494f 2829 0a20 2020 2020 2020 2077 6974  IO().        wit
+0000ea70: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
+0000ea80: 7274 626f 742e 7574 696c 2e73 6574 5f75  rtbot.util.set_u
+0000ea90: 705f 636f 7265 5f64 6972 2729 2061 7320  p_core_dir') as 
+0000eaa0: 6d6f 636b 5f73 6574 5f75 705f 636f 7265  mock_set_up_core
+0000eab0: 5f64 6972 3a0a 2020 2020 2020 2020 2020  _dir:.          
+0000eac0: 2020 7769 7468 2074 6573 745f 7574 696c    with test_util
+0000ead0: 2e70 6174 6368 5f64 6973 706c 6179 5f75  .patch_display_u
+0000eae0: 7469 6c5f 7769 7468 5f73 7464 6f75 7428  til_with_stdout(
+0000eaf0: 7374 646f 7574 3d73 7464 6f75 7429 3a0a  stdout=stdout):.
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 6d6f 636b 5f73 6574 5f75 705f 636f 7265  mock_set_up_core
+0000eb20: 5f64 6972 2e73 6964 655f 6566 6665 6374  _dir.side_effect
+0000eb30: 203d 2074 6872 6f77 5f65 7272 6f72 0a20   = throw_error. 
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0000eb50: 2c20 7374 646f 7574 2c20 5f2c 205f 203d  , stdout, _, _ =
+0000eb60: 2073 656c 662e 5f63 616c 6c28 5b27 706c   self._call(['pl
+0000eb70: 7567 696e 7327 5d2c 2073 7464 6f75 7429  ugins'], stdout)
+0000eb80: 0a0a 2020 2020 2020 2020 706c 7567 696e  ..        plugin
+0000eb90: 732e 7669 7369 626c 652e 6173 7365 7274  s.visible.assert
+0000eba0: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+0000ebb0: 6828 290a 2020 2020 2020 2020 706c 7567  h().        plug
+0000ebc0: 696e 732e 7669 7369 626c 6528 292e 6966  ins.visible().if
+0000ebd0: 6163 6573 2e61 7373 6572 745f 6361 6c6c  aces.assert_call
+0000ebe0: 6564 5f6f 6e63 655f 7769 7468 2869 6661  ed_once_with(ifa
+0000ebf0: 6365 7329 0a20 2020 2020 2020 2066 696c  ces).        fil
+0000ec00: 7465 7265 6420 3d20 706c 7567 696e 732e  tered = plugins.
+0000ec10: 7669 7369 626c 6528 292e 6966 6163 6573  visible().ifaces
+0000ec20: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
+0000ec30: 7420 7374 646f 7574 2e67 6574 7661 6c75  t stdout.getvalu
+0000ec40: 6528 292e 7374 7269 7028 2920 3d3d 2073  e().strip() == s
+0000ec50: 7472 2866 696c 7465 7265 6429 0a0a 2020  tr(filtered)..  
+0000ec60: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+0000ec70: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+0000ec80: 2e6d 6169 6e2e 706c 7567 696e 735f 6469  .main.plugins_di
+0000ec90: 7363 6f27 290a 2020 2020 406d 6f63 6b2e  sco').    @mock.
+0000eca0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0000ecb0: 696e 7465 726e 616c 2e6d 6169 6e2e 636c  internal.main.cl
+0000ecc0: 692e 4865 6c70 6675 6c41 7267 756d 656e  i.HelpfulArgumen
+0000ecd0: 7450 6172 7365 722e 6465 7465 726d 696e  tParser.determin
+0000ece0: 655f 6865 6c70 5f74 6f70 6963 7327 290a  e_help_topics').
+0000ecf0: 2020 2020 6465 6620 7465 7374 5f70 6c75      def test_plu
+0000ed00: 6769 6e73 5f69 6e69 7428 7365 6c66 2c20  gins_init(self, 
+0000ed10: 5f64 6574 2c20 6d6f 636b 5f64 6973 636f  _det, mock_disco
+0000ed20: 293a 0a20 2020 2020 2020 2069 6661 6365  ):.        iface
+0000ed30: 733a 204c 6973 745b 696e 7465 7266 6163  s: List[interfac
+0000ed40: 6573 2e50 6c75 6769 6e5d 203d 205b 5d0a  es.Plugin] = [].
+0000ed50: 2020 2020 2020 2020 706c 7567 696e 7320          plugins 
+0000ed60: 3d20 6d6f 636b 5f64 6973 636f 2e50 6c75  = mock_disco.Plu
+0000ed70: 6769 6e73 5265 6769 7374 7279 2e66 696e  ginsRegistry.fin
+0000ed80: 645f 616c 6c28 290a 0a20 2020 2020 2020  d_all()..       
+0000ed90: 2073 7464 6f75 7420 3d20 696f 2e53 7472   stdout = io.Str
+0000eda0: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
+0000edb0: 7769 7468 2074 6573 745f 7574 696c 2e70  with test_util.p
+0000edc0: 6174 6368 5f64 6973 706c 6179 5f75 7469  atch_display_uti
+0000edd0: 6c5f 7769 7468 5f73 7464 6f75 7428 7374  l_with_stdout(st
+0000ede0: 646f 7574 3d73 7464 6f75 7429 3a0a 2020  dout=stdout):.  
+0000edf0: 2020 2020 2020 2020 2020 5f2c 2073 7464            _, std
+0000ee00: 6f75 742c 205f 2c20 5f20 3d20 7365 6c66  out, _, _ = self
+0000ee10: 2e5f 6361 6c6c 285b 2770 6c75 6769 6e73  ._call(['plugins
+0000ee20: 272c 2027 2d2d 696e 6974 275d 2c20 7374  ', '--init'], st
+0000ee30: 646f 7574 290a 0a20 2020 2020 2020 2070  dout)..        p
+0000ee40: 6c75 6769 6e73 2e76 6973 6962 6c65 2e61  lugins.visible.a
+0000ee50: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
+0000ee60: 655f 7769 7468 2829 0a20 2020 2020 2020  e_with().       
+0000ee70: 2070 6c75 6769 6e73 2e76 6973 6962 6c65   plugins.visible
+0000ee80: 2829 2e69 6661 6365 732e 6173 7365 7274  ().ifaces.assert
+0000ee90: 5f63 616c 6c65 645f 6f6e 6365 5f77 6974  _called_once_wit
+0000eea0: 6828 6966 6163 6573 290a 2020 2020 2020  h(ifaces).      
+0000eeb0: 2020 6669 6c74 6572 6564 203d 2070 6c75    filtered = plu
+0000eec0: 6769 6e73 2e76 6973 6962 6c65 2829 2e69  gins.visible().i
+0000eed0: 6661 6365 7328 290a 2020 2020 2020 2020  faces().        
+0000eee0: 6173 7365 7274 2066 696c 7465 7265 642e  assert filtered.
+0000eef0: 696e 6974 2e63 616c 6c5f 636f 756e 7420  init.call_count 
+0000ef00: 3d3d 2031 0a20 2020 2020 2020 2061 7373  == 1.        ass
+0000ef10: 6572 7420 7374 646f 7574 2e67 6574 7661  ert stdout.getva
+0000ef20: 6c75 6528 292e 7374 7269 7028 2920 3d3d  lue().strip() ==
+0000ef30: 2073 7472 2866 696c 7465 7265 6429 0a0a   str(filtered)..
+0000ef40: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+0000ef50: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000ef60: 616c 2e6d 6169 6e2e 706c 7567 696e 735f  al.main.plugins_
+0000ef70: 6469 7363 6f27 290a 2020 2020 406d 6f63  disco').    @moc
+0000ef80: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+0000ef90: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
+0000efa0: 636c 692e 4865 6c70 6675 6c41 7267 756d  cli.HelpfulArgum
+0000efb0: 656e 7450 6172 7365 722e 6465 7465 726d  entParser.determ
+0000efc0: 696e 655f 6865 6c70 5f74 6f70 6963 7327  ine_help_topics'
+0000efd0: 290a 2020 2020 6465 6620 7465 7374 5f70  ).    def test_p
+0000efe0: 6c75 6769 6e73 5f70 7265 7061 7265 2873  lugins_prepare(s
+0000eff0: 656c 662c 205f 6465 742c 206d 6f63 6b5f  elf, _det, mock_
+0000f000: 6469 7363 6f29 3a0a 2020 2020 2020 2020  disco):.        
+0000f010: 6966 6163 6573 3a20 4c69 7374 5b69 6e74  ifaces: List[int
+0000f020: 6572 6661 6365 732e 506c 7567 696e 5d20  erfaces.Plugin] 
+0000f030: 3d20 5b5d 0a20 2020 2020 2020 2070 6c75  = [].        plu
+0000f040: 6769 6e73 203d 206d 6f63 6b5f 6469 7363  gins = mock_disc
+0000f050: 6f2e 506c 7567 696e 7352 6567 6973 7472  o.PluginsRegistr
+0000f060: 792e 6669 6e64 5f61 6c6c 2829 0a0a 2020  y.find_all()..  
+0000f070: 2020 2020 2020 7374 646f 7574 203d 2069        stdout = i
+0000f080: 6f2e 5374 7269 6e67 494f 2829 0a20 2020  o.StringIO().   
+0000f090: 2020 2020 2077 6974 6820 7465 7374 5f75       with test_u
+0000f0a0: 7469 6c2e 7061 7463 685f 6469 7370 6c61  til.patch_displa
+0000f0b0: 795f 7574 696c 5f77 6974 685f 7374 646f  y_util_with_stdo
+0000f0c0: 7574 2873 7464 6f75 743d 7374 646f 7574  ut(stdout=stdout
+0000f0d0: 293a 0a20 2020 2020 2020 2020 2020 205f  ):.            _
+0000f0e0: 2c20 7374 646f 7574 2c20 5f2c 205f 203d  , stdout, _, _ =
+0000f0f0: 2073 656c 662e 5f63 616c 6c28 5b27 706c   self._call(['pl
+0000f100: 7567 696e 7327 2c20 272d 2d69 6e69 7427  ugins', '--init'
+0000f110: 2c20 272d 2d70 7265 7061 7265 275d 2c20  , '--prepare'], 
+0000f120: 7374 646f 7574 290a 0a20 2020 2020 2020  stdout)..       
+0000f130: 2070 6c75 6769 6e73 2e76 6973 6962 6c65   plugins.visible
+0000f140: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
+0000f150: 6e63 655f 7769 7468 2829 0a20 2020 2020  nce_with().     
+0000f160: 2020 2070 6c75 6769 6e73 2e76 6973 6962     plugins.visib
+0000f170: 6c65 2829 2e69 6661 6365 732e 6173 7365  le().ifaces.asse
+0000f180: 7274 5f63 616c 6c65 645f 6f6e 6365 5f77  rt_called_once_w
+0000f190: 6974 6828 6966 6163 6573 290a 2020 2020  ith(ifaces).    
+0000f1a0: 2020 2020 6669 6c74 6572 6564 203d 2070      filtered = p
+0000f1b0: 6c75 6769 6e73 2e76 6973 6962 6c65 2829  lugins.visible()
+0000f1c0: 2e69 6661 6365 7328 290a 2020 2020 2020  .ifaces().      
+0000f1d0: 2020 6173 7365 7274 2066 696c 7465 7265    assert filtere
+0000f1e0: 642e 696e 6974 2e63 616c 6c5f 636f 756e  d.init.call_coun
+0000f1f0: 7420 3d3d 2031 0a20 2020 2020 2020 2066  t == 1.        f
+0000f200: 696c 7465 7265 642e 7072 6570 6172 652e  iltered.prepare.
+0000f210: 6173 7365 7274 5f63 616c 6c65 645f 6f6e  assert_called_on
+0000f220: 6365 5f77 6974 6828 290a 2020 2020 2020  ce_with().      
+0000f230: 2020 6669 6c74 6572 6564 2e61 7661 696c    filtered.avail
+0000f240: 6162 6c65 2e61 7373 6572 745f 6361 6c6c  able.assert_call
+0000f250: 6564 5f6f 6e63 655f 7769 7468 2829 0a20  ed_once_with(). 
+0000f260: 2020 2020 2020 2061 7661 696c 6162 6c65         available
+0000f270: 203d 2066 696c 7465 7265 642e 6176 6169   = filtered.avai
+0000f280: 6c61 626c 6528 290a 2020 2020 2020 2020  lable().        
+0000f290: 6173 7365 7274 2073 7464 6f75 742e 6765  assert stdout.ge
+0000f2a0: 7476 616c 7565 2829 2e73 7472 6970 2829  tvalue().strip()
+0000f2b0: 203d 3d20 7374 7228 6176 6169 6c61 626c   == str(availabl
+0000f2c0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
+0000f2d0: 5f63 6572 746f 6e6c 795f 6162 7370 6174  _certonly_abspat
+0000f2e0: 6828 7365 6c66 293a 0a20 2020 2020 2020  h(self):.       
+0000f2f0: 2063 6572 7420 3d20 2763 6572 7427 0a20   cert = 'cert'. 
+0000f300: 2020 2020 2020 206b 6579 203d 2027 6b65         key = 'ke
+0000f310: 7927 0a20 2020 2020 2020 2063 6861 696e  y'.        chain
+0000f320: 203d 2027 6368 6169 6e27 0a20 2020 2020   = 'chain'.     
+0000f330: 2020 2066 756c 6c63 6861 696e 203d 2027     fullchain = '
+0000f340: 6675 6c6c 6368 6169 6e27 0a0a 2020 2020  fullchain'..    
+0000f350: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
+0000f360: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+0000f370: 7465 726e 616c 2e6d 6169 6e2e 6365 7274  ternal.main.cert
+0000f380: 6f6e 6c79 2729 2061 7320 6d6f 636b 5f63  only') as mock_c
+0000f390: 6572 746f 6e6c 793a 0a20 2020 2020 2020  ertonly:.       
+0000f3a0: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
+0000f3b0: 5b27 6365 7274 6f6e 6c79 272c 2027 2d2d  ['certonly', '--
+0000f3c0: 6365 7274 2d70 6174 6827 2c20 6365 7274  cert-path', cert
+0000f3d0: 2c20 272d 2d6b 6579 2d70 6174 6827 2c20  , '--key-path', 
+0000f3e0: 276b 6579 272c 0a20 2020 2020 2020 2020  'key',.         
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000f400: 2d2d 6368 6169 6e2d 7061 7468 272c 2027  --chain-path', '
+0000f410: 6368 6169 6e27 2c0a 2020 2020 2020 2020  chain',.        
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f430: 272d 2d66 756c 6c63 6861 696e 2d70 6174  '--fullchain-pat
+0000f440: 6827 2c20 2766 756c 6c63 6861 696e 275d  h', 'fullchain']
+0000f450: 290a 0a20 2020 2020 2020 2063 6f6e 6669  )..        confi
+0000f460: 672c 2075 6e75 7365 645f 706c 7567 696e  g, unused_plugin
+0000f470: 7320 3d20 6d6f 636b 5f63 6572 746f 6e6c  s = mock_certonl
+0000f480: 792e 6361 6c6c 5f61 7267 735b 305d 0a20  y.call_args[0]. 
+0000f490: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
+0000f4a0: 6e66 6967 2e63 6572 745f 7061 7468 203d  nfig.cert_path =
+0000f4b0: 3d20 6f73 2e70 6174 682e 6162 7370 6174  = os.path.abspat
+0000f4c0: 6828 6365 7274 290a 2020 2020 2020 2020  h(cert).        
+0000f4d0: 6173 7365 7274 2063 6f6e 6669 672e 6b65  assert config.ke
+0000f4e0: 795f 7061 7468 203d 3d20 6f73 2e70 6174  y_path == os.pat
+0000f4f0: 682e 6162 7370 6174 6828 6b65 7929 0a20  h.abspath(key). 
+0000f500: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
+0000f510: 6e66 6967 2e63 6861 696e 5f70 6174 6820  nfig.chain_path 
+0000f520: 3d3d 206f 732e 7061 7468 2e61 6273 7061  == os.path.abspa
+0000f530: 7468 2863 6861 696e 290a 2020 2020 2020  th(chain).      
+0000f540: 2020 6173 7365 7274 2063 6f6e 6669 672e    assert config.
+0000f550: 6675 6c6c 6368 6169 6e5f 7061 7468 203d  fullchain_path =
+0000f560: 3d20 6f73 2e70 6174 682e 6162 7370 6174  = os.path.abspat
+0000f570: 6828 6675 6c6c 6368 6169 6e29 0a0a 2020  h(fullchain)..  
+0000f580: 2020 6465 6620 7465 7374 5f63 6572 746f    def test_certo
+0000f590: 6e6c 795f 6261 645f 6172 6773 2873 656c  nly_bad_args(sel
+0000f5a0: 6629 3a0a 2020 2020 2020 2020 7472 793a  f):.        try:
+0000f5b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f5c0: 662e 5f63 616c 6c28 5b27 2d61 272c 2027  f._call(['-a', '
+0000f5d0: 6261 645f 6175 7468 272c 2027 6365 7274  bad_auth', 'cert
+0000f5e0: 6f6e 6c79 275d 290a 2020 2020 2020 2020  only']).        
+0000f5f0: 2020 2020 6173 7365 7274 2046 616c 7365      assert False
+0000f600: 2c20 2245 7863 6570 7469 6f6e 2073 686f  , "Exception sho
+0000f610: 756c 6420 6861 7665 2062 6565 6e20 7261  uld have been ra
+0000f620: 6973 6564 220a 2020 2020 2020 2020 6578  ised".        ex
+0000f630: 6365 7074 2065 7272 6f72 732e 506c 7567  cept errors.Plug
+0000f640: 696e 5365 6c65 6374 696f 6e45 7272 6f72  inSelectionError
+0000f650: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0000f660: 2020 2061 7373 6572 7420 2754 6865 2072     assert 'The r
+0000f670: 6571 7565 7374 6564 2062 6164 5f61 7574  equested bad_aut
+0000f680: 6820 706c 7567 696e 2064 6f65 7320 6e6f  h plugin does no
+0000f690: 7420 6170 7065 6172 2720 696e 2073 7472  t appear' in str
+0000f6a0: 2865 290a 0a20 2020 2064 6566 2074 6573  (e)..    def tes
+0000f6b0: 745f 6368 6563 6b5f 636f 6e66 6967 5f73  t_check_config_s
+0000f6c0: 616e 6974 795f 646f 6d61 696e 2873 656c  anity_domain(sel
+0000f6d0: 6629 3a0a 2020 2020 2020 2020 2320 4651  f):.        # FQ
+0000f6e0: 444e 0a20 2020 2020 2020 2077 6974 6820  DN.        with 
+0000f6f0: 7079 7465 7374 2e72 6169 7365 7328 6572  pytest.raises(er
+0000f700: 726f 7273 2e43 6f6e 6669 6775 7261 7469  rors.Configurati
+0000f710: 6f6e 4572 726f 7229 3a0a 2020 2020 2020  onError):.      
+0000f720: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
+0000f730: 285b 272d 6427 2c20 2761 2720 2a20 3634  (['-d', 'a' * 64
+0000f740: 5d29 0a20 2020 2020 2020 2023 2046 5144  ]).        # FQD
+0000f750: 4e20 320a 2020 2020 2020 2020 7769 7468  N 2.        with
+0000f760: 2070 7974 6573 742e 7261 6973 6573 2865   pytest.raises(e
+0000f770: 7272 6f72 732e 436f 6e66 6967 7572 6174  rrors.Configurat
+0000f780: 696f 6e45 7272 6f72 293a 0a20 2020 2020  ionError):.     
+0000f790: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+0000f7a0: 6c28 5b27 2d64 272c 2028 2827 6127 202a  l(['-d', (('a' *
+0000f7b0: 2035 3029 202b 2027 2e27 2920 2a20 3130   50) + '.') * 10
+0000f7c0: 5d29 0a20 2020 2020 2020 2023 2042 6172  ]).        # Bar
+0000f7d0: 6520 4950 2061 6464 7265 7373 2028 7468  e IP address (th
+0000f7e0: 6973 2069 7320 6163 7475 616c 6c79 2061  is is actually a
+0000f7f0: 2064 6966 6665 7265 6e74 2065 7272 6f72   different error
+0000f800: 206d 6573 7361 6765 206e 6f77 290a 2020   message now).  
+0000f810: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+0000f820: 742e 7261 6973 6573 2865 7272 6f72 732e  t.raises(errors.
+0000f830: 436f 6e66 6967 7572 6174 696f 6e45 7272  ConfigurationErr
+0000f840: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0000f850: 2073 656c 662e 5f63 616c 6c28 5b27 2d64   self._call(['-d
+0000f860: 272c 2027 3230 342e 3131 2e32 3331 2e33  ', '204.11.231.3
+0000f870: 3527 5d29 0a20 2020 2020 2020 2023 2042  5']).        # B
+0000f880: 6172 6520 4950 7636 2061 6464 7265 7373  are IPv6 address
+0000f890: 0a20 2020 2020 2020 2077 6974 6820 7079  .        with py
+0000f8a0: 7465 7374 2e72 6169 7365 7328 6572 726f  test.raises(erro
+0000f8b0: 7273 2e43 6f6e 6669 6775 7261 7469 6f6e  rs.Configuration
+0000f8c0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0000f8d0: 2020 2020 7365 6c66 2e5f 6361 6c6c 285b      self._call([
+0000f8e0: 272d 6427 2c20 2732 3030 313a 6462 383a  '-d', '2001:db8:
+0000f8f0: 6163 3639 3a33 6666 3a62 3163 623a 6338  ac69:3ff:b1cb:c8
+0000f900: 6336 3a35 6138 343a 6133 3162 275d 290a  c6:5a84:a31b']).
+0000f910: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
+0000f920: 725f 7769 7468 5f62 6573 7465 6666 6f72  r_with_besteffor
+0000f930: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000f940: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+0000f950: 7365 7328 6572 726f 7273 2e45 7272 6f72  ses(errors.Error
+0000f960: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000f970: 656c 662e 5f63 616c 6c28 2763 6572 746f  elf._call('certo
+0000f980: 6e6c 7920 2d2d 6373 7220 7b30 7d20 2d2d  nly --csr {0} --
+0000f990: 616c 6c6f 772d 7375 6273 6574 2d6f 662d  allow-subset-of-
+0000f9a0: 6e61 6d65 7327 2e66 6f72 6d61 7428 4353  names'.format(CS
+0000f9b0: 5229 2e73 706c 6974 2829 290a 0a20 2020  R).split())..   
+0000f9c0: 2064 6566 2074 6573 745f 7275 6e5f 7769   def test_run_wi
+0000f9d0: 7468 5f63 7372 2873 656c 6629 3a0a 2020  th_csr(self):.  
+0000f9e0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
+0000f9f0: 616e 2065 7272 6f72 2062 6563 6175 7365  an error because
+0000fa00: 2079 6f75 2063 616e 206f 6e6c 7920 7573   you can only us
+0000fa10: 6520 2d2d 6373 7220 7769 7468 2063 6572  e --csr with cer
+0000fa20: 746f 6e6c 790a 2020 2020 2020 2020 7472  tonly.        tr
+0000fa30: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+0000fa40: 656c 662e 5f63 616c 6c28 5b27 2d2d 6373  elf._call(['--cs
+0000fa50: 7227 2c20 4353 525d 290a 2020 2020 2020  r', CSR]).      
+0000fa60: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
+0000fa70: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+0000fa80: 2020 2020 2020 2020 6173 7365 7274 2022          assert "
+0000fa90: 506c 6561 7365 2074 7279 2074 6865 2063  Please try the c
+0000faa0: 6572 746f 6e6c 7922 2069 6e20 7265 7072  ertonly" in repr
+0000fab0: 2865 290a 2020 2020 2020 2020 2020 2020  (e).            
+0000fac0: 7265 7475 726e 0a20 2020 2020 2020 2061  return.        a
+0000fad0: 7373 6572 7420 4661 6c73 652c 2022 4578  ssert False, "Ex
+0000fae0: 7065 6374 6564 2073 7570 706c 7969 6e67  pected supplying
+0000faf0: 202d 2d63 7372 2074 6f20 6661 696c 2077   --csr to fail w
+0000fb00: 6974 6820 6465 6661 756c 7420 7665 7262  ith default verb
+0000fb10: 220a 0a20 2020 2064 6566 2074 6573 745f  "..    def test_
+0000fb20: 6373 725f 7769 7468 5f6e 6f5f 646f 6d61  csr_with_no_doma
+0000fb30: 696e 7328 7365 6c66 293a 0a20 2020 2020  ins(self):.     
+0000fb40: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+0000fb50: 6169 7365 7328 6572 726f 7273 2e45 7272  aises(errors.Err
+0000fb60: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0000fb70: 2073 656c 662e 5f63 616c 6c28 2763 6572   self._call('cer
+0000fb80: 746f 6e6c 7920 2d2d 6373 7220 7b30 7d27  tonly --csr {0}'
+0000fb90: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+0000fba0: 2020 2020 2020 2020 2074 6573 745f 7574           test_ut
+0000fbb0: 696c 2e76 6563 746f 725f 7061 7468 2827  il.vector_path('
+0000fbc0: 6373 722d 6e6f 6e61 6d65 735f 3531 322e  csr-nonames_512.
+0000fbd0: 7065 6d27 2929 2e73 706c 6974 2829 290a  pem')).split()).
+0000fbe0: 0a20 2020 2064 6566 2074 6573 745f 6373  .    def test_cs
+0000fbf0: 725f 7769 7468 5f69 6e63 6f6e 7369 7374  r_with_inconsist
+0000fc00: 656e 745f 646f 6d61 696e 7328 7365 6c66  ent_domains(self
+0000fc10: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+0000fc20: 7079 7465 7374 2e72 6169 7365 7328 6572  pytest.raises(er
+0000fc30: 726f 7273 2e45 7272 6f72 293a 0a20 2020  rors.Error):.   
+0000fc40: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0000fc50: 616c 6c28 2763 6572 746f 6e6c 7920 2d64  all('certonly -d
+0000fc60: 2065 7861 6d70 6c65 2e6f 7267 202d 2d63   example.org --c
+0000fc70: 7372 207b 307d 272e 666f 726d 6174 2843  sr {0}'.format(C
+0000fc80: 5352 292e 7370 6c69 7428 2929 0a0a 2020  SR).split())..  
+0000fc90: 2020 6465 6620 5f63 6572 746f 6e6c 795f    def _certonly_
+0000fca0: 6e65 775f 7265 7175 6573 745f 636f 6d6d  new_request_comm
+0000fcb0: 6f6e 2873 656c 662c 206d 6f63 6b5f 636c  on(self, mock_cl
+0000fcc0: 6965 6e74 2c20 6172 6773 3d4e 6f6e 6529  ient, args=None)
+0000fcd0: 3a0a 2020 2020 2020 2020 7769 7468 206d  :.        with m
+0000fce0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+0000fcf0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+0000fd00: 6e2e 5f66 696e 645f 6c69 6e65 6167 655f  n._find_lineage_
+0000fd10: 666f 725f 646f 6d61 696e 735f 616e 645f  for_domains_and_
+0000fd20: 6365 7274 6e61 6d65 2729 205c 0a20 2020  certname') \.   
+0000fd30: 2020 2020 2020 2020 2061 7320 6d6f 636b           as mock
+0000fd40: 5f72 656e 6577 616c 3a0a 2020 2020 2020  _renewal:.      
+0000fd50: 2020 2020 2020 6d6f 636b 5f72 656e 6577        mock_renew
+0000fd60: 616c 2e72 6574 7572 6e5f 7661 6c75 6520  al.return_value 
+0000fd70: 3d20 2822 6e65 7763 6572 7422 2c20 4e6f  = ("newcert", No
+0000fd80: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+0000fd90: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
+0000fda0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0000fdb0: 616c 2e6d 6169 6e2e 5f69 6e69 745f 6c65  al.main._init_le
+0000fdc0: 5f63 6c69 656e 7427 2920 6173 206d 6f63  _client') as moc
+0000fdd0: 6b5f 696e 6974 3a0a 2020 2020 2020 2020  k_init:.        
+0000fde0: 2020 2020 2020 2020 6d6f 636b 5f69 6e69          mock_ini
+0000fdf0: 742e 7265 7475 726e 5f76 616c 7565 203d  t.return_value =
+0000fe00: 206d 6f63 6b5f 636c 6965 6e74 0a20 2020   mock_client.   
+0000fe10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000fe20: 6172 6773 2069 7320 4e6f 6e65 3a0a 2020  args is None:.  
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe40: 2020 6172 6773 203d 205b 5d0a 2020 2020    args = [].    
+0000fe50: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0000fe60: 202b 3d20 272d 6420 666f 6f2e 6261 7220   += '-d foo.bar 
+0000fe70: 2d61 2073 7461 6e64 616c 6f6e 6520 6365  -a standalone ce
+0000fe80: 7274 6f6e 6c79 272e 7370 6c69 7428 290a  rtonly'.split().
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 7365 6c66 2e5f 6361 6c6c 2861 7267 7329  self._call(args)
+0000feb0: 0a0a 2020 2020 406d 6f63 6b2e 7061 7463  ..    @mock.patc
+0000fec0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+0000fed0: 726e 616c 2e6d 6169 6e2e 5f72 6570 6f72  rnal.main._repor
+0000fee0: 745f 6e65 775f 6365 7274 2729 0a20 2020  t_new_cert').   
+0000fef0: 2064 6566 2074 6573 745f 6365 7274 6f6e   def test_certon
+0000ff00: 6c79 5f64 7279 5f72 756e 5f6e 6577 5f72  ly_dry_run_new_r
+0000ff10: 6571 7565 7374 5f73 7563 6365 7373 2873  equest_success(s
+0000ff20: 656c 662c 206d 6f63 6b5f 7265 706f 7274  elf, mock_report
+0000ff30: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
+0000ff40: 636c 6965 6e74 203d 206d 6f63 6b2e 4d61  client = mock.Ma
+0000ff50: 6769 634d 6f63 6b28 290a 2020 2020 2020  gicMock().      
+0000ff60: 2020 6d6f 636b 5f63 6c69 656e 742e 6f62    mock_client.ob
+0000ff70: 7461 696e 5f61 6e64 5f65 6e72 6f6c 6c5f  tain_and_enroll_
+0000ff80: 6365 7274 6966 6963 6174 652e 7265 7475  certificate.retu
+0000ff90: 726e 5f76 616c 7565 203d 204e 6f6e 650a  rn_value = None.
+0000ffa0: 2020 2020 2020 2020 7365 6c66 2e5f 6365          self._ce
+0000ffb0: 7274 6f6e 6c79 5f6e 6577 5f72 6571 7565  rtonly_new_reque
+0000ffc0: 7374 5f63 6f6d 6d6f 6e28 6d6f 636b 5f63  st_common(mock_c
+0000ffd0: 6c69 656e 742c 205b 272d 2d64 7279 2d72  lient, ['--dry-r
+0000ffe0: 756e 275d 290a 2020 2020 2020 2020 6173  un']).        as
+0000fff0: 7365 7274 206d 6f63 6b5f 636c 6965 6e74  sert mock_client
+00010000: 2e6f 6274 6169 6e5f 616e 645f 656e 726f  .obtain_and_enro
+00010010: 6c6c 5f63 6572 7469 6669 6361 7465 2e63  ll_certificate.c
+00010020: 616c 6c5f 636f 756e 7420 3d3d 2031 0a20  all_count == 1. 
+00010030: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
+00010040: 636b 5f72 6570 6f72 742e 6361 6c6c 5f63  ck_report.call_c
+00010050: 6f75 6e74 203d 3d20 310a 2020 2020 2020  ount == 1.      
+00010060: 2020 6173 7365 7274 206d 6f63 6b5f 7265    assert mock_re
+00010070: 706f 7274 2e63 616c 6c5f 6172 6773 5b30  port.call_args[0
+00010080: 5d5b 305d 2e64 7279 5f72 756e 2069 7320  ][0].dry_run is 
+00010090: 5472 7565 0a0a 2020 2020 406d 6f63 6b2e  True..    @mock.
+000100a0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+000100b0: 696e 7465 726e 616c 2e6d 6169 6e2e 5f72  internal.main._r
+000100c0: 6570 6f72 745f 6e65 775f 6365 7274 2729  eport_new_cert')
+000100d0: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+000100e0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+000100f0: 6e61 6c2e 6d61 696e 2e75 7469 6c2e 6174  nal.main.util.at
+00010100: 6578 6974 5f72 6567 6973 7465 7227 290a  exit_register').
+00010110: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+00010120: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00010130: 616c 2e65 6666 2e68 616e 646c 655f 7375  al.eff.handle_su
+00010140: 6273 6372 6970 7469 6f6e 2729 0a20 2020  bscription').   
+00010150: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+00010160: 7274 626f 742e 6372 7970 746f 5f75 7469  rtbot.crypto_uti
+00010170: 6c2e 6e6f 7441 6674 6572 2729 0a20 2020  l.notAfter').   
+00010180: 2064 6566 2074 6573 745f 6365 7274 6f6e   def test_certon
+00010190: 6c79 5f6e 6577 5f72 6571 7565 7374 5f73  ly_new_request_s
+000101a0: 7563 6365 7373 2873 656c 662c 206d 6f63  uccess(self, moc
+000101b0: 6b5f 6e6f 7441 6674 6572 2c0a 2020 2020  k_notAfter,.    
+000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101e0: 2020 2020 2020 6d6f 636b 5f73 7562 7363        mock_subsc
+000101f0: 7269 7074 696f 6e2c 206d 6f63 6b5f 7265  ription, mock_re
+00010200: 6769 7374 6572 2c20 6d6f 636b 5f72 6570  gister, mock_rep
+00010210: 6f72 7429 3a0a 2020 2020 2020 2020 6365  ort):.        ce
+00010220: 7274 5f70 6174 6820 3d20 6f73 2e70 6174  rt_path = os.pat
+00010230: 682e 6e6f 726d 7061 7468 286f 732e 7061  h.normpath(os.pa
+00010240: 7468 2e6a 6f69 6e28 7365 6c66 2e63 6f6e  th.join(self.con
+00010250: 6669 672e 636f 6e66 6967 5f64 6972 2c20  fig.config_dir, 
+00010260: 276c 6976 652f 666f 6f2e 6261 7227 2929  'live/foo.bar'))
+00010270: 0a20 2020 2020 2020 206b 6579 5f70 6174  .        key_pat
+00010280: 6820 3d20 6f73 2e70 6174 682e 6e6f 726d  h = os.path.norm
+00010290: 7061 7468 286f 732e 7061 7468 2e6a 6f69  path(os.path.joi
+000102a0: 6e28 7365 6c66 2e63 6f6e 6669 672e 636f  n(self.config.co
+000102b0: 6e66 6967 5f64 6972 2c20 276c 6976 652f  nfig_dir, 'live/
+000102c0: 6261 7a2e 7175 7827 2929 0a20 2020 2020  baz.qux')).     
+000102d0: 2020 2064 6174 6520 3d20 2731 3937 302d     date = '1970-
+000102e0: 3031 2d30 3127 0a20 2020 2020 2020 206d  01-01'.        m
+000102f0: 6f63 6b5f 6e6f 7441 6674 6572 2829 2e64  ock_notAfter().d
+00010300: 6174 652e 7265 7475 726e 5f76 616c 7565  ate.return_value
+00010310: 203d 2064 6174 650a 0a20 2020 2020 2020   = date..       
+00010320: 206d 6f63 6b5f 6c69 6e65 6167 6520 3d20   mock_lineage = 
+00010330: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2863  mock.MagicMock(c
+00010340: 6572 743d 6365 7274 5f70 6174 682c 2066  ert=cert_path, f
+00010350: 756c 6c63 6861 696e 3d63 6572 745f 7061  ullchain=cert_pa
+00010360: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010380: 2020 2020 2020 2020 2020 6675 6c6c 6368            fullch
+00010390: 6169 6e5f 7061 7468 3d63 6572 745f 7061  ain_path=cert_pa
+000103a0: 7468 2c20 6b65 795f 7061 7468 3d6b 6579  th, key_path=key
+000103b0: 5f70 6174 6829 0a20 2020 2020 2020 206d  _path).        m
+000103c0: 6f63 6b5f 636c 6965 6e74 203d 206d 6f63  ock_client = moc
+000103d0: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
+000103e0: 2020 2020 2020 6d6f 636b 5f63 6c69 656e        mock_clien
+000103f0: 742e 6f62 7461 696e 5f61 6e64 5f65 6e72  t.obtain_and_enr
+00010400: 6f6c 6c5f 6365 7274 6966 6963 6174 652e  oll_certificate.
+00010410: 7265 7475 726e 5f76 616c 7565 203d 206d  return_value = m
+00010420: 6f63 6b5f 6c69 6e65 6167 650a 2020 2020  ock_lineage.    
+00010430: 2020 2020 7365 6c66 2e5f 6365 7274 6f6e      self._certon
+00010440: 6c79 5f6e 6577 5f72 6571 7565 7374 5f63  ly_new_request_c
+00010450: 6f6d 6d6f 6e28 6d6f 636b 5f63 6c69 656e  ommon(mock_clien
+00010460: 7429 0a20 2020 2020 2020 2061 7373 6572  t).        asser
+00010470: 7420 6d6f 636b 5f63 6c69 656e 742e 6f62  t mock_client.ob
+00010480: 7461 696e 5f61 6e64 5f65 6e72 6f6c 6c5f  tain_and_enroll_
+00010490: 6365 7274 6966 6963 6174 652e 6361 6c6c  certificate.call
+000104a0: 5f63 6f75 6e74 203d 3d20 310a 2020 2020  _count == 1.    
+000104b0: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
+000104c0: 7265 706f 7274 2e63 616c 6c5f 636f 756e  report.call_coun
+000104d0: 7420 3d3d 2031 0a20 2020 2020 2020 2061  t == 1.        a
+000104e0: 7373 6572 7420 6365 7274 5f70 6174 6820  ssert cert_path 
+000104f0: 696e 206d 6f63 6b5f 7265 706f 7274 2e63  in mock_report.c
+00010500: 616c 6c5f 6172 6773 5b30 5d5b 325d 0a20  all_args[0][2]. 
+00010510: 2020 2020 2020 2061 7373 6572 7420 6b65         assert ke
+00010520: 795f 7061 7468 2069 6e20 6d6f 636b 5f72  y_path in mock_r
+00010530: 6570 6f72 742e 6361 6c6c 5f61 7267 735b  eport.call_args[
+00010540: 305d 5b33 5d0a 2020 2020 2020 2020 6173  0][3].        as
+00010550: 7365 7274 2027 646f 6e61 7465 2720 696e  sert 'donate' in
+00010560: 206d 6f63 6b5f 7265 6769 7374 6572 2e63   mock_register.c
+00010570: 616c 6c5f 6172 6773 5b30 5d5b 315d 0a20  all_args[0][1]. 
+00010580: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
+00010590: 636b 5f73 7562 7363 7269 7074 696f 6e2e  ck_subscription.
+000105a0: 6361 6c6c 6564 2069 7320 5472 7565 0a0a  called is True..
+000105b0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+000105c0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+000105d0: 616c 2e65 6666 2e68 616e 646c 655f 7375  al.eff.handle_su
+000105e0: 6273 6372 6970 7469 6f6e 2729 0a20 2020  bscription').   
+000105f0: 2064 6566 2074 6573 745f 6365 7274 6f6e   def test_certon
+00010600: 6c79 5f6e 6577 5f72 6571 7565 7374 5f66  ly_new_request_f
+00010610: 6169 6c75 7265 2873 656c 662c 206d 6f63  ailure(self, moc
+00010620: 6b5f 7375 6273 6372 6970 7469 6f6e 293a  k_subscription):
+00010630: 0a20 2020 2020 2020 206d 6f63 6b5f 636c  .        mock_cl
+00010640: 6965 6e74 203d 206d 6f63 6b2e 4d61 6769  ient = mock.Magi
+00010650: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
+00010660: 6d6f 636b 5f63 6c69 656e 742e 6f62 7461  mock_client.obta
+00010670: 696e 5f61 6e64 5f65 6e72 6f6c 6c5f 6365  in_and_enroll_ce
+00010680: 7274 6966 6963 6174 652e 7265 7475 726e  rtificate.return
+00010690: 5f76 616c 7565 203d 2046 616c 7365 0a20  _value = False. 
+000106a0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+000106b0: 7374 2e72 6169 7365 7328 6572 726f 7273  st.raises(errors
+000106c0: 2e45 7272 6f72 293a 0a20 2020 2020 2020  .Error):.       
+000106d0: 2020 2020 2073 656c 662e 5f63 6572 746f       self._certo
+000106e0: 6e6c 795f 6e65 775f 7265 7175 6573 745f  nly_new_request_
+000106f0: 636f 6d6d 6f6e 286d 6f63 6b5f 636c 6965  common(mock_clie
+00010700: 6e74 290a 2020 2020 2020 2020 6173 7365  nt).        asse
+00010710: 7274 206d 6f63 6b5f 7375 6273 6372 6970  rt mock_subscrip
+00010720: 7469 6f6e 2e63 616c 6c65 6420 6973 2046  tion.called is F
+00010730: 616c 7365 0a0a 2020 2020 6465 6620 5f74  alse..    def _t
+00010740: 6573 745f 7265 6e65 7761 6c5f 636f 6d6d  est_renewal_comm
+00010750: 6f6e 2873 656c 662c 2064 7565 5f66 6f72  on(self, due_for
+00010760: 5f72 656e 6577 616c 2c20 6578 7472 615f  _renewal, extra_
+00010770: 6172 6773 2c20 6c6f 675f 6f75 743d 4e6f  args, log_out=No
+00010780: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
 00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 2022 556e 6578 7065 6374         "Unexpect
-000107c0: 6564 2072 656e 6577 616c 2065 7272 6f72  ed renewal error
-000107d0: 3a5c 6e22 202b 0a20 2020 2020 2020 2020  :\n" +.         
+000107a0: 2061 7267 733d 4e6f 6e65 2c20 7368 6f75   args=None, shou
+000107b0: 6c64 5f72 656e 6577 3d54 7275 652c 2065  ld_renew=True, e
+000107c0: 7272 6f72 5f65 7870 6563 7465 643d 4661  rror_expected=Fa
+000107d0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
 000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 2074 7261 6365 6261 636b 2e66 6f72     traceback.for
-00010810: 6d61 745f 6578 6328 2929 0a0a 2020 2020  mat_exc())..    
-00010820: 2020 2020 2020 2020 6966 2073 686f 756c          if shoul
-00010830: 645f 7265 6e65 773a 0a20 2020 2020 2020  d_renew:.       
-00010840: 2020 2020 2020 2020 2069 6620 7265 7573           if reus
-00010850: 655f 6b65 7920 616e 6420 6e6f 7420 6e65  e_key and not ne
-00010860: 775f 6b65 793a 0a20 2020 2020 2020 2020  w_key:.         
-00010870: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-00010880: 206c 6f63 6174 696f 6e20 6f66 2074 6865   location of the
-00010890: 2070 7265 7669 6f75 7320 6c69 7665 2070   previous live p
-000108a0: 7269 766b 6579 2e70 656d 2069 7320 7061  rivkey.pem is pa
-000108b0: 7373 6564 0a20 2020 2020 2020 2020 2020  ssed.           
-000108c0: 2020 2020 2020 2020 2023 2074 6f20 6f62           # to ob
-000108d0: 7461 696e 5f63 6572 7469 6669 6361 7465  tain_certificate
-000108e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108f0: 2020 2020 206d 6f63 6b5f 636c 6965 6e74       mock_client
-00010900: 2e6f 6274 6169 6e5f 6365 7274 6966 6963  .obtain_certific
-00010910: 6174 652e 6173 7365 7274 5f63 616c 6c65  ate.assert_calle
-00010920: 645f 6f6e 6365 5f77 6974 6828 5b6d 6f63  d_once_with([moc
-00010930: 6b2e 414e 595d 2c0a 2020 2020 2020 2020  k.ANY],.        
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 6f73 2e70 6174 682e 6e6f 726d 7061 7468  os.path.normpath
-00010960: 286f 732e 7061 7468 2e6a 6f69 6e28 0a20  (os.path.join(. 
-00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010990: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
-000109a0: 722c 2022 6c69 7665 2f73 616d 706c 652d  r, "live/sample-
-000109b0: 7265 6e65 7761 6c2f 7072 6976 6b65 792e  renewal/privkey.
-000109c0: 7065 6d22 2929 290a 2020 2020 2020 2020  pem"))).        
-000109d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 6d6f 636b 5f63 6c69 656e 742e 6f62    mock_client.ob
-00010a00: 7461 696e 5f63 6572 7469 6669 6361 7465  tain_certificate
-00010a10: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
-00010a20: 6e63 655f 7769 7468 285b 6d6f 636b 2e41  nce_with([mock.A
-00010a30: 4e59 5d2c 204e 6f6e 6529 0a20 2020 2020  NY], None).     
-00010a40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00010a50: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00010a60: 6572 7420 6d6f 636b 5f63 6c69 656e 742e  ert mock_client.
-00010a70: 6f62 7461 696e 5f63 6572 7469 6669 6361  obtain_certifica
-00010a80: 7465 2e63 616c 6c5f 636f 756e 7420 3d3d  te.call_count ==
-00010a90: 2030 0a20 2020 2020 2020 2065 7863 6570   0.        excep
-00010aa0: 743a 0a20 2020 2020 2020 2020 2020 2073  t:.            s
-00010ab0: 656c 662e 5f64 756d 705f 6c6f 6728 290a  elf._dump_log().
-00010ac0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00010ad0: 650a 2020 2020 2020 2020 6669 6e61 6c6c  e.        finall
-00010ae0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-00010af0: 6620 6c6f 675f 6f75 743a 0a20 2020 2020  f log_out:.     
-00010b00: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00010b10: 6f70 656e 286f 732e 7061 7468 2e6a 6f69  open(os.path.joi
-00010b20: 6e28 7365 6c66 2e63 6f6e 6669 672e 6c6f  n(self.config.lo
-00010b30: 6773 5f64 6972 2c20 226c 6574 7365 6e63  gs_dir, "letsenc
-00010b40: 7279 7074 2e6c 6f67 2229 2920 6173 206c  rypt.log")) as l
-00010b50: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-00010b60: 2020 2020 2020 2061 7373 6572 7420 6c6f         assert lo
-00010b70: 675f 6f75 7420 696e 206c 662e 7265 6164  g_out in lf.read
-00010b80: 2829 0a0a 2020 2020 2020 2020 7265 7475  ()..        retu
-00010b90: 726e 206d 6f63 6b5f 6c69 6e65 6167 652c  rn mock_lineage,
-00010ba0: 206d 6f63 6b5f 6469 7370 6c61 792c 2073   mock_display, s
-00010bb0: 7464 6f75 740a 0a20 2020 2040 6d6f 636b  tdout..    @mock
-00010bc0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-00010bd0: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e5f  _internal.main._
-00010be0: 7265 706f 7274 5f6e 6577 5f63 6572 7427  report_new_cert'
-00010bf0: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-00010c00: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00010c10: 726e 616c 2e6d 6169 6e2e 7574 696c 2e61  rnal.main.util.a
-00010c20: 7465 7869 745f 7265 6769 7374 6572 2729  texit_register')
-00010c30: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-00010c40: 2827 6365 7274 626f 742e 6372 7970 746f  ('certbot.crypto
-00010c50: 5f75 7469 6c2e 6e6f 7441 6674 6572 2729  _util.notAfter')
-00010c60: 0a20 2020 2064 6566 2074 6573 745f 6365  .    def test_ce
-00010c70: 7274 6f6e 6c79 5f72 656e 6577 616c 2873  rtonly_renewal(s
-00010c80: 656c 662c 205f 2c20 6d6f 636b 5f72 6567  elf, _, mock_reg
-00010c90: 6973 7465 722c 206d 6f63 6b5f 7265 706f  ister, mock_repo
-00010ca0: 7274 293a 0a20 2020 2020 2020 206c 696e  rt):.        lin
-00010cb0: 6561 6765 2c20 5f2c 205f 203d 2073 656c  eage, _, _ = sel
-00010cc0: 662e 5f74 6573 745f 7265 6e65 7761 6c5f  f._test_renewal_
-00010cd0: 636f 6d6d 6f6e 2854 7275 652c 205b 5d29  common(True, [])
-00010ce0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010cf0: 6c69 6e65 6167 652e 7361 7665 5f73 7563  lineage.save_suc
-00010d00: 6365 7373 6f72 2e63 616c 6c5f 636f 756e  cessor.call_coun
-00010d10: 7420 3d3d 2031 0a20 2020 2020 2020 206c  t == 1.        l
-00010d20: 696e 6561 6765 2e75 7064 6174 655f 616c  ineage.update_al
-00010d30: 6c5f 6c69 6e6b 735f 746f 2e61 7373 6572  l_links_to.asser
-00010d40: 745f 6361 6c6c 6564 5f6f 6e63 655f 7769  t_called_once_wi
-00010d50: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
-00010d60: 6c69 6e65 6167 652e 6c61 7465 7374 5f63  lineage.latest_c
-00010d70: 6f6d 6d6f 6e5f 7665 7273 696f 6e28 2929  ommon_version())
-00010d80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010d90: 6d6f 636b 5f72 6570 6f72 742e 6361 6c6c  mock_report.call
-00010da0: 5f63 6f75 6e74 203d 3d20 310a 2020 2020  _count == 1.    
-00010db0: 2020 2020 6173 7365 7274 2027 6675 6c6c      assert 'full
-00010dc0: 6368 6169 6e2e 7065 6d27 2069 6e20 6d6f  chain.pem' in mo
-00010dd0: 636b 5f72 6570 6f72 742e 6361 6c6c 5f61  ck_report.call_a
-00010de0: 7267 735b 305d 5b32 5d0a 2020 2020 2020  rgs[0][2].      
-00010df0: 2020 6173 7365 7274 2027 646f 6e61 7465    assert 'donate
-00010e00: 2720 696e 206d 6f63 6b5f 7265 6769 7374  ' in mock_regist
-00010e10: 6572 2e63 616c 6c5f 6172 6773 5b30 5d5b  er.call_args[0][
-00010e20: 315d 0a0a 2020 2020 406d 6f63 6b2e 7061  1]..    @mock.pa
-00010e30: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-00010e40: 7465 726e 616c 2e6d 6169 6e2e 6469 7370  ternal.main.disp
-00010e50: 6c61 795f 7574 696c 2e6e 6f74 6966 7927  lay_util.notify'
-00010e60: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-00010e70: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00010e80: 726e 616c 2e6c 6f67 2e6c 6f67 6769 6e67  rnal.log.logging
-00010e90: 2e68 616e 646c 6572 732e 526f 7461 7469  .handlers.Rotati
-00010ea0: 6e67 4669 6c65 4861 6e64 6c65 722e 646f  ngFileHandler.do
-00010eb0: 526f 6c6c 6f76 6572 2729 0a20 2020 2040  Rollover').    @
-00010ec0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00010ed0: 626f 742e 6372 7970 746f 5f75 7469 6c2e  bot.crypto_util.
-00010ee0: 6e6f 7441 6674 6572 2729 0a20 2020 2064  notAfter').    d
-00010ef0: 6566 2074 6573 745f 6365 7274 6f6e 6c79  ef test_certonly
-00010f00: 5f72 656e 6577 616c 5f74 7269 6767 6572  _renewal_trigger
-00010f10: 7328 7365 6c66 2c20 5f2c 205f 5f2c 206d  s(self, _, __, m
-00010f20: 6f63 6b5f 6e6f 7469 6679 293a 0a20 2020  ock_notify):.   
-00010f30: 2020 2020 2023 202d 2d64 7279 2d72 756e       # --dry-run
-00010f40: 2073 686f 756c 6420 666f 7263 6520 7265   should force re
-00010f50: 6e65 7761 6c0a 2020 2020 2020 2020 5f2c  newal.        _,
-00010f60: 205f 2c20 5f20 3d20 7365 6c66 2e5f 7465   _, _ = self._te
-00010f70: 7374 5f72 656e 6577 616c 5f63 6f6d 6d6f  st_renewal_commo
-00010f80: 6e28 4661 6c73 652c 205b 272d 2d64 7279  n(False, ['--dry
-00010f90: 2d72 756e 272c 2027 2d2d 6b65 6570 275d  -run', '--keep']
-00010fa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fd0: 2020 2020 2020 2020 6c6f 675f 6f75 743d          log_out=
-00010fe0: 2273 696d 756c 6174 696e 6720 7265 6e65  "simulating rene
-00010ff0: 7761 6c22 290a 2020 2020 2020 2020 6d6f  wal").        mo
-00011000: 636b 5f6e 6f74 6966 792e 6173 7365 7274  ck_notify.assert
-00011010: 5f61 6e79 5f63 616c 6c28 2754 6865 2064  _any_call('The d
-00011020: 7279 2072 756e 2077 6173 2073 7563 6365  ry run was succe
-00011030: 7373 6675 6c2e 2729 0a0a 2020 2020 2020  ssful.')..      
-00011040: 2020 7365 6c66 2e5f 7465 7374 5f72 656e    self._test_ren
-00011050: 6577 616c 5f63 6f6d 6d6f 6e28 4661 6c73  ewal_common(Fals
-00011060: 652c 205b 272d 2d72 656e 6577 2d62 792d  e, ['--renew-by-
-00011070: 6465 6661 756c 7427 2c20 272d 7476 7627  default', '-tvv'
-00011080: 2c20 272d 2d64 6562 7567 275d 2c0a 2020  , '--debug'],.  
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 6c6f 675f 6f75 743d 2241 7574 6f2d 7265  log_out="Auto-re
-000110c0: 6e65 7761 6c20 666f 7263 6564 2229 0a0a  newal forced")..
-000110d0: 2020 2020 2020 2020 5f2c 206d 6f63 6b5f          _, mock_
-000110e0: 6469 7370 6c61 7965 722c 205f 203d 2073  displayer, _ = s
-000110f0: 656c 662e 5f74 6573 745f 7265 6e65 7761  elf._test_renewa
-00011100: 6c5f 636f 6d6d 6f6e 2846 616c 7365 2c20  l_common(False, 
-00011110: 5b27 2d74 7676 272c 2027 2d2d 6465 6275  ['-tvv', '--debu
-00011120: 6727 2c20 272d 2d6b 6565 7027 5d2c 0a20  g', '--keep'],. 
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107f0: 2020 7175 6965 745f 6d6f 6465 3d46 616c    quiet_mode=Fal
+00010800: 7365 2c20 6578 7069 7279 5f64 6174 653d  se, expiry_date=
+00010810: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00010820: 652e 6e6f 7728 292c 0a20 2020 2020 2020  e.now(),.       
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 2020 2020 7265 7573 655f 6b65 793d        reuse_key=
+00010850: 4661 6c73 652c 206e 6577 5f6b 6579 3d46  False, new_key=F
+00010860: 616c 7365 293a 0a20 2020 2020 2020 2063  alse):.        c
+00010870: 6572 745f 7061 7468 203d 2074 6573 745f  ert_path = test_
+00010880: 7574 696c 2e76 6563 746f 725f 7061 7468  util.vector_path
+00010890: 2827 6365 7274 5f35 3132 2e70 656d 2729  ('cert_512.pem')
+000108a0: 0a20 2020 2020 2020 2063 6861 696e 5f70  .        chain_p
+000108b0: 6174 6820 3d20 6f73 2e70 6174 682e 6e6f  ath = os.path.no
+000108c0: 726d 7061 7468 286f 732e 7061 7468 2e6a  rmpath(os.path.j
+000108d0: 6f69 6e28 7365 6c66 2e63 6f6e 6669 672e  oin(self.config.
+000108e0: 636f 6e66 6967 5f64 6972 2c0a 2020 2020  config_dir,.    
+000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010910: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00010920: 6c69 7665 2f66 6f6f 2e62 6172 2f66 756c  live/foo.bar/ful
+00010930: 6c63 6861 696e 2e70 656d 2729 290a 2020  lchain.pem')).  
+00010940: 2020 2020 2020 6d6f 636b 5f6c 696e 6561        mock_linea
+00010950: 6765 203d 206d 6f63 6b2e 4d61 6769 634d  ge = mock.MagicM
+00010960: 6f63 6b28 6365 7274 3d63 6572 745f 7061  ock(cert=cert_pa
+00010970: 7468 2c20 6675 6c6c 6368 6169 6e3d 6368  th, fullchain=ch
+00010980: 6169 6e5f 7061 7468 2c0a 2020 2020 2020  ain_path,.      
+00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 6365 7274 5f70 6174 683d 6365 7274 5f70  cert_path=cert_p
+000109c0: 6174 682c 2066 756c 6c63 6861 696e 5f70  ath, fullchain_p
+000109d0: 6174 683d 6368 6169 6e5f 7061 7468 290a  ath=chain_path).
+000109e0: 2020 2020 2020 2020 6d6f 636b 5f6c 696e          mock_lin
+000109f0: 6561 6765 2e73 686f 756c 645f 6175 746f  eage.should_auto
+00010a00: 7265 6e65 772e 7265 7475 726e 5f76 616c  renew.return_val
+00010a10: 7565 203d 2064 7565 5f66 6f72 5f72 656e  ue = due_for_ren
+00010a20: 6577 616c 0a20 2020 2020 2020 206d 6f63  ewal.        moc
+00010a30: 6b5f 6c69 6e65 6167 652e 6861 735f 7065  k_lineage.has_pe
+00010a40: 6e64 696e 675f 6465 706c 6f79 6d65 6e74  nding_deployment
+00010a50: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00010a60: 4661 6c73 650a 2020 2020 2020 2020 6d6f  False.        mo
+00010a70: 636b 5f6c 696e 6561 6765 2e6e 616d 6573  ck_lineage.names
+00010a80: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00010a90: 5b27 6973 6e6f 742e 6f72 6727 5d0a 2020  ['isnot.org'].  
+00010aa0: 2020 2020 2020 6d6f 636b 5f6c 696e 6561        mock_linea
+00010ab0: 6765 2e70 7269 7661 7465 5f6b 6579 5f74  ge.private_key_t
+00010ac0: 7970 6520 3d20 2765 6364 7361 270a 2020  ype = 'ecdsa'.  
+00010ad0: 2020 2020 2020 6d6f 636b 5f6c 696e 6561        mock_linea
+00010ae0: 6765 2e65 6c6c 6970 7469 635f 6375 7276  ge.elliptic_curv
+00010af0: 6520 3d20 2773 6563 7032 3536 7231 270a  e = 'secp256r1'.
+00010b00: 2020 2020 2020 2020 6d6f 636b 5f6c 696e          mock_lin
+00010b10: 6561 6765 2e72 6575 7365 5f6b 6579 203d  eage.reuse_key =
+00010b20: 2072 6575 7365 5f6b 6579 0a20 2020 2020   reuse_key.     
+00010b30: 2020 206d 6f63 6b5f 6365 7274 7220 3d20     mock_certr = 
+00010b40: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
+00010b50: 0a20 2020 2020 2020 206d 6f63 6b5f 6b65  .        mock_ke
+00010b60: 7920 3d20 6d6f 636b 2e4d 6167 6963 4d6f  y = mock.MagicMo
+00010b70: 636b 2870 656d 3d27 7065 6d5f 6b65 7927  ck(pem='pem_key'
+00010b80: 290a 2020 2020 2020 2020 6d6f 636b 5f63  ).        mock_c
+00010b90: 6c69 656e 7420 3d20 6d6f 636b 2e4d 6167  lient = mock.Mag
+00010ba0: 6963 4d6f 636b 2829 0a20 2020 2020 2020  icMock().       
+00010bb0: 2073 7464 6f75 7420 3d20 696f 2e53 7472   stdout = io.Str
+00010bc0: 696e 6749 4f28 290a 2020 2020 2020 2020  ingIO().        
+00010bd0: 6d6f 636b 5f63 6c69 656e 742e 6f62 7461  mock_client.obta
+00010be0: 696e 5f63 6572 7469 6669 6361 7465 2e72  in_certificate.r
+00010bf0: 6574 7572 6e5f 7661 6c75 6520 3d20 286d  eturn_value = (m
+00010c00: 6f63 6b5f 6365 7274 722c 2027 6368 6169  ock_certr, 'chai
+00010c10: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
+00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c40: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
+00010c50: 6b65 792c 2027 6373 7227 290a 0a20 2020  key, 'csr')..   
+00010c60: 2020 2020 2064 6566 2077 7269 7465 5f6d       def write_m
+00010c70: 7367 286d 6573 7361 6765 2c20 2a61 7267  sg(message, *arg
+00010c80: 732c 202a 2a6b 7761 7267 7329 3a20 2023  s, **kwargs):  #
+00010c90: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+00010ca0: 3d75 6e75 7365 642d 6172 6775 6d65 6e74  =unused-argument
+00010cb0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+00010cc0: 5772 6974 6520 6d65 7373 6167 6520 746f  Write message to
+00010cd0: 2073 7464 6f75 742e 2222 220a 2020 2020   stdout.""".    
+00010ce0: 2020 2020 2020 2020 7374 646f 7574 2e77          stdout.w
+00010cf0: 7269 7465 286d 6573 7361 6765 290a 0a20  rite(message).. 
+00010d00: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010d10: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
+00010d20: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00010d30: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
+00010d40: 6d61 6e61 6765 722e 6669 6e64 5f64 7570  manager.find_dup
+00010d50: 6c69 6361 7469 7665 5f63 6572 7473 2729  licative_certs')
+00010d60: 2061 7320 6d6f 636b 5f66 6463 3a0a 2020   as mock_fdc:.  
+00010d70: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00010d80: 636b 5f66 6463 2e72 6574 7572 6e5f 7661  ck_fdc.return_va
+00010d90: 6c75 6520 3d20 286d 6f63 6b5f 6c69 6e65  lue = (mock_line
+00010da0: 6167 652c 204e 6f6e 6529 0a20 2020 2020  age, None).     
+00010db0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00010dc0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+00010dd0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+00010de0: 696e 2e5f 696e 6974 5f6c 655f 636c 6965  in._init_le_clie
+00010df0: 6e74 2729 2061 7320 6d6f 636b 5f69 6e69  nt') as mock_ini
+00010e00: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00010e10: 2020 2020 2020 206d 6f63 6b5f 696e 6974         mock_init
+00010e20: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00010e30: 6d6f 636b 5f63 6c69 656e 740a 2020 2020  mock_client.    
+00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e50: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
+00010e60: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00010e70: 616c 2e64 6973 706c 6179 2e6f 626a 2e67  al.display.obj.g
+00010e80: 6574 5f64 6973 706c 6179 2729 2061 7320  et_display') as 
+00010e90: 6d6f 636b 5f64 6973 706c 6179 3a0a 2020  mock_display:.  
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010eb0: 2020 2020 2020 6966 206e 6f74 2071 7569        if not qui
+00010ec0: 6574 5f6d 6f64 653a 0a20 2020 2020 2020  et_mode:.       
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ee0: 2020 2020 206d 6f63 6b5f 6469 7370 6c61       mock_displa
+00010ef0: 7928 292e 6e6f 7469 6669 6361 7469 6f6e  y().notification
+00010f00: 2e73 6964 655f 6566 6665 6374 203d 2077  .side_effect = w
+00010f10: 7269 7465 5f6d 7367 0a20 2020 2020 2020  rite_msg.       
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+00010f40: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00010f50: 6e61 6c2e 6d61 696e 2e72 656e 6577 616c  nal.main.renewal
+00010f60: 2e63 7279 7074 6f5f 7574 696c 2729 205c  .crypto_util') \
+00010f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f80: 2020 2020 2020 2020 2020 2020 2061 7320               as 
+00010f90: 6d6f 636b 5f63 7279 7074 6f5f 7574 696c  mock_crypto_util
+00010fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00010fc0: 636b 5f63 7279 7074 6f5f 7574 696c 2e6e  ck_crypto_util.n
+00010fd0: 6f74 4166 7465 722e 7265 7475 726e 5f76  otAfter.return_v
+00010fe0: 616c 7565 203d 2065 7870 6972 795f 6461  alue = expiry_da
+00010ff0: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+00011000: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00011010: 6974 6820 6d6f 636b 2e70 6174 6368 2827  ith mock.patch('
+00011020: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00011030: 6c2e 6566 662e 6861 6e64 6c65 5f73 7562  l.eff.handle_sub
+00011040: 7363 7269 7074 696f 6e27 293a 0a20 2020  scription'):.   
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011070: 6e6f 7420 6172 6773 3a0a 2020 2020 2020  not args:.      
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+000110a0: 6773 203d 205b 272d 6427 2c20 2769 736e  gs = ['-d', 'isn
+000110b0: 6f74 2e6f 7267 272c 2027 2d61 272c 2027  ot.org', '-a', '
+000110c0: 7374 616e 6461 6c6f 6e65 272c 2027 6365  standalone', 'ce
+000110d0: 7274 6f6e 6c79 275d 0a20 2020 2020 2020  rtonly'].       
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2020 2020 2020 2069 6620 6578 7472           if extr
+00011100: 615f 6172 6773 3a0a 2020 2020 2020 2020  a_args:.        
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00011130: 202b 3d20 6578 7472 615f 6172 6773 0a20   += extra_args. 
 00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011150: 2073 686f 756c 645f 7265 6e65 773d 4661   should_renew=Fa
-00011160: 6c73 6529 0a20 2020 2020 2020 2061 7373  lse).        ass
-00011170: 6572 7420 276e 6f74 2079 6574 2064 7565  ert 'not yet due
-00011180: 2720 696e 206d 6f63 6b5f 6469 7370 6c61  ' in mock_displa
-00011190: 7965 7228 292e 6e6f 7469 6669 6361 7469  yer().notificati
-000111a0: 6f6e 2e63 616c 6c5f 6172 6773 5b30 5d5b  on.call_args[0][
-000111b0: 305d 0a0a 2020 2020 6465 6620 5f64 756d  0]..    def _dum
-000111c0: 705f 6c6f 6728 7365 6c66 293a 0a20 2020  p_log(self):.   
-000111d0: 2020 2020 2070 7269 6e74 2822 4c6f 6773       print("Logs
-000111e0: 3a22 290a 2020 2020 2020 2020 6c6f 675f  :").        log_
-000111f0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00011200: 6f69 6e28 7365 6c66 2e63 6f6e 6669 672e  oin(self.config.
-00011210: 6c6f 6773 5f64 6972 2c20 226c 6574 7365  logs_dir, "letse
-00011220: 6e63 7279 7074 2e6c 6f67 2229 0a20 2020  ncrypt.log").   
-00011230: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00011240: 6578 6973 7473 286c 6f67 5f70 6174 6829  exists(log_path)
-00011250: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00011260: 7468 206f 7065 6e28 6c6f 675f 7061 7468  th open(log_path
-00011270: 2920 6173 206c 663a 0a20 2020 2020 2020  ) as lf:.       
-00011280: 2020 2020 2020 2020 2070 7269 6e74 286c           print(l
-00011290: 662e 7265 6164 2829 290a 0a20 2020 2064  f.read())..    d
-000112a0: 6566 2074 6573 745f 7265 6e65 775f 7665  ef test_renew_ve
-000112b0: 7262 2873 656c 6629 3a0a 2020 2020 2020  rb(self):.      
-000112c0: 2020 7465 7374 5f75 7469 6c2e 6d61 6b65    test_util.make
-000112d0: 5f6c 696e 6561 6765 2873 656c 662e 636f  _lineage(self.co
-000112e0: 6e66 6967 2e63 6f6e 6669 675f 6469 722c  nfig.config_dir,
-000112f0: 2027 7361 6d70 6c65 2d72 656e 6577 616c   'sample-renewal
-00011300: 2e63 6f6e 6627 290a 2020 2020 2020 2020  .conf').        
-00011310: 6172 6773 203d 205b 2272 656e 6577 222c  args = ["renew",
-00011320: 2022 2d2d 6472 792d 7275 6e22 2c20 222d   "--dry-run", "-
-00011330: 7476 7622 5d0a 2020 2020 2020 2020 7365  tvv"].        se
-00011340: 6c66 2e5f 7465 7374 5f72 656e 6577 616c  lf._test_renewal
-00011350: 5f63 6f6d 6d6f 6e28 5472 7565 2c20 5b5d  _common(True, []
-00011360: 2c20 6172 6773 3d61 7267 732c 2073 686f  , args=args, sho
-00011370: 756c 645f 7265 6e65 773d 5472 7565 290a  uld_renew=True).
-00011380: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-00011390: 7573 655f 6b65 7928 7365 6c66 293a 0a20  use_key(self):. 
-000113a0: 2020 2020 2020 2074 6573 745f 7574 696c         test_util
-000113b0: 2e6d 616b 655f 6c69 6e65 6167 6528 7365  .make_lineage(se
-000113c0: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
-000113d0: 5f64 6972 2c20 2773 616d 706c 652d 7265  _dir, 'sample-re
-000113e0: 6e65 7761 6c2e 636f 6e66 272c 2065 633d  newal.conf', ec=
-000113f0: 4661 6c73 6529 0a20 2020 2020 2020 2061  False).        a
-00011400: 7267 7320 3d20 5b22 7265 6e65 7722 2c20  rgs = ["renew", 
-00011410: 222d 2d64 7279 2d72 756e 222c 2022 2d2d  "--dry-run", "--
-00011420: 7265 7573 652d 6b65 7922 5d0a 2020 2020  reuse-key"].    
-00011430: 2020 2020 7365 6c66 2e5f 7465 7374 5f72      self._test_r
-00011440: 656e 6577 616c 5f63 6f6d 6d6f 6e28 5472  enewal_common(Tr
-00011450: 7565 2c20 5b5d 2c20 6172 6773 3d61 7267  ue, [], args=arg
-00011460: 732c 2073 686f 756c 645f 7265 6e65 773d  s, should_renew=
-00011470: 5472 7565 2c20 7265 7573 655f 6b65 793d  True, reuse_key=
-00011480: 5472 7565 290a 0a20 2020 2040 6d6f 636b  True)..    @mock
-00011490: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-000114a0: 5f69 6e74 6572 6e61 6c2e 7374 6f72 6167  _internal.storag
-000114b0: 652e 5265 6e65 7761 626c 6543 6572 742e  e.RenewableCert.
-000114c0: 7361 7665 5f73 7563 6365 7373 6f72 2729  save_successor')
-000114d0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-000114e0: 7573 655f 6b65 795f 6e6f 5f64 7279 5f72  use_key_no_dry_r
-000114f0: 756e 2873 656c 662c 2075 6e75 7365 645f  un(self, unused_
-00011500: 7361 7665 5f73 7563 6365 7373 6f72 293a  save_successor):
-00011510: 0a20 2020 2020 2020 2074 6573 745f 7574  .        test_ut
-00011520: 696c 2e6d 616b 655f 6c69 6e65 6167 6528  il.make_lineage(
-00011530: 7365 6c66 2e63 6f6e 6669 672e 636f 6e66  self.config.conf
-00011540: 6967 5f64 6972 2c20 2773 616d 706c 652d  ig_dir, 'sample-
-00011550: 7265 6e65 7761 6c2e 636f 6e66 272c 2065  renewal.conf', e
-00011560: 633d 4661 6c73 6529 0a20 2020 2020 2020  c=False).       
-00011570: 2061 7267 7320 3d20 5b22 7265 6e65 7722   args = ["renew"
-00011580: 2c20 222d 2d72 6575 7365 2d6b 6579 225d  , "--reuse-key"]
-00011590: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-000115a0: 6573 745f 7265 6e65 7761 6c5f 636f 6d6d  est_renewal_comm
-000115b0: 6f6e 2854 7275 652c 205b 5d2c 2061 7267  on(True, [], arg
-000115c0: 733d 6172 6773 2c20 7368 6f75 6c64 5f72  s=args, should_r
-000115d0: 656e 6577 3d54 7275 652c 2072 6575 7365  enew=True, reuse
-000115e0: 5f6b 6579 3d54 7275 6529 0a0a 2020 2020  _key=True)..    
-000115f0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-00011600: 7462 6f74 2e5f 696e 7465 726e 616c 2e73  tbot._internal.s
-00011610: 746f 7261 6765 2e52 656e 6577 6162 6c65  torage.Renewable
-00011620: 4365 7274 2e73 6176 655f 7375 6363 6573  Cert.save_succes
-00011630: 736f 7227 290a 2020 2020 6465 6620 7465  sor').    def te
-00011640: 7374 5f6e 6577 5f6b 6579 2873 656c 662c  st_new_key(self,
-00011650: 2075 6e75 7365 645f 7361 7665 5f73 7563   unused_save_suc
-00011660: 6365 7373 6f72 293a 0a20 2020 2020 2020  cessor):.       
-00011670: 2074 6573 745f 7574 696c 2e6d 616b 655f   test_util.make_
-00011680: 6c69 6e65 6167 6528 7365 6c66 2e63 6f6e  lineage(self.con
-00011690: 6669 672e 636f 6e66 6967 5f64 6972 2c20  fig.config_dir, 
-000116a0: 2773 616d 706c 652d 7265 6e65 7761 6c2e  'sample-renewal.
-000116b0: 636f 6e66 2729 0a20 2020 2020 2020 2061  conf').        a
-000116c0: 7267 7320 3d20 5b22 7265 6e65 7722 2c20  rgs = ["renew", 
-000116d0: 222d 2d72 6575 7365 2d6b 6579 222c 2022  "--reuse-key", "
-000116e0: 2d2d 6e65 772d 6b65 7922 5d0a 2020 2020  --new-key"].    
-000116f0: 2020 2020 7365 6c66 2e5f 7465 7374 5f72      self._test_r
-00011700: 656e 6577 616c 5f63 6f6d 6d6f 6e28 5472  enewal_common(Tr
-00011710: 7565 2c20 5b5d 2c20 6172 6773 3d61 7267  ue, [], args=arg
-00011720: 732c 2073 686f 756c 645f 7265 6e65 773d  s, should_renew=
-00011730: 5472 7565 2c20 7265 7573 655f 6b65 793d  True, reuse_key=
-00011740: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011760: 2020 2020 2020 2020 6e65 775f 6b65 793d          new_key=
-00011770: 5472 7565 290a 0a20 2020 2040 6d6f 636b  True)..    @mock
-00011780: 2e70 6174 6368 2827 7379 732e 7374 6469  .patch('sys.stdi
-00011790: 6e27 290a 2020 2020 6465 6620 7465 7374  n').    def test
-000117a0: 5f6e 6f6e 696e 7465 7261 6374 6976 655f  _noninteractive_
-000117b0: 7265 6e65 7761 6c5f 6465 6c61 7928 7365  renewal_delay(se
-000117c0: 6c66 2c20 7374 6469 6e29 3a0a 2020 2020  lf, stdin):.    
-000117d0: 2020 2020 7374 6469 6e2e 6973 6174 7479      stdin.isatty
-000117e0: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-000117f0: 4661 6c73 650a 2020 2020 2020 2020 7465  False.        te
-00011800: 7374 5f75 7469 6c2e 6d61 6b65 5f6c 696e  st_util.make_lin
-00011810: 6561 6765 2873 656c 662e 636f 6e66 6967  eage(self.config
-00011820: 2e63 6f6e 6669 675f 6469 722c 2027 7361  .config_dir, 'sa
-00011830: 6d70 6c65 2d72 656e 6577 616c 2e63 6f6e  mple-renewal.con
-00011840: 6627 290a 2020 2020 2020 2020 6172 6773  f').        args
-00011850: 203d 205b 2272 656e 6577 222c 2022 2d2d   = ["renew", "--
-00011860: 6472 792d 7275 6e22 2c20 222d 7476 7622  dry-run", "-tvv"
-00011870: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
-00011880: 7465 7374 5f72 656e 6577 616c 5f63 6f6d  test_renewal_com
-00011890: 6d6f 6e28 5472 7565 2c20 5b5d 2c20 6172  mon(True, [], ar
-000118a0: 6773 3d61 7267 732c 2073 686f 756c 645f  gs=args, should_
-000118b0: 7265 6e65 773d 5472 7565 290a 2020 2020  renew=True).    
-000118c0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-000118d0: 6d6f 636b 5f73 6c65 6570 2e63 616c 6c5f  mock_sleep.call_
-000118e0: 636f 756e 7420 3d3d 2031 0a20 2020 2020  count == 1.     
-000118f0: 2020 2023 2069 6e20 6d61 696e 2e70 793a     # in main.py:
-00011900: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
-00011910: 6c65 6570 5f74 696d 6520 3d20 7261 6e64  leep_time = rand
-00011920: 6f6d 2e72 616e 6469 6e74 2831 2c20 3630  om.randint(1, 60
-00011930: 2a38 290a 2020 2020 2020 2020 736c 6565  *8).        slee
-00011940: 705f 6361 6c6c 5f61 7267 203d 2073 656c  p_call_arg = sel
-00011950: 662e 6d6f 636b 5f73 6c65 6570 2e63 616c  f.mock_sleep.cal
-00011960: 6c5f 6172 6773 5b30 5d5b 305d 0a20 2020  l_args[0][0].   
-00011970: 2020 2020 2061 7373 6572 7420 3120 3c3d       assert 1 <=
-00011980: 2073 6c65 6570 5f63 616c 6c5f 6172 6720   sleep_call_arg 
-00011990: 3c3d 2036 302a 380a 0a20 2020 2040 6d6f  <= 60*8..    @mo
-000119a0: 636b 2e70 6174 6368 2827 7379 732e 7374  ck.patch('sys.st
-000119b0: 6469 6e27 290a 2020 2020 6465 6620 7465  din').    def te
-000119c0: 7374 5f69 6e74 6572 6163 7469 7665 5f6e  st_interactive_n
-000119d0: 6f5f 7265 6e65 7761 6c5f 6465 6c61 7928  o_renewal_delay(
-000119e0: 7365 6c66 2c20 7374 6469 6e29 3a0a 2020  self, stdin):.  
-000119f0: 2020 2020 2020 7374 6469 6e2e 6973 6174        stdin.isat
-00011a00: 7479 2e72 6574 7572 6e5f 7661 6c75 6520  ty.return_value 
-00011a10: 3d20 5472 7565 0a20 2020 2020 2020 2074  = True.        t
-00011a20: 6573 745f 7574 696c 2e6d 616b 655f 6c69  est_util.make_li
-00011a30: 6e65 6167 6528 7365 6c66 2e63 6f6e 6669  neage(self.confi
-00011a40: 672e 636f 6e66 6967 5f64 6972 2c20 2773  g.config_dir, 's
-00011a50: 616d 706c 652d 7265 6e65 7761 6c2e 636f  ample-renewal.co
-00011a60: 6e66 2729 0a20 2020 2020 2020 2061 7267  nf').        arg
-00011a70: 7320 3d20 5b22 7265 6e65 7722 2c20 222d  s = ["renew", "-
-00011a80: 2d64 7279 2d72 756e 222c 2022 2d74 7676  -dry-run", "-tvv
-00011a90: 225d 0a20 2020 2020 2020 2073 656c 662e  "].        self.
-00011aa0: 5f74 6573 745f 7265 6e65 7761 6c5f 636f  _test_renewal_co
-00011ab0: 6d6d 6f6e 2854 7275 652c 205b 5d2c 2061  mmon(True, [], a
-00011ac0: 7267 733d 6172 6773 2c20 7368 6f75 6c64  rgs=args, should
-00011ad0: 5f72 656e 6577 3d54 7275 6529 0a20 2020  _renew=True).   
-00011ae0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-00011af0: 2e6d 6f63 6b5f 736c 6565 702e 6361 6c6c  .mock_sleep.call
-00011b00: 5f63 6f75 6e74 203d 3d20 300a 0a20 2020  _count == 0..   
-00011b10: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-00011b20: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00011b30: 7265 6e65 7761 6c2e 7368 6f75 6c64 5f72  renewal.should_r
-00011b40: 656e 6577 2729 0a20 2020 2064 6566 2074  enew').    def t
-00011b50: 6573 745f 7265 6e65 775f 736b 6970 735f  est_renew_skips_
-00011b60: 7265 6365 6e74 5f63 6572 7473 2873 656c  recent_certs(sel
-00011b70: 662c 2073 686f 756c 645f 7265 6e65 7729  f, should_renew)
-00011b80: 3a0a 2020 2020 2020 2020 7368 6f75 6c64  :.        should
-00011b90: 5f72 656e 6577 2e72 6574 7572 6e5f 7661  _renew.return_va
-00011ba0: 6c75 6520 3d20 4661 6c73 650a 2020 2020  lue = False.    
-00011bb0: 2020 2020 7465 7374 5f75 7469 6c2e 6d61      test_util.ma
-00011bc0: 6b65 5f6c 696e 6561 6765 2873 656c 662e  ke_lineage(self.
-00011bd0: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
-00011be0: 722c 2027 7361 6d70 6c65 2d72 656e 6577  r, 'sample-renew
-00011bf0: 616c 2e63 6f6e 6627 290a 2020 2020 2020  al.conf').      
-00011c00: 2020 6578 7069 7279 203d 2064 6174 6574    expiry = datet
-00011c10: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-00011c20: 2829 202b 2064 6174 6574 696d 652e 7469  () + datetime.ti
-00011c30: 6d65 6465 6c74 6128 6461 7973 3d39 3029  medelta(days=90)
-00011c40: 0a20 2020 2020 2020 205f 2c20 5f2c 2073  .        _, _, s
-00011c50: 7464 6f75 7420 3d20 7365 6c66 2e5f 7465  tdout = self._te
-00011c60: 7374 5f72 656e 6577 616c 5f63 6f6d 6d6f  st_renewal_commo
-00011c70: 6e28 4661 6c73 652c 2065 7874 7261 5f61  n(False, extra_a
-00011c80: 7267 733d 4e6f 6e65 2c20 7368 6f75 6c64  rgs=None, should
-00011c90: 5f72 656e 6577 3d46 616c 7365 2c0a 2020  _renew=False,.  
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011cd0: 7267 733d 5b27 7265 6e65 7727 5d2c 2065  rgs=['renew'], e
-00011ce0: 7870 6972 795f 6461 7465 3d65 7870 6972  xpiry_date=expir
-00011cf0: 7929 0a20 2020 2020 2020 2061 7373 6572  y).        asser
-00011d00: 7420 274e 6f20 7265 6e65 7761 6c73 2077  t 'No renewals w
-00011d10: 6572 6520 6174 7465 6d70 7465 642e 2720  ere attempted.' 
-00011d20: 696e 2073 7464 6f75 742e 6765 7476 616c  in stdout.getval
-00011d30: 7565 2829 0a20 2020 2020 2020 2061 7373  ue().        ass
-00011d40: 6572 7420 2754 6865 2066 6f6c 6c6f 7769  ert 'The followi
-00011d50: 6e67 2063 6572 7469 6669 6361 7465 7320  ng certificates 
-00011d60: 6172 6520 6e6f 7420 6475 6520 666f 7220  are not due for 
-00011d70: 7265 6e65 7761 6c20 7965 743a 2720 696e  renewal yet:' in
-00011d80: 2073 7464 6f75 742e 6765 7476 616c 7565   stdout.getvalue
-00011d90: 2829 0a0a 2020 2020 406d 6f63 6b2e 7061  ()..    @mock.pa
-00011da0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-00011db0: 7465 726e 616c 2e6c 6f67 2e70 6f73 745f  ternal.log.post_
-00011dc0: 6172 675f 7061 7273 655f 7365 7475 7027  arg_parse_setup'
-00011dd0: 290a 2020 2020 6465 6620 7465 7374 5f71  ).    def test_q
-00011de0: 7569 6574 5f72 656e 6577 2873 656c 662c  uiet_renew(self,
-00011df0: 205f 293a 0a20 2020 2020 2020 2074 6573   _):.        tes
-00011e00: 745f 7574 696c 2e6d 616b 655f 6c69 6e65  t_util.make_line
-00011e10: 6167 6528 7365 6c66 2e63 6f6e 6669 672e  age(self.config.
-00011e20: 636f 6e66 6967 5f64 6972 2c20 2773 616d  config_dir, 'sam
-00011e30: 706c 652d 7265 6e65 7761 6c2e 636f 6e66  ple-renewal.conf
-00011e40: 2729 0a20 2020 2020 2020 2061 7267 7320  ').        args 
-00011e50: 3d20 5b22 7265 6e65 7722 2c20 222d 2d64  = ["renew", "--d
-00011e60: 7279 2d72 756e 225d 0a20 2020 2020 2020  ry-run"].       
-00011e70: 205f 2c20 5f2c 2073 7464 6f75 7420 3d20   _, _, stdout = 
-00011e80: 7365 6c66 2e5f 7465 7374 5f72 656e 6577  self._test_renew
-00011e90: 616c 5f63 6f6d 6d6f 6e28 5472 7565 2c20  al_common(True, 
-00011ea0: 5b5d 2c20 6172 6773 3d61 7267 732c 2073  [], args=args, s
-00011eb0: 686f 756c 645f 7265 6e65 773d 5472 7565  hould_renew=True
-00011ec0: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
-00011ed0: 7374 646f 7574 2e67 6574 7661 6c75 6528  stdout.getvalue(
-00011ee0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00011ef0: 2022 7265 6e65 7722 2069 6e20 6f75 740a   "renew" in out.
-00011f00: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-00011f10: 5b22 7265 6e65 7722 2c20 222d 2d64 7279  ["renew", "--dry
-00011f20: 2d72 756e 222c 2022 2d71 225d 0a20 2020  -run", "-q"].   
-00011f30: 2020 2020 205f 2c20 5f2c 2073 7464 6f75       _, _, stdou
-00011f40: 7420 3d20 7365 6c66 2e5f 7465 7374 5f72  t = self._test_r
-00011f50: 656e 6577 616c 5f63 6f6d 6d6f 6e28 5472  enewal_common(Tr
-00011f60: 7565 2c20 5b5d 2c20 6172 6773 3d61 7267  ue, [], args=arg
-00011f70: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 7368 6f75 6c64 5f72 656e 6577      should_renew
-00011fb0: 3d54 7275 652c 2071 7569 6574 5f6d 6f64  =True, quiet_mod
-00011fc0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-00011fd0: 6f75 7420 3d20 7374 646f 7574 2e67 6574  out = stdout.get
-00011fe0: 7661 6c75 6528 290a 2020 2020 2020 2020  value().        
-00011ff0: 6173 7365 7274 2022 2220 3d3d 206f 7574  assert "" == out
-00012000: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
-00012010: 656e 6577 5f68 6f6f 6b5f 7661 6c69 6461  enew_hook_valida
-00012020: 7469 6f6e 2873 656c 6629 3a0a 2020 2020  tion(self):.    
-00012030: 2020 2020 7465 7374 5f75 7469 6c2e 6d61      test_util.ma
-00012040: 6b65 5f6c 696e 6561 6765 2873 656c 662e  ke_lineage(self.
-00012050: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
-00012060: 722c 2027 7361 6d70 6c65 2d72 656e 6577  r, 'sample-renew
-00012070: 616c 2e63 6f6e 6627 290a 2020 2020 2020  al.conf').      
-00012080: 2020 6172 6773 203d 205b 2272 656e 6577    args = ["renew
-00012090: 222c 2022 2d2d 6472 792d 7275 6e22 2c20  ", "--dry-run", 
-000120a0: 222d 2d70 6f73 742d 686f 6f6b 3d6e 6f2d  "--post-hook=no-
-000120b0: 7375 6368 2d63 6f6d 6d61 6e64 225d 0a20  such-command"]. 
-000120c0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-000120d0: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
-000120e0: 2854 7275 652c 205b 5d2c 2061 7267 733d  (True, [], args=
-000120f0: 6172 6773 2c20 7368 6f75 6c64 5f72 656e  args, should_ren
-00012100: 6577 3d46 616c 7365 2c0a 2020 2020 2020  ew=False,.      
-00012110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012120: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00012130: 725f 6578 7065 6374 6564 3d54 7275 6529  r_expected=True)
-00012140: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
-00012150: 656e 6577 5f6e 6f5f 686f 6f6b 5f76 616c  enew_no_hook_val
-00012160: 6964 6174 696f 6e28 7365 6c66 293a 0a20  idation(self):. 
-00012170: 2020 2020 2020 2074 6573 745f 7574 696c         test_util
-00012180: 2e6d 616b 655f 6c69 6e65 6167 6528 7365  .make_lineage(se
-00012190: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
-000121a0: 5f64 6972 2c20 2773 616d 706c 652d 7265  _dir, 'sample-re
-000121b0: 6e65 7761 6c2e 636f 6e66 2729 0a20 2020  newal.conf').   
-000121c0: 2020 2020 2061 7267 7320 3d20 5b22 7265       args = ["re
-000121d0: 6e65 7722 2c20 222d 2d64 7279 2d72 756e  new", "--dry-run
-000121e0: 222c 2022 2d2d 706f 7374 2d68 6f6f 6b3d  ", "--post-hook=
-000121f0: 6e6f 2d73 7563 682d 636f 6d6d 616e 6422  no-such-command"
-00012200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012210: 2020 222d 2d64 6973 6162 6c65 2d68 6f6f    "--disable-hoo
-00012220: 6b2d 7661 6c69 6461 7469 6f6e 225d 0a20  k-validation"]. 
-00012230: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
-00012240: 2e70 6174 6368 2822 6365 7274 626f 742e  .patch("certbot.
-00012250: 5f69 6e74 6572 6e61 6c2e 686f 6f6b 732e  _internal.hooks.
-00012260: 706f 7374 5f68 6f6f 6b22 293a 0a20 2020  post_hook"):.   
-00012270: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-00012280: 6573 745f 7265 6e65 7761 6c5f 636f 6d6d  est_renewal_comm
-00012290: 6f6e 2854 7275 652c 205b 5d2c 2061 7267  on(True, [], arg
-000122a0: 733d 6172 6773 2c20 7368 6f75 6c64 5f72  s=args, should_r
-000122b0: 656e 6577 3d54 7275 652c 0a20 2020 2020  enew=True,.     
-000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122e0: 2065 7272 6f72 5f65 7870 6563 7465 643d   error_expected=
-000122f0: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
-00012300: 7465 7374 5f72 656e 6577 5f76 6572 625f  test_renew_verb_
-00012310: 656d 7074 795f 636f 6e66 6967 2873 656c  empty_config(sel
-00012320: 6629 3a0a 2020 2020 2020 2020 7264 203d  f):.        rd =
-00012330: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00012340: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
-00012350: 5f64 6972 2c20 2772 656e 6577 616c 2729  _dir, 'renewal')
-00012360: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00012370: 6f73 2e70 6174 682e 6578 6973 7473 2872  os.path.exists(r
-00012380: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-00012390: 6669 6c65 7379 7374 656d 2e6d 616b 6564  filesystem.maked
-000123a0: 6972 7328 7264 290a 2020 2020 2020 2020  irs(rd).        
-000123b0: 7769 7468 206f 7065 6e28 6f73 2e70 6174  with open(os.pat
-000123c0: 682e 6a6f 696e 2872 642c 2027 656d 7074  h.join(rd, 'empt
-000123d0: 792e 636f 6e66 2729 2c20 2777 2729 3a0a  y.conf'), 'w'):.
-000123e0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000123f0: 2020 2320 6c65 6176 6520 7468 6520 6669    # leave the fi
-00012400: 6c65 2065 6d70 7479 0a20 2020 2020 2020  le empty.       
-00012410: 2061 7267 7320 3d20 5b22 7265 6e65 7722   args = ["renew"
-00012420: 2c20 222d 2d64 7279 2d72 756e 222c 2022  , "--dry-run", "
-00012430: 2d74 7676 225d 0a20 2020 2020 2020 2073  -tvv"].        s
-00012440: 656c 662e 5f74 6573 745f 7265 6e65 7761  elf._test_renewa
-00012450: 6c5f 636f 6d6d 6f6e 2846 616c 7365 2c20  l_common(False, 
-00012460: 5b5d 2c20 6172 6773 3d61 7267 732c 2073  [], args=args, s
-00012470: 686f 756c 645f 7265 6e65 773d 4661 6c73  hould_renew=Fals
-00012480: 652c 2065 7272 6f72 5f65 7870 6563 7465  e, error_expecte
-00012490: 643d 5472 7565 290a 0a20 2020 2064 6566  d=True)..    def
-000124a0: 2074 6573 745f 7265 6e65 775f 7769 7468   test_renew_with
-000124b0: 5f63 6572 746e 616d 6528 7365 6c66 293a  _certname(self):
-000124c0: 0a20 2020 2020 2020 2074 6573 745f 7574  .        test_ut
-000124d0: 696c 2e6d 616b 655f 6c69 6e65 6167 6528  il.make_lineage(
-000124e0: 7365 6c66 2e63 6f6e 6669 672e 636f 6e66  self.config.conf
-000124f0: 6967 5f64 6972 2c20 2773 616d 706c 652d  ig_dir, 'sample-
-00012500: 7265 6e65 7761 6c2e 636f 6e66 2729 0a20  renewal.conf'). 
-00012510: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-00012520: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
-00012530: 2854 7275 652c 205b 5d2c 2073 686f 756c  (True, [], shoul
-00012540: 645f 7265 6e65 773d 5472 7565 2c0a 2020  d_renew=True,.  
-00012550: 2020 2020 2020 2020 2020 6172 6773 3d5b            args=[
-00012560: 2772 656e 6577 272c 2027 2d2d 6472 792d  'renew', '--dry-
-00012570: 7275 6e27 2c20 272d 2d63 6572 742d 6e61  run', '--cert-na
-00012580: 6d65 272c 2027 7361 6d70 6c65 2d72 656e  me', 'sample-ren
-00012590: 6577 616c 275d 290a 0a20 2020 2064 6566  ewal'])..    def
-000125a0: 2074 6573 745f 7265 6e65 775f 7769 7468   test_renew_with
-000125b0: 5f62 6164 5f63 6572 746e 616d 6528 7365  _bad_certname(se
-000125c0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-000125d0: 662e 5f74 6573 745f 7265 6e65 7761 6c5f  f._test_renewal_
-000125e0: 636f 6d6d 6f6e 2854 7275 652c 205b 5d2c  common(True, [],
-000125f0: 2073 686f 756c 645f 7265 6e65 773d 4661   should_renew=Fa
-00012600: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00012610: 2061 7267 733d 5b27 7265 6e65 7727 2c20   args=['renew', 
-00012620: 272d 2d64 7279 2d72 756e 272c 2027 2d2d  '--dry-run', '--
-00012630: 6365 7274 2d6e 616d 6527 2c20 2773 616d  cert-name', 'sam
-00012640: 706c 652d 7265 6e65 7761 6c27 5d2c 0a20  ple-renewal'],. 
-00012650: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00012660: 5f65 7870 6563 7465 643d 5472 7565 290a  _expected=True).
-00012670: 0a20 2020 2064 6566 205f 6d61 6b65 5f64  .    def _make_d
-00012680: 756d 6d79 5f72 656e 6577 616c 5f63 6f6e  ummy_renewal_con
-00012690: 6669 6728 7365 6c66 293a 0a20 2020 2020  fig(self):.     
-000126a0: 2020 2072 656e 6577 6572 5f63 6f6e 6669     renewer_confi
-000126b0: 6773 5f64 6972 203d 206f 732e 7061 7468  gs_dir = os.path
-000126c0: 2e6a 6f69 6e28 7365 6c66 2e63 6f6e 6669  .join(self.confi
-000126d0: 672e 636f 6e66 6967 5f64 6972 2c20 2772  g.config_dir, 'r
-000126e0: 656e 6577 616c 2729 0a20 2020 2020 2020  enewal').       
-000126f0: 2066 696c 6573 7973 7465 6d2e 6d61 6b65   filesystem.make
-00012700: 6469 7273 2872 656e 6577 6572 5f63 6f6e  dirs(renewer_con
-00012710: 6669 6773 5f64 6972 290a 2020 2020 2020  figs_dir).      
-00012720: 2020 7769 7468 206f 7065 6e28 6f73 2e70    with open(os.p
-00012730: 6174 682e 6a6f 696e 2872 656e 6577 6572  ath.join(renewer
-00012740: 5f63 6f6e 6669 6773 5f64 6972 2c20 2774  _configs_dir, 't
-00012750: 6573 742e 636f 6e66 2729 2c20 2777 2729  est.conf'), 'w')
-00012760: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00012770: 2020 2066 2e77 7269 7465 2822 4d79 2063     f.write("My c
-00012780: 6f6e 7465 6e74 7320 646f 6e27 7420 6d61  ontents don't ma
-00012790: 7474 6572 2229 0a0a 2020 2020 6465 6620  tter")..    def 
-000127a0: 5f74 6573 745f 7265 6e65 775f 636f 6d6d  _test_renew_comm
-000127b0: 6f6e 2873 656c 662c 2072 656e 6577 616c  on(self, renewal
-000127c0: 7061 7261 6d73 3d4e 6f6e 652c 206e 616d  params=None, nam
-000127d0: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 2020 6173 7365 7274 5f6f 635f 6361      assert_oc_ca
-00012800: 6c6c 6564 3d4e 6f6e 652c 202a 2a6b 7761  lled=None, **kwa
-00012810: 7267 7329 3a0a 2020 2020 2020 2020 7365  rgs):.        se
-00012820: 6c66 2e5f 6d61 6b65 5f64 756d 6d79 5f72  lf._make_dummy_r
-00012830: 656e 6577 616c 5f63 6f6e 6669 6728 290a  enewal_config().
-00012840: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
-00012850: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-00012860: 2e5f 696e 7465 726e 616c 2e73 746f 7261  ._internal.stora
-00012870: 6765 2e52 656e 6577 6162 6c65 4365 7274  ge.RenewableCert
-00012880: 2729 2061 7320 6d6f 636b 5f72 633a 0a20  ') as mock_rc:. 
-00012890: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
-000128a0: 6c69 6e65 6167 6520 3d20 6d6f 636b 2e4d  lineage = mock.M
-000128b0: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-000128c0: 2020 2020 2020 206d 6f63 6b5f 6c69 6e65         mock_line
-000128d0: 6167 652e 6675 6c6c 6368 6169 6e20 3d20  age.fullchain = 
-000128e0: 2273 6f6d 6570 6174 682f 6675 6c6c 6368  "somepath/fullch
-000128f0: 6169 6e2e 7065 6d22 0a20 2020 2020 2020  ain.pem".       
-00012900: 2020 2020 2069 6620 7265 6e65 7761 6c70       if renewalp
-00012910: 6172 616d 7320 6973 206e 6f74 204e 6f6e  arams is not Non
-00012920: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012930: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
-00012940: 636f 6e66 6967 7572 6174 696f 6e20 3d20  configuration = 
-00012950: 7b27 7265 6e65 7761 6c70 6172 616d 7327  {'renewalparams'
-00012960: 3a20 7265 6e65 7761 6c70 6172 616d 737d  : renewalparams}
-00012970: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012980: 6e61 6d65 7320 6973 206e 6f74 204e 6f6e  names is not Non
-00012990: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000129a0: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
-000129b0: 6e61 6d65 732e 7265 7475 726e 5f76 616c  names.return_val
-000129c0: 7565 203d 206e 616d 6573 0a20 2020 2020  ue = names.     
-000129d0: 2020 2020 2020 206d 6f63 6b5f 7263 2e72         mock_rc.r
-000129e0: 6574 7572 6e5f 7661 6c75 6520 3d20 6d6f  eturn_value = mo
-000129f0: 636b 5f6c 696e 6561 6765 0a20 2020 2020  ck_lineage.     
-00012a00: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
-00012a10: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-00012a20: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e72  _internal.main.r
-00012a30: 656e 6577 5f63 6572 7427 2920 6173 206d  enew_cert') as m
-00012a40: 6f63 6b5f 7265 6e65 775f 6365 7274 3a0a  ock_renew_cert:.
-00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a60: 6b77 6172 6773 2e73 6574 6465 6661 756c  kwargs.setdefaul
-00012a70: 7428 2761 7267 7327 2c20 5b27 7265 6e65  t('args', ['rene
-00012a80: 7727 5d29 0a20 2020 2020 2020 2020 2020  w']).           
-00012a90: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-00012aa0: 7265 6e65 7761 6c5f 636f 6d6d 6f6e 2854  renewal_common(T
-00012ab0: 7275 652c 204e 6f6e 652c 2073 686f 756c  rue, None, shoul
-00012ac0: 645f 7265 6e65 773d 4661 6c73 652c 202a  d_renew=False, *
-00012ad0: 2a6b 7761 7267 7329 0a0a 2020 2020 2020  *kwargs)..      
-00012ae0: 2020 2020 2020 6966 2061 7373 6572 745f        if assert_
-00012af0: 6f63 5f63 616c 6c65 6420 6973 206e 6f74  oc_called is not
-00012b00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012b10: 2020 2020 2020 2069 6620 6173 7365 7274         if assert
-00012b20: 5f6f 635f 6361 6c6c 6564 3a0a 2020 2020  _oc_called:.    
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 6173 7365 7274 206d 6f63 6b5f 7265 6e65  assert mock_rene
-00012b50: 775f 6365 7274 2e63 616c 6c65 640a 2020  w_cert.called.  
-00012b60: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00012b70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012b80: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-00012b90: 6f63 6b5f 7265 6e65 775f 6365 7274 2e63  ock_renew_cert.c
-00012ba0: 616c 6c65 6420 6973 2046 616c 7365 0a0a  alled is False..
-00012bb0: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
-00012bc0: 6577 5f6e 6f5f 7265 6e65 7761 6c70 6172  ew_no_renewalpar
-00012bd0: 616d 7328 7365 6c66 293a 0a20 2020 2020  ams(self):.     
-00012be0: 2020 2073 656c 662e 5f74 6573 745f 7265     self._test_re
-00012bf0: 6e65 775f 636f 6d6d 6f6e 2861 7373 6572  new_common(asser
-00012c00: 745f 6f63 5f63 616c 6c65 643d 4661 6c73  t_oc_called=Fals
-00012c10: 652c 2065 7272 6f72 5f65 7870 6563 7465  e, error_expecte
-00012c20: 643d 5472 7565 290a 0a20 2020 2064 6566  d=True)..    def
-00012c30: 2074 6573 745f 7265 6e65 775f 6e6f 5f61   test_renew_no_a
-00012c40: 7574 6865 6e74 6963 6174 6f72 2873 656c  uthenticator(sel
-00012c50: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00012c60: 2e5f 7465 7374 5f72 656e 6577 5f63 6f6d  ._test_renew_com
-00012c70: 6d6f 6e28 7265 6e65 7761 6c70 6172 616d  mon(renewalparam
-00012c80: 733d 7b7d 2c20 6173 7365 7274 5f6f 635f  s={}, assert_oc_
-00012c90: 6361 6c6c 6564 3d46 616c 7365 2c0a 2020  called=False,.  
-00012ca0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
-00012cb0: 6578 7065 6374 6564 3d54 7275 6529 0a0a  expected=True)..
-00012cc0: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
-00012cd0: 6577 5f77 6974 685f 6261 645f 696e 7428  ew_with_bad_int(
-00012ce0: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00012cf0: 656e 6577 616c 7061 7261 6d73 203d 207b  enewalparams = {
-00012d00: 2761 7574 6865 6e74 6963 6174 6f72 273a  'authenticator':
-00012d10: 2027 7765 6272 6f6f 7427 2c0a 2020 2020   'webroot',.    
-00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d30: 2020 2020 2027 7273 615f 6b65 795f 7369       'rsa_key_si
-00012d40: 7a65 273a 2027 6f76 6572 2039 3030 3027  ze': 'over 9000'
-00012d50: 7d0a 2020 2020 2020 2020 7365 6c66 2e5f  }.        self._
-00012d60: 7465 7374 5f72 656e 6577 5f63 6f6d 6d6f  test_renew_commo
-00012d70: 6e28 7265 6e65 7761 6c70 6172 616d 733d  n(renewalparams=
-00012d80: 7265 6e65 7761 6c70 6172 616d 732c 2065  renewalparams, e
-00012d90: 7272 6f72 5f65 7870 6563 7465 643d 5472  rror_expected=Tr
-00012da0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dc0: 2020 2020 6173 7365 7274 5f6f 635f 6361      assert_oc_ca
-00012dd0: 6c6c 6564 3d46 616c 7365 290a 0a20 2020  lled=False)..   
-00012de0: 2064 6566 2074 6573 745f 7265 6e65 775f   def test_renew_
-00012df0: 7769 7468 5f6e 6f6e 6574 7970 655f 6874  with_nonetype_ht
-00012e00: 7470 3031 2873 656c 6629 3a0a 2020 2020  tp01(self):.    
-00012e10: 2020 2020 7265 6e65 7761 6c70 6172 616d      renewalparam
-00012e20: 7320 3d20 7b27 6175 7468 656e 7469 6361  s = {'authentica
-00012e30: 746f 7227 3a20 2777 6562 726f 6f74 272c  tor': 'webroot',
-00012e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e50: 2020 2020 2020 2020 2020 2768 7474 7030            'http0
-00012e60: 315f 706f 7274 273a 2027 4e6f 6e65 277d  1_port': 'None'}
-00012e70: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00012e80: 6573 745f 7265 6e65 775f 636f 6d6d 6f6e  est_renew_common
-00012e90: 2872 656e 6577 616c 7061 7261 6d73 3d72  (renewalparams=r
-00012ea0: 656e 6577 616c 7061 7261 6d73 2c0a 2020  enewalparams,.  
+00011150: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011160: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011180: 2020 2020 2020 2020 7265 742c 2073 7464          ret, std
+00011190: 6f75 742c 205f 2c20 5f20 3d20 7365 6c66  out, _, _ = self
+000111a0: 2e5f 6361 6c6c 2861 7267 732c 2073 7464  ._call(args, std
+000111b0: 6f75 7429 0a20 2020 2020 2020 2020 2020  out).           
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2020 2020 2020 2069 6620 7265 743a           if ret:
+000111e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011200: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00011210: 5265 7475 726e 6564 222c 2072 6574 290a  Returned", ret).
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011240: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
+00011250: 7365 7274 696f 6e45 7272 6f72 2872 6574  sertionError(ret
+00011260: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011280: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
+00011290: 2065 7272 6f72 5f65 7870 6563 7465 642c   error_expected,
+000112a0: 2022 7265 6e65 7761 6c20 7368 6f75 6c64   "renewal should
+000112b0: 2068 6176 6520 6572 726f 7265 6422 0a20   have errored". 
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000112e0: 7863 6570 743a 2023 2070 796c 696e 743a  xcept: # pylint:
+000112f0: 2064 6973 6162 6c65 3d62 6172 652d 6578   disable=bare-ex
+00011300: 6365 7074 0a20 2020 2020 2020 2020 2020  cept.           
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00011330: 6572 726f 725f 6578 7065 6374 6564 3a0a  error_expected:.
+00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
+00011370: 7365 7274 696f 6e45 7272 6f72 280a 2020  sertionError(.  
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113a0: 2020 2020 2020 2020 2020 2255 6e65 7870            "Unexp
+000113b0: 6563 7465 6420 7265 6e65 7761 6c20 6572  ected renewal er
+000113c0: 726f 723a 5c6e 2220 2b0a 2020 2020 2020  ror:\n" +.      
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 7472 6163 6562 6163 6b2e        traceback.
+00011400: 666f 726d 6174 5f65 7863 2829 290a 0a20  format_exc()).. 
+00011410: 2020 2020 2020 2020 2020 2069 6620 7368             if sh
+00011420: 6f75 6c64 5f72 656e 6577 3a0a 2020 2020  ould_renew:.    
+00011430: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+00011440: 6575 7365 5f6b 6579 2061 6e64 206e 6f74  euse_key and not
+00011450: 206e 6577 5f6b 6579 3a0a 2020 2020 2020   new_key:.      
+00011460: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00011470: 5468 6520 6c6f 6361 7469 6f6e 206f 6620  The location of 
+00011480: 7468 6520 7072 6576 696f 7573 206c 6976  the previous liv
+00011490: 6520 7072 6976 6b65 792e 7065 6d20 6973  e privkey.pem is
+000114a0: 2070 6173 7365 640a 2020 2020 2020 2020   passed.        
+000114b0: 2020 2020 2020 2020 2020 2020 2320 746f              # to
+000114c0: 206f 6274 6169 6e5f 6365 7274 6966 6963   obtain_certific
+000114d0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+000114e0: 2020 2020 2020 2020 6d6f 636b 5f63 6c69          mock_cli
+000114f0: 656e 742e 6f62 7461 696e 5f63 6572 7469  ent.obtain_certi
+00011500: 6669 6361 7465 2e61 7373 6572 745f 6361  ficate.assert_ca
+00011510: 6c6c 6564 5f6f 6e63 655f 7769 7468 285b  lled_once_with([
+00011520: 6d6f 636b 2e41 4e59 5d2c 0a20 2020 2020  mock.ANY],.     
+00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011540: 2020 206f 732e 7061 7468 2e6e 6f72 6d70     os.path.normp
+00011550: 6174 6828 6f73 2e70 6174 682e 6a6f 696e  ath(os.path.join
+00011560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011570: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011580: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
+00011590: 5f64 6972 2c20 226c 6976 652f 7361 6d70  _dir, "live/samp
+000115a0: 6c65 2d72 656e 6577 616c 2f70 7269 766b  le-renewal/privk
+000115b0: 6579 2e70 656d 2229 2929 0a20 2020 2020  ey.pem"))).     
+000115c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000115d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000115e0: 2020 2020 206d 6f63 6b5f 636c 6965 6e74       mock_client
+000115f0: 2e6f 6274 6169 6e5f 6365 7274 6966 6963  .obtain_certific
+00011600: 6174 652e 6173 7365 7274 5f63 616c 6c65  ate.assert_calle
+00011610: 645f 6f6e 6365 5f77 6974 6828 5b6d 6f63  d_once_with([moc
+00011620: 6b2e 414e 595d 2c20 4e6f 6e65 290a 2020  k.ANY], None).  
+00011630: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 6173 7365 7274 206d 6f63 6b5f 636c 6965  assert mock_clie
+00011660: 6e74 2e6f 6274 6169 6e5f 6365 7274 6966  nt.obtain_certif
+00011670: 6963 6174 652e 6361 6c6c 5f63 6f75 6e74  icate.call_count
+00011680: 203d 3d20 300a 2020 2020 2020 2020 6578   == 0.        ex
+00011690: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+000116a0: 2020 7365 6c66 2e5f 6475 6d70 5f6c 6f67    self._dump_log
+000116b0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+000116c0: 6169 7365 0a20 2020 2020 2020 2066 696e  aise.        fin
+000116d0: 616c 6c79 3a0a 2020 2020 2020 2020 2020  ally:.          
+000116e0: 2020 6966 206c 6f67 5f6f 7574 3a0a 2020    if log_out:.  
+000116f0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00011700: 7468 206f 7065 6e28 6f73 2e70 6174 682e  th open(os.path.
+00011710: 6a6f 696e 2873 656c 662e 636f 6e66 6967  join(self.config
+00011720: 2e6c 6f67 735f 6469 722c 2022 6c65 7473  .logs_dir, "lets
+00011730: 656e 6372 7970 742e 6c6f 6722 2929 2061  encrypt.log")) a
+00011740: 7320 6c66 3a0a 2020 2020 2020 2020 2020  s lf:.          
+00011750: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00011760: 206c 6f67 5f6f 7574 2069 6e20 6c66 2e72   log_out in lf.r
+00011770: 6561 6428 290a 0a20 2020 2020 2020 2072  ead()..        r
+00011780: 6574 7572 6e20 6d6f 636b 5f6c 696e 6561  eturn mock_linea
+00011790: 6765 2c20 6d6f 636b 5f64 6973 706c 6179  ge, mock_display
+000117a0: 2c20 7374 646f 7574 0a0a 2020 2020 406d  , stdout..    @m
+000117b0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+000117c0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+000117d0: 6e2e 5f72 6570 6f72 745f 6e65 775f 6365  n._report_new_ce
+000117e0: 7274 2729 0a20 2020 2040 6d6f 636b 2e70  rt').    @mock.p
+000117f0: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+00011800: 6e74 6572 6e61 6c2e 6d61 696e 2e75 7469  nternal.main.uti
+00011810: 6c2e 6174 6578 6974 5f72 6567 6973 7465  l.atexit_registe
+00011820: 7227 290a 2020 2020 406d 6f63 6b2e 7061  r').    @mock.pa
+00011830: 7463 6828 2763 6572 7462 6f74 2e63 7279  tch('certbot.cry
+00011840: 7074 6f5f 7574 696c 2e6e 6f74 4166 7465  pto_util.notAfte
+00011850: 7227 290a 2020 2020 6465 6620 7465 7374  r').    def test
+00011860: 5f63 6572 746f 6e6c 795f 7265 6e65 7761  _certonly_renewa
+00011870: 6c28 7365 6c66 2c20 5f2c 206d 6f63 6b5f  l(self, _, mock_
+00011880: 7265 6769 7374 6572 2c20 6d6f 636b 5f72  register, mock_r
+00011890: 6570 6f72 7429 3a0a 2020 2020 2020 2020  eport):.        
+000118a0: 6c69 6e65 6167 652c 205f 2c20 5f20 3d20  lineage, _, _ = 
+000118b0: 7365 6c66 2e5f 7465 7374 5f72 656e 6577  self._test_renew
+000118c0: 616c 5f63 6f6d 6d6f 6e28 5472 7565 2c20  al_common(True, 
+000118d0: 5b5d 290a 2020 2020 2020 2020 6173 7365  []).        asse
+000118e0: 7274 206c 696e 6561 6765 2e73 6176 655f  rt lineage.save_
+000118f0: 7375 6363 6573 736f 722e 6361 6c6c 5f63  successor.call_c
+00011900: 6f75 6e74 203d 3d20 310a 2020 2020 2020  ount == 1.      
+00011910: 2020 6c69 6e65 6167 652e 7570 6461 7465    lineage.update
+00011920: 5f61 6c6c 5f6c 696e 6b73 5f74 6f2e 6173  _all_links_to.as
+00011930: 7365 7274 5f63 616c 6c65 645f 6f6e 6365  sert_called_once
+00011940: 5f77 6974 6828 0a20 2020 2020 2020 2020  _with(.         
+00011950: 2020 206c 696e 6561 6765 2e6c 6174 6573     lineage.lates
+00011960: 745f 636f 6d6d 6f6e 5f76 6572 7369 6f6e  t_common_version
+00011970: 2829 290a 2020 2020 2020 2020 6173 7365  ()).        asse
+00011980: 7274 206d 6f63 6b5f 7265 706f 7274 2e63  rt mock_report.c
+00011990: 616c 6c5f 636f 756e 7420 3d3d 2031 0a20  all_count == 1. 
+000119a0: 2020 2020 2020 2061 7373 6572 7420 2766         assert 'f
+000119b0: 756c 6c63 6861 696e 2e70 656d 2720 696e  ullchain.pem' in
+000119c0: 206d 6f63 6b5f 7265 706f 7274 2e63 616c   mock_report.cal
+000119d0: 6c5f 6172 6773 5b30 5d5b 325d 0a20 2020  l_args[0][2].   
+000119e0: 2020 2020 2061 7373 6572 7420 2764 6f6e       assert 'don
+000119f0: 6174 6527 2069 6e20 6d6f 636b 5f72 6567  ate' in mock_reg
+00011a00: 6973 7465 722e 6361 6c6c 5f61 7267 735b  ister.call_args[
+00011a10: 305d 5b31 5d0a 0a20 2020 2040 6d6f 636b  0][1]..    @mock
+00011a20: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+00011a30: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e64  _internal.main.d
+00011a40: 6973 706c 6179 5f75 7469 6c2e 6e6f 7469  isplay_util.noti
+00011a50: 6679 2729 0a20 2020 2040 6d6f 636b 2e70  fy').    @mock.p
+00011a60: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+00011a70: 6e74 6572 6e61 6c2e 6c6f 672e 6c6f 6767  nternal.log.logg
+00011a80: 696e 672e 6861 6e64 6c65 7273 2e52 6f74  ing.handlers.Rot
+00011a90: 6174 696e 6746 696c 6548 616e 646c 6572  atingFileHandler
+00011aa0: 2e64 6f52 6f6c 6c6f 7665 7227 290a 2020  .doRollover').  
+00011ab0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+00011ac0: 6572 7462 6f74 2e63 7279 7074 6f5f 7574  ertbot.crypto_ut
+00011ad0: 696c 2e6e 6f74 4166 7465 7227 290a 2020  il.notAfter').  
+00011ae0: 2020 6465 6620 7465 7374 5f63 6572 746f    def test_certo
+00011af0: 6e6c 795f 7265 6e65 7761 6c5f 7472 6967  nly_renewal_trig
+00011b00: 6765 7273 2873 656c 662c 205f 2c20 5f5f  gers(self, _, __
+00011b10: 2c20 6d6f 636b 5f6e 6f74 6966 7929 3a0a  , mock_notify):.
+00011b20: 2020 2020 2020 2020 2320 2d2d 6472 792d          # --dry-
+00011b30: 7275 6e20 7368 6f75 6c64 2066 6f72 6365  run should force
+00011b40: 2072 656e 6577 616c 0a20 2020 2020 2020   renewal.       
+00011b50: 205f 2c20 5f2c 205f 203d 2073 656c 662e   _, _, _ = self.
+00011b60: 5f74 6573 745f 7265 6e65 7761 6c5f 636f  _test_renewal_co
+00011b70: 6d6d 6f6e 2846 616c 7365 2c20 5b27 2d2d  mmon(False, ['--
+00011b80: 6472 792d 7275 6e27 2c20 272d 2d6b 6565  dry-run', '--kee
+00011b90: 7027 5d2c 0a20 2020 2020 2020 2020 2020  p'],.           
+00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bc0: 2020 2020 2020 2020 2020 206c 6f67 5f6f             log_o
+00011bd0: 7574 3d22 7369 6d75 6c61 7469 6e67 2072  ut="simulating r
+00011be0: 656e 6577 616c 2229 0a20 2020 2020 2020  enewal").       
+00011bf0: 206d 6f63 6b5f 6e6f 7469 6679 2e61 7373   mock_notify.ass
+00011c00: 6572 745f 616e 795f 6361 6c6c 2827 5468  ert_any_call('Th
+00011c10: 6520 6472 7920 7275 6e20 7761 7320 7375  e dry run was su
+00011c20: 6363 6573 7366 756c 2e27 290a 0a20 2020  ccessful.')..   
+00011c30: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
+00011c40: 7265 6e65 7761 6c5f 636f 6d6d 6f6e 2846  renewal_common(F
+00011c50: 616c 7365 2c20 5b27 2d2d 7265 6e65 772d  alse, ['--renew-
+00011c60: 6279 2d64 6566 6175 6c74 272c 2027 2d74  by-default', '-t
+00011c70: 7676 272c 2027 2d2d 6465 6275 6727 5d2c  vv', '--debug'],
+00011c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 206c 6f67 5f6f 7574 3d22 4175 746f     log_out="Auto
+00011cb0: 2d72 656e 6577 616c 2066 6f72 6365 6422  -renewal forced"
+00011cc0: 290a 0a20 2020 2020 2020 205f 2c20 6d6f  )..        _, mo
+00011cd0: 636b 5f64 6973 706c 6179 6572 2c20 5f20  ck_displayer, _ 
+00011ce0: 3d20 7365 6c66 2e5f 7465 7374 5f72 656e  = self._test_ren
+00011cf0: 6577 616c 5f63 6f6d 6d6f 6e28 4661 6c73  ewal_common(Fals
+00011d00: 652c 205b 272d 7476 7627 2c20 272d 2d64  e, ['-tvv', '--d
+00011d10: 6562 7567 272c 2027 2d2d 6b65 6570 275d  ebug', '--keep']
+00011d20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 7368 6f75 6c64 5f72 656e 6577      should_renew
+00011d50: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00011d60: 6173 7365 7274 2027 6e6f 7420 7965 7420  assert 'not yet 
+00011d70: 6475 6527 2069 6e20 6d6f 636b 5f64 6973  due' in mock_dis
+00011d80: 706c 6179 6572 2829 2e6e 6f74 6966 6963  player().notific
+00011d90: 6174 696f 6e2e 6361 6c6c 5f61 7267 735b  ation.call_args[
+00011da0: 305d 5b30 5d0a 0a20 2020 2064 6566 205f  0][0]..    def _
+00011db0: 6475 6d70 5f6c 6f67 2873 656c 6629 3a0a  dump_log(self):.
+00011dc0: 2020 2020 2020 2020 7072 696e 7428 224c          print("L
+00011dd0: 6f67 733a 2229 0a20 2020 2020 2020 206c  ogs:").        l
+00011de0: 6f67 5f70 6174 6820 3d20 6f73 2e70 6174  og_path = os.pat
+00011df0: 682e 6a6f 696e 2873 656c 662e 636f 6e66  h.join(self.conf
+00011e00: 6967 2e6c 6f67 735f 6469 722c 2022 6c65  ig.logs_dir, "le
+00011e10: 7473 656e 6372 7970 742e 6c6f 6722 290a  tsencrypt.log").
+00011e20: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00011e30: 7468 2e65 7869 7374 7328 6c6f 675f 7061  th.exists(log_pa
+00011e40: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
+00011e50: 2077 6974 6820 6f70 656e 286c 6f67 5f70   with open(log_p
+00011e60: 6174 6829 2061 7320 6c66 3a0a 2020 2020  ath) as lf:.    
+00011e70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011e80: 7428 6c66 2e72 6561 6428 2929 0a0a 2020  t(lf.read())..  
+00011e90: 2020 6465 6620 7465 7374 5f72 656e 6577    def test_renew
+00011ea0: 5f76 6572 6228 7365 6c66 293a 0a20 2020  _verb(self):.   
+00011eb0: 2020 2020 2074 6573 745f 7574 696c 2e6d       test_util.m
+00011ec0: 616b 655f 6c69 6e65 6167 6528 7365 6c66  ake_lineage(self
+00011ed0: 2e63 6f6e 6669 672e 636f 6e66 6967 5f64  .config.config_d
+00011ee0: 6972 2c20 2773 616d 706c 652d 7265 6e65  ir, 'sample-rene
+00011ef0: 7761 6c2e 636f 6e66 2729 0a20 2020 2020  wal.conf').     
+00011f00: 2020 2061 7267 7320 3d20 5b22 7265 6e65     args = ["rene
+00011f10: 7722 2c20 222d 2d64 7279 2d72 756e 222c  w", "--dry-run",
+00011f20: 2022 2d74 7676 225d 0a20 2020 2020 2020   "-tvv"].       
+00011f30: 2073 656c 662e 5f74 6573 745f 7265 6e65   self._test_rene
+00011f40: 7761 6c5f 636f 6d6d 6f6e 2854 7275 652c  wal_common(True,
+00011f50: 205b 5d2c 2061 7267 733d 6172 6773 2c20   [], args=args, 
+00011f60: 7368 6f75 6c64 5f72 656e 6577 3d54 7275  should_renew=Tru
+00011f70: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
+00011f80: 5f72 6575 7365 5f6b 6579 2873 656c 6629  _reuse_key(self)
+00011f90: 3a0a 2020 2020 2020 2020 7465 7374 5f75  :.        test_u
+00011fa0: 7469 6c2e 6d61 6b65 5f6c 696e 6561 6765  til.make_lineage
+00011fb0: 2873 656c 662e 636f 6e66 6967 2e63 6f6e  (self.config.con
+00011fc0: 6669 675f 6469 722c 2027 7361 6d70 6c65  fig_dir, 'sample
+00011fd0: 2d72 656e 6577 616c 2e63 6f6e 6627 2c20  -renewal.conf', 
+00011fe0: 6563 3d46 616c 7365 290a 2020 2020 2020  ec=False).      
+00011ff0: 2020 6172 6773 203d 205b 2272 656e 6577    args = ["renew
+00012000: 222c 2022 2d2d 6472 792d 7275 6e22 2c20  ", "--dry-run", 
+00012010: 222d 2d72 6575 7365 2d6b 6579 225d 0a20  "--reuse-key"]. 
+00012020: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
+00012030: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
+00012040: 2854 7275 652c 205b 5d2c 2061 7267 733d  (True, [], args=
+00012050: 6172 6773 2c20 7368 6f75 6c64 5f72 656e  args, should_ren
+00012060: 6577 3d54 7275 652c 2072 6575 7365 5f6b  ew=True, reuse_k
+00012070: 6579 3d54 7275 6529 0a0a 2020 2020 406d  ey=True)..    @m
+00012080: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00012090: 6f74 2e5f 696e 7465 726e 616c 2e73 746f  ot._internal.sto
+000120a0: 7261 6765 2e52 656e 6577 6162 6c65 4365  rage.RenewableCe
+000120b0: 7274 2e73 6176 655f 7375 6363 6573 736f  rt.save_successo
+000120c0: 7227 290a 2020 2020 6465 6620 7465 7374  r').    def test
+000120d0: 5f72 6575 7365 5f6b 6579 5f6e 6f5f 6472  _reuse_key_no_dr
+000120e0: 795f 7275 6e28 7365 6c66 2c20 756e 7573  y_run(self, unus
+000120f0: 6564 5f73 6176 655f 7375 6363 6573 736f  ed_save_successo
+00012100: 7229 3a0a 2020 2020 2020 2020 7465 7374  r):.        test
+00012110: 5f75 7469 6c2e 6d61 6b65 5f6c 696e 6561  _util.make_linea
+00012120: 6765 2873 656c 662e 636f 6e66 6967 2e63  ge(self.config.c
+00012130: 6f6e 6669 675f 6469 722c 2027 7361 6d70  onfig_dir, 'samp
+00012140: 6c65 2d72 656e 6577 616c 2e63 6f6e 6627  le-renewal.conf'
+00012150: 2c20 6563 3d46 616c 7365 290a 2020 2020  , ec=False).    
+00012160: 2020 2020 6172 6773 203d 205b 2272 656e      args = ["ren
+00012170: 6577 222c 2022 2d2d 7265 7573 652d 6b65  ew", "--reuse-ke
+00012180: 7922 5d0a 2020 2020 2020 2020 7365 6c66  y"].        self
+00012190: 2e5f 7465 7374 5f72 656e 6577 616c 5f63  ._test_renewal_c
+000121a0: 6f6d 6d6f 6e28 5472 7565 2c20 5b5d 2c20  ommon(True, [], 
+000121b0: 6172 6773 3d61 7267 732c 2073 686f 756c  args=args, shoul
+000121c0: 645f 7265 6e65 773d 5472 7565 2c20 7265  d_renew=True, re
+000121d0: 7573 655f 6b65 793d 5472 7565 290a 0a20  use_key=True).. 
+000121e0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+000121f0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00012200: 6c2e 7374 6f72 6167 652e 5265 6e65 7761  l.storage.Renewa
+00012210: 626c 6543 6572 742e 7361 7665 5f73 7563  bleCert.save_suc
+00012220: 6365 7373 6f72 2729 0a20 2020 2064 6566  cessor').    def
+00012230: 2074 6573 745f 6e65 775f 6b65 7928 7365   test_new_key(se
+00012240: 6c66 2c20 756e 7573 6564 5f73 6176 655f  lf, unused_save_
+00012250: 7375 6363 6573 736f 7229 3a0a 2020 2020  successor):.    
+00012260: 2020 2020 7465 7374 5f75 7469 6c2e 6d61      test_util.ma
+00012270: 6b65 5f6c 696e 6561 6765 2873 656c 662e  ke_lineage(self.
+00012280: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
+00012290: 722c 2027 7361 6d70 6c65 2d72 656e 6577  r, 'sample-renew
+000122a0: 616c 2e63 6f6e 6627 290a 2020 2020 2020  al.conf').      
+000122b0: 2020 6172 6773 203d 205b 2272 656e 6577    args = ["renew
+000122c0: 222c 2022 2d2d 7265 7573 652d 6b65 7922  ", "--reuse-key"
+000122d0: 2c20 222d 2d6e 6577 2d6b 6579 225d 0a20  , "--new-key"]. 
+000122e0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
+000122f0: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
+00012300: 2854 7275 652c 205b 5d2c 2061 7267 733d  (True, [], args=
+00012310: 6172 6773 2c20 7368 6f75 6c64 5f72 656e  args, should_ren
+00012320: 6577 3d54 7275 652c 2072 6575 7365 5f6b  ew=True, reuse_k
+00012330: 6579 3d54 7275 652c 0a20 2020 2020 2020  ey=True,.       
+00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012350: 2020 2020 2020 2020 2020 206e 6577 5f6b             new_k
+00012360: 6579 3d54 7275 6529 0a0a 2020 2020 406d  ey=True)..    @m
+00012370: 6f63 6b2e 7061 7463 6828 2773 7973 2e73  ock.patch('sys.s
+00012380: 7464 696e 2729 0a20 2020 2064 6566 2074  tdin').    def t
+00012390: 6573 745f 6e6f 6e69 6e74 6572 6163 7469  est_noninteracti
+000123a0: 7665 5f72 656e 6577 616c 5f64 656c 6179  ve_renewal_delay
+000123b0: 2873 656c 662c 2073 7464 696e 293a 0a20  (self, stdin):. 
+000123c0: 2020 2020 2020 2073 7464 696e 2e69 7361         stdin.isa
+000123d0: 7474 792e 7265 7475 726e 5f76 616c 7565  tty.return_value
+000123e0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+000123f0: 2074 6573 745f 7574 696c 2e6d 616b 655f   test_util.make_
+00012400: 6c69 6e65 6167 6528 7365 6c66 2e63 6f6e  lineage(self.con
+00012410: 6669 672e 636f 6e66 6967 5f64 6972 2c20  fig.config_dir, 
+00012420: 2773 616d 706c 652d 7265 6e65 7761 6c2e  'sample-renewal.
+00012430: 636f 6e66 2729 0a20 2020 2020 2020 2061  conf').        a
+00012440: 7267 7320 3d20 5b22 7265 6e65 7722 2c20  rgs = ["renew", 
+00012450: 222d 2d64 7279 2d72 756e 222c 2022 2d74  "--dry-run", "-t
+00012460: 7676 225d 0a20 2020 2020 2020 2073 656c  vv"].        sel
+00012470: 662e 5f74 6573 745f 7265 6e65 7761 6c5f  f._test_renewal_
+00012480: 636f 6d6d 6f6e 2854 7275 652c 205b 5d2c  common(True, [],
+00012490: 2061 7267 733d 6172 6773 2c20 7368 6f75   args=args, shou
+000124a0: 6c64 5f72 656e 6577 3d54 7275 6529 0a20  ld_renew=True). 
+000124b0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+000124c0: 6c66 2e6d 6f63 6b5f 736c 6565 702e 6361  lf.mock_sleep.ca
+000124d0: 6c6c 5f63 6f75 6e74 203d 3d20 310a 2020  ll_count == 1.  
+000124e0: 2020 2020 2020 2320 696e 206d 6169 6e2e        # in main.
+000124f0: 7079 3a0a 2020 2020 2020 2020 2320 2020  py:.        #   
+00012500: 2020 736c 6565 705f 7469 6d65 203d 2072    sleep_time = r
+00012510: 616e 646f 6d2e 7261 6e64 696e 7428 312c  andom.randint(1,
+00012520: 2036 302a 3829 0a20 2020 2020 2020 2073   60*8).        s
+00012530: 6c65 6570 5f63 616c 6c5f 6172 6720 3d20  leep_call_arg = 
+00012540: 7365 6c66 2e6d 6f63 6b5f 736c 6565 702e  self.mock_sleep.
+00012550: 6361 6c6c 5f61 7267 735b 305d 5b30 5d0a  call_args[0][0].
+00012560: 2020 2020 2020 2020 6173 7365 7274 2031          assert 1
+00012570: 203c 3d20 736c 6565 705f 6361 6c6c 5f61   <= sleep_call_a
+00012580: 7267 203c 3d20 3630 2a38 0a0a 2020 2020  rg <= 60*8..    
+00012590: 406d 6f63 6b2e 7061 7463 6828 2773 7973  @mock.patch('sys
+000125a0: 2e73 7464 696e 2729 0a20 2020 2064 6566  .stdin').    def
+000125b0: 2074 6573 745f 696e 7465 7261 6374 6976   test_interactiv
+000125c0: 655f 6e6f 5f72 656e 6577 616c 5f64 656c  e_no_renewal_del
+000125d0: 6179 2873 656c 662c 2073 7464 696e 293a  ay(self, stdin):
+000125e0: 0a20 2020 2020 2020 2073 7464 696e 2e69  .        stdin.i
+000125f0: 7361 7474 792e 7265 7475 726e 5f76 616c  satty.return_val
+00012600: 7565 203d 2054 7275 650a 2020 2020 2020  ue = True.      
+00012610: 2020 7465 7374 5f75 7469 6c2e 6d61 6b65    test_util.make
+00012620: 5f6c 696e 6561 6765 2873 656c 662e 636f  _lineage(self.co
+00012630: 6e66 6967 2e63 6f6e 6669 675f 6469 722c  nfig.config_dir,
+00012640: 2027 7361 6d70 6c65 2d72 656e 6577 616c   'sample-renewal
+00012650: 2e63 6f6e 6627 290a 2020 2020 2020 2020  .conf').        
+00012660: 6172 6773 203d 205b 2272 656e 6577 222c  args = ["renew",
+00012670: 2022 2d2d 6472 792d 7275 6e22 2c20 222d   "--dry-run", "-
+00012680: 7476 7622 5d0a 2020 2020 2020 2020 7365  tvv"].        se
+00012690: 6c66 2e5f 7465 7374 5f72 656e 6577 616c  lf._test_renewal
+000126a0: 5f63 6f6d 6d6f 6e28 5472 7565 2c20 5b5d  _common(True, []
+000126b0: 2c20 6172 6773 3d61 7267 732c 2073 686f  , args=args, sho
+000126c0: 756c 645f 7265 6e65 773d 5472 7565 290a  uld_renew=True).
+000126d0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+000126e0: 656c 662e 6d6f 636b 5f73 6c65 6570 2e63  elf.mock_sleep.c
+000126f0: 616c 6c5f 636f 756e 7420 3d3d 2030 0a0a  all_count == 0..
+00012700: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+00012710: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00012720: 616c 2e72 656e 6577 616c 2e73 686f 756c  al.renewal.shoul
+00012730: 645f 7265 6e65 7727 290a 2020 2020 6465  d_renew').    de
+00012740: 6620 7465 7374 5f72 656e 6577 5f73 6b69  f test_renew_ski
+00012750: 7073 5f72 6563 656e 745f 6365 7274 7328  ps_recent_certs(
+00012760: 7365 6c66 2c20 7368 6f75 6c64 5f72 656e  self, should_ren
+00012770: 6577 293a 0a20 2020 2020 2020 2073 686f  ew):.        sho
+00012780: 756c 645f 7265 6e65 772e 7265 7475 726e  uld_renew.return
+00012790: 5f76 616c 7565 203d 2046 616c 7365 0a20  _value = False. 
+000127a0: 2020 2020 2020 2074 6573 745f 7574 696c         test_util
+000127b0: 2e6d 616b 655f 6c69 6e65 6167 6528 7365  .make_lineage(se
+000127c0: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
+000127d0: 5f64 6972 2c20 2773 616d 706c 652d 7265  _dir, 'sample-re
+000127e0: 6e65 7761 6c2e 636f 6e66 2729 0a20 2020  newal.conf').   
+000127f0: 2020 2020 2065 7870 6972 7920 3d20 6461       expiry = da
+00012800: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00012810: 6e6f 7728 2920 2b20 6461 7465 7469 6d65  now() + datetime
+00012820: 2e74 696d 6564 656c 7461 2864 6179 733d  .timedelta(days=
+00012830: 3930 290a 2020 2020 2020 2020 5f2c 205f  90).        _, _
+00012840: 2c20 7374 646f 7574 203d 2073 656c 662e  , stdout = self.
+00012850: 5f74 6573 745f 7265 6e65 7761 6c5f 636f  _test_renewal_co
+00012860: 6d6d 6f6e 2846 616c 7365 2c20 6578 7472  mmon(False, extr
+00012870: 615f 6172 6773 3d4e 6f6e 652c 2073 686f  a_args=None, sho
+00012880: 756c 645f 7265 6e65 773d 4661 6c73 652c  uld_renew=False,
+00012890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000128a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128c0: 2020 6172 6773 3d5b 2772 656e 6577 275d    args=['renew']
+000128d0: 2c20 6578 7069 7279 5f64 6174 653d 6578  , expiry_date=ex
+000128e0: 7069 7279 290a 2020 2020 2020 2020 6173  piry).        as
+000128f0: 7365 7274 2027 4e6f 2072 656e 6577 616c  sert 'No renewal
+00012900: 7320 7765 7265 2061 7474 656d 7074 6564  s were attempted
+00012910: 2e27 2069 6e20 7374 646f 7574 2e67 6574  .' in stdout.get
+00012920: 7661 6c75 6528 290a 2020 2020 2020 2020  value().        
+00012930: 6173 7365 7274 2027 5468 6520 666f 6c6c  assert 'The foll
+00012940: 6f77 696e 6720 6365 7274 6966 6963 6174  owing certificat
+00012950: 6573 2061 7265 206e 6f74 2064 7565 2066  es are not due f
+00012960: 6f72 2072 656e 6577 616c 2079 6574 3a27  or renewal yet:'
+00012970: 2069 6e20 7374 646f 7574 2e67 6574 7661   in stdout.getva
+00012980: 6c75 6528 290a 0a20 2020 2040 6d6f 636b  lue()..    @mock
+00012990: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+000129a0: 5f69 6e74 6572 6e61 6c2e 6c6f 672e 706f  _internal.log.po
+000129b0: 7374 5f61 7267 5f70 6172 7365 5f73 6574  st_arg_parse_set
+000129c0: 7570 2729 0a20 2020 2064 6566 2074 6573  up').    def tes
+000129d0: 745f 7175 6965 745f 7265 6e65 7728 7365  t_quiet_renew(se
+000129e0: 6c66 2c20 5f29 3a0a 2020 2020 2020 2020  lf, _):.        
+000129f0: 7465 7374 5f75 7469 6c2e 6d61 6b65 5f6c  test_util.make_l
+00012a00: 696e 6561 6765 2873 656c 662e 636f 6e66  ineage(self.conf
+00012a10: 6967 2e63 6f6e 6669 675f 6469 722c 2027  ig.config_dir, '
+00012a20: 7361 6d70 6c65 2d72 656e 6577 616c 2e63  sample-renewal.c
+00012a30: 6f6e 6627 290a 2020 2020 2020 2020 6172  onf').        ar
+00012a40: 6773 203d 205b 2272 656e 6577 222c 2022  gs = ["renew", "
+00012a50: 2d2d 6472 792d 7275 6e22 5d0a 2020 2020  --dry-run"].    
+00012a60: 2020 2020 5f2c 205f 2c20 7374 646f 7574      _, _, stdout
+00012a70: 203d 2073 656c 662e 5f74 6573 745f 7265   = self._test_re
+00012a80: 6e65 7761 6c5f 636f 6d6d 6f6e 2854 7275  newal_common(Tru
+00012a90: 652c 205b 5d2c 2061 7267 733d 6172 6773  e, [], args=args
+00012aa0: 2c20 7368 6f75 6c64 5f72 656e 6577 3d54  , should_renew=T
+00012ab0: 7275 6529 0a20 2020 2020 2020 206f 7574  rue).        out
+00012ac0: 203d 2073 7464 6f75 742e 6765 7476 616c   = stdout.getval
+00012ad0: 7565 2829 0a20 2020 2020 2020 2061 7373  ue().        ass
+00012ae0: 6572 7420 2272 656e 6577 2220 696e 206f  ert "renew" in o
+00012af0: 7574 0a0a 2020 2020 2020 2020 6172 6773  ut..        args
+00012b00: 203d 205b 2272 656e 6577 222c 2022 2d2d   = ["renew", "--
+00012b10: 6472 792d 7275 6e22 2c20 222d 7122 5d0a  dry-run", "-q"].
+00012b20: 2020 2020 2020 2020 5f2c 205f 2c20 7374          _, _, st
+00012b30: 646f 7574 203d 2073 656c 662e 5f74 6573  dout = self._tes
+00012b40: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
+00012b50: 2854 7275 652c 205b 5d2c 2061 7267 733d  (True, [], args=
+00012b60: 6172 6773 2c0a 2020 2020 2020 2020 2020  args,.          
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2020 2020 2020 2073 686f 756c 645f 7265         should_re
+00012ba0: 6e65 773d 5472 7565 2c20 7175 6965 745f  new=True, quiet_
+00012bb0: 6d6f 6465 3d54 7275 6529 0a20 2020 2020  mode=True).     
+00012bc0: 2020 206f 7574 203d 2073 7464 6f75 742e     out = stdout.
+00012bd0: 6765 7476 616c 7565 2829 0a20 2020 2020  getvalue().     
+00012be0: 2020 2061 7373 6572 7420 2222 203d 3d20     assert "" == 
+00012bf0: 6f75 740a 0a20 2020 2064 6566 2074 6573  out..    def tes
+00012c00: 745f 7265 6e65 775f 686f 6f6b 5f76 616c  t_renew_hook_val
+00012c10: 6964 6174 696f 6e28 7365 6c66 293a 0a20  idation(self):. 
+00012c20: 2020 2020 2020 2074 6573 745f 7574 696c         test_util
+00012c30: 2e6d 616b 655f 6c69 6e65 6167 6528 7365  .make_lineage(se
+00012c40: 6c66 2e63 6f6e 6669 672e 636f 6e66 6967  lf.config.config
+00012c50: 5f64 6972 2c20 2773 616d 706c 652d 7265  _dir, 'sample-re
+00012c60: 6e65 7761 6c2e 636f 6e66 2729 0a20 2020  newal.conf').   
+00012c70: 2020 2020 2061 7267 7320 3d20 5b22 7265       args = ["re
+00012c80: 6e65 7722 2c20 222d 2d64 7279 2d72 756e  new", "--dry-run
+00012c90: 222c 2022 2d2d 706f 7374 2d68 6f6f 6b3d  ", "--post-hook=
+00012ca0: 6e6f 2d73 7563 682d 636f 6d6d 616e 6422  no-such-command"
+00012cb0: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
+00012cc0: 7465 7374 5f72 656e 6577 616c 5f63 6f6d  test_renewal_com
+00012cd0: 6d6f 6e28 5472 7565 2c20 5b5d 2c20 6172  mon(True, [], ar
+00012ce0: 6773 3d61 7267 732c 2073 686f 756c 645f  gs=args, should_
+00012cf0: 7265 6e65 773d 4661 6c73 652c 0a20 2020  renew=False,.   
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00012d20: 7272 6f72 5f65 7870 6563 7465 643d 5472  rror_expected=Tr
+00012d30: 7565 290a 0a20 2020 2064 6566 2074 6573  ue)..    def tes
+00012d40: 745f 7265 6e65 775f 6e6f 5f68 6f6f 6b5f  t_renew_no_hook_
+00012d50: 7661 6c69 6461 7469 6f6e 2873 656c 6629  validation(self)
+00012d60: 3a0a 2020 2020 2020 2020 7465 7374 5f75  :.        test_u
+00012d70: 7469 6c2e 6d61 6b65 5f6c 696e 6561 6765  til.make_lineage
+00012d80: 2873 656c 662e 636f 6e66 6967 2e63 6f6e  (self.config.con
+00012d90: 6669 675f 6469 722c 2027 7361 6d70 6c65  fig_dir, 'sample
+00012da0: 2d72 656e 6577 616c 2e63 6f6e 6627 290a  -renewal.conf').
+00012db0: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
+00012dc0: 2272 656e 6577 222c 2022 2d2d 6472 792d  "renew", "--dry-
+00012dd0: 7275 6e22 2c20 222d 2d70 6f73 742d 686f  run", "--post-ho
+00012de0: 6f6b 3d6e 6f2d 7375 6368 2d63 6f6d 6d61  ok=no-such-comma
+00012df0: 6e64 222c 0a20 2020 2020 2020 2020 2020  nd",.           
+00012e00: 2020 2020 2022 2d2d 6469 7361 626c 652d       "--disable-
+00012e10: 686f 6f6b 2d76 616c 6964 6174 696f 6e22  hook-validation"
+00012e20: 5d0a 2020 2020 2020 2020 7769 7468 206d  ].        with m
+00012e30: 6f63 6b2e 7061 7463 6828 2263 6572 7462  ock.patch("certb
+00012e40: 6f74 2e5f 696e 7465 726e 616c 2e68 6f6f  ot._internal.hoo
+00012e50: 6b73 2e70 6f73 745f 686f 6f6b 2229 3a0a  ks.post_hook"):.
+00012e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012e70: 2e5f 7465 7374 5f72 656e 6577 616c 5f63  ._test_renewal_c
+00012e80: 6f6d 6d6f 6e28 5472 7565 2c20 5b5d 2c20  ommon(True, [], 
+00012e90: 6172 6773 3d61 7267 732c 2073 686f 756c  args=args, shoul
+00012ea0: 645f 7265 6e65 773d 5472 7565 2c0a 2020  d_renew=True,.  
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00012ed0: 7365 7274 5f6f 635f 6361 6c6c 6564 3d54  sert_oc_called=T
-00012ee0: 7275 6529 0a0a 2020 2020 6465 6620 7465  rue)..    def te
-00012ef0: 7374 5f72 656e 6577 5f77 6974 685f 6261  st_renew_with_ba
-00012f00: 645f 646f 6d61 696e 2873 656c 6629 3a0a  d_domain(self):.
-00012f10: 2020 2020 2020 2020 7265 6e65 7761 6c70          renewalp
-00012f20: 6172 616d 7320 3d20 7b27 6175 7468 656e  arams = {'authen
-00012f30: 7469 6361 746f 7227 3a20 2777 6562 726f  ticator': 'webro
-00012f40: 6f74 277d 0a20 2020 2020 2020 206e 616d  ot'}.        nam
-00012f50: 6573 203d 205b 2775 6e69 c3a7 6f64 c3a9  es = ['uni..od..
-00012f60: 2e63 6f6d 275d 0a20 2020 2020 2020 2073  .com'].        s
-00012f70: 656c 662e 5f74 6573 745f 7265 6e65 775f  elf._test_renew_
-00012f80: 636f 6d6d 6f6e 2872 656e 6577 616c 7061  common(renewalpa
-00012f90: 7261 6d73 3d72 656e 6577 616c 7061 7261  rams=renewalpara
-00012fa0: 6d73 2c20 6572 726f 725f 6578 7065 6374  ms, error_expect
-00012fb0: 6564 3d54 7275 652c 0a20 2020 2020 2020  ed=True,.       
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fd0: 2020 2020 2020 2020 206e 616d 6573 3d6e           names=n
-00012fe0: 616d 6573 2c20 6173 7365 7274 5f6f 635f  ames, assert_oc_
-00012ff0: 6361 6c6c 6564 3d46 616c 7365 290a 0a20  called=False).. 
-00013000: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00013010: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00013020: 6c2e 706c 7567 696e 732e 7365 6c65 6374  l.plugins.select
-00013030: 696f 6e2e 6368 6f6f 7365 5f63 6f6e 6669  ion.choose_confi
-00013040: 6775 7261 746f 725f 706c 7567 696e 7327  gurator_plugins'
-00013050: 290a 2020 2020 6465 6620 7465 7374 5f72  ).    def test_r
-00013060: 656e 6577 5f77 6974 685f 636f 6e66 6967  enew_with_config
-00013070: 7572 6174 6f72 2873 656c 662c 206d 6f63  urator(self, moc
-00013080: 6b5f 7365 6c29 3a0a 2020 2020 2020 2020  k_sel):.        
-00013090: 6d6f 636b 5f73 656c 2e72 6574 7572 6e5f  mock_sel.return_
-000130a0: 7661 6c75 6520 3d20 286d 6f63 6b2e 4d61  value = (mock.Ma
-000130b0: 6769 634d 6f63 6b28 292c 206d 6f63 6b2e  gicMock(), mock.
-000130c0: 4d61 6769 634d 6f63 6b28 2929 0a20 2020  MagicMock()).   
-000130d0: 2020 2020 2072 656e 6577 616c 7061 7261       renewalpara
-000130e0: 6d73 203d 207b 2761 7574 6865 6e74 6963  ms = {'authentic
-000130f0: 6174 6f72 273a 2027 7765 6272 6f6f 7427  ator': 'webroot'
-00013100: 7d0a 2020 2020 2020 2020 7365 6c66 2e5f  }.        self._
-00013110: 7465 7374 5f72 656e 6577 5f63 6f6d 6d6f  test_renew_commo
-00013120: 6e28 0a20 2020 2020 2020 2020 2020 2072  n(.            r
-00013130: 656e 6577 616c 7061 7261 6d73 3d72 656e  enewalparams=ren
-00013140: 6577 616c 7061 7261 6d73 2c20 6173 7365  ewalparams, asse
-00013150: 7274 5f6f 635f 6361 6c6c 6564 3d54 7275  rt_oc_called=Tru
-00013160: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
-00013170: 7267 733d 2772 656e 6577 202d 2d63 6f6e  rgs='renew --con
-00013180: 6669 6775 7261 746f 7220 6170 6163 6865  figurator apache
-00013190: 272e 7370 6c69 7428 2929 0a0a 2020 2020  '.split())..    
-000131a0: 6465 6620 7465 7374 5f72 656e 6577 5f70  def test_renew_p
-000131b0: 6c75 6769 6e5f 636f 6e66 6967 5f72 6573  lugin_config_res
-000131c0: 746f 7261 7469 6f6e 2873 656c 6629 3a0a  toration(self):.
-000131d0: 2020 2020 2020 2020 7265 6e65 7761 6c70          renewalp
-000131e0: 6172 616d 7320 3d20 7b27 6175 7468 656e  arams = {'authen
-000131f0: 7469 6361 746f 7227 3a20 2777 6562 726f  ticator': 'webro
-00013200: 6f74 272c 0a20 2020 2020 2020 2020 2020  ot',.           
-00013210: 2020 2020 2020 2020 2020 2020 2020 2777                'w
-00013220: 6562 726f 6f74 5f70 6174 6827 3a20 274e  ebroot_path': 'N
-00013230: 6f6e 6527 2c0a 2020 2020 2020 2020 2020  one',.          
-00013240: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013250: 7765 6272 6f6f 745f 696d 6167 696e 6172  webroot_imaginar
-00013260: 795f 666c 6167 273a 2027 3432 277d 0a20  y_flag': '42'}. 
-00013270: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-00013280: 745f 7265 6e65 775f 636f 6d6d 6f6e 2872  t_renew_common(r
-00013290: 656e 6577 616c 7061 7261 6d73 3d72 656e  enewalparams=ren
-000132a0: 6577 616c 7061 7261 6d73 2c0a 2020 2020  ewalparams,.    
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132c0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000132d0: 7274 5f6f 635f 6361 6c6c 6564 3d54 7275  rt_oc_called=Tru
-000132e0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
-000132f0: 5f72 656e 6577 5f77 6974 685f 7765 6272  _renew_with_webr
-00013300: 6f6f 745f 6d61 7028 7365 6c66 293a 0a20  oot_map(self):. 
-00013310: 2020 2020 2020 2072 656e 6577 616c 7061         renewalpa
-00013320: 7261 6d73 203d 207b 2761 7574 6865 6e74  rams = {'authent
-00013330: 6963 6174 6f72 273a 2027 7765 6272 6f6f  icator': 'webroo
-00013340: 7427 7d0a 2020 2020 2020 2020 7365 6c66  t'}.        self
-00013350: 2e5f 7465 7374 5f72 656e 6577 5f63 6f6d  ._test_renew_com
-00013360: 6d6f 6e28 0a20 2020 2020 2020 2020 2020  mon(.           
-00013370: 2072 656e 6577 616c 7061 7261 6d73 3d72   renewalparams=r
-00013380: 656e 6577 616c 7061 7261 6d73 2c20 6173  enewalparams, as
-00013390: 7365 7274 5f6f 635f 6361 6c6c 6564 3d54  sert_oc_called=T
-000133a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000133b0: 2061 7267 733d 5b27 7265 6e65 7727 2c20   args=['renew', 
-000133c0: 272d 2d77 6562 726f 6f74 2d6d 6170 272c  '--webroot-map',
-000133d0: 206a 736f 6e2e 6475 6d70 7328 7b27 6578   json.dumps({'ex
-000133e0: 616d 706c 652e 636f 6d27 3a20 7465 6d70  ample.com': temp
-000133f0: 6669 6c65 2e67 6574 7465 6d70 6469 7228  file.gettempdir(
-00013400: 297d 295d 290a 0a20 2020 2064 6566 2074  )})])..    def t
-00013410: 6573 745f 7265 6e65 775f 7265 636f 6e73  est_renew_recons
-00013420: 7469 7475 7465 5f65 7272 6f72 2873 656c  titute_error(sel
-00013430: 6629 3a0a 2020 2020 2020 2020 2320 7079  f):.        # py
-00013440: 6c69 6e74 3a20 6469 7361 626c 653d 7072  lint: disable=pr
-00013450: 6f74 6563 7465 642d 6163 6365 7373 0a20  otected-access. 
-00013460: 2020 2020 2020 2077 6974 6820 6d6f 636b         with mock
-00013470: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-00013480: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e72  _internal.main.r
-00013490: 656e 6577 616c 2e72 6563 6f6e 7374 6974  enewal.reconstit
-000134a0: 7574 6527 2920 6173 206d 6f63 6b5f 7265  ute') as mock_re
-000134b0: 636f 6e73 7469 7475 7465 3a0a 2020 2020  constitute:.    
-000134c0: 2020 2020 2020 2020 6d6f 636b 5f72 6563          mock_rec
-000134d0: 6f6e 7374 6974 7574 652e 7369 6465 5f65  onstitute.side_e
-000134e0: 6666 6563 7420 3d20 4578 6365 7074 696f  ffect = Exceptio
-000134f0: 6e0a 2020 2020 2020 2020 2020 2020 7365  n.            se
-00013500: 6c66 2e5f 7465 7374 5f72 656e 6577 5f63  lf._test_renew_c
-00013510: 6f6d 6d6f 6e28 6173 7365 7274 5f6f 635f  ommon(assert_oc_
-00013520: 6361 6c6c 6564 3d46 616c 7365 2c20 6572  called=False, er
-00013530: 726f 725f 6578 7065 6374 6564 3d54 7275  ror_expected=Tru
-00013540: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
-00013550: 5f72 656e 6577 5f6f 6274 6169 6e5f 6365  _renew_obtain_ce
-00013560: 7274 5f65 7272 6f72 2873 656c 6629 3a0a  rt_error(self):.
-00013570: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
-00013580: 6b65 5f64 756d 6d79 5f72 656e 6577 616c  ke_dummy_renewal
-00013590: 5f63 6f6e 6669 6728 290a 2020 2020 2020  _config().      
-000135a0: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
-000135b0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-000135c0: 726e 616c 2e73 746f 7261 6765 2e52 656e  rnal.storage.Ren
-000135d0: 6577 6162 6c65 4365 7274 2729 2061 7320  ewableCert') as 
-000135e0: 6d6f 636b 5f72 633a 0a20 2020 2020 2020  mock_rc:.       
-000135f0: 2020 2020 206d 6f63 6b5f 6c69 6e65 6167       mock_lineag
-00013600: 6520 3d20 6d6f 636b 2e4d 6167 6963 4d6f  e = mock.MagicMo
-00013610: 636b 2829 0a20 2020 2020 2020 2020 2020  ck().           
-00013620: 206d 6f63 6b5f 6c69 6e65 6167 652e 6675   mock_lineage.fu
-00013630: 6c6c 6368 6169 6e20 3d20 2273 6f6d 6577  llchain = "somew
-00013640: 6865 7265 2f66 756c 6c63 6861 696e 2e70  here/fullchain.p
-00013650: 656d 220a 2020 2020 2020 2020 2020 2020  em".            
-00013660: 6d6f 636b 5f72 632e 7265 7475 726e 5f76  mock_rc.return_v
-00013670: 616c 7565 203d 206d 6f63 6b5f 6c69 6e65  alue = mock_line
-00013680: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
-00013690: 6d6f 636b 5f6c 696e 6561 6765 2e63 6f6e  mock_lineage.con
-000136a0: 6669 6775 7261 7469 6f6e 203d 207b 0a20  figuration = {. 
-000136b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000136c0: 7265 6e65 7761 6c70 6172 616d 7327 3a20  renewalparams': 
-000136d0: 7b27 6175 7468 656e 7469 6361 746f 7227  {'authenticator'
-000136e0: 3a20 2777 6562 726f 6f74 277d 7d0a 2020  : 'webroot'}}.  
-000136f0: 2020 2020 2020 2020 2020 7769 7468 206d            with m
-00013700: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00013710: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-00013720: 6e2e 7265 6e65 775f 6365 7274 2729 2061  n.renew_cert') a
-00013730: 7320 6d6f 636b 5f72 656e 6577 5f63 6572  s mock_renew_cer
-00013740: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00013750: 2020 206d 6f63 6b5f 7265 6e65 775f 6365     mock_renew_ce
-00013760: 7274 2e73 6964 655f 6566 6665 6374 203d  rt.side_effect =
-00013770: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
-00013780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013790: 5f74 6573 745f 7265 6e65 7761 6c5f 636f  _test_renewal_co
-000137a0: 6d6d 6f6e 2854 7275 652c 204e 6f6e 652c  mmon(True, None,
-000137b0: 2065 7272 6f72 5f65 7870 6563 7465 643d   error_expected=
-000137c0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137f0: 6172 6773 3d5b 2772 656e 6577 275d 2c20  args=['renew'], 
-00013800: 7368 6f75 6c64 5f72 656e 6577 3d46 616c  should_renew=Fal
-00013810: 7365 290a 0a20 2020 2064 6566 2074 6573  se)..    def tes
-00013820: 745f 7265 6e65 775f 7769 7468 5f62 6164  t_renew_with_bad
-00013830: 5f63 6c69 5f61 7267 7328 7365 6c66 293a  _cli_args(self):
-00013840: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00013850: 6573 745f 7265 6e65 7761 6c5f 636f 6d6d  est_renewal_comm
-00013860: 6f6e 2854 7275 652c 204e 6f6e 652c 2061  on(True, None, a
-00013870: 7267 733d 2772 656e 6577 202d 6420 6578  rgs='renew -d ex
-00013880: 616d 706c 652e 636f 6d27 2e73 706c 6974  ample.com'.split
-00013890: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
-000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 2020 7368 6f75 6c64 5f72 656e        should_ren
-000138c0: 6577 3d46 616c 7365 2c20 6572 726f 725f  ew=False, error_
-000138d0: 6578 7065 6374 6564 3d54 7275 6529 0a20  expected=True). 
-000138e0: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-000138f0: 745f 7265 6e65 7761 6c5f 636f 6d6d 6f6e  t_renewal_common
-00013900: 2854 7275 652c 204e 6f6e 652c 2061 7267  (True, None, arg
-00013910: 733d 2772 656e 6577 202d 2d63 7372 207b  s='renew --csr {
-00013920: 307d 272e 666f 726d 6174 2843 5352 292e  0}'.format(CSR).
-00013930: 7370 6c69 7428 292c 0a20 2020 2020 2020  split(),.       
-00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013950: 2020 2020 2020 2020 2020 2073 686f 756c             shoul
-00013960: 645f 7265 6e65 773d 4661 6c73 652c 2065  d_renew=False, e
-00013970: 7272 6f72 5f65 7870 6563 7465 643d 5472  rror_expected=Tr
-00013980: 7565 290a 0a20 2020 2064 6566 2074 6573  ue)..    def tes
-00013990: 745f 6e6f 5f72 656e 6577 616c 5f77 6974  t_no_renewal_wit
-000139a0: 685f 686f 6f6b 7328 7365 6c66 293a 0a20  h_hooks(self):. 
-000139b0: 2020 2020 2020 205f 2c20 5f2c 2073 7464         _, _, std
-000139c0: 6f75 7420 3d20 7365 6c66 2e5f 7465 7374  out = self._test
-000139d0: 5f72 656e 6577 616c 5f63 6f6d 6d6f 6e28  _renewal_common(
-000139e0: 0a20 2020 2020 2020 2020 2020 2064 7565  .            due
-000139f0: 5f66 6f72 5f72 656e 6577 616c 3d46 616c  _for_renewal=Fal
-00013a00: 7365 2c20 6578 7472 615f 6172 6773 3d4e  se, extra_args=N
-00013a10: 6f6e 652c 2073 686f 756c 645f 7265 6e65  one, should_rene
-00013a20: 773d 4661 6c73 652c 0a20 2020 2020 2020  w=False,.       
-00013a30: 2020 2020 2061 7267 733d 5b27 7265 6e65       args=['rene
-00013a40: 7727 2c20 272d 2d70 6f73 742d 686f 6f6b  w', '--post-hook
-00013a50: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00013a60: 2020 2020 2027 7b30 7d20 2d63 2022 7072       '{0} -c "pr
-00013a70: 696e 7428 5c27 6865 6c6c 6f20 776f 726c  int(\'hello worl
-00013a80: 645c 2729 3b22 270a 2020 2020 2020 2020  d\');"'.        
-00013a90: 2020 2020 2020 2020 2020 2e66 6f72 6d61            .forma
-00013aa0: 7428 7379 732e 6578 6563 7574 6162 6c65  t(sys.executable
-00013ab0: 295d 290a 2020 2020 2020 2020 6173 7365  )]).        asse
-00013ac0: 7274 2027 4e6f 2068 6f6f 6b73 2077 6572  rt 'No hooks wer
-00013ad0: 6520 7275 6e2e 2720 696e 2073 7464 6f75  e run.' in stdou
-00013ae0: 742e 6765 7476 616c 7565 2829 0a0a 2020  t.getvalue()..  
-00013af0: 2020 4074 6573 745f 7574 696c 2e70 6174    @test_util.pat
-00013b00: 6368 5f64 6973 706c 6179 5f75 7469 6c28  ch_display_util(
-00013b10: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
-00013b20: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00013b30: 726e 616c 2e6d 6169 6e2e 5f66 696e 645f  rnal.main._find_
-00013b40: 6c69 6e65 6167 655f 666f 725f 646f 6d61  lineage_for_doma
-00013b50: 696e 735f 616e 645f 6365 7274 6e61 6d65  ins_and_certname
-00013b60: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
-00013b70: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-00013b80: 6572 6e61 6c2e 6d61 696e 2e5f 696e 6974  ernal.main._init
-00013b90: 5f6c 655f 636c 6965 6e74 2729 0a20 2020  _le_client').   
-00013ba0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-00013bb0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00013bc0: 6d61 696e 2e5f 7265 706f 7274 5f6e 6577  main._report_new
-00013bd0: 5f63 6572 7427 290a 2020 2020 6465 6620  _cert').    def 
-00013be0: 7465 7374 5f63 6572 746f 6e6c 795f 7265  test_certonly_re
-00013bf0: 696e 7374 616c 6c28 7365 6c66 2c20 6d6f  install(self, mo
-00013c00: 636b 5f72 6570 6f72 745f 6e65 775f 6365  ck_report_new_ce
-00013c10: 7274 2c20 6d6f 636b 5f69 6e69 742c 0a20  rt, mock_init,. 
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00013c40: 6f63 6b5f 7265 6e65 7761 6c2c 206d 6f63  ock_renewal, moc
-00013c50: 6b5f 6765 745f 7574 696c 6974 7929 3a0a  k_get_utility):.
-00013c60: 2020 2020 2020 2020 6d6f 636b 5f72 656e          mock_ren
-00013c70: 6577 616c 2e72 6574 7572 6e5f 7661 6c75  ewal.return_valu
-00013c80: 6520 3d20 2827 7265 696e 7374 616c 6c27  e = ('reinstall'
-00013c90: 2c20 6d6f 636b 2e4d 6167 6963 4d6f 636b  , mock.MagicMock
-00013ca0: 2829 290a 2020 2020 2020 2020 6d6f 636b  ()).        mock
-00013cb0: 5f69 6e69 742e 7265 7475 726e 5f76 616c  _init.return_val
-00013cc0: 7565 203d 206d 6f63 6b5f 636c 6965 6e74  ue = mock_client
-00013cd0: 203d 206d 6f63 6b2e 4d61 6769 634d 6f63   = mock.MagicMoc
-00013ce0: 6b28 290a 2020 2020 2020 2020 7365 6c66  k().        self
-00013cf0: 2e5f 6361 6c6c 285b 272d 6427 2c20 2766  ._call(['-d', 'f
-00013d00: 6f6f 2e62 6172 272c 2027 2d61 272c 2027  oo.bar', '-a', '
-00013d10: 7374 616e 6461 6c6f 6e65 272c 2027 6365  standalone', 'ce
-00013d20: 7274 6f6e 6c79 275d 290a 2020 2020 2020  rtonly']).      
-00013d30: 2020 6173 7365 7274 206d 6f63 6b5f 636c    assert mock_cl
-00013d40: 6965 6e74 2e6f 6274 6169 6e5f 6365 7274  ient.obtain_cert
-00013d50: 6966 6963 6174 652e 6361 6c6c 6564 2069  ificate.called i
-00013d60: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
-00013d70: 6173 7365 7274 206d 6f63 6b5f 636c 6965  assert mock_clie
-00013d80: 6e74 2e6f 6274 6169 6e5f 616e 645f 656e  nt.obtain_and_en
-00013d90: 726f 6c6c 5f63 6572 7469 6669 6361 7465  roll_certificate
-00013da0: 2e63 616c 6c65 6420 6973 2046 616c 7365  .called is False
-00013db0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00013dc0: 6d6f 636b 5f67 6574 5f75 7469 6c69 7479  mock_get_utility
-00013dd0: 2829 2e61 6464 5f6d 6573 7361 6765 2e63  ().add_message.c
-00013de0: 616c 6c5f 636f 756e 7420 3d3d 2030 0a20  all_count == 0. 
-00013df0: 2020 2020 2020 206d 6f63 6b5f 7265 706f         mock_repo
-00013e00: 7274 5f6e 6577 5f63 6572 742e 6173 7365  rt_new_cert.asse
-00013e10: 7274 5f6e 6f74 5f63 616c 6c65 6428 290a  rt_not_called().
-00013e20: 2020 2020 2020 2020 2373 656c 662e 6173          #self.as
-00013e30: 7365 7274 5472 7565 2827 646f 6e61 7465  sertTrue('donate
-00013e40: 2720 6e6f 7420 696e 206d 6f63 6b5f 6765  ' not in mock_ge
-00013e50: 745f 7574 696c 6974 7928 292e 6164 645f  t_utility().add_
-00013e60: 6d65 7373 6167 652e 6361 6c6c 5f61 7267  message.call_arg
-00013e70: 735b 305d 5b30 5d29 0a0a 2020 2020 6465  s[0][0])..    de
-00013e80: 6620 5f74 6573 745f 6365 7274 6f6e 6c79  f _test_certonly
-00013e90: 5f63 7372 5f63 6f6d 6d6f 6e28 7365 6c66  _csr_common(self
-00013ea0: 2c20 6578 7472 615f 6172 6773 3d4e 6f6e  , extra_args=Non
-00013eb0: 6529 3a0a 2020 2020 2020 2020 6365 7274  e):.        cert
-00013ec0: 7220 3d20 2763 6572 7472 270a 2020 2020  r = 'certr'.    
-00013ed0: 2020 2020 6368 6169 6e20 3d20 2763 6861      chain = 'cha
-00013ee0: 696e 270a 2020 2020 2020 2020 6d6f 636b  in'.        mock
-00013ef0: 5f63 6c69 656e 7420 3d20 6d6f 636b 2e4d  _client = mock.M
-00013f00: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-00013f10: 2020 206d 6f63 6b5f 636c 6965 6e74 2e6f     mock_client.o
-00013f20: 6274 6169 6e5f 6365 7274 6966 6963 6174  btain_certificat
-00013f30: 655f 6672 6f6d 5f63 7372 2e72 6574 7572  e_from_csr.retur
-00013f40: 6e5f 7661 6c75 6520 3d20 2863 6572 7472  n_value = (certr
-00013f50: 2c20 6368 6169 6e29 0a20 2020 2020 2020  , chain).       
-00013f60: 2063 6572 745f 7061 7468 203d 206f 732e   cert_path = os.
-00013f70: 7061 7468 2e6e 6f72 6d70 6174 6828 6f73  path.normpath(os
-00013f80: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00013f90: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00013fa0: 6669 672e 636f 6e66 6967 5f64 6972 2c0a  fig.config_dir,.
-00013fb0: 2020 2020 2020 2020 2020 2020 276c 6976              'liv
-00013fc0: 652f 6578 616d 706c 652e 636f 6d2f 6365  e/example.com/ce
-00013fd0: 7274 5f35 3132 2e70 656d 2729 290a 2020  rt_512.pem')).  
-00013fe0: 2020 2020 2020 6675 6c6c 5f70 6174 6820        full_path 
-00013ff0: 3d20 6f73 2e70 6174 682e 6e6f 726d 7061  = os.path.normpa
-00014000: 7468 286f 732e 7061 7468 2e6a 6f69 6e28  th(os.path.join(
-00014010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014020: 662e 636f 6e66 6967 2e63 6f6e 6669 675f  f.config.config_
-00014030: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
-00014040: 2027 6c69 7665 2f65 7861 6d70 6c65 2e63   'live/example.c
-00014050: 6f6d 2f66 756c 6c63 6861 696e 2e70 656d  om/fullchain.pem
-00014060: 2729 290a 2020 2020 2020 2020 6d6f 636b  ')).        mock
-00014070: 5f63 6c69 656e 742e 7361 7665 5f63 6572  _client.save_cer
-00014080: 7469 6669 6361 7465 2e72 6574 7572 6e5f  tificate.return_
-00014090: 7661 6c75 6520 3d20 6365 7274 5f70 6174  value = cert_pat
-000140a0: 682c 204e 6f6e 652c 2066 756c 6c5f 7061  h, None, full_pa
-000140b0: 7468 0a20 2020 2020 2020 2077 6974 6820  th.        with 
-000140c0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-000140d0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-000140e0: 696e 2e5f 696e 6974 5f6c 655f 636c 6965  in._init_le_clie
-000140f0: 6e74 2729 2061 7320 6d6f 636b 5f69 6e69  nt') as mock_ini
-00014100: 743a 0a20 2020 2020 2020 2020 2020 206d  t:.            m
-00014110: 6f63 6b5f 696e 6974 2e72 6574 7572 6e5f  ock_init.return_
-00014120: 7661 6c75 6520 3d20 6d6f 636b 5f63 6c69  value = mock_cli
-00014130: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-00014140: 6368 6169 6e5f 7061 7468 203d 206f 732e  chain_path = os.
-00014150: 7061 7468 2e6e 6f72 6d70 6174 6828 6f73  path.normpath(os
-00014160: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00014170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014180: 2e63 6f6e 6669 672e 636f 6e66 6967 5f64  .config.config_d
-00014190: 6972 2c0a 2020 2020 2020 2020 2020 2020  ir,.            
-000141a0: 2020 2020 276c 6976 652f 6578 616d 706c      'live/exampl
-000141b0: 652e 636f 6d2f 6368 6169 6e2e 7065 6d27  e.com/chain.pem'
-000141c0: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
-000141d0: 7267 7320 3d20 2827 2d61 2073 7461 6e64  rgs = ('-a stand
-000141e0: 616c 6f6e 6520 6365 7274 6f6e 6c79 202d  alone certonly -
-000141f0: 2d63 7372 207b 307d 202d 2d63 6572 742d  -csr {0} --cert-
-00014200: 7061 7468 207b 317d 2027 0a20 2020 2020  path {1} '.     
-00014210: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014220: 2d2d 6368 6169 6e2d 7061 7468 207b 327d  --chain-path {2}
-00014230: 202d 2d66 756c 6c63 6861 696e 2d70 6174   --fullchain-pat
-00014240: 6820 7b33 7d27 292e 666f 726d 6174 280a  h {3}').format(.
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2020 2020 2020 2020 4353 522c 2063 6572          CSR, cer
-00014270: 745f 7061 7468 2c20 6368 6169 6e5f 7061  t_path, chain_pa
-00014280: 7468 2c20 6675 6c6c 5f70 6174 6829 2e73  th, full_path).s
-00014290: 706c 6974 2829 0a20 2020 2020 2020 2020  plit().         
-000142a0: 2020 2069 6620 6578 7472 615f 6172 6773     if extra_args
-000142b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000142c0: 2020 6172 6773 202b 3d20 6578 7472 615f    args += extra_
-000142d0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-000142e0: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
-000142f0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00014300: 6e61 6c2e 6d61 696e 2e63 7279 7074 6f5f  nal.main.crypto_
-00014310: 7574 696c 2729 3a0a 2020 2020 2020 2020  util'):.        
-00014320: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-00014330: 6c6c 2861 7267 7329 0a0a 2020 2020 2020  ll(args)..      
-00014340: 2020 6966 2027 2d2d 6472 792d 7275 6e27    if '--dry-run'
-00014350: 2069 6e20 6172 6773 3a0a 2020 2020 2020   in args:.      
-00014360: 2020 2020 2020 6173 7365 7274 206d 6f63        assert moc
-00014370: 6b5f 636c 6965 6e74 2e73 6176 655f 6365  k_client.save_ce
-00014380: 7274 6966 6963 6174 652e 6361 6c6c 6564  rtificate.called
-00014390: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
-000143a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000143b0: 2020 2020 6d6f 636b 5f63 6c69 656e 742e      mock_client.
-000143c0: 7361 7665 5f63 6572 7469 6669 6361 7465  save_certificate
-000143d0: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
-000143e0: 6e63 655f 7769 7468 280a 2020 2020 2020  nce_with(.      
-000143f0: 2020 2020 2020 2020 2020 6365 7274 722c            certr,
-00014400: 2063 6861 696e 2c20 6365 7274 5f70 6174   chain, cert_pat
-00014410: 682c 2063 6861 696e 5f70 6174 682c 2066  h, chain_path, f
-00014420: 756c 6c5f 7061 7468 290a 0a20 2020 2040  ull_path)..    @
-00014430: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00014440: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00014450: 696e 2e5f 6373 725f 7265 706f 7274 5f6e  in._csr_report_n
-00014460: 6577 5f63 6572 7427 290a 2020 2020 406d  ew_cert').    @m
-00014470: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00014480: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-00014490: 6e2e 7574 696c 2e61 7465 7869 745f 7265  n.util.atexit_re
-000144a0: 6769 7374 6572 2729 0a20 2020 2040 6d6f  gister').    @mo
-000144b0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-000144c0: 742e 5f69 6e74 6572 6e61 6c2e 6566 662e  t._internal.eff.
-000144d0: 6861 6e64 6c65 5f73 7562 7363 7269 7074  handle_subscript
-000144e0: 696f 6e27 290a 2020 2020 6465 6620 7465  ion').    def te
-000144f0: 7374 5f63 6572 746f 6e6c 795f 6373 7228  st_certonly_csr(
-00014500: 7365 6c66 2c20 6d6f 636b 5f73 7562 7363  self, mock_subsc
-00014510: 7269 7074 696f 6e2c 206d 6f63 6b5f 7265  ription, mock_re
-00014520: 6769 7374 6572 2c20 6d6f 636b 5f63 7372  gister, mock_csr
-00014530: 5f72 6570 6f72 7429 3a0a 2020 2020 2020  _report):.      
-00014540: 2020 7365 6c66 2e5f 7465 7374 5f63 6572    self._test_cer
-00014550: 746f 6e6c 795f 6373 725f 636f 6d6d 6f6e  tonly_csr_common
-00014560: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
-00014570: 7420 6d6f 636b 5f63 7372 5f72 6570 6f72  t mock_csr_repor
-00014580: 742e 6361 6c6c 5f63 6f75 6e74 203d 3d20  t.call_count == 
-00014590: 310a 2020 2020 2020 2020 6173 7365 7274  1.        assert
-000145a0: 2027 6365 7274 5f35 3132 2e70 656d 2720   'cert_512.pem' 
-000145b0: 696e 206d 6f63 6b5f 6373 725f 7265 706f  in mock_csr_repo
-000145c0: 7274 2e63 616c 6c5f 6172 6773 5b30 5d5b  rt.call_args[0][
-000145d0: 315d 0a20 2020 2020 2020 2061 7373 6572  1].        asser
-000145e0: 7420 6d6f 636b 5f63 7372 5f72 6570 6f72  t mock_csr_repor
-000145f0: 742e 6361 6c6c 5f61 7267 735b 305d 5b32  t.call_args[0][2
-00014600: 5d20 6973 204e 6f6e 650a 2020 2020 2020  ] is None.      
-00014610: 2020 6173 7365 7274 2027 6675 6c6c 6368    assert 'fullch
-00014620: 6169 6e2e 7065 6d27 2069 6e20 6d6f 636b  ain.pem' in mock
-00014630: 5f63 7372 5f72 6570 6f72 742e 6361 6c6c  _csr_report.call
-00014640: 5f61 7267 735b 305d 5b33 5d0a 2020 2020  _args[0][3].    
-00014650: 2020 2020 6173 7365 7274 2027 646f 6e61      assert 'dona
-00014660: 7465 2720 696e 206d 6f63 6b5f 7265 6769  te' in mock_regi
-00014670: 7374 6572 2e63 616c 6c5f 6172 6773 5b30  ster.call_args[0
-00014680: 5d5b 315d 0a20 2020 2020 2020 2061 7373  ][1].        ass
-00014690: 6572 7420 6d6f 636b 5f73 7562 7363 7269  ert mock_subscri
-000146a0: 7074 696f 6e2e 6361 6c6c 6564 2069 7320  ption.called is 
-000146b0: 5472 7565 0a0a 2020 2020 406d 6f63 6b2e  True..    @mock.
-000146c0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-000146d0: 696e 7465 726e 616c 2e6d 6169 6e2e 5f63  internal.main._c
-000146e0: 7372 5f72 6570 6f72 745f 6e65 775f 6365  sr_report_new_ce
-000146f0: 7274 2729 0a20 2020 2064 6566 2074 6573  rt').    def tes
-00014700: 745f 6365 7274 6f6e 6c79 5f63 7372 5f64  t_certonly_csr_d
-00014710: 7279 5f72 756e 2873 656c 662c 206d 6f63  ry_run(self, moc
-00014720: 6b5f 6373 725f 7265 706f 7274 293a 0a20  k_csr_report):. 
-00014730: 2020 2020 2020 2073 656c 662e 5f74 6573         self._tes
-00014740: 745f 6365 7274 6f6e 6c79 5f63 7372 5f63  t_certonly_csr_c
-00014750: 6f6d 6d6f 6e28 5b27 2d2d 6472 792d 7275  ommon(['--dry-ru
-00014760: 6e27 5d29 0a20 2020 2020 2020 2061 7373  n']).        ass
-00014770: 6572 7420 6d6f 636b 5f63 7372 5f72 6570  ert mock_csr_rep
-00014780: 6f72 742e 6361 6c6c 5f63 6f75 6e74 203d  ort.call_count =
-00014790: 3d20 310a 2020 2020 2020 2020 6173 7365  = 1.        asse
-000147a0: 7274 206d 6f63 6b5f 6373 725f 7265 706f  rt mock_csr_repo
-000147b0: 7274 2e63 616c 6c5f 6172 6773 5b30 5d5b  rt.call_args[0][
-000147c0: 305d 2e64 7279 5f72 756e 2069 7320 5472  0].dry_run is Tr
-000147d0: 7565 0a0a 2020 2020 406d 6f63 6b2e 7061  ue..    @mock.pa
-000147e0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-000147f0: 7465 726e 616c 2e6d 6169 6e2e 5f64 656c  ternal.main._del
-00014800: 6574 655f 6966 5f61 7070 726f 7072 6961  ete_if_appropria
-00014810: 7465 2729 0a20 2020 2040 6d6f 636b 2e70  te').    @mock.p
-00014820: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00014830: 6e74 6572 6e61 6c2e 6d61 696e 2e63 6c69  nternal.main.cli
-00014840: 656e 742e 6163 6d65 5f63 6c69 656e 7427  ent.acme_client'
-00014850: 290a 2020 2020 6465 6620 7465 7374 5f72  ).    def test_r
-00014860: 6576 6f6b 655f 7769 7468 5f6b 6579 2873  evoke_with_key(s
-00014870: 656c 662c 206d 6f63 6b5f 6163 6d65 5f63  elf, mock_acme_c
-00014880: 6c69 656e 742c 0a20 2020 2020 2020 2020  lient,.         
-00014890: 2020 206d 6f63 6b5f 6465 6c65 7465 5f69     mock_delete_i
-000148a0: 665f 6170 7072 6f70 7269 6174 6529 3a0a  f_appropriate):.
-000148b0: 2020 2020 2020 2020 6d6f 636b 5f64 656c          mock_del
-000148c0: 6574 655f 6966 5f61 7070 726f 7072 6961  ete_if_appropria
-000148d0: 7465 2e72 6574 7572 6e5f 7661 6c75 6520  te.return_value 
-000148e0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-000148f0: 7365 7276 6572 203d 2027 666f 6f2e 6261  server = 'foo.ba
-00014900: 7227 0a20 2020 2020 2020 2073 656c 662e  r'.        self.
-00014910: 5f63 616c 6c5f 6e6f 5f63 6c69 656e 746d  _call_no_clientm
-00014920: 6f63 6b28 5b27 2d2d 6365 7274 2d70 6174  ock(['--cert-pat
-00014930: 6827 2c20 5353 5f43 4552 545f 5041 5448  h', SS_CERT_PATH
-00014940: 2c20 272d 2d6b 6579 2d70 6174 6827 2c20  , '--key-path', 
-00014950: 5253 4132 3034 385f 4b45 595f 5041 5448  RSA2048_KEY_PATH
-00014960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 2027 2d2d 7365 7276 6572 272c 2073     '--server', s
-00014990: 6572 7665 722c 2027 7265 766f 6b65 275d  erver, 'revoke']
-000149a0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
-000149b0: 7065 6e28 5253 4132 3034 385f 4b45 595f  pen(RSA2048_KEY_
-000149c0: 5041 5448 2c20 2772 6227 2920 6173 2066  PATH, 'rb') as f
-000149d0: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-000149e0: 7365 7274 206d 6f63 6b5f 6163 6d65 5f63  sert mock_acme_c
-000149f0: 6c69 656e 742e 436c 6965 6e74 5632 2e63  lient.ClientV2.c
-00014a00: 616c 6c5f 636f 756e 7420 3d3d 2031 0a20  all_count == 1. 
-00014a10: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00014a20: 7420 6d6f 636b 5f61 636d 655f 636c 6965  t mock_acme_clie
-00014a30: 6e74 2e43 6c69 656e 744e 6574 776f 726b  nt.ClientNetwork
-00014a40: 2e63 616c 6c5f 6172 6773 5b30 5d5b 305d  .call_args[0][0]
-00014a50: 203d 3d20 5c0a 2020 2020 2020 2020 2020   == \.          
-00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a70: 2020 206a 6f73 652e 4a57 4b2e 6c6f 6164     jose.JWK.load
-00014a80: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
-00014a90: 2020 2077 6974 6820 6f70 656e 2853 535f     with open(SS_
-00014aa0: 4345 5254 5f50 4154 482c 2027 7262 2729  CERT_PATH, 'rb')
-00014ab0: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
-00014ac0: 2020 2063 6572 7420 3d20 6372 7970 746f     cert = crypto
-00014ad0: 5f75 7469 6c2e 7079 6f70 656e 7373 6c5f  _util.pyopenssl_
-00014ae0: 6c6f 6164 5f63 6572 7469 6669 6361 7465  load_certificate
-00014af0: 2866 2e72 6561 6428 2929 5b30 5d0a 2020  (f.read())[0].  
-00014b00: 2020 2020 2020 2020 2020 6d6f 636b 5f72            mock_r
-00014b10: 6576 6f6b 6520 3d20 6d6f 636b 5f61 636d  evoke = mock_acm
-00014b20: 655f 636c 6965 6e74 2e43 6c69 656e 7456  e_client.ClientV
-00014b30: 3228 292e 7265 766f 6b65 0a20 2020 2020  2().revoke.     
-00014b40: 2020 2020 2020 206d 6f63 6b5f 7265 766f         mock_revo
-00014b50: 6b65 2e61 7373 6572 745f 6361 6c6c 6564  ke.assert_called
-00014b60: 5f6f 6e63 655f 7769 7468 280a 2020 2020  _once_with(.    
-00014b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b80: 6a6f 7365 2e43 6f6d 7061 7261 626c 6558  jose.ComparableX
-00014b90: 3530 3928 6365 7274 292c 0a20 2020 2020  509(cert),.     
-00014ba0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00014bb0: 6f63 6b2e 414e 5929 0a0a 2020 2020 6465  ock.ANY)..    de
-00014bc0: 6620 7465 7374 5f72 6576 6f6b 655f 7769  f test_revoke_wi
-00014bd0: 7468 5f6b 6579 5f6d 6973 6d61 7463 6828  th_key_mismatch(
-00014be0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00014bf0: 6572 7665 7220 3d20 2766 6f6f 2e62 6172  erver = 'foo.bar
-00014c00: 270a 2020 2020 2020 2020 7769 7468 2070  '.        with p
-00014c10: 7974 6573 742e 7261 6973 6573 2865 7272  ytest.raises(err
-00014c20: 6f72 732e 4572 726f 7229 3a0a 2020 2020  ors.Error):.    
-00014c30: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-00014c40: 6c6c 5f6e 6f5f 636c 6965 6e74 6d6f 636b  ll_no_clientmock
-00014c50: 285b 272d 2d63 6572 742d 7061 7468 272c  (['--cert-path',
-00014c60: 2043 4552 542c 2027 2d2d 6b65 792d 7061   CERT, '--key-pa
-00014c70: 7468 272c 204b 4559 2c0a 2020 2020 2020  th', KEY,.      
-00014c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c90: 2020 2020 2020 2020 2020 2027 2d2d 7365             '--se
-00014ca0: 7276 6572 272c 2073 6572 7665 722c 2027  rver', server, '
-00014cb0: 7265 766f 6b65 275d 290a 0a20 2020 2040  revoke'])..    @
-00014cc0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00014cd0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00014ce0: 696e 2e5f 6465 6c65 7465 5f69 665f 6170  in._delete_if_ap
-00014cf0: 7072 6f70 7269 6174 6527 290a 2020 2020  propriate').    
-00014d00: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-00014d10: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-00014d20: 6169 6e2e 5f64 6574 6572 6d69 6e65 5f61  ain._determine_a
-00014d30: 6363 6f75 6e74 2729 0a20 2020 2064 6566  ccount').    def
-00014d40: 2074 6573 745f 7265 766f 6b65 5f77 6974   test_revoke_wit
-00014d50: 686f 7574 5f6b 6579 2873 656c 662c 206d  hout_key(self, m
-00014d60: 6f63 6b5f 6465 7465 726d 696e 655f 6163  ock_determine_ac
-00014d70: 636f 756e 742c 0a20 2020 2020 2020 2020  count,.         
-00014d80: 2020 206d 6f63 6b5f 6465 6c65 7465 5f69     mock_delete_i
-00014d90: 665f 6170 7072 6f70 7269 6174 6529 3a0a  f_appropriate):.
-00014da0: 2020 2020 2020 2020 6d6f 636b 5f64 656c          mock_del
-00014db0: 6574 655f 6966 5f61 7070 726f 7072 6961  ete_if_appropria
-00014dc0: 7465 2e72 6574 7572 6e5f 7661 6c75 6520  te.return_value 
-00014dd0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00014de0: 6d6f 636b 5f64 6574 6572 6d69 6e65 5f61  mock_determine_a
-00014df0: 6363 6f75 6e74 2e72 6574 7572 6e5f 7661  ccount.return_va
-00014e00: 6c75 6520 3d20 286d 6f63 6b2e 4d61 6769  lue = (mock.Magi
-00014e10: 634d 6f63 6b28 292c 204e 6f6e 6529 0a20  cMock(), None). 
-00014e20: 2020 2020 2020 205f 2c20 5f2c 205f 2c20         _, _, _, 
-00014e30: 636c 6965 6e74 203d 2073 656c 662e 5f63  client = self._c
-00014e40: 616c 6c28 5b27 2d2d 6365 7274 2d70 6174  all(['--cert-pat
-00014e50: 6827 2c20 4345 5254 2c20 2772 6576 6f6b  h', CERT, 'revok
-00014e60: 6527 5d29 0a20 2020 2020 2020 2077 6974  e']).        wit
-00014e70: 6820 6f70 656e 2843 4552 5429 2061 7320  h open(CERT) as 
-00014e80: 663a 0a20 2020 2020 2020 2020 2020 2063  f:.            c
-00014e90: 6572 7420 3d20 6372 7970 746f 5f75 7469  ert = crypto_uti
-00014ea0: 6c2e 7079 6f70 656e 7373 6c5f 6c6f 6164  l.pyopenssl_load
-00014eb0: 5f63 6572 7469 6669 6361 7465 2866 2e72  _certificate(f.r
-00014ec0: 6561 6428 2929 5b30 5d0a 2020 2020 2020  ead())[0].      
-00014ed0: 2020 2020 2020 6d6f 636b 5f72 6576 6f6b        mock_revok
-00014ee0: 6520 3d20 636c 6965 6e74 2e61 636d 655f  e = client.acme_
-00014ef0: 6672 6f6d 5f63 6f6e 6669 675f 6b65 7928  from_config_key(
-00014f00: 292e 7265 766f 6b65 0a20 2020 2020 2020  ).revoke.       
-00014f10: 2020 2020 206d 6f63 6b5f 7265 766f 6b65       mock_revoke
-00014f20: 2e61 7373 6572 745f 6361 6c6c 6564 5f6f  .assert_called_o
-00014f30: 6e63 655f 7769 7468 280a 2020 2020 2020  nce_with(.      
-00014f40: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
-00014f50: 7365 2e43 6f6d 7061 7261 626c 6558 3530  se.ComparableX50
-00014f60: 3928 6365 7274 292c 0a20 2020 2020 2020  9(cert),.       
-00014f70: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
-00014f80: 6b2e 414e 5929 0a0a 2020 2020 406d 6f63  k.ANY)..    @moc
-00014f90: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-00014fa0: 2e5f 696e 7465 726e 616c 2e6c 6f67 2e70  ._internal.log.p
-00014fb0: 6f73 745f 6172 675f 7061 7273 655f 7365  ost_arg_parse_se
-00014fc0: 7475 7027 290a 2020 2020 6465 6620 7465  tup').    def te
-00014fd0: 7374 5f72 6567 6973 7465 7228 7365 6c66  st_register(self
-00014fe0: 2c20 5f29 3a0a 2020 2020 2020 2020 7769  , _):.        wi
-00014ff0: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-00015000: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00015010: 2e6d 6169 6e2e 636c 6965 6e74 2729 2061  .main.client') a
-00015020: 7320 6d6f 636b 6564 5f63 6c69 656e 743a  s mocked_client:
-00015030: 0a20 2020 2020 2020 2020 2020 2061 6363  .            acc
-00015040: 203d 206d 6f63 6b2e 4d61 6769 634d 6f63   = mock.MagicMoc
-00015050: 6b28 290a 2020 2020 2020 2020 2020 2020  k().            
-00015060: 6163 632e 6964 203d 2022 696d 6167 696e  acc.id = "imagin
-00015070: 6172 795f 6163 636f 756e 7422 0a20 2020  ary_account".   
-00015080: 2020 2020 2020 2020 206d 6f63 6b65 645f           mocked_
-00015090: 636c 6965 6e74 2e72 6567 6973 7465 722e  client.register.
-000150a0: 7265 7475 726e 5f76 616c 7565 203d 2028  return_value = (
-000150b0: 6163 632c 2022 776f 726b 6564 2229 0a20  acc, "worked"). 
-000150c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000150d0: 5f63 616c 6c5f 6e6f 5f63 6c69 656e 746d  _call_no_clientm
-000150e0: 6f63 6b28 5b22 7265 6769 7374 6572 222c  ock(["register",
-000150f0: 2022 2d2d 656d 6169 6c22 2c20 2275 7365   "--email", "use
-00015100: 7240 6578 616d 706c 652e 6f72 6722 5d29  r@example.org"])
-00015110: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00015120: 4f44 4f3a 2049 7420 776f 756c 6420 6265  ODO: It would be
-00015130: 206d 6f72 6520 636f 7272 6563 7420 746f   more correct to
-00015140: 2065 7870 6c69 6369 746c 7920 6368 6563   explicitly chec
-00015150: 6b20 7468 6174 0a20 2020 2020 2020 2020  k that.         
-00015160: 2020 2023 2020 2020 2020 205f 6465 7465     #       _dete
-00015170: 726d 696e 655f 6163 636f 756e 7428 2920  rmine_account() 
-00015180: 6765 7473 2063 616c 6c65 6420 696e 2074  gets called in t
-00015190: 6865 2061 626f 7665 2063 6173 652c 0a20  he above case,. 
-000151a0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-000151b0: 2020 2062 7574 2063 6f76 6572 6167 6520     but coverage 
-000151c0: 7374 6174 6973 7469 6373 2073 686f 756c  statistics shoul
-000151d0: 6420 616c 736f 2073 686f 7720 7468 6174  d also show that
-000151e0: 2069 7420 6469 642e 0a20 2020 2020 2020   it did..       
-000151f0: 2020 2020 2077 6974 6820 6d6f 636b 2e70       with mock.p
-00015200: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00015210: 6e74 6572 6e61 6c2e 6d61 696e 2e61 6363  nternal.main.acc
-00015220: 6f75 6e74 2729 2061 7320 6d6f 636b 6564  ount') as mocked
-00015230: 5f61 6363 6f75 6e74 3a0a 2020 2020 2020  _account:.      
-00015240: 2020 2020 2020 2020 2020 6d6f 636b 6564            mocked
-00015250: 5f73 746f 7261 6765 203d 206d 6f63 6b2e  _storage = mock.
-00015260: 4d61 6769 634d 6f63 6b28 290a 2020 2020  MagicMock().    
-00015270: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-00015280: 6564 5f61 6363 6f75 6e74 2e41 6363 6f75  ed_account.Accou
-00015290: 6e74 4669 6c65 5374 6f72 6167 652e 7265  ntFileStorage.re
-000152a0: 7475 726e 5f76 616c 7565 203d 206d 6f63  turn_value = moc
-000152b0: 6b65 645f 7374 6f72 6167 650a 2020 2020  ked_storage.    
-000152c0: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-000152d0: 6564 5f73 746f 7261 6765 2e66 696e 645f  ed_storage.find_
-000152e0: 616c 6c2e 7265 7475 726e 5f76 616c 7565  all.return_value
-000152f0: 203d 205b 2261 6e20 6163 636f 756e 7422   = ["an account"
-00015300: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015310: 2020 7820 3d20 7365 6c66 2e5f 6361 6c6c    x = self._call
-00015320: 5f6e 6f5f 636c 6965 6e74 6d6f 636b 285b  _no_clientmock([
-00015330: 2272 6567 6973 7465 7222 2c20 222d 2d65  "register", "--e
-00015340: 6d61 696c 222c 2022 7573 6572 4065 7861  mail", "user@exa
-00015350: 6d70 6c65 2e6f 7267 225d 290a 2020 2020  mple.org"]).    
-00015360: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00015370: 7274 2022 5468 6572 6520 6973 2061 6e20  rt "There is an 
-00015380: 6578 6973 7469 6e67 2061 6363 6f75 6e74  existing account
-00015390: 2220 696e 2078 5b30 5d0a 0a20 2020 2040  " in x[0]..    @
-000153a0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-000153b0: 626f 742e 5f69 6e74 6572 6e61 6c2e 706c  bot._internal.pl
-000153c0: 7567 696e 732e 7365 6c65 6374 696f 6e2e  ugins.selection.
-000153d0: 6368 6f6f 7365 5f63 6f6e 6669 6775 7261  choose_configura
-000153e0: 746f 725f 706c 7567 696e 7327 290a 2020  tor_plugins').  
-000153f0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-00015400: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00015410: 2e75 7064 6174 6572 2e5f 7275 6e5f 7570  .updater._run_up
-00015420: 6461 7465 7273 2729 0a20 2020 2064 6566  daters').    def
-00015430: 2074 6573 745f 706c 7567 696e 5f73 656c   test_plugin_sel
-00015440: 6563 7469 6f6e 5f65 7272 6f72 2873 656c  ection_error(sel
-00015450: 662c 206d 6f63 6b5f 7275 6e2c 206d 6f63  f, mock_run, moc
-00015460: 6b5f 6368 6f6f 7365 293a 0a20 2020 2020  k_choose):.     
-00015470: 2020 206d 6f63 6b5f 6368 6f6f 7365 2e73     mock_choose.s
-00015480: 6964 655f 6566 6665 6374 203d 2065 7272  ide_effect = err
-00015490: 6f72 732e 506c 7567 696e 5365 6c65 6374  ors.PluginSelect
-000154a0: 696f 6e45 7272 6f72 0a20 2020 2020 2020  ionError.       
-000154b0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-000154c0: 7365 7328 6572 726f 7273 2e50 6c75 6769  ses(errors.Plugi
-000154d0: 6e53 656c 6563 7469 6f6e 4572 726f 7229  nSelectionError)
-000154e0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-000154f0: 696e 2e72 656e 6577 5f63 6572 7428 4e6f  in.renew_cert(No
-00015500: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 290a  ne, None, None).
-00015510: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00015520: 6e66 6967 2e64 7279 5f72 756e 203d 2046  nfig.dry_run = F
-00015530: 616c 7365 0a20 2020 2020 2020 2075 7064  alse.        upd
-00015540: 6174 6572 2e72 756e 5f67 656e 6572 6963  ater.run_generic
-00015550: 5f75 7064 6174 6572 7328 7365 6c66 2e63  _updaters(self.c
-00015560: 6f6e 6669 672c 204e 6f6e 652c 204e 6f6e  onfig, None, Non
-00015570: 6529 0a20 2020 2020 2020 2023 204d 616b  e).        # Mak
-00015580: 6520 7375 7265 2077 6527 7265 2072 6574  e sure we're ret
-00015590: 7572 6e69 6e67 204e 6f6e 652c 2061 6e64  urning None, and
-000155a0: 2068 656e 6365 206e 6f74 2074 7279 696e   hence not tryin
-000155b0: 6720 746f 2072 756e 2074 6865 0a20 2020  g to run the.   
-000155c0: 2020 2020 2023 2077 6974 686f 7574 2069       # without i
-000155d0: 6e73 7461 6c6c 6572 0a20 2020 2020 2020  nstaller.       
-000155e0: 2061 7373 6572 7420 6d6f 636b 5f72 756e   assert mock_run
-000155f0: 2e63 616c 6c65 6420 6973 2046 616c 7365  .called is False
-00015600: 0a0a 2020 2020 406d 6f63 6b2e 7061 7463  ..    @mock.patc
-00015610: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00015620: 726e 616c 2e6d 6169 6e2e 7570 6461 7465  rnal.main.update
-00015630: 722e 7275 6e5f 7265 6e65 7761 6c5f 6465  r.run_renewal_de
-00015640: 706c 6f79 6572 2729 0a20 2020 2040 6d6f  ployer').    @mo
-00015650: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-00015660: 742e 5f69 6e74 6572 6e61 6c2e 706c 7567  t._internal.plug
-00015670: 696e 732e 7365 6c65 6374 696f 6e2e 6368  ins.selection.ch
-00015680: 6f6f 7365 5f63 6f6e 6669 6775 7261 746f  oose_configurato
-00015690: 725f 706c 7567 696e 7327 290a 2020 2020  r_plugins').    
-000156a0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-000156b0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-000156c0: 6169 6e2e 5f69 6e69 745f 6c65 5f63 6c69  ain._init_le_cli
-000156d0: 656e 7427 290a 2020 2020 406d 6f63 6b2e  ent').    @mock.
-000156e0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-000156f0: 696e 7465 726e 616c 2e6d 6169 6e2e 5f67  internal.main._g
-00015700: 6574 5f61 6e64 5f73 6176 655f 6365 7274  et_and_save_cert
-00015710: 2729 0a20 2020 2064 6566 2074 6573 745f  ').    def test_
-00015720: 7265 6e65 775f 646f 6573 6e74 5f72 6573  renew_doesnt_res
-00015730: 7461 7274 5f6f 6e5f 6472 7972 756e 2873  tart_on_dryrun(s
-00015740: 656c 662c 206d 6f63 6b5f 6765 745f 6365  elf, mock_get_ce
-00015750: 7274 2c20 6d6f 636b 5f69 6e69 742c 206d  rt, mock_init, m
-00015760: 6f63 6b5f 6368 6f6f 7365 2c0a 2020 2020  ock_choose,.    
-00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015790: 2020 2020 2020 2020 6d6f 636b 5f72 756e          mock_run
-000157a0: 5f72 656e 6577 616c 5f64 6570 6c6f 7965  _renewal_deploye
-000157b0: 7229 3a0a 2020 2020 2020 2020 2222 2241  r):.        """A
-000157c0: 2064 7279 2d72 756e 2072 656e 6577 616c   dry-run renewal
-000157d0: 2073 686f 756c 646e 2774 2074 7279 2074   shouldn't try t
-000157e0: 6f20 7265 7374 6172 7420 7468 6520 696e  o restart the in
-000157f0: 7374 616c 6c65 7222 2222 0a20 2020 2020  staller""".     
-00015800: 2020 2073 656c 662e 636f 6e66 6967 2e64     self.config.d
-00015810: 7279 5f72 756e 203d 2054 7275 650a 2020  ry_run = True.  
-00015820: 2020 2020 2020 696e 7374 616c 6c65 7220        installer 
-00015830: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
-00015840: 2829 0a20 2020 2020 2020 206d 6f63 6b5f  ().        mock_
-00015850: 6368 6f6f 7365 2e72 6574 7572 6e5f 7661  choose.return_va
-00015860: 6c75 6520 3d20 2869 6e73 7461 6c6c 6572  lue = (installer
-00015870: 2c20 6d6f 636b 2e4d 6167 6963 4d6f 636b  , mock.MagicMock
-00015880: 2829 290a 0a20 2020 2020 2020 206d 6169  ())..        mai
-00015890: 6e2e 7265 6e65 775f 6365 7274 2873 656c  n.renew_cert(sel
-000158a0: 662e 636f 6e66 6967 2c20 4e6f 6e65 2c20  f.config, None, 
-000158b0: 4e6f 6e65 290a 0a20 2020 2020 2020 2061  None)..        a
-000158c0: 7373 6572 7420 6d6f 636b 5f69 6e69 742e  ssert mock_init.
-000158d0: 6361 6c6c 5f63 6f75 6e74 203d 3d20 310a  call_count == 1.
-000158e0: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-000158f0: 6f63 6b5f 6765 745f 6365 7274 2e63 616c  ock_get_cert.cal
-00015900: 6c5f 636f 756e 7420 3d3d 2031 0a20 2020  l_count == 1.   
-00015910: 2020 2020 2069 6e73 7461 6c6c 6572 2e72       installer.r
-00015920: 6573 7461 7274 2e61 7373 6572 745f 6e6f  estart.assert_no
-00015930: 745f 6361 6c6c 6564 2829 0a20 2020 2020  t_called().     
-00015940: 2020 206d 6f63 6b5f 7275 6e5f 7265 6e65     mock_run_rene
-00015950: 7761 6c5f 6465 706c 6f79 6572 2e61 7373  wal_deployer.ass
-00015960: 6572 745f 6e6f 745f 6361 6c6c 6564 2829  ert_not_called()
-00015970: 0a0a 0a63 6c61 7373 2055 6e72 6567 6973  ...class Unregis
-00015980: 7465 7254 6573 7428 756e 6974 7465 7374  terTest(unittest
-00015990: 2e54 6573 7443 6173 6529 3a0a 2020 2020  .TestCase):.    
-000159a0: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
-000159b0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-000159c0: 7463 6865 7273 203d 207b 0a20 2020 2020  tchers = {.     
-000159d0: 2020 2020 2020 2027 5f64 6574 6572 6d69         '_determi
-000159e0: 6e65 5f61 6363 6f75 6e74 273a 206d 6f63  ne_account': moc
-000159f0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-00015a00: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-00015a10: 5f64 6574 6572 6d69 6e65 5f61 6363 6f75  _determine_accou
-00015a20: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
-00015a30: 2020 2761 6363 6f75 6e74 273a 206d 6f63    'account': moc
-00015a40: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-00015a50: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-00015a60: 6163 636f 756e 7427 292c 0a20 2020 2020  account'),.     
-00015a70: 2020 2020 2020 2027 636c 6965 6e74 273a         'client':
-00015a80: 206d 6f63 6b2e 7061 7463 6828 2763 6572   mock.patch('cer
-00015a90: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-00015aa0: 6169 6e2e 636c 6965 6e74 2729 2c0a 2020  ain.client'),.  
-00015ab0: 2020 2020 2020 2020 2020 2767 6574 5f75            'get_u
-00015ac0: 7469 6c69 7479 273a 2074 6573 745f 7574  tility': test_ut
-00015ad0: 696c 2e70 6174 6368 5f64 6973 706c 6179  il.patch_display
-00015ae0: 5f75 7469 6c28 297d 0a20 2020 2020 2020  _util()}.       
-00015af0: 2073 656c 662e 6d6f 636b 7320 3d20 7b6b   self.mocks = {k
-00015b00: 3a20 762e 7374 6172 7428 2920 666f 7220  : v.start() for 
-00015b10: 6b2c 2076 2069 6e20 7365 6c66 2e70 6174  k, v in self.pat
-00015b20: 6368 6572 732e 6974 656d 7328 297d 0a0a  chers.items()}..
-00015b30: 2020 2020 6465 6620 7465 6172 446f 776e      def tearDown
-00015b40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00015b50: 666f 7220 7061 7463 6820 696e 2073 656c  for patch in sel
-00015b60: 662e 7061 7463 6865 7273 2e76 616c 7565  f.patchers.value
-00015b70: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00015b80: 2070 6174 6368 2e73 746f 7028 290a 0a20   patch.stop().. 
-00015b90: 2020 2064 6566 2074 6573 745f 6162 6f72     def test_abor
-00015ba0: 745f 756e 7265 6769 7374 6572 2873 656c  t_unregister(sel
-00015bb0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00015bc0: 2e6d 6f63 6b73 5b27 6163 636f 756e 7427  .mocks['account'
-00015bd0: 5d2e 4163 636f 756e 7446 696c 6553 746f  ].AccountFileSto
-00015be0: 7261 6765 2e72 6574 7572 6e5f 7661 6c75  rage.return_valu
-00015bf0: 6520 3d20 6d6f 636b 2e4d 6f63 6b28 290a  e = mock.Mock().
-00015c00: 0a20 2020 2020 2020 2075 7469 6c5f 6d6f  .        util_mo
-00015c10: 636b 203d 2073 656c 662e 6d6f 636b 735b  ck = self.mocks[
-00015c20: 2767 6574 5f75 7469 6c69 7479 275d 2829  'get_utility']()
-00015c30: 0a20 2020 2020 2020 2075 7469 6c5f 6d6f  .        util_mo
-00015c40: 636b 2e79 6573 6e6f 2e72 6574 7572 6e5f  ck.yesno.return_
-00015c50: 7661 6c75 6520 3d20 4661 6c73 650a 0a20  value = False.. 
-00015c60: 2020 2020 2020 2063 6f6e 6669 6720 3d20         config = 
-00015c70: 6d6f 636b 2e4d 6f63 6b28 290a 2020 2020  mock.Mock().    
-00015c80: 2020 2020 756e 7573 6564 5f70 6c75 6769      unused_plugi
-00015c90: 6e73 203d 206d 6f63 6b2e 4d6f 636b 2829  ns = mock.Mock()
-00015ca0: 0a0a 2020 2020 2020 2020 7265 7320 3d20  ..        res = 
-00015cb0: 6d61 696e 2e75 6e72 6567 6973 7465 7228  main.unregister(
-00015cc0: 636f 6e66 6967 2c20 756e 7573 6564 5f70  config, unused_p
-00015cd0: 6c75 6769 6e73 290a 2020 2020 2020 2020  lugins).        
-00015ce0: 6173 7365 7274 2072 6573 203d 3d20 2244  assert res == "D
-00015cf0: 6561 6374 6976 6174 696f 6e20 6162 6f72  eactivation abor
-00015d00: 7465 642e 220a 0a20 2020 2040 6d6f 636b  ted."..    @mock
-00015d10: 2e70 6174 6368 2822 6365 7274 626f 742e  .patch("certbot.
-00015d20: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e64  _internal.main.d
-00015d30: 6973 706c 6179 5f75 7469 6c2e 6e6f 7469  isplay_util.noti
-00015d40: 6679 2229 0a20 2020 2064 6566 2074 6573  fy").    def tes
-00015d50: 745f 756e 7265 6769 7374 6572 2873 656c  t_unregister(sel
-00015d60: 662c 206d 6f63 6b5f 6e6f 7469 6679 293a  f, mock_notify):
-00015d70: 0a20 2020 2020 2020 206d 6f63 6b65 645f  .        mocked_
-00015d80: 7374 6f72 6167 6520 3d20 6d6f 636b 2e4d  storage = mock.M
-00015d90: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-00015da0: 2020 206d 6f63 6b65 645f 7374 6f72 6167     mocked_storag
-00015db0: 652e 6669 6e64 5f61 6c6c 2e72 6574 7572  e.find_all.retur
-00015dc0: 6e5f 7661 6c75 6520 3d20 5b22 616e 2061  n_value = ["an a
-00015dd0: 6363 6f75 6e74 225d 0a0a 2020 2020 2020  ccount"]..      
-00015de0: 2020 7365 6c66 2e6d 6f63 6b73 5b27 6163    self.mocks['ac
-00015df0: 636f 756e 7427 5d2e 4163 636f 756e 7446  count'].AccountF
-00015e00: 696c 6553 746f 7261 6765 2e72 6574 7572  ileStorage.retur
-00015e10: 6e5f 7661 6c75 6520 3d20 6d6f 636b 6564  n_value = mocked
-00015e20: 5f73 746f 7261 6765 0a20 2020 2020 2020  _storage.       
-00015e30: 2073 656c 662e 6d6f 636b 735b 275f 6465   self.mocks['_de
-00015e40: 7465 726d 696e 655f 6163 636f 756e 7427  termine_account'
-00015e50: 5d2e 7265 7475 726e 5f76 616c 7565 203d  ].return_value =
-00015e60: 2028 6d6f 636b 2e4d 6167 6963 4d6f 636b   (mock.MagicMock
-00015e70: 2829 2c20 2266 6f6f 2229 0a0a 2020 2020  (), "foo")..    
-00015e80: 2020 2020 6362 5f63 6c69 656e 7420 3d20      cb_client = 
-00015e90: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
-00015ea0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00015eb0: 636b 735b 2763 6c69 656e 7427 5d2e 436c  cks['client'].Cl
-00015ec0: 6965 6e74 2e72 6574 7572 6e5f 7661 6c75  ient.return_valu
-00015ed0: 6520 3d20 6362 5f63 6c69 656e 740a 0a20  e = cb_client.. 
-00015ee0: 2020 2020 2020 2063 6f6e 6669 6720 3d20         config = 
-00015ef0: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
-00015f00: 0a20 2020 2020 2020 2075 6e75 7365 645f  .        unused_
-00015f10: 706c 7567 696e 7320 3d20 6d6f 636b 2e4d  plugins = mock.M
-00015f20: 6167 6963 4d6f 636b 2829 0a0a 2020 2020  agicMock()..    
-00015f30: 2020 2020 7265 7320 3d20 6d61 696e 2e75      res = main.u
-00015f40: 6e72 6567 6973 7465 7228 636f 6e66 6967  nregister(config
-00015f50: 2c20 756e 7573 6564 5f70 6c75 6769 6e73  , unused_plugins
-00015f60: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00015f70: 7420 7265 7320 6973 204e 6f6e 650a 2020  t res is None.  
-00015f80: 2020 2020 2020 6d6f 636b 5f6e 6f74 6966        mock_notif
-00015f90: 792e 6173 7365 7274 5f63 616c 6c65 645f  y.assert_called_
-00015fa0: 6f6e 6365 5f77 6974 6828 2241 6363 6f75  once_with("Accou
-00015fb0: 6e74 2064 6561 6374 6976 6174 6564 2e22  nt deactivated."
-00015fc0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00015fd0: 756e 7265 6769 7374 6572 5f6e 6f5f 6163  unregister_no_ac
-00015fe0: 636f 756e 7428 7365 6c66 293a 0a20 2020  count(self):.   
-00015ff0: 2020 2020 206d 6f63 6b65 645f 7374 6f72       mocked_stor
-00016000: 6167 6520 3d20 6d6f 636b 2e4d 6167 6963  age = mock.Magic
-00016010: 4d6f 636b 2829 0a20 2020 2020 2020 206d  Mock().        m
-00016020: 6f63 6b65 645f 7374 6f72 6167 652e 6669  ocked_storage.fi
-00016030: 6e64 5f61 6c6c 2e72 6574 7572 6e5f 7661  nd_all.return_va
-00016040: 6c75 6520 3d20 5b5d 0a20 2020 2020 2020  lue = [].       
-00016050: 2073 656c 662e 6d6f 636b 735b 2761 6363   self.mocks['acc
-00016060: 6f75 6e74 275d 2e41 6363 6f75 6e74 4669  ount'].AccountFi
-00016070: 6c65 5374 6f72 6167 652e 7265 7475 726e  leStorage.return
-00016080: 5f76 616c 7565 203d 206d 6f63 6b65 645f  _value = mocked_
-00016090: 7374 6f72 6167 650a 0a20 2020 2020 2020  storage..       
-000160a0: 2063 625f 636c 6965 6e74 203d 206d 6f63   cb_client = moc
-000160b0: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
-000160c0: 2020 2020 2020 7365 6c66 2e6d 6f63 6b73        self.mocks
-000160d0: 5b27 636c 6965 6e74 275d 2e43 6c69 656e  ['client'].Clien
-000160e0: 742e 7265 7475 726e 5f76 616c 7565 203d  t.return_value =
-000160f0: 2063 625f 636c 6965 6e74 0a0a 2020 2020   cb_client..    
-00016100: 2020 2020 636f 6e66 6967 203d 206d 6f63      config = moc
-00016110: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
-00016120: 2020 2020 2020 636f 6e66 6967 2e73 6572        config.ser
-00016130: 7665 7220 3d20 2268 7474 7073 3a2f 2f61  ver = "https://a
-00016140: 636d 652e 6578 616d 706c 652e 636f 6d2f  cme.example.com/
-00016150: 6469 7265 6374 6f72 7922 0a20 2020 2020  directory".     
-00016160: 2020 2075 6e75 7365 645f 706c 7567 696e     unused_plugin
-00016170: 7320 3d20 6d6f 636b 2e4d 6167 6963 4d6f  s = mock.MagicMo
-00016180: 636b 2829 0a0a 2020 2020 2020 2020 7265  ck()..        re
-00016190: 7320 3d20 6d61 696e 2e75 6e72 6567 6973  s = main.unregis
-000161a0: 7465 7228 636f 6e66 6967 2c20 756e 7573  ter(config, unus
-000161b0: 6564 5f70 6c75 6769 6e73 290a 2020 2020  ed_plugins).    
-000161c0: 2020 2020 6d20 3d20 2243 6f75 6c64 206e      m = "Could n
-000161d0: 6f74 2066 696e 6420 6578 6973 7469 6e67  ot find existing
-000161e0: 2061 6363 6f75 6e74 2066 6f72 2073 6572   account for ser
-000161f0: 7665 7220 6874 7470 733a 2f2f 6163 6d65  ver https://acme
-00016200: 2e65 7861 6d70 6c65 2e63 6f6d 2f64 6972  .example.com/dir
-00016210: 6563 746f 7279 2e22 0a20 2020 2020 2020  ectory.".       
-00016220: 2061 7373 6572 7420 7265 7320 3d3d 206d   assert res == m
-00016230: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00016240: 6362 5f63 6c69 656e 742e 6163 6d65 2e64  cb_client.acme.d
-00016250: 6561 6374 6976 6174 655f 7265 6769 7374  eactivate_regist
-00016260: 7261 7469 6f6e 2e63 616c 6c65 6420 6973  ration.called is
-00016270: 2046 616c 7365 0a0a 0a63 6c61 7373 204d   False...class M
-00016280: 616b 654f 7256 6572 6966 794e 6565 6465  akeOrVerifyNeede
-00016290: 6444 6972 7328 7465 7374 5f75 7469 6c2e  dDirs(test_util.
-000162a0: 436f 6e66 6967 5465 7374 4361 7365 293a  ConfigTestCase):
-000162b0: 0a20 2020 2022 2222 5465 7374 7320 666f  .    """Tests fo
-000162c0: 7220 6365 7274 626f 742e 5f69 6e74 6572  r certbot._inter
-000162d0: 6e61 6c2e 6d61 696e 2e6d 616b 655f 6f72  nal.main.make_or
-000162e0: 5f76 6572 6966 795f 6e65 6564 6564 5f64  _verify_needed_d
-000162f0: 6972 732e 2222 220a 0a20 2020 2040 6d6f  irs."""..    @mo
-00016300: 636b 2e70 6174 6368 2822 6365 7274 626f  ck.patch("certbo
-00016310: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-00016320: 2e75 7469 6c22 290a 2020 2020 6465 6620  .util").    def 
-00016330: 7465 7374 5f69 7428 7365 6c66 2c20 6d6f  test_it(self, mo
-00016340: 636b 5f75 7469 6c29 3a0a 2020 2020 2020  ck_util):.      
-00016350: 2020 6d61 696e 2e6d 616b 655f 6f72 5f76    main.make_or_v
-00016360: 6572 6966 795f 6e65 6564 6564 5f64 6972  erify_needed_dir
-00016370: 7328 7365 6c66 2e63 6f6e 6669 6729 0a20  s(self.config). 
-00016380: 2020 2020 2020 2066 6f72 2063 6f72 655f         for core_
-00016390: 6469 7220 696e 2028 7365 6c66 2e63 6f6e  dir in (self.con
-000163a0: 6669 672e 636f 6e66 6967 5f64 6972 2c20  fig.config_dir, 
-000163b0: 7365 6c66 2e63 6f6e 6669 672e 776f 726b  self.config.work
-000163c0: 5f64 6972 2c29 3a0a 2020 2020 2020 2020  _dir,):.        
-000163d0: 2020 2020 6d6f 636b 5f75 7469 6c2e 7365      mock_util.se
-000163e0: 745f 7570 5f63 6f72 655f 6469 722e 6173  t_up_core_dir.as
-000163f0: 7365 7274 5f61 6e79 5f63 616c 6c28 0a20  sert_any_call(. 
-00016400: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00016410: 6f72 655f 6469 722c 2063 6f6e 7374 616e  ore_dir, constan
-00016420: 7473 2e43 4f4e 4649 475f 4449 5253 5f4d  ts.CONFIG_DIRS_M
-00016430: 4f44 452c 0a20 2020 2020 2020 2020 2020  ODE,.           
-00016440: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-00016450: 2e73 7472 6963 745f 7065 726d 6973 7369  .strict_permissi
-00016460: 6f6e 730a 2020 2020 2020 2020 2020 2020  ons.            
-00016470: 290a 0a20 2020 2020 2020 2068 6f6f 6b5f  )..        hook_
-00016480: 6469 7273 203d 2028 7365 6c66 2e63 6f6e  dirs = (self.con
-00016490: 6669 672e 7265 6e65 7761 6c5f 7072 655f  fig.renewal_pre_
-000164a0: 686f 6f6b 735f 6469 722c 0a20 2020 2020  hooks_dir,.     
-000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164c0: 7365 6c66 2e63 6f6e 6669 672e 7265 6e65  self.config.rene
-000164d0: 7761 6c5f 6465 706c 6f79 5f68 6f6f 6b73  wal_deploy_hooks
-000164e0: 5f64 6972 2c0a 2020 2020 2020 2020 2020  _dir,.          
-000164f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016500: 636f 6e66 6967 2e72 656e 6577 616c 5f70  config.renewal_p
-00016510: 6f73 745f 686f 6f6b 735f 6469 722c 290a  ost_hooks_dir,).
-00016520: 2020 2020 2020 2020 666f 7220 686f 6f6b          for hook
-00016530: 5f64 6972 2069 6e20 686f 6f6b 5f64 6972  _dir in hook_dir
-00016540: 733a 0a20 2020 2020 2020 2020 2020 2023  s:.            #
-00016550: 2064 6566 6175 6c74 206d 6f64 6520 6f66   default mode of
-00016560: 2037 3535 2069 7320 7573 6564 0a20 2020   755 is used.   
-00016570: 2020 2020 2020 2020 206d 6f63 6b5f 7574           mock_ut
-00016580: 696c 2e6d 616b 655f 6f72 5f76 6572 6966  il.make_or_verif
-00016590: 795f 6469 722e 6173 7365 7274 5f61 6e79  y_dir.assert_any
-000165a0: 5f63 616c 6c28 0a20 2020 2020 2020 2020  _call(.         
-000165b0: 2020 2020 2020 2068 6f6f 6b5f 6469 722c         hook_dir,
-000165c0: 2073 7472 6963 743d 7365 6c66 2e63 6f6e   strict=self.con
-000165d0: 6669 672e 7374 7269 6374 5f70 6572 6d69  fig.strict_permi
-000165e0: 7373 696f 6e73 290a 0a0a 636c 6173 7320  ssions)...class 
-000165f0: 456e 6861 6e63 6554 6573 7428 7465 7374  EnhanceTest(test
-00016600: 5f75 7469 6c2e 436f 6e66 6967 5465 7374  _util.ConfigTest
-00016610: 4361 7365 293a 0a20 2020 2022 2222 5465  Case):.    """Te
-00016620: 7374 7320 666f 7220 6365 7274 626f 742e  sts for certbot.
-00016630: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e65  _internal.main.e
-00016640: 6e68 616e 6365 2e22 2222 0a0a 2020 2020  nhance."""..    
-00016650: 6465 6620 7365 7455 7028 7365 6c66 293a  def setUp(self):
-00016660: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00016670: 2e73 6574 5570 2829 0a20 2020 2020 2020  .setUp().       
-00016680: 2073 656c 662e 6765 745f 7574 696c 6974   self.get_utilit
-00016690: 795f 7061 7463 6820 3d20 7465 7374 5f75  y_patch = test_u
-000166a0: 7469 6c2e 7061 7463 685f 6469 7370 6c61  til.patch_displa
-000166b0: 795f 7574 696c 2829 0a20 2020 2020 2020  y_util().       
-000166c0: 2073 656c 662e 6d6f 636b 5f67 6574 5f75   self.mock_get_u
-000166d0: 7469 6c69 7479 203d 2073 656c 662e 6765  tility = self.ge
-000166e0: 745f 7574 696c 6974 795f 7061 7463 682e  t_utility_patch.
-000166f0: 7374 6172 7428 290a 2020 2020 2020 2020  start().        
-00016700: 7365 6c66 2e6d 6f63 6b69 6e73 7461 6c6c  self.mockinstall
-00016710: 6572 203d 206d 6f63 6b2e 4d61 6769 634d  er = mock.MagicM
-00016720: 6f63 6b28 7370 6563 3d65 6e68 616e 6365  ock(spec=enhance
-00016730: 6d65 6e74 732e 4175 746f 4853 5453 456e  ments.AutoHSTSEn
-00016740: 6861 6e63 656d 656e 7429 0a0a 2020 2020  hancement)..    
-00016750: 6465 6620 7465 6172 446f 776e 2873 656c  def tearDown(sel
-00016760: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00016770: 2e67 6574 5f75 7469 6c69 7479 5f70 6174  .get_utility_pat
-00016780: 6368 2e73 746f 7028 290a 0a20 2020 2064  ch.stop()..    d
-00016790: 6566 205f 6361 6c6c 2873 656c 662c 2061  ef _call(self, a
-000167a0: 7267 7329 3a0a 2020 2020 2020 2020 706c  rgs):.        pl
-000167b0: 7567 696e 7320 3d20 6469 7363 6f2e 506c  ugins = disco.Pl
-000167c0: 7567 696e 7352 6567 6973 7472 792e 6669  uginsRegistry.fi
-000167d0: 6e64 5f61 6c6c 2829 0a20 2020 2020 2020  nd_all().       
-000167e0: 2063 6f6e 6669 6720 3d20 636c 692e 7072   config = cli.pr
-000167f0: 6570 6172 655f 616e 645f 7061 7273 655f  epare_and_parse_
-00016800: 6172 6773 2870 6c75 6769 6e73 2c20 6172  args(plugins, ar
-00016810: 6773 290a 0a20 2020 2020 2020 2077 6974  gs)..        wit
-00016820: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
-00016830: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00016840: 6365 7274 5f6d 616e 6167 6572 2e67 6574  cert_manager.get
-00016850: 5f63 6572 746e 616d 6573 2729 2061 7320  _certnames') as 
-00016860: 6d6f 636b 5f63 6572 7473 3a0a 2020 2020  mock_certs:.    
-00016870: 2020 2020 2020 2020 6d6f 636b 5f63 6572          mock_cer
-00016880: 7473 2e72 6574 7572 6e5f 7661 6c75 6520  ts.return_value 
-00016890: 3d20 5b27 6578 616d 706c 652e 636f 6d27  = ['example.com'
-000168a0: 5d0a 2020 2020 2020 2020 2020 2020 7769  ].            wi
-000168b0: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-000168c0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-000168d0: 2e63 6572 745f 6d61 6e61 6765 722e 646f  .cert_manager.do
-000168e0: 6d61 696e 735f 666f 725f 6365 7274 6e61  mains_for_certna
-000168f0: 6d65 2729 2061 7320 6d6f 636b 5f64 6f6d  me') as mock_dom
-00016900: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016910: 2020 6d6f 636b 5f64 6f6d 2e72 6574 7572    mock_dom.retur
-00016920: 6e5f 7661 6c75 6520 3d20 5b27 6578 616d  n_value = ['exam
-00016930: 706c 652e 636f 6d27 5d0a 2020 2020 2020  ple.com'].      
-00016940: 2020 2020 2020 2020 2020 7769 7468 206d            with m
-00016950: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00016960: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-00016970: 6e2e 5f69 6e69 745f 6c65 5f63 6c69 656e  n._init_le_clien
-00016980: 7427 2920 6173 206d 6f63 6b5f 696e 6974  t') as mock_init
-00016990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000169a0: 2020 2020 2020 6d6f 636b 5f63 6c69 656e        mock_clien
-000169b0: 7420 3d20 6d6f 636b 2e4d 6167 6963 4d6f  t = mock.MagicMo
-000169c0: 636b 2829 0a20 2020 2020 2020 2020 2020  ck().           
-000169d0: 2020 2020 2020 2020 206d 6f63 6b5f 636c           mock_cl
-000169e0: 6965 6e74 2e63 6f6e 6669 6720 3d20 636f  ient.config = co
-000169f0: 6e66 6967 0a20 2020 2020 2020 2020 2020  nfig.           
-00016a00: 2020 2020 2020 2020 206d 6f63 6b5f 696e           mock_in
-00016a10: 6974 2e72 6574 7572 6e5f 7661 6c75 6520  it.return_value 
-00016a20: 3d20 6d6f 636b 5f63 6c69 656e 740a 2020  = mock_client.  
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 2020 6d61 696e 2e65 6e68 616e 6365 2863    main.enhance(c
-00016a50: 6f6e 6669 672c 2070 6c75 6769 6e73 290a  onfig, plugins).
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 2020 2020 7265 7475 726e 206d 6f63 6b5f      return mock_
-00016a80: 636c 6965 6e74 2023 2072 6574 7572 6e73  client # returns
-00016a90: 2074 6865 2063 6c69 656e 740a 0a20 2020   the client..   
-00016aa0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-00016ab0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00016ac0: 6d61 696e 2e70 6c75 675f 7365 6c2e 7265  main.plug_sel.re
-00016ad0: 636f 7264 5f63 686f 7365 6e5f 706c 7567  cord_chosen_plug
-00016ae0: 696e 7327 290a 2020 2020 406d 6f63 6b2e  ins').    @mock.
-00016af0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-00016b00: 696e 7465 726e 616c 2e63 6572 745f 6d61  internal.cert_ma
-00016b10: 6e61 6765 722e 6c69 6e65 6167 655f 666f  nager.lineage_fo
-00016b20: 725f 6365 7274 6e61 6d65 2729 0a20 2020  r_certname').   
-00016b30: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
-00016b40: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00016b50: 6d61 696e 2e64 6973 706c 6179 5f6f 7073  main.display_ops
-00016b60: 2e63 686f 6f73 655f 7661 6c75 6573 2729  .choose_values')
-00016b70: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-00016b80: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00016b90: 6e61 6c2e 6d61 696e 2e5f 6669 6e64 5f64  nal.main._find_d
-00016ba0: 6f6d 6169 6e73 5f6f 725f 6365 7274 6e61  omains_or_certna
-00016bb0: 6d65 2729 0a20 2020 2064 6566 2074 6573  me').    def tes
-00016bc0: 745f 7365 6c65 6374 696f 6e5f 7175 6573  t_selection_ques
-00016bd0: 7469 6f6e 2873 656c 662c 206d 6f63 6b5f  tion(self, mock_
-00016be0: 6669 6e64 2c20 6d6f 636b 5f63 686f 6f73  find, mock_choos
-00016bf0: 652c 206d 6f63 6b5f 6c69 6e65 6167 652c  e, mock_lineage,
-00016c00: 205f 7265 6329 3a0a 2020 2020 2020 2020   _rec):.        
-00016c10: 6d6f 636b 5f6c 696e 6561 6765 2e72 6574  mock_lineage.ret
-00016c20: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
-00016c30: 2e4d 6167 6963 4d6f 636b 2863 6861 696e  .MagicMock(chain
-00016c40: 5f70 6174 683d 222f 746d 702f 6e6f 6e65  _path="/tmp/none
-00016c50: 7869 7374 656e 7422 290a 2020 2020 2020  xistent").      
-00016c60: 2020 6d6f 636b 5f63 686f 6f73 652e 7265    mock_choose.re
-00016c70: 7475 726e 5f76 616c 7565 203d 205b 2765  turn_value = ['e
-00016c80: 7861 6d70 6c65 2e63 6f6d 275d 0a20 2020  xample.com'].   
-00016c90: 2020 2020 206d 6f63 6b5f 6669 6e64 2e72       mock_find.r
-00016ca0: 6574 7572 6e5f 7661 6c75 6520 3d20 284e  eturn_value = (N
-00016cb0: 6f6e 652c 204e 6f6e 6529 0a20 2020 2020  one, None).     
-00016cc0: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
-00016cd0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-00016ce0: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
-00016cf0: 7365 6c2e 7069 636b 5f69 6e73 7461 6c6c  sel.pick_install
-00016d00: 6572 2729 2061 7320 6d6f 636b 5f70 6963  er') as mock_pic
-00016d10: 6b3a 0a20 2020 2020 2020 2020 2020 2073  k:.            s
-00016d20: 656c 662e 5f63 616c 6c28 5b27 656e 6861  elf._call(['enha
-00016d30: 6e63 6527 2c20 272d 2d72 6564 6972 6563  nce', '--redirec
-00016d40: 7427 5d29 0a20 2020 2020 2020 2020 2020  t']).           
-00016d50: 2061 7373 6572 7420 6d6f 636b 5f70 6963   assert mock_pic
-00016d60: 6b2e 6361 6c6c 6564 0a20 2020 2020 2020  k.called.       
-00016d70: 2020 2020 2023 2043 6865 636b 2074 6861       # Check tha
-00016d80: 7420 7468 6520 6d65 7373 6167 6520 696e  t the message in
-00016d90: 636c 7564 6573 2022 656e 6861 6e63 656d  cludes "enhancem
-00016da0: 656e 7473 220a 2020 2020 2020 2020 2020  ents".          
-00016db0: 2020 6173 7365 7274 2022 656e 6861 6e63    assert "enhanc
-00016dc0: 656d 656e 7473 2220 696e 206d 6f63 6b5f  ements" in mock_
-00016dd0: 7069 636b 2e63 616c 6c5f 6172 6773 5b30  pick.call_args[0
-00016de0: 5d5b 335d 0a0a 2020 2020 406d 6f63 6b2e  ][3]..    @mock.
-00016df0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-00016e00: 696e 7465 726e 616c 2e6d 6169 6e2e 706c  internal.main.pl
-00016e10: 7567 5f73 656c 2e72 6563 6f72 645f 6368  ug_sel.record_ch
-00016e20: 6f73 656e 5f70 6c75 6769 6e73 2729 0a20  osen_plugins'). 
-00016e30: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00016e40: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00016e50: 6c2e 6365 7274 5f6d 616e 6167 6572 2e6c  l.cert_manager.l
-00016e60: 696e 6561 6765 5f66 6f72 5f63 6572 746e  ineage_for_certn
-00016e70: 616d 6527 290a 2020 2020 406d 6f63 6b2e  ame').    @mock.
-00016e80: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-00016e90: 696e 7465 726e 616c 2e6d 6169 6e2e 6469  internal.main.di
-00016ea0: 7370 6c61 795f 6f70 732e 6368 6f6f 7365  splay_ops.choose
-00016eb0: 5f76 616c 7565 7327 290a 2020 2020 406d  _values').    @m
-00016ec0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00016ed0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-00016ee0: 6e2e 5f66 696e 645f 646f 6d61 696e 735f  n._find_domains_
-00016ef0: 6f72 5f63 6572 746e 616d 6527 290a 2020  or_certname').  
-00016f00: 2020 6465 6620 7465 7374 5f73 656c 6563    def test_selec
-00016f10: 7469 6f6e 5f61 7574 685f 7761 726e 696e  tion_auth_warnin
-00016f20: 6728 7365 6c66 2c20 6d6f 636b 5f66 696e  g(self, mock_fin
-00016f30: 642c 206d 6f63 6b5f 6368 6f6f 7365 2c20  d, mock_choose, 
-00016f40: 6d6f 636b 5f6c 696e 6561 6765 2c20 5f72  mock_lineage, _r
-00016f50: 6563 293a 0a20 2020 2020 2020 206d 6f63  ec):.        moc
-00016f60: 6b5f 6c69 6e65 6167 652e 7265 7475 726e  k_lineage.return
-00016f70: 5f76 616c 7565 203d 206d 6f63 6b2e 4d61  _value = mock.Ma
-00016f80: 6769 634d 6f63 6b28 6368 6169 6e5f 7061  gicMock(chain_pa
-00016f90: 7468 3d22 2f74 6d70 2f6e 6f6e 6578 6973  th="/tmp/nonexis
-00016fa0: 7465 6e74 2229 0a20 2020 2020 2020 206d  tent").        m
-00016fb0: 6f63 6b5f 6368 6f6f 7365 2e72 6574 7572  ock_choose.retur
-00016fc0: 6e5f 7661 6c75 6520 3d20 5b22 6578 616d  n_value = ["exam
-00016fd0: 706c 652e 636f 6d22 5d0a 2020 2020 2020  ple.com"].      
-00016fe0: 2020 6d6f 636b 5f66 696e 642e 7265 7475    mock_find.retu
-00016ff0: 726e 5f76 616c 7565 203d 2028 4e6f 6e65  rn_value = (None
-00017000: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-00017010: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
-00017020: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00017030: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
-00017040: 2e70 6963 6b5f 696e 7374 616c 6c65 7227  .pick_installer'
-00017050: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-00017060: 6974 6820 6d6f 636b 2e70 6174 6368 2827  ith mock.patch('
-00017070: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00017080: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
-00017090: 6c6f 6767 6572 2e77 6172 6e69 6e67 2729  logger.warning')
-000170a0: 2061 7320 6d6f 636b 5f6c 6f67 3a0a 2020   as mock_log:.  
-000170b0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-000170c0: 636b 5f63 6c69 656e 7420 3d20 7365 6c66  ck_client = self
-000170d0: 2e5f 6361 6c6c 285b 2765 6e68 616e 6365  ._call(['enhance
-000170e0: 272c 2027 2d61 272c 2027 7765 6272 6f6f  ', '-a', 'webroo
-000170f0: 7427 2c20 272d 2d72 6564 6972 6563 7427  t', '--redirect'
-00017100: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00017110: 2020 2061 7373 6572 7420 6d6f 636b 5f6c     assert mock_l
-00017120: 6f67 2e63 616c 6c65 640a 2020 2020 2020  og.called.      
-00017130: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00017140: 2022 6d61 6b65 2073 656e 7365 2220 696e   "make sense" in
-00017150: 206d 6f63 6b5f 6c6f 672e 6361 6c6c 5f61   mock_log.call_a
-00017160: 7267 735b 305d 5b30 5d0a 2020 2020 2020  rgs[0][0].      
-00017170: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00017180: 206d 6f63 6b5f 636c 6965 6e74 2e65 6e68   mock_client.enh
-00017190: 616e 6365 5f63 6f6e 6669 672e 6361 6c6c  ance_config.call
-000171a0: 6564 0a0a 2020 2020 406d 6f63 6b2e 7061  ed..    @mock.pa
-000171b0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-000171c0: 7465 726e 616c 2e63 6572 745f 6d61 6e61  ternal.cert_mana
-000171d0: 6765 722e 6c69 6e65 6167 655f 666f 725f  ger.lineage_for_
-000171e0: 6365 7274 6e61 6d65 2729 0a20 2020 2040  certname').    @
-000171f0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00017200: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00017210: 696e 2e64 6973 706c 6179 5f6f 7073 2e63  in.display_ops.c
-00017220: 686f 6f73 655f 7661 6c75 6573 2729 0a20  hoose_values'). 
-00017230: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00017240: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00017250: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
-00017260: 7265 636f 7264 5f63 686f 7365 6e5f 706c  record_chosen_pl
-00017270: 7567 696e 7327 290a 2020 2020 6465 6620  ugins').    def 
-00017280: 7465 7374 5f65 6e68 616e 6365 5f63 6f6e  test_enhance_con
-00017290: 6669 675f 6361 6c6c 2873 656c 662c 205f  fig_call(self, _
-000172a0: 7265 632c 206d 6f63 6b5f 6368 6f6f 7365  rec, mock_choose
-000172b0: 2c20 6d6f 636b 5f6c 696e 6561 6765 293a  , mock_lineage):
-000172c0: 0a20 2020 2020 2020 206d 6f63 6b5f 6c69  .        mock_li
-000172d0: 6e65 6167 652e 7265 7475 726e 5f76 616c  neage.return_val
-000172e0: 7565 203d 206d 6f63 6b2e 4d61 6769 634d  ue = mock.MagicM
-000172f0: 6f63 6b28 6368 6169 6e5f 7061 7468 3d22  ock(chain_path="
-00017300: 2f74 6d70 2f6e 6f6e 6578 6973 7465 6e74  /tmp/nonexistent
-00017310: 2229 0a20 2020 2020 2020 206d 6f63 6b5f  ").        mock_
-00017320: 6368 6f6f 7365 2e72 6574 7572 6e5f 7661  choose.return_va
-00017330: 6c75 6520 3d20 5b22 6578 616d 706c 652e  lue = ["example.
-00017340: 636f 6d22 5d0a 2020 2020 2020 2020 7769  com"].        wi
-00017350: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
-00017360: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00017370: 2e6d 6169 6e2e 706c 7567 5f73 656c 2e70  .main.plug_sel.p
-00017380: 6963 6b5f 696e 7374 616c 6c65 7227 293a  ick_installer'):
-00017390: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
-000173a0: 6b5f 636c 6965 6e74 203d 2073 656c 662e  k_client = self.
-000173b0: 5f63 616c 6c28 5b27 656e 6861 6e63 6527  _call(['enhance'
-000173c0: 2c20 272d 2d72 6564 6972 6563 7427 2c20  , '--redirect', 
-000173d0: 272d 2d68 7374 7327 5d29 0a20 2020 2020  '--hsts']).     
-000173e0: 2020 2020 2020 2072 6571 5f65 6e68 203d         req_enh =
-000173f0: 205b 2272 6564 6972 6563 7422 2c20 2268   ["redirect", "h
-00017400: 7374 7322 5d0a 2020 2020 2020 2020 2020  sts"].          
-00017410: 2020 6e6f 745f 7265 715f 656e 6820 3d20    not_req_enh = 
-00017420: 5b22 7569 7222 5d0a 2020 2020 2020 2020  ["uir"].        
-00017430: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
-00017440: 636c 6965 6e74 2e65 6e68 616e 6365 5f63  client.enhance_c
-00017450: 6f6e 6669 672e 6361 6c6c 6564 0a20 2020  onfig.called.   
-00017460: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00017470: 616c 6c28 6765 7461 7474 7228 6d6f 636b  all(getattr(mock
-00017480: 5f63 6c69 656e 742e 636f 6e66 6967 2c20  _client.config, 
-00017490: 6529 2066 6f72 2065 2069 6e20 7265 715f  e) for e in req_
-000174a0: 656e 6829 0a20 2020 2020 2020 2020 2020  enh).           
-000174b0: 2061 7373 6572 7420 6e6f 7420 616e 7928   assert not any(
-000174c0: 6765 7461 7474 7228 6d6f 636b 5f63 6c69  getattr(mock_cli
-000174d0: 656e 742e 636f 6e66 6967 2c20 6529 2066  ent.config, e) f
-000174e0: 6f72 2065 2069 6e20 6e6f 745f 7265 715f  or e in not_req_
-000174f0: 656e 6829 0a20 2020 2020 2020 2020 2020  enh).           
-00017500: 2061 7373 6572 7420 2265 7861 6d70 6c65   assert "example
-00017510: 2e63 6f6d 2220 696e 206d 6f63 6b5f 636c  .com" in mock_cl
-00017520: 6965 6e74 2e65 6e68 616e 6365 5f63 6f6e  ient.enhance_con
-00017530: 6669 672e 6361 6c6c 5f61 7267 735b 305d  fig.call_args[0]
-00017540: 5b30 5d0a 0a20 2020 2040 6d6f 636b 2e70  [0]..    @mock.p
-00017550: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-00017560: 6e74 6572 6e61 6c2e 6365 7274 5f6d 616e  nternal.cert_man
-00017570: 6167 6572 2e6c 696e 6561 6765 5f66 6f72  ager.lineage_for
-00017580: 5f63 6572 746e 616d 6527 290a 2020 2020  _certname').    
-00017590: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-000175a0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-000175b0: 6169 6e2e 6469 7370 6c61 795f 6f70 732e  ain.display_ops.
-000175c0: 6368 6f6f 7365 5f76 616c 7565 7327 290a  choose_values').
-000175d0: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-000175e0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-000175f0: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
-00017600: 2e72 6563 6f72 645f 6368 6f73 656e 5f70  .record_chosen_p
-00017610: 6c75 6769 6e73 2729 0a20 2020 2064 6566  lugins').    def
-00017620: 2074 6573 745f 656e 6861 6e63 655f 6e6f   test_enhance_no
-00017630: 6e69 6e74 6572 6163 7469 7665 2873 656c  ninteractive(sel
-00017640: 662c 205f 7265 632c 206d 6f63 6b5f 6368  f, _rec, mock_ch
-00017650: 6f6f 7365 2c20 6d6f 636b 5f6c 696e 6561  oose, mock_linea
-00017660: 6765 293a 0a20 2020 2020 2020 206d 6f63  ge):.        moc
-00017670: 6b5f 6c69 6e65 6167 652e 7265 7475 726e  k_lineage.return
-00017680: 5f76 616c 7565 203d 206d 6f63 6b2e 4d61  _value = mock.Ma
-00017690: 6769 634d 6f63 6b28 0a20 2020 2020 2020  gicMock(.       
-000176a0: 2020 2020 2063 6861 696e 5f70 6174 683d       chain_path=
-000176b0: 222f 746d 702f 6e6f 6e65 7869 7374 656e  "/tmp/nonexisten
-000176c0: 7422 290a 2020 2020 2020 2020 6d6f 636b  t").        mock
-000176d0: 5f63 686f 6f73 652e 7265 7475 726e 5f76  _choose.return_v
-000176e0: 616c 7565 203d 205b 2265 7861 6d70 6c65  alue = ["example
-000176f0: 2e63 6f6d 225d 0a20 2020 2020 2020 2077  .com"].        w
-00017700: 6974 6820 6d6f 636b 2e70 6174 6368 2827  ith mock.patch('
-00017710: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00017720: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
-00017730: 7069 636b 5f69 6e73 7461 6c6c 6572 2729  pick_installer')
-00017740: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00017750: 636b 5f63 6c69 656e 7420 3d20 7365 6c66  ck_client = self
-00017760: 2e5f 6361 6c6c 285b 2765 6e68 616e 6365  ._call(['enhance
-00017770: 272c 2027 2d2d 7265 6469 7265 6374 272c  ', '--redirect',
-00017780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 2020 2020 2027 2d2d 6873 7473 272c         '--hsts',
-000177b0: 2027 2d2d 6e6f 6e2d 696e 7465 7261 6374   '--non-interact
-000177c0: 6976 6527 5d29 0a20 2020 2020 2020 2020  ive']).         
-000177d0: 2020 2061 7373 6572 7420 6d6f 636b 5f63     assert mock_c
-000177e0: 6c69 656e 742e 656e 6861 6e63 655f 636f  lient.enhance_co
-000177f0: 6e66 6967 2e63 616c 6c65 640a 2020 2020  nfig.called.    
-00017800: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-00017810: 6f63 6b5f 6368 6f6f 7365 2e63 616c 6c65  ock_choose.calle
-00017820: 6420 6973 2046 616c 7365 0a0a 2020 2020  d is False..    
-00017830: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-00017840: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-00017850: 6169 6e2e 6469 7370 6c61 795f 6f70 732e  ain.display_ops.
-00017860: 6368 6f6f 7365 5f76 616c 7565 7327 290a  choose_values').
-00017870: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-00017880: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00017890: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
-000178a0: 2e72 6563 6f72 645f 6368 6f73 656e 5f70  .record_chosen_p
-000178b0: 6c75 6769 6e73 2729 0a20 2020 2064 6566  lugins').    def
-000178c0: 2074 6573 745f 7573 6572 5f61 626f 7274   test_user_abort
-000178d0: 5f64 6f6d 6169 6e73 2873 656c 662c 205f  _domains(self, _
-000178e0: 7265 632c 206d 6f63 6b5f 6368 6f6f 7365  rec, mock_choose
-000178f0: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
-00017900: 6368 6f6f 7365 2e72 6574 7572 6e5f 7661  choose.return_va
-00017910: 6c75 6520 3d20 5b5d 0a20 2020 2020 2020  lue = [].       
-00017920: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
-00017930: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00017940: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
-00017950: 6c2e 7069 636b 5f69 6e73 7461 6c6c 6572  l.pick_installer
-00017960: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-00017970: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-00017980: 6573 2865 7272 6f72 732e 4572 726f 7229  es(errors.Error)
-00017990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000179a0: 2020 7365 6c66 2e5f 6361 6c6c 285b 2765    self._call(['e
-000179b0: 6e68 616e 6365 272c 2027 2d2d 7265 6469  nhance', '--redi
-000179c0: 7265 6374 272c 2027 2d2d 6873 7473 275d  rect', '--hsts']
-000179d0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-000179e0: 6e6f 5f65 6e68 616e 6365 6d65 6e74 735f  no_enhancements_
-000179f0: 6465 6669 6e65 6428 7365 6c66 293a 0a20  defined(self):. 
-00017a00: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
-00017a10: 7374 2e72 6169 7365 7328 6572 726f 7273  st.raises(errors
-00017a20: 2e4d 6973 636f 6e66 6967 7572 6174 696f  .Misconfiguratio
-00017a30: 6e45 7272 6f72 293a 0a20 2020 2020 2020  nError):.       
-00017a40: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
-00017a50: 5b27 656e 6861 6e63 6527 2c20 272d 6127  ['enhance', '-a'
-00017a60: 2c20 276e 756c 6c27 5d29 0a0a 2020 2020  , 'null'])..    
-00017a70: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-00017a80: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-00017a90: 6169 6e2e 706c 7567 5f73 656c 2e63 686f  ain.plug_sel.cho
-00017aa0: 6f73 655f 636f 6e66 6967 7572 6174 6f72  ose_configurator
-00017ab0: 5f70 6c75 6769 6e73 2729 0a20 2020 2040  _plugins').    @
-00017ac0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00017ad0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00017ae0: 696e 2e64 6973 706c 6179 5f6f 7073 2e63  in.display_ops.c
-00017af0: 686f 6f73 655f 7661 6c75 6573 2729 0a20  hoose_values'). 
-00017b00: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00017b10: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00017b20: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
-00017b30: 7265 636f 7264 5f63 686f 7365 6e5f 706c  record_chosen_pl
-00017b40: 7567 696e 7327 290a 2020 2020 6465 6620  ugins').    def 
-00017b50: 7465 7374 5f70 6c75 6769 6e5f 7365 6c65  test_plugin_sele
-00017b60: 6374 696f 6e5f 6572 726f 7228 7365 6c66  ction_error(self
-00017b70: 2c20 5f72 6563 2c20 6d6f 636b 5f63 686f  , _rec, mock_cho
-00017b80: 6f73 652c 206d 6f63 6b5f 7069 636b 293a  ose, mock_pick):
-00017b90: 0a20 2020 2020 2020 206d 6f63 6b5f 6368  .        mock_ch
-00017ba0: 6f6f 7365 2e72 6574 7572 6e5f 7661 6c75  oose.return_valu
-00017bb0: 6520 3d20 5b22 6578 616d 706c 652e 636f  e = ["example.co
-00017bc0: 6d22 5d0a 2020 2020 2020 2020 6d6f 636b  m"].        mock
-00017bd0: 5f70 6963 6b2e 7265 7475 726e 5f76 616c  _pick.return_val
-00017be0: 7565 203d 2028 4e6f 6e65 2c20 4e6f 6e65  ue = (None, None
-00017bf0: 290a 2020 2020 2020 2020 6d6f 636b 5f70  ).        mock_p
-00017c00: 6963 6b2e 7369 6465 5f65 6666 6563 7420  ick.side_effect 
-00017c10: 3d20 6572 726f 7273 2e50 6c75 6769 6e53  = errors.PluginS
-00017c20: 656c 6563 7469 6f6e 4572 726f 7228 290a  electionError().
-00017c30: 2020 2020 2020 2020 6d6f 636b 5f63 6c69          mock_cli
-00017c40: 656e 7420 3d20 7365 6c66 2e5f 6361 6c6c  ent = self._call
-00017c50: 285b 2765 6e68 616e 6365 272c 2027 2d2d  (['enhance', '--
-00017c60: 6873 7473 275d 290a 2020 2020 2020 2020  hsts']).        
-00017c70: 6173 7365 7274 206d 6f63 6b5f 636c 6965  assert mock_clie
-00017c80: 6e74 2e65 6e68 616e 6365 5f63 6f6e 6669  nt.enhance_confi
-00017c90: 672e 6361 6c6c 6564 2069 7320 4661 6c73  g.called is Fals
-00017ca0: 650a 0a20 2020 2040 6d6f 636b 2e70 6174  e..    @mock.pat
-00017cb0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-00017cc0: 6572 6e61 6c2e 6365 7274 5f6d 616e 6167  ernal.cert_manag
-00017cd0: 6572 2e6c 696e 6561 6765 5f66 6f72 5f63  er.lineage_for_c
-00017ce0: 6572 746e 616d 6527 290a 2020 2020 406d  ertname').    @m
-00017cf0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-00017d00: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-00017d10: 6e2e 6469 7370 6c61 795f 6f70 732e 6368  n.display_ops.ch
-00017d20: 6f6f 7365 5f76 616c 7565 7327 290a 2020  oose_values').  
-00017d30: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
-00017d40: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
-00017d50: 2e6d 6169 6e2e 706c 7567 5f73 656c 2e70  .main.plug_sel.p
-00017d60: 6963 6b5f 696e 7374 616c 6c65 7227 290a  ick_installer').
-00017d70: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
-00017d80: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-00017d90: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
-00017da0: 2e72 6563 6f72 645f 6368 6f73 656e 5f70  .record_chosen_p
-00017db0: 6c75 6769 6e73 2729 0a20 2020 2040 7465  lugins').    @te
-00017dc0: 7374 5f75 7469 6c2e 7061 7463 685f 6469  st_util.patch_di
-00017dd0: 7370 6c61 795f 7574 696c 2829 0a20 2020  splay_util().   
-00017de0: 2064 6566 2074 6573 745f 656e 6861 6e63   def test_enhanc
-00017df0: 656d 656e 745f 656e 6162 6c65 2873 656c  ement_enable(sel
-00017e00: 662c 205f 2c20 5f72 6563 2c20 6d6f 636b  f, _, _rec, mock
-00017e10: 5f69 6e73 742c 206d 6f63 6b5f 6368 6f6f  _inst, mock_choo
-00017e20: 7365 2c20 6d6f 636b 5f6c 696e 6561 6765  se, mock_lineage
-00017e30: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
-00017e40: 696e 7374 2e72 6574 7572 6e5f 7661 6c75  inst.return_valu
-00017e50: 6520 3d20 7365 6c66 2e6d 6f63 6b69 6e73  e = self.mockins
-00017e60: 7461 6c6c 6572 0a20 2020 2020 2020 206d  taller.        m
-00017e70: 6f63 6b5f 6368 6f6f 7365 2e72 6574 7572  ock_choose.retur
-00017e80: 6e5f 7661 6c75 6520 3d20 5b22 6578 616d  n_value = ["exam
-00017e90: 706c 652e 636f 6d22 2c20 2261 6e6f 7468  ple.com", "anoth
-00017ea0: 6572 2e74 6c64 225d 0a20 2020 2020 2020  er.tld"].       
-00017eb0: 206d 6f63 6b5f 6c69 6e65 6167 652e 7265   mock_lineage.re
-00017ec0: 7475 726e 5f76 616c 7565 203d 206d 6f63  turn_value = moc
-00017ed0: 6b2e 4d61 6769 634d 6f63 6b28 6368 6169  k.MagicMock(chai
-00017ee0: 6e5f 7061 7468 3d22 2f74 6d70 2f6e 6f6e  n_path="/tmp/non
-00017ef0: 6578 6973 7465 6e74 2229 0a20 2020 2020  existent").     
-00017f00: 2020 2073 656c 662e 5f63 616c 6c28 5b27     self._call(['
-00017f10: 656e 6861 6e63 6527 2c20 272d 2d61 7574  enhance', '--aut
-00017f20: 6f2d 6873 7473 275d 290a 2020 2020 2020  o-hsts']).      
-00017f30: 2020 6173 7365 7274 2073 656c 662e 6d6f    assert self.mo
-00017f40: 636b 696e 7374 616c 6c65 722e 656e 6162  ckinstaller.enab
-00017f50: 6c65 5f61 7574 6f68 7374 732e 6361 6c6c  le_autohsts.call
-00017f60: 6564 0a20 2020 2020 2020 2061 7373 6572  ed.        asser
-00017f70: 7420 7365 6c66 2e6d 6f63 6b69 6e73 7461  t self.mockinsta
-00017f80: 6c6c 6572 2e65 6e61 626c 655f 6175 746f  ller.enable_auto
-00017f90: 6873 7473 2e63 616c 6c5f 6172 6773 5b30  hsts.call_args[0
-00017fa0: 5d5b 315d 203d 3d20 5c0a 2020 2020 2020  ][1] == \.      
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fc0: 2020 2020 5b22 6578 616d 706c 652e 636f      ["example.co
-00017fd0: 6d22 2c20 2261 6e6f 7468 6572 2e74 6c64  m", "another.tld
-00017fe0: 225d 0a0a 2020 2020 406d 6f63 6b2e 7061  "]..    @mock.pa
-00017ff0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-00018000: 7465 726e 616c 2e63 6572 745f 6d61 6e61  ternal.cert_mana
-00018010: 6765 722e 6c69 6e65 6167 655f 666f 725f  ger.lineage_for_
-00018020: 6365 7274 6e61 6d65 2729 0a20 2020 2040  certname').    @
-00018030: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
-00018040: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00018050: 696e 2e64 6973 706c 6179 5f6f 7073 2e63  in.display_ops.c
-00018060: 686f 6f73 655f 7661 6c75 6573 2729 0a20  hoose_values'). 
-00018070: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
-00018080: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00018090: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
-000180a0: 7069 636b 5f69 6e73 7461 6c6c 6572 2729  pick_installer')
-000180b0: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-000180c0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-000180d0: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
-000180e0: 6c2e 7265 636f 7264 5f63 686f 7365 6e5f  l.record_chosen_
-000180f0: 706c 7567 696e 7327 290a 2020 2020 4074  plugins').    @t
-00018100: 6573 745f 7574 696c 2e70 6174 6368 5f64  est_util.patch_d
-00018110: 6973 706c 6179 5f75 7469 6c28 290a 2020  isplay_util().  
-00018120: 2020 6465 6620 7465 7374 5f65 6e68 616e    def test_enhan
-00018130: 6365 6d65 6e74 5f65 6e61 626c 655f 6e6f  cement_enable_no
-00018140: 745f 7375 7070 6f72 7465 6428 7365 6c66  t_supported(self
-00018150: 2c20 5f2c 205f 7265 632c 206d 6f63 6b5f  , _, _rec, mock_
-00018160: 696e 7374 2c20 6d6f 636b 5f63 686f 6f73  inst, mock_choos
-00018170: 652c 206d 6f63 6b5f 6c69 6e65 6167 6529  e, mock_lineage)
-00018180: 3a0a 2020 2020 2020 2020 6d6f 636b 5f69  :.        mock_i
-00018190: 6e73 742e 7265 7475 726e 5f76 616c 7565  nst.return_value
-000181a0: 203d 206e 756c 6c2e 496e 7374 616c 6c65   = null.Installe
-000181b0: 7228 7365 6c66 2e63 6f6e 6669 672c 2022  r(self.config, "
-000181c0: 6e75 6c6c 2229 0a20 2020 2020 2020 206d  null").        m
-000181d0: 6f63 6b5f 6368 6f6f 7365 2e72 6574 7572  ock_choose.retur
-000181e0: 6e5f 7661 6c75 6520 3d20 5b22 6578 616d  n_value = ["exam
-000181f0: 706c 652e 636f 6d22 2c20 2261 6e6f 7468  ple.com", "anoth
-00018200: 6572 2e74 6c64 225d 0a20 2020 2020 2020  er.tld"].       
-00018210: 206d 6f63 6b5f 6c69 6e65 6167 652e 7265   mock_lineage.re
-00018220: 7475 726e 5f76 616c 7565 203d 206d 6f63  turn_value = moc
-00018230: 6b2e 4d61 6769 634d 6f63 6b28 6368 6169  k.MagicMock(chai
-00018240: 6e5f 7061 7468 3d22 2f74 6d70 2f6e 6f6e  n_path="/tmp/non
-00018250: 6578 6973 7465 6e74 2229 0a20 2020 2020  existent").     
-00018260: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-00018270: 6169 7365 7328 6572 726f 7273 2e4e 6f74  aises(errors.Not
-00018280: 5375 7070 6f72 7465 6445 7272 6f72 293a  SupportedError):
-00018290: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000182a0: 662e 5f63 616c 6c28 5b27 656e 6861 6e63  f._call(['enhanc
-000182b0: 6527 2c20 272d 2d61 7574 6f2d 6873 7473  e', '--auto-hsts
-000182c0: 275d 290a 0a20 2020 2064 6566 2074 6573  '])..    def tes
-000182d0: 745f 656e 6861 6e63 656d 656e 745f 656e  t_enhancement_en
-000182e0: 6162 6c65 5f63 6f6e 666c 6963 7428 7365  able_conflict(se
-000182f0: 6c66 293a 0a20 2020 2020 2020 2077 6974  lf):.        wit
-00018300: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-00018310: 6572 726f 7273 2e45 7272 6f72 293a 0a20  errors.Error):. 
-00018320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018330: 5f63 616c 6c28 5b27 656e 6861 6e63 6527  _call(['enhance'
-00018340: 2c20 272d 2d61 7574 6f2d 6873 7473 272c  , '--auto-hsts',
-00018350: 2027 2d2d 6873 7473 275d 290a 0a0a 636c   '--hsts'])...cl
-00018360: 6173 7320 496e 7374 616c 6c54 6573 7428  ass InstallTest(
-00018370: 7465 7374 5f75 7469 6c2e 436f 6e66 6967  test_util.Config
-00018380: 5465 7374 4361 7365 293a 0a20 2020 2022  TestCase):.    "
-00018390: 2222 5465 7374 7320 666f 7220 6365 7274  ""Tests for cert
-000183a0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-000183b0: 696e 2e69 6e73 7461 6c6c 2e22 2222 0a0a  in.install."""..
-000183c0: 2020 2020 6465 6620 7365 7455 7028 7365      def setUp(se
-000183d0: 6c66 293a 0a20 2020 2020 2020 2073 7570  lf):.        sup
-000183e0: 6572 2829 2e73 6574 5570 2829 0a20 2020  er().setUp().   
-000183f0: 2020 2020 2073 656c 662e 6d6f 636b 696e       self.mockin
-00018400: 7374 616c 6c65 7220 3d20 6d6f 636b 2e4d  staller = mock.M
-00018410: 6167 6963 4d6f 636b 2873 7065 633d 656e  agicMock(spec=en
-00018420: 6861 6e63 656d 656e 7473 2e41 7574 6f48  hancements.AutoH
-00018430: 5354 5345 6e68 616e 6365 6d65 6e74 290a  STSEnhancement).
-00018440: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
-00018450: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
-00018460: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
-00018470: 6c2e 7265 636f 7264 5f63 686f 7365 6e5f  l.record_chosen_
-00018480: 706c 7567 696e 7327 290a 2020 2020 406d  plugins').    @m
-00018490: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-000184a0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-000184b0: 6e2e 706c 7567 5f73 656c 2e70 6963 6b5f  n.plug_sel.pick_
-000184c0: 696e 7374 616c 6c65 7227 290a 2020 2020  installer').    
-000184d0: 6465 6620 7465 7374 5f69 6e73 7461 6c6c  def test_install
-000184e0: 5f65 6e68 616e 6365 6d65 6e74 5f6e 6f74  _enhancement_not
-000184f0: 5f73 7570 706f 7274 6564 2873 656c 662c  _supported(self,
-00018500: 206d 6f63 6b5f 696e 7374 2c20 5f72 6563   mock_inst, _rec
-00018510: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
-00018520: 696e 7374 2e72 6574 7572 6e5f 7661 6c75  inst.return_valu
-00018530: 6520 3d20 6e75 6c6c 2e49 6e73 7461 6c6c  e = null.Install
-00018540: 6572 2873 656c 662e 636f 6e66 6967 2c20  er(self.config, 
-00018550: 226e 756c 6c22 290a 2020 2020 2020 2020  "null").        
-00018560: 706c 7567 696e 7320 3d20 6469 7363 6f2e  plugins = disco.
-00018570: 506c 7567 696e 7352 6567 6973 7472 792e  PluginsRegistry.
-00018580: 6669 6e64 5f61 6c6c 2829 0a20 2020 2020  find_all().     
-00018590: 2020 2073 656c 662e 636f 6e66 6967 2e61     self.config.a
-000185a0: 7574 6f5f 6873 7473 203d 2054 7275 650a  uto_hsts = True.
-000185b0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000185c0: 6669 672e 6365 7274 6e61 6d65 203d 2022  fig.certname = "
-000185d0: 6e6f 6e65 7869 7374 656e 7422 0a20 2020  nonexistent".   
-000185e0: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-000185f0: 2e72 6169 7365 7328 6572 726f 7273 2e4e  .raises(errors.N
-00018600: 6f74 5375 7070 6f72 7465 6445 7272 6f72  otSupportedError
-00018610: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
-00018620: 6169 6e2e 696e 7374 616c 6c28 7365 6c66  ain.install(self
-00018630: 2e63 6f6e 6669 672c 2070 6c75 6769 6e73  .config, plugins
-00018640: 290a 0a20 2020 2040 6d6f 636b 2e70 6174  )..    @mock.pat
-00018650: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-00018660: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
-00018670: 7365 6c2e 7265 636f 7264 5f63 686f 7365  sel.record_chose
-00018680: 6e5f 706c 7567 696e 7327 290a 2020 2020  n_plugins').    
-00018690: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
-000186a0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-000186b0: 6169 6e2e 706c 7567 5f73 656c 2e70 6963  ain.plug_sel.pic
-000186c0: 6b5f 696e 7374 616c 6c65 7227 290a 2020  k_installer').  
-000186d0: 2020 6465 6620 7465 7374 5f69 6e73 7461    def test_insta
-000186e0: 6c6c 5f65 6e68 616e 6365 6d65 6e74 5f6e  ll_enhancement_n
-000186f0: 6f5f 6365 7274 6e61 6d65 2873 656c 662c  o_certname(self,
-00018700: 206d 6f63 6b5f 696e 7374 2c20 5f72 6563   mock_inst, _rec
-00018710: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
-00018720: 696e 7374 2e72 6574 7572 6e5f 7661 6c75  inst.return_valu
-00018730: 6520 3d20 7365 6c66 2e6d 6f63 6b69 6e73  e = self.mockins
-00018740: 7461 6c6c 6572 0a20 2020 2020 2020 2070  taller.        p
-00018750: 6c75 6769 6e73 203d 2064 6973 636f 2e50  lugins = disco.P
-00018760: 6c75 6769 6e73 5265 6769 7374 7279 2e66  luginsRegistry.f
-00018770: 696e 645f 616c 6c28 290a 2020 2020 2020  ind_all().      
-00018780: 2020 7365 6c66 2e63 6f6e 6669 672e 6175    self.config.au
-00018790: 746f 5f68 7374 7320 3d20 5472 7565 0a20  to_hsts = True. 
-000187a0: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-000187b0: 6967 2e63 6572 746e 616d 6520 3d20 4e6f  ig.certname = No
-000187c0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-000187d0: 636f 6e66 6967 2e6b 6579 5f70 6174 6820  config.key_path 
-000187e0: 3d20 222f 746d 702f 6e6f 6e65 7869 7374  = "/tmp/nonexist
-000187f0: 656e 7422 0a20 2020 2020 2020 2073 656c  ent".        sel
-00018800: 662e 636f 6e66 6967 2e63 6572 745f 7061  f.config.cert_pa
-00018810: 7468 203d 2022 2f74 6d70 2f6e 6f6e 6578  th = "/tmp/nonex
-00018820: 6973 7465 6e74 220a 2020 2020 2020 2020  istent".        
-00018830: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-00018840: 6573 2865 7272 6f72 732e 436f 6e66 6967  es(errors.Config
-00018850: 7572 6174 696f 6e45 7272 6f72 293a 0a20  urationError):. 
-00018860: 2020 2020 2020 2020 2020 206d 6169 6e2e             main.
-00018870: 696e 7374 616c 6c28 7365 6c66 2e63 6f6e  install(self.con
-00018880: 6669 672c 2070 6c75 6769 6e73 290a 0a0a  fig, plugins)...
-00018890: 636c 6173 7320 5265 706f 7274 4e65 7743  class ReportNewC
-000188a0: 6572 7454 6573 7428 756e 6974 7465 7374  ertTest(unittest
-000188b0: 2e54 6573 7443 6173 6529 3a0a 2020 2020  .TestCase):.    
-000188c0: 2222 2254 6573 7473 2066 6f72 2063 6572  """Tests for cer
-000188d0: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
-000188e0: 6169 6e2e 5f72 6570 6f72 745f 6e65 775f  ain._report_new_
-000188f0: 6365 7274 2061 6e64 0a20 2020 2020 2020  cert and.       
-00018900: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00018910: 6c2e 6d61 696e 2e5f 6373 725f 7265 706f  l.main._csr_repo
-00018920: 7274 5f6e 6577 5f63 6572 742e 0a20 2020  rt_new_cert..   
-00018930: 2022 2222 0a0a 2020 2020 6465 6620 7365   """..    def se
-00018940: 7455 7028 7365 6c66 293a 0a20 2020 2020  tUp(self):.     
-00018950: 2020 2073 656c 662e 6e6f 7469 6679 5f70     self.notify_p
-00018960: 6174 6368 203d 206d 6f63 6b2e 7061 7463  atch = mock.patc
-00018970: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-00018980: 726e 616c 2e6d 6169 6e2e 6469 7370 6c61  rnal.main.displa
-00018990: 795f 7574 696c 2e6e 6f74 6966 7927 290a  y_util.notify').
-000189a0: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
-000189b0: 6b5f 6e6f 7469 6679 203d 2073 656c 662e  k_notify = self.
-000189c0: 6e6f 7469 6679 5f70 6174 6368 2e73 7461  notify_patch.sta
-000189d0: 7274 2829 0a0a 2020 2020 2020 2020 7365  rt()..        se
-000189e0: 6c66 2e6e 6f74 6166 7465 725f 7061 7463  lf.notafter_patc
-000189f0: 6820 3d20 6d6f 636b 2e70 6174 6368 2827  h = mock.patch('
-00018a00: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-00018a10: 6c2e 6d61 696e 2e63 7279 7074 6f5f 7574  l.main.crypto_ut
-00018a20: 696c 2e6e 6f74 4166 7465 7227 290a 2020  il.notAfter').  
-00018a30: 2020 2020 2020 7365 6c66 2e6d 6f63 6b5f        self.mock_
-00018a40: 6e6f 7461 6674 6572 203d 2073 656c 662e  notafter = self.
-00018a50: 6e6f 7461 6674 6572 5f70 6174 6368 2e73  notafter_patch.s
-00018a60: 7461 7274 2829 0a20 2020 2020 2020 2073  tart().        s
-00018a70: 656c 662e 6d6f 636b 5f6e 6f74 6166 7465  elf.mock_notafte
-00018a80: 722e 7265 7475 726e 5f76 616c 7565 203d  r.return_value =
-00018a90: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-00018aa0: 6d65 2831 3937 302c 2031 2c20 312c 2030  me(1970, 1, 1, 0
-00018ab0: 2c20 3029 0a0a 2020 2020 6465 6620 7465  , 0)..    def te
-00018ac0: 6172 446f 776e 2873 656c 6629 3a0a 2020  arDown(self):.  
-00018ad0: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
-00018ae0: 795f 7061 7463 682e 7374 6f70 2829 0a20  y_patch.stop(). 
-00018af0: 2020 2020 2020 2073 656c 662e 6e6f 7461         self.nota
-00018b00: 6674 6572 5f70 6174 6368 2e73 746f 7028  fter_patch.stop(
-00018b10: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-00018b20: 686f 640a 2020 2020 6465 6620 5f63 616c  hod.    def _cal
-00018b30: 6c28 636c 732c 202a 6172 6773 2c20 2a2a  l(cls, *args, **
-00018b40: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00018b50: 2066 726f 6d20 6365 7274 626f 742e 5f69   from certbot._i
-00018b60: 6e74 6572 6e61 6c2e 6d61 696e 2069 6d70  nternal.main imp
-00018b70: 6f72 7420 5f72 6570 6f72 745f 6e65 775f  ort _report_new_
-00018b80: 6365 7274 0a20 2020 2020 2020 2072 6574  cert.        ret
-00018b90: 7572 6e20 5f72 6570 6f72 745f 6e65 775f  urn _report_new_
-00018ba0: 6365 7274 282a 6172 6773 2c20 2a2a 6b77  cert(*args, **kw
-00018bb0: 6172 6773 290a 0a20 2020 2040 636c 6173  args)..    @clas
-00018bc0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00018bd0: 5f63 616c 6c5f 6373 7228 636c 732c 202a  _call_csr(cls, *
-00018be0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00018bf0: 0a20 2020 2020 2020 2066 726f 6d20 6365  .        from ce
-00018c00: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-00018c10: 6d61 696e 2069 6d70 6f72 7420 5f63 7372  main import _csr
-00018c20: 5f72 6570 6f72 745f 6e65 775f 6365 7274  _report_new_cert
-00018c30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018c40: 5f63 7372 5f72 6570 6f72 745f 6e65 775f  _csr_report_new_
-00018c50: 6365 7274 282a 6172 6773 2c20 2a2a 6b77  cert(*args, **kw
-00018c60: 6172 6773 290a 0a20 2020 2064 6566 2074  args)..    def t
-00018c70: 6573 745f 7265 706f 7274 5f64 7279 5f72  est_report_dry_r
-00018c80: 756e 2873 656c 6629 3a0a 2020 2020 2020  un(self):.      
-00018c90: 2020 7365 6c66 2e5f 6361 6c6c 286d 6f63    self._call(moc
-00018ca0: 6b2e 4d6f 636b 2864 7279 5f72 756e 3d54  k.Mock(dry_run=T
-00018cb0: 7275 6529 2c20 4e6f 6e65 2c20 4e6f 6e65  rue), None, None
-00018cc0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-00018cd0: 7365 6c66 2e6d 6f63 6b5f 6e6f 7469 6679  self.mock_notify
-00018ce0: 2e61 7373 6572 745f 6361 6c6c 6564 5f77  .assert_called_w
-00018cf0: 6974 6828 2254 6865 2064 7279 2072 756e  ith("The dry run
-00018d00: 2077 6173 2073 7563 6365 7373 6675 6c2e   was successful.
-00018d10: 2229 0a0a 2020 2020 6465 6620 7465 7374  ")..    def test
-00018d20: 5f63 7372 5f72 6570 6f72 745f 6472 795f  _csr_report_dry_
-00018d30: 7275 6e28 7365 6c66 293a 0a20 2020 2020  run(self):.     
-00018d40: 2020 2073 656c 662e 5f63 616c 6c5f 6373     self._call_cs
-00018d50: 7228 6d6f 636b 2e4d 6f63 6b28 6472 795f  r(mock.Mock(dry_
-00018d60: 7275 6e3d 5472 7565 292c 204e 6f6e 652c  run=True), None,
-00018d70: 204e 6f6e 652c 204e 6f6e 6529 0a20 2020   None, None).   
-00018d80: 2020 2020 2073 656c 662e 6d6f 636b 5f6e       self.mock_n
-00018d90: 6f74 6966 792e 6173 7365 7274 5f63 616c  otify.assert_cal
-00018da0: 6c65 645f 7769 7468 2822 5468 6520 6472  led_with("The dr
-00018db0: 7920 7275 6e20 7761 7320 7375 6363 6573  y run was succes
-00018dc0: 7366 756c 2e22 290a 0a20 2020 2064 6566  sful.")..    def
-00018dd0: 2074 6573 745f 7265 706f 7274 5f6e 6f5f   test_report_no_
-00018de0: 7061 7468 7328 7365 6c66 293a 0a20 2020  paths(self):.   
-00018df0: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-00018e00: 2e72 6169 7365 7328 4173 7365 7274 696f  .raises(Assertio
-00018e10: 6e45 7272 6f72 293a 0a20 2020 2020 2020  nError):.       
-00018e20: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
-00018e30: 6d6f 636b 2e4d 6f63 6b28 6472 795f 7275  mock.Mock(dry_ru
-00018e40: 6e3d 4661 6c73 6529 2c20 4e6f 6e65 2c20  n=False), None, 
-00018e50: 4e6f 6e65 2c20 4e6f 6e65 290a 0a20 2020  None, None)..   
-00018e60: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-00018e70: 2e72 6169 7365 7328 4173 7365 7274 696f  .raises(Assertio
-00018e80: 6e45 7272 6f72 293a 0a20 2020 2020 2020  nError):.       
-00018e90: 2020 2020 2073 656c 662e 5f63 616c 6c5f       self._call_
-00018ea0: 6373 7228 6d6f 636b 2e4d 6f63 6b28 6472  csr(mock.Mock(dr
-00018eb0: 795f 7275 6e3d 4661 6c73 6529 2c20 4e6f  y_run=False), No
-00018ec0: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 290a  ne, None, None).
-00018ed0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-00018ee0: 706f 7274 2873 656c 6629 3a0a 2020 2020  port(self):.    
-00018ef0: 2020 2020 7365 6c66 2e5f 6361 6c6c 286d      self._call(m
-00018f00: 6f63 6b2e 4d6f 636b 2864 7279 5f72 756e  ock.Mock(dry_run
-00018f10: 3d46 616c 7365 292c 0a20 2020 2020 2020  =False),.       
-00018f20: 2020 2020 2020 2020 2020 2027 2f70 6174             '/pat
-00018f30: 682f 746f 2f63 6572 742e 7065 6d27 2c20  h/to/cert.pem', 
-00018f40: 272f 7061 7468 2f74 6f2f 6675 6c6c 6368  '/path/to/fullch
-00018f50: 6169 6e2e 7065 6d27 2c0a 2020 2020 2020  ain.pem',.      
-00018f60: 2020 2020 2020 2020 2020 2020 272f 7061              '/pa
-00018f70: 7468 2f74 6f2f 7072 6976 6b65 792e 7065  th/to/privkey.pe
-00018f80: 6d27 290a 0a20 2020 2020 2020 2073 656c  m')..        sel
-00018f90: 662e 6d6f 636b 5f6e 6f74 6966 792e 6173  f.mock_notify.as
-00018fa0: 7365 7274 5f63 616c 6c65 645f 7769 7468  sert_called_with
-00018fb0: 280a 2020 2020 2020 2020 2020 2020 275c  (.            '\
-00018fc0: 6e53 7563 6365 7373 6675 6c6c 7920 7265  nSuccessfully re
-00018fd0: 6365 6976 6564 2063 6572 7469 6669 6361  ceived certifica
-00018fe0: 7465 2e5c 6e27 0a20 2020 2020 2020 2020  te.\n'.         
-00018ff0: 2020 2027 4365 7274 6966 6963 6174 6520     'Certificate 
-00019000: 6973 2073 6176 6564 2061 743a 202f 7061  is saved at: /pa
-00019010: 7468 2f74 6f2f 6675 6c6c 6368 6169 6e2e  th/to/fullchain.
-00019020: 7065 6d5c 6e27 0a20 2020 2020 2020 2020  pem\n'.         
-00019030: 2020 2027 4b65 7920 6973 2073 6176 6564     'Key is saved
-00019040: 2061 743a 2020 2020 2020 2020 202f 7061   at:         /pa
-00019050: 7468 2f74 6f2f 7072 6976 6b65 792e 7065  th/to/privkey.pe
-00019060: 6d5c 6e27 0a20 2020 2020 2020 2020 2020  m\n'.           
-00019070: 2027 5468 6973 2063 6572 7469 6669 6361   'This certifica
-00019080: 7465 2065 7870 6972 6573 206f 6e20 3139  te expires on 19
-00019090: 3730 2d30 312d 3031 2e5c 6e27 0a20 2020  70-01-01.\n'.   
-000190a0: 2020 2020 2020 2020 2027 5468 6573 6520           'These 
-000190b0: 6669 6c65 7320 7769 6c6c 2062 6520 7570  files will be up
-000190c0: 6461 7465 6420 7768 656e 2074 6865 2063  dated when the c
-000190d0: 6572 7469 6669 6361 7465 2072 656e 6577  ertificate renew
-000190e0: 732e 5c6e 270a 2020 2020 2020 2020 2020  s.\n'.          
-000190f0: 2020 2743 6572 7462 6f74 2068 6173 2073    'Certbot has s
-00019100: 6574 2075 7020 6120 7363 6865 6475 6c65  et up a schedule
-00019110: 6420 7461 736b 2074 6f20 6175 746f 6d61  d task to automa
-00019120: 7469 6361 6c6c 7920 7265 6e65 7720 7468  tically renew th
-00019130: 6973 2027 0a20 2020 2020 2020 2020 2020  is '.           
-00019140: 2027 6365 7274 6966 6963 6174 6520 696e   'certificate in
-00019150: 2074 6865 2062 6163 6b67 726f 756e 642e   the background.
-00019160: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-00019170: 2064 6566 2074 6573 745f 7265 706f 7274   def test_report
-00019180: 5f6e 6f5f 6b65 7928 7365 6c66 293a 0a20  _no_key(self):. 
-00019190: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-000191a0: 6c28 6d6f 636b 2e4d 6f63 6b28 6472 795f  l(mock.Mock(dry_
-000191b0: 7275 6e3d 4661 6c73 6529 2c0a 2020 2020  run=False),.    
-000191c0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
-000191d0: 7061 7468 2f74 6f2f 6365 7274 2e70 656d  path/to/cert.pem
-000191e0: 272c 2027 2f70 6174 682f 746f 2f66 756c  ', '/path/to/ful
-000191f0: 6c63 6861 696e 2e70 656d 272c 0a20 2020  lchain.pem',.   
-00019200: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00019210: 6f6e 6529 0a0a 2020 2020 2020 2020 7365  one)..        se
-00019220: 6c66 2e6d 6f63 6b5f 6e6f 7469 6679 2e61  lf.mock_notify.a
-00019230: 7373 6572 745f 6361 6c6c 6564 5f77 6974  ssert_called_wit
-00019240: 6828 0a20 2020 2020 2020 2020 2020 2027  h(.            '
-00019250: 5c6e 5375 6363 6573 7366 756c 6c79 2072  \nSuccessfully r
-00019260: 6563 6569 7665 6420 6365 7274 6966 6963  eceived certific
-00019270: 6174 652e 5c6e 270a 2020 2020 2020 2020  ate.\n'.        
-00019280: 2020 2020 2743 6572 7469 6669 6361 7465      'Certificate
-00019290: 2069 7320 7361 7665 6420 6174 3a20 2f70   is saved at: /p
-000192a0: 6174 682f 746f 2f66 756c 6c63 6861 696e  ath/to/fullchain
-000192b0: 2e70 656d 5c6e 270a 2020 2020 2020 2020  .pem\n'.        
-000192c0: 2020 2020 2754 6869 7320 6365 7274 6966      'This certif
-000192d0: 6963 6174 6520 6578 7069 7265 7320 6f6e  icate expires on
-000192e0: 2031 3937 302d 3031 2d30 312e 5c6e 270a   1970-01-01.\n'.
-000192f0: 2020 2020 2020 2020 2020 2020 2754 6865              'The
-00019300: 7365 2066 696c 6573 2077 696c 6c20 6265  se files will be
-00019310: 2075 7064 6174 6564 2077 6865 6e20 7468   updated when th
-00019320: 6520 6365 7274 6966 6963 6174 6520 7265  e certificate re
-00019330: 6e65 7773 2e5c 6e27 0a20 2020 2020 2020  news.\n'.       
-00019340: 2020 2020 2027 4365 7274 626f 7420 6861       'Certbot ha
-00019350: 7320 7365 7420 7570 2061 2073 6368 6564  s set up a sched
-00019360: 756c 6564 2074 6173 6b20 746f 2061 7574  uled task to aut
-00019370: 6f6d 6174 6963 616c 6c79 2072 656e 6577  omatically renew
-00019380: 2074 6869 7320 270a 2020 2020 2020 2020   this '.        
-00019390: 2020 2020 2763 6572 7469 6669 6361 7465      'certificate
-000193a0: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
-000193b0: 6e64 2e27 0a20 2020 2020 2020 2029 0a0a  nd.'.        )..
-000193c0: 2020 2020 6465 6620 7465 7374 5f72 6570      def test_rep
-000193d0: 6f72 745f 6e6f 5f70 7265 636f 6e66 6967  ort_no_preconfig
-000193e0: 7572 6564 5f72 656e 6577 616c 2873 656c  ured_renewal(sel
-000193f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00019400: 2e5f 6361 6c6c 286d 6f63 6b2e 4d6f 636b  ._call(mock.Mock
-00019410: 2864 7279 5f72 756e 3d46 616c 7365 2c20  (dry_run=False, 
-00019420: 7072 6563 6f6e 6669 6775 7265 645f 7265  preconfigured_re
-00019430: 6e65 7761 6c3d 4661 6c73 6529 2c0a 2020  newal=False),.  
-00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019450: 272f 7061 7468 2f74 6f2f 6365 7274 2e70  '/path/to/cert.p
-00019460: 656d 272c 2027 2f70 6174 682f 746f 2f66  em', '/path/to/f
-00019470: 756c 6c63 6861 696e 2e70 656d 272c 0a20  ullchain.pem',. 
-00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019490: 2027 2f70 6174 682f 746f 2f70 7269 766b   '/path/to/privk
-000194a0: 6579 2e70 656d 2729 0a0a 2020 2020 2020  ey.pem')..      
-000194b0: 2020 7365 6c66 2e6d 6f63 6b5f 6e6f 7469    self.mock_noti
-000194c0: 6679 2e61 7373 6572 745f 6361 6c6c 6564  fy.assert_called
-000194d0: 5f77 6974 6828 0a20 2020 2020 2020 2020  _with(.         
-000194e0: 2020 2027 5c6e 5375 6363 6573 7366 756c     '\nSuccessful
-000194f0: 6c79 2072 6563 6569 7665 6420 6365 7274  ly received cert
-00019500: 6966 6963 6174 652e 5c6e 270a 2020 2020  ificate.\n'.    
-00019510: 2020 2020 2020 2020 2743 6572 7469 6669          'Certifi
-00019520: 6361 7465 2069 7320 7361 7665 6420 6174  cate is saved at
-00019530: 3a20 2f70 6174 682f 746f 2f66 756c 6c63  : /path/to/fullc
-00019540: 6861 696e 2e70 656d 5c6e 270a 2020 2020  hain.pem\n'.    
-00019550: 2020 2020 2020 2020 274b 6579 2069 7320          'Key is 
-00019560: 7361 7665 6420 6174 3a20 2020 2020 2020  saved at:       
-00019570: 2020 2f70 6174 682f 746f 2f70 7269 766b    /path/to/privk
-00019580: 6579 2e70 656d 5c6e 270a 2020 2020 2020  ey.pem\n'.      
-00019590: 2020 2020 2020 2754 6869 7320 6365 7274        'This cert
-000195a0: 6966 6963 6174 6520 6578 7069 7265 7320  ificate expires 
-000195b0: 6f6e 2031 3937 302d 3031 2d30 312e 5c6e  on 1970-01-01.\n
-000195c0: 270a 2020 2020 2020 2020 2020 2020 2754  '.            'T
-000195d0: 6865 7365 2066 696c 6573 2077 696c 6c20  hese files will 
-000195e0: 6265 2075 7064 6174 6564 2077 6865 6e20  be updated when 
-000195f0: 7468 6520 6365 7274 6966 6963 6174 6520  the certificate 
-00019600: 7265 6e65 7773 2e27 0a20 2020 2020 2020  renews.'.       
-00019610: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-00019620: 5f63 7372 5f72 6570 6f72 7428 7365 6c66  _csr_report(self
-00019630: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00019640: 5f63 616c 6c5f 6373 7228 6d6f 636b 2e4d  _call_csr(mock.M
-00019650: 6f63 6b28 6472 795f 7275 6e3d 4661 6c73  ock(dry_run=Fals
-00019660: 6529 2c20 272f 7061 7468 2f74 6f2f 6365  e), '/path/to/ce
-00019670: 7274 2e70 656d 272c 0a20 2020 2020 2020  rt.pem',.       
-00019680: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00019690: 2f70 6174 682f 746f 2f63 6861 696e 2e70  /path/to/chain.p
-000196a0: 656d 272c 2027 2f70 6174 682f 746f 2f66  em', '/path/to/f
-000196b0: 756c 6c63 6861 696e 2e70 656d 2729 0a0a  ullchain.pem')..
-000196c0: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
-000196d0: 6b5f 6e6f 7469 6679 2e61 7373 6572 745f  k_notify.assert_
-000196e0: 6361 6c6c 6564 5f77 6974 6828 0a20 2020  called_with(.   
-000196f0: 2020 2020 2020 2020 2027 5c6e 5375 6363           '\nSucc
-00019700: 6573 7366 756c 6c79 2072 6563 6569 7665  essfully receive
-00019710: 6420 6365 7274 6966 6963 6174 652e 5c6e  d certificate.\n
-00019720: 270a 2020 2020 2020 2020 2020 2020 2743  '.            'C
-00019730: 6572 7469 6669 6361 7465 2069 7320 7361  ertificate is sa
-00019740: 7665 6420 6174 3a20 2020 2020 2020 2020  ved at:         
-00019750: 2020 202f 7061 7468 2f74 6f2f 6365 7274     /path/to/cert
-00019760: 2e70 656d 5c6e 270a 2020 2020 2020 2020  .pem\n'.        
-00019770: 2020 2020 2749 6e74 6572 6d65 6469 6174      'Intermediat
-00019780: 6520 4341 2063 6861 696e 2069 7320 7361  e CA chain is sa
-00019790: 7665 6420 6174 3a20 202f 7061 7468 2f74  ved at:  /path/t
-000197a0: 6f2f 6368 6169 6e2e 7065 6d5c 6e27 0a20  o/chain.pem\n'. 
-000197b0: 2020 2020 2020 2020 2020 2027 4675 6c6c             'Full
-000197c0: 2063 6572 7469 6669 6361 7465 2063 6861   certificate cha
-000197d0: 696e 2069 7320 7361 7665 6420 6174 3a20  in is saved at: 
-000197e0: 2f70 6174 682f 746f 2f66 756c 6c63 6861  /path/to/fullcha
-000197f0: 696e 2e70 656d 5c6e 270a 2020 2020 2020  in.pem\n'.      
-00019800: 2020 2020 2020 2754 6869 7320 6365 7274        'This cert
-00019810: 6966 6963 6174 6520 6578 7069 7265 7320  ificate expires 
-00019820: 6f6e 2031 3937 302d 3031 2d30 312e 270a  on 1970-01-01.'.
-00019830: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00019840: 6566 2074 6573 745f 6d61 6e75 616c 5f6e  ef test_manual_n
-00019850: 6f5f 686f 6f6b 735f 7265 706f 7274 2873  o_hooks_report(s
-00019860: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00019870: 2253 686f 756c 646e 2774 2067 6574 2061  "Shouldn't get a
-00019880: 206d 6573 7361 6765 2061 626f 7574 2061   message about a
-00019890: 7574 6f72 656e 6577 616c 2069 6620 6e6f  utorenewal if no
-000198a0: 202d 2d6d 616e 7561 6c2d 6175 7468 2d68   --manual-auth-h
-000198b0: 6f6f 6b22 2222 0a20 2020 2020 2020 2073  ook""".        s
-000198c0: 656c 662e 5f63 616c 6c28 6d6f 636b 2e4d  elf._call(mock.M
-000198d0: 6f63 6b28 6472 795f 7275 6e3d 4661 6c73  ock(dry_run=Fals
-000198e0: 652c 2061 7574 6865 6e74 6963 6174 6f72  e, authenticator
-000198f0: 3d27 6d61 6e75 616c 272c 206d 616e 7561  ='manual', manua
-00019900: 6c5f 6175 7468 5f68 6f6f 6b3d 4e6f 6e65  l_auth_hook=None
-00019910: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00019920: 2020 2020 2027 2f70 6174 682f 746f 2f63       '/path/to/c
-00019930: 6572 742e 7065 6d27 2c20 272f 7061 7468  ert.pem', '/path
-00019940: 2f74 6f2f 6675 6c6c 6368 6169 6e2e 7065  /to/fullchain.pe
-00019950: 6d27 2c0a 2020 2020 2020 2020 2020 2020  m',.            
-00019960: 2020 2020 2020 272f 7061 7468 2f74 6f2f        '/path/to/
-00019970: 7072 6976 6b65 792e 7065 6d27 290a 0a20  privkey.pem').. 
-00019980: 2020 2020 2020 2073 656c 662e 6d6f 636b         self.mock
-00019990: 5f6e 6f74 6966 792e 6173 7365 7274 5f63  _notify.assert_c
-000199a0: 616c 6c65 645f 7769 7468 280a 2020 2020  alled_with(.    
-000199b0: 2020 2020 2020 2020 275c 6e53 7563 6365          '\nSucce
-000199c0: 7373 6675 6c6c 7920 7265 6365 6976 6564  ssfully received
-000199d0: 2063 6572 7469 6669 6361 7465 2e5c 6e27   certificate.\n'
-000199e0: 0a20 2020 2020 2020 2020 2020 2027 4365  .            'Ce
-000199f0: 7274 6966 6963 6174 6520 6973 2073 6176  rtificate is sav
-00019a00: 6564 2061 743a 202f 7061 7468 2f74 6f2f  ed at: /path/to/
-00019a10: 6675 6c6c 6368 6169 6e2e 7065 6d5c 6e27  fullchain.pem\n'
-00019a20: 0a20 2020 2020 2020 2020 2020 2027 4b65  .            'Ke
-00019a30: 7920 6973 2073 6176 6564 2061 743a 2020  y is saved at:  
-00019a40: 2020 2020 2020 202f 7061 7468 2f74 6f2f         /path/to/
-00019a50: 7072 6976 6b65 792e 7065 6d5c 6e27 0a20  privkey.pem\n'. 
-00019a60: 2020 2020 2020 2020 2020 2027 5468 6973             'This
-00019a70: 2063 6572 7469 6669 6361 7465 2065 7870   certificate exp
-00019a80: 6972 6573 206f 6e20 3139 3730 2d30 312d  ires on 1970-01-
-00019a90: 3031 2e5c 6e27 0a20 2020 2020 2020 2020  01.\n'.         
-00019aa0: 2020 2027 5468 6573 6520 6669 6c65 7320     'These files 
-00019ab0: 7769 6c6c 2062 6520 7570 6461 7465 6420  will be updated 
-00019ac0: 7768 656e 2074 6865 2063 6572 7469 6669  when the certifi
-00019ad0: 6361 7465 2072 656e 6577 732e 270a 2020  cate renews.'.  
-00019ae0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-00019af0: 5265 706f 7274 4e65 7874 5374 6570 7354  ReportNextStepsT
-00019b00: 6573 7428 756e 6974 7465 7374 2e54 6573  est(unittest.Tes
-00019b10: 7443 6173 6529 3a0a 2020 2020 2222 2254  tCase):.    """T
-00019b20: 6573 7473 2066 6f72 2063 6572 7462 6f74  ests for certbot
-00019b30: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-00019b40: 5f72 6570 6f72 745f 6e65 7874 5f73 7465  _report_next_ste
-00019b50: 7073 2222 220a 0a20 2020 2064 6566 2073  ps"""..    def s
-00019b60: 6574 5570 2873 656c 6629 3a0a 2020 2020  etUp(self):.    
-00019b70: 2020 2020 7365 6c66 2e63 6f6e 6669 6720      self.config 
-00019b80: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
-00019b90: 280a 2020 2020 2020 2020 2020 2020 6365  (.            ce
-00019ba0: 7274 5f6e 616d 653d 2265 7861 6d70 6c65  rt_name="example
-00019bb0: 2e63 6f6d 222c 2070 7265 636f 6e66 6967  .com", preconfig
-00019bc0: 7572 6564 5f72 656e 6577 616c 3d54 7275  ured_renewal=Tru
-00019bd0: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
-00019be0: 7372 3d4e 6f6e 652c 2061 7574 6865 6e74  sr=None, authent
-00019bf0: 6963 6174 6f72 3d22 6e67 696e 7822 2c20  icator="nginx", 
-00019c00: 6d61 6e75 616c 5f61 7574 685f 686f 6f6b  manual_auth_hook
-00019c10: 3d4e 6f6e 6529 0a20 2020 2020 2020 206e  =None).        n
-00019c20: 6f74 6966 795f 7061 7463 6820 3d20 6d6f  otify_patch = mo
-00019c30: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-00019c40: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-00019c50: 2e64 6973 706c 6179 5f75 7469 6c2e 6e6f  .display_util.no
-00019c60: 7469 6679 2729 0a20 2020 2020 2020 2073  tify').        s
-00019c70: 656c 662e 6d6f 636b 5f6e 6f74 6966 7920  elf.mock_notify 
-00019c80: 3d20 6e6f 7469 6679 5f70 6174 6368 2e73  = notify_patch.s
-00019c90: 7461 7274 2829 0a20 2020 2020 2020 2073  tart().        s
-00019ca0: 656c 662e 6164 6443 6c65 616e 7570 286e  elf.addCleanup(n
-00019cb0: 6f74 6966 795f 7061 7463 682e 7374 6f70  otify_patch.stop
-00019cc0: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00019cd0: 6c64 5f73 7464 6f75 7420 3d20 7379 732e  ld_stdout = sys.
-00019ce0: 7374 646f 7574 0a20 2020 2020 2020 2073  stdout.        s
-00019cf0: 7973 2e73 7464 6f75 7420 3d20 696f 2e53  ys.stdout = io.S
-00019d00: 7472 696e 6749 4f28 290a 0a20 2020 2064  tringIO()..    d
-00019d10: 6566 2074 6561 7244 6f77 6e28 7365 6c66  ef tearDown(self
-00019d20: 293a 0a20 2020 2020 2020 2073 7973 2e73  ):.        sys.s
-00019d30: 7464 6f75 7420 3d20 7365 6c66 2e6f 6c64  tdout = self.old
-00019d40: 5f73 7464 6f75 740a 0a20 2020 2040 636c  _stdout..    @cl
-00019d50: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00019d60: 6620 5f63 616c 6c28 636c 732c 202a 6172  f _call(cls, *ar
-00019d70: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-00019d80: 2020 2020 2020 2066 726f 6d20 6365 7274         from cert
-00019d90: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
-00019da0: 696e 2069 6d70 6f72 7420 5f72 6570 6f72  in import _repor
-00019db0: 745f 6e65 7874 5f73 7465 7073 0a20 2020  t_next_steps.   
-00019dc0: 2020 2020 205f 7265 706f 7274 5f6e 6578       _report_nex
-00019dd0: 745f 7374 6570 7328 2a61 7267 732c 202a  t_steps(*args, *
-00019de0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-00019df0: 6620 5f6f 7574 7075 7428 7365 6c66 2920  f _output(self) 
-00019e00: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00019e10: 6173 7365 7274 2073 656c 662e 6d6f 636b  assert self.mock
-00019e20: 5f6e 6f74 6966 792e 6361 6c6c 5f63 6f75  _notify.call_cou
-00019e30: 6e74 203d 3d20 320a 2020 2020 2020 2020  nt == 2.        
-00019e40: 6173 7365 7274 2073 656c 662e 6d6f 636b  assert self.mock
-00019e50: 5f6e 6f74 6966 792e 6361 6c6c 5f61 7267  _notify.call_arg
-00019e60: 735f 6c69 7374 5b30 5d5b 305d 5b30 5d20  s_list[0][0][0] 
-00019e70: 3d3d 2027 4e45 5854 2053 5445 5053 3a27  == 'NEXT STEPS:'
-00019e80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019e90: 7365 6c66 2e6d 6f63 6b5f 6e6f 7469 6679  self.mock_notify
-00019ea0: 2e63 616c 6c5f 6172 6773 5f6c 6973 745b  .call_args_list[
-00019eb0: 315d 5b30 5d5b 305d 0a0a 2020 2020 6465  1][0][0]..    de
-00019ec0: 6620 7465 7374 5f72 6570 6f72 7428 7365  f test_report(se
-00019ed0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00019ee0: 4e6f 2073 7465 7073 2066 6f72 2061 206e  No steps for a n
-00019ef0: 6f72 6d61 6c20 7265 6e65 7761 6c22 2222  ormal renewal"""
-00019f00: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00019f10: 6e66 6967 2e61 7574 6865 6e74 6963 6174  nfig.authenticat
-00019f20: 6f72 203d 2022 6d61 6e75 616c 220a 2020  or = "manual".  
-00019f30: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
-00019f40: 672e 6d61 6e75 616c 5f61 7574 685f 686f  g.manual_auth_ho
-00019f50: 6f6b 203d 2022 2f62 696e 2f74 7275 6522  ok = "/bin/true"
-00019f60: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00019f70: 616c 6c28 7365 6c66 2e63 6f6e 6669 672c  all(self.config,
-00019f80: 204e 6f6e 652c 204e 6f6e 6529 0a20 2020   None, None).   
-00019f90: 2020 2020 2073 656c 662e 6d6f 636b 5f6e       self.mock_n
-00019fa0: 6f74 6966 792e 6173 7365 7274 5f6e 6f74  otify.assert_not
-00019fb0: 5f63 616c 6c65 6428 290a 0a20 2020 2064  _called()..    d
-00019fc0: 6566 2074 6573 745f 6373 725f 7265 706f  ef test_csr_repo
-00019fd0: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
-00019fe0: 2020 2222 222d 2d63 7372 2072 6571 7569    """--csr requi
-00019ff0: 7265 7320 6d61 6e75 616c 2072 656e 6577  res manual renew
-0001a000: 616c 2222 220a 2020 2020 2020 2020 7365  al""".        se
-0001a010: 6c66 2e63 6f6e 6669 672e 6373 7220 3d20  lf.config.csr = 
-0001a020: 2266 6f6f 2e63 7372 220a 2020 2020 2020  "foo.csr".      
-0001a030: 2020 7365 6c66 2e5f 6361 6c6c 2873 656c    self._call(sel
-0001a040: 662e 636f 6e66 6967 2c20 4e6f 6e65 2c20  f.config, None, 
-0001a050: 4e6f 6e65 290a 2020 2020 2020 2020 6173  None).        as
-0001a060: 7365 7274 2022 2d2d 6373 7220 7769 6c6c  sert "--csr will
-0001a070: 206e 6f74 2062 6520 7265 6e65 7765 6422   not be renewed"
-0001a080: 2069 6e20 7365 6c66 2e5f 6f75 7470 7574   in self._output
-0001a090: 2829 0a0a 2020 2020 6465 6620 7465 7374  ()..    def test
-0001a0a0: 5f6d 616e 7561 6c5f 6e6f 5f68 6f6f 6b5f  _manual_no_hook_
-0001a0b0: 7265 6e65 7761 6c28 7365 6c66 293a 0a20  renewal(self):. 
-0001a0c0: 2020 2020 2020 2022 2222 2d2d 6d61 6e75         """--manu
-0001a0d0: 616c 2077 6974 686f 7574 2061 2068 6f6f  al without a hoo
-0001a0e0: 6b20 7265 7175 6972 6573 206d 616e 7561  k requires manua
-0001a0f0: 6c20 7265 6e65 7761 6c22 2222 0a20 2020  l renewal""".   
-0001a100: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-0001a110: 2e61 7574 6865 6e74 6963 6174 6f72 203d  .authenticator =
-0001a120: 2022 6d61 6e75 616c 220a 2020 2020 2020   "manual".      
-0001a130: 2020 7365 6c66 2e5f 6361 6c6c 2873 656c    self._call(sel
-0001a140: 662e 636f 6e66 6967 2c20 4e6f 6e65 2c20  f.config, None, 
-0001a150: 4e6f 6e65 290a 2020 2020 2020 2020 6173  None).        as
-0001a160: 7365 7274 2022 2d2d 6d61 6e75 616c 2063  sert "--manual c
-0001a170: 6572 7469 6669 6361 7465 7320 7265 7175  ertificates requ
-0001a180: 6972 6573 2220 696e 2073 656c 662e 5f6f  ires" in self._o
-0001a190: 7574 7075 7428 290a 0a20 2020 2064 6566  utput()..    def
-0001a1a0: 2074 6573 745f 6e6f 5f70 7265 636f 6e66   test_no_preconf
-0001a1b0: 6967 7572 6564 5f72 656e 6577 616c 2873  igured_renewal(s
-0001a1c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0001a1d0: 224e 6f20 2d2d 7072 6563 6f6e 6669 6775  "No --preconfigu
-0001a1e0: 7265 642d 7265 6e65 7761 6c20 6e65 6564  red-renewal need
-0001a1f0: 7320 6d61 6e75 616c 2063 726f 6e20 7365  s manual cron se
-0001a200: 7475 7022 2222 0a20 2020 2020 2020 2073  tup""".        s
-0001a210: 656c 662e 636f 6e66 6967 2e70 7265 636f  elf.config.preco
-0001a220: 6e66 6967 7572 6564 5f72 656e 6577 616c  nfigured_renewal
-0001a230: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001a240: 2073 656c 662e 5f63 616c 6c28 7365 6c66   self._call(self
-0001a250: 2e63 6f6e 6669 672c 204e 6f6e 652c 204e  .config, None, N
-0001a260: 6f6e 6529 0a20 2020 2020 2020 2061 7373  one).        ass
-0001a270: 6572 7420 2268 7474 7073 3a2f 2f63 6572  ert "https://cer
-0001a280: 7462 6f74 2e6f 7267 2f72 656e 6577 616c  tbot.org/renewal
-0001a290: 2d73 6574 7570 2220 696e 2073 656c 662e  -setup" in self.
-0001a2a0: 5f6f 7574 7075 7428 290a 0a0a 636c 6173  _output()...clas
-0001a2b0: 7320 5570 6461 7465 4163 636f 756e 7454  s UpdateAccountT
-0001a2c0: 6573 7428 7465 7374 5f75 7469 6c2e 436f  est(test_util.Co
-0001a2d0: 6e66 6967 5465 7374 4361 7365 293a 0a20  nfigTestCase):. 
-0001a2e0: 2020 2022 2222 5465 7374 7320 666f 7220     """Tests for 
-0001a2f0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-0001a300: 6c2e 6d61 696e 2e75 7064 6174 655f 6163  l.main.update_ac
-0001a310: 636f 756e 7422 2222 0a0a 2020 2020 6465  count"""..    de
-0001a320: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
-0001a330: 2020 2020 2020 2070 6174 6368 6573 203d         patches =
-0001a340: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0001a350: 6163 636f 756e 7427 3a20 6d6f 636b 2e70  account': mock.p
-0001a360: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
-0001a370: 6e74 6572 6e61 6c2e 6d61 696e 2e61 6363  nternal.main.acc
-0001a380: 6f75 6e74 2729 2c0a 2020 2020 2020 2020  ount'),.        
-0001a390: 2020 2020 2761 7465 7869 7427 3a20 6d6f      'atexit': mo
-0001a3a0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
-0001a3b0: 742e 7574 696c 2e61 7465 7869 7427 292c  t.util.atexit'),
-0001a3c0: 0a20 2020 2020 2020 2020 2020 2027 636c  .            'cl
-0001a3d0: 6965 6e74 273a 206d 6f63 6b2e 7061 7463  ient': mock.patc
-0001a3e0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
-0001a3f0: 726e 616c 2e6d 6169 6e2e 636c 6965 6e74  rnal.main.client
-0001a400: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0001a410: 2764 6574 6572 6d69 6e65 5f61 6363 6f75  'determine_accou
-0001a420: 6e74 273a 206d 6f63 6b2e 7061 7463 6828  nt': mock.patch(
-0001a430: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
-0001a440: 616c 2e6d 6169 6e2e 5f64 6574 6572 6d69  al.main._determi
-0001a450: 6e65 5f61 6363 6f75 6e74 2729 2c0a 2020  ne_account'),.  
-0001a460: 2020 2020 2020 2020 2020 276e 6f74 6966            'notif
-0001a470: 7927 3a20 6d6f 636b 2e70 6174 6368 2827  y': mock.patch('
-0001a480: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
-0001a490: 6c2e 6d61 696e 2e64 6973 706c 6179 5f75  l.main.display_u
-0001a4a0: 7469 6c2e 6e6f 7469 6679 2729 2c0a 2020  til.notify'),.  
-0001a4b0: 2020 2020 2020 2020 2020 2770 7265 7061            'prepa
-0001a4c0: 7265 5f73 7562 273a 206d 6f63 6b2e 7061  re_sub': mock.pa
-0001a4d0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0001a4e0: 7465 726e 616c 2e65 6666 2e70 7265 7061  ternal.eff.prepa
-0001a4f0: 7265 5f73 7562 7363 7269 7074 696f 6e27  re_subscription'
-0001a500: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
-0001a510: 7574 696c 273a 2074 6573 745f 7574 696c  util': test_util
-0001a520: 2e70 6174 6368 5f64 6973 706c 6179 5f75  .patch_display_u
-0001a530: 7469 6c28 290a 2020 2020 2020 2020 7d0a  til().        }.
-0001a540: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
-0001a550: 6b73 203d 207b 206b 3a20 7061 7463 6865  ks = { k: patche
-0001a560: 735b 6b5d 2e73 7461 7274 2829 2066 6f72  s[k].start() for
-0001a570: 206b 2069 6e20 7061 7463 6865 7320 7d0a   k in patches }.
-0001a580: 2020 2020 2020 2020 666f 7220 7061 7463          for patc
-0001a590: 6820 696e 2070 6174 6368 6573 2e76 616c  h in patches.val
-0001a5a0: 7565 7328 293a 0a20 2020 2020 2020 2020  ues():.         
-0001a5b0: 2020 2073 656c 662e 6164 6443 6c65 616e     self.addClean
-0001a5c0: 7570 2870 6174 6368 2e73 746f 7029 0a0a  up(patch.stop)..
-0001a5d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001a5e0: 7570 6572 2829 2e73 6574 5570 2829 0a0a  uper().setUp()..
-0001a5f0: 2020 2020 6465 6620 5f63 616c 6c28 7365      def _call(se
-0001a600: 6c66 2c20 6172 6773 293a 0a20 2020 2020  lf, args):.     
-0001a610: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
-0001a620: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0001a630: 6572 6e61 6c2e 6d61 696e 2e73 7973 2e73  ernal.main.sys.s
-0001a640: 7464 6f75 7427 292c 205c 0a20 2020 2020  tdout'), \.     
-0001a650: 2020 2020 2020 2020 6d6f 636b 2e70 6174          mock.pat
-0001a660: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
-0001a670: 6572 6e61 6c2e 6d61 696e 2e73 7973 2e73  ernal.main.sys.s
-0001a680: 7464 6572 7227 293a 0a20 2020 2020 2020  tderr'):.       
-0001a690: 2020 2020 2061 7267 7320 3d20 5b27 2d2d       args = ['--
-0001a6a0: 636f 6e66 6967 2d64 6972 272c 2073 656c  config-dir', sel
-0001a6b0: 662e 636f 6e66 6967 2e63 6f6e 6669 675f  f.config.config_
-0001a6c0: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
-0001a6d0: 2020 2020 2020 2020 2027 2d2d 776f 726b           '--work
-0001a6e0: 2d64 6972 272c 2073 656c 662e 636f 6e66  -dir', self.conf
-0001a6f0: 6967 2e77 6f72 6b5f 6469 722c 0a20 2020  ig.work_dir,.   
-0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a710: 2027 2d2d 6c6f 6773 2d64 6972 272c 2073   '--logs-dir', s
-0001a720: 656c 662e 636f 6e66 6967 2e6c 6f67 735f  elf.config.logs_
-0001a730: 6469 722c 2027 2d2d 7465 7874 275d 202b  dir, '--text'] +
-0001a740: 2061 7267 730a 2020 2020 2020 2020 2020   args.          
-0001a750: 2020 7265 7475 726e 206d 6169 6e2e 6d61    return main.ma
-0001a760: 696e 2861 7267 735b 3a5d 2920 2320 4e4f  in(args[:]) # NO
-0001a770: 5445 3a20 7061 7273 6572 2063 616e 2061  TE: parser can a
-0001a780: 6c74 6572 2069 7473 2061 7267 7321 0a0a  lter its args!..
-0001a790: 2020 2020 6465 6620 5f70 7265 7061 7265      def _prepare
-0001a7a0: 5f6d 6f63 6b5f 6163 636f 756e 7428 7365  _mock_account(se
-0001a7b0: 6c66 293a 0a20 2020 2020 2020 206d 6f63  lf):.        moc
-0001a7c0: 6b5f 7374 6f72 6167 6520 3d20 6d6f 636b  k_storage = mock
-0001a7d0: 2e4d 6167 6963 4d6f 636b 2829 0a20 2020  .MagicMock().   
-0001a7e0: 2020 2020 206d 6f63 6b5f 6163 636f 756e       mock_accoun
-0001a7f0: 7420 3d20 6d6f 636b 2e4d 6167 6963 4d6f  t = mock.MagicMo
-0001a800: 636b 2829 0a20 2020 2020 2020 206d 6f63  ck().        moc
-0001a810: 6b5f 7265 6772 203d 206d 6f63 6b2e 4d61  k_regr = mock.Ma
-0001a820: 6769 634d 6f63 6b28 290a 2020 2020 2020  gicMock().      
-0001a830: 2020 6d6f 636b 5f73 746f 7261 6765 2e66    mock_storage.f
-0001a840: 696e 645f 616c 6c2e 7265 7475 726e 5f76  ind_all.return_v
-0001a850: 616c 7565 203d 205b 6d6f 636b 5f61 6363  alue = [mock_acc
-0001a860: 6f75 6e74 5d0a 2020 2020 2020 2020 7365  ount].        se
-0001a870: 6c66 2e6d 6f63 6b73 5b27 6163 636f 756e  lf.mocks['accoun
-0001a880: 7427 5d2e 4163 636f 756e 7446 696c 6553  t'].AccountFileS
-0001a890: 746f 7261 6765 2e72 6574 7572 6e5f 7661  torage.return_va
-0001a8a0: 6c75 6520 3d20 6d6f 636b 5f73 746f 7261  lue = mock_stora
-0001a8b0: 6765 0a20 2020 2020 2020 206d 6f63 6b5f  ge.        mock_
-0001a8c0: 6163 636f 756e 742e 7265 6772 2e62 6f64  account.regr.bod
-0001a8d0: 7920 3d20 6d6f 636b 5f72 6567 722e 626f  y = mock_regr.bo
-0001a8e0: 6479 0a20 2020 2020 2020 2073 656c 662e  dy.        self.
-0001a8f0: 6d6f 636b 735b 2764 6574 6572 6d69 6e65  mocks['determine
-0001a900: 5f61 6363 6f75 6e74 275d 2e72 6574 7572  _account'].retur
-0001a910: 6e5f 7661 6c75 6520 3d20 286d 6f63 6b5f  n_value = (mock_
-0001a920: 6163 636f 756e 742c 206d 6f63 6b2e 4d61  account, mock.Ma
-0001a930: 6769 634d 6f63 6b28 2929 0a20 2020 2020  gicMock()).     
-0001a940: 2020 2072 6574 7572 6e20 286d 6f63 6b5f     return (mock_
-0001a950: 6163 636f 756e 742c 206d 6f63 6b5f 7374  account, mock_st
-0001a960: 6f72 6167 652c 206d 6f63 6b5f 7265 6772  orage, mock_regr
-0001a970: 290a 0a20 2020 2064 6566 205f 7465 7374  )..    def _test
-0001a980: 5f75 7064 6174 655f 6e6f 5f63 6f6e 7461  _update_no_conta
-0001a990: 6374 2873 656c 662c 2061 7267 7329 3a0a  ct(self, args):.
-0001a9a0: 2020 2020 2020 2020 2222 2255 7469 6c69          """Utili
-0001a9b0: 7479 2074 6f20 6173 7365 7274 2074 6861  ty to assert tha
-0001a9c0: 7420 656d 6169 6c20 7265 6d6f 7661 6c20  t email removal 
-0001a9d0: 6973 2068 616e 646c 6564 2063 6f72 7265  is handled corre
-0001a9e0: 6374 6c79 2222 220a 2020 2020 2020 2020  ctly""".        
-0001a9f0: 285f 2c20 6d6f 636b 5f73 746f 7261 6765  (_, mock_storage
-0001aa00: 2c20 6d6f 636b 5f72 6567 7229 203d 2073  , mock_regr) = s
-0001aa10: 656c 662e 5f70 7265 7061 7265 5f6d 6f63  elf._prepare_moc
-0001aa20: 6b5f 6163 636f 756e 7428 290a 2020 2020  k_account().    
-0001aa30: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-0001aa40: 662e 5f63 616c 6c28 6172 6773 290a 2020  f._call(args).  
-0001aa50: 2020 2020 2020 2320 5768 656e 2075 7064        # When upd
-0001aa60: 6174 6520 7375 6363 6565 6473 2c20 7468  ate succeeds, th
-0001aa70: 6520 7265 7475 726e 2076 616c 7565 206f  e return value o
-0001aa80: 6620 7570 6461 7465 5f61 6363 6f75 6e74  f update_account
-0001aa90: 2829 2069 7320 4e6f 6e65 0a20 2020 2020  () is None.     
-0001aaa0: 2020 2061 7373 6572 7420 7265 7375 6c74     assert result
-0001aab0: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
-0001aac0: 2023 2057 6520 7375 626d 6974 7465 6420   # We submitted 
-0001aad0: 6120 7265 6769 7374 7261 7469 6f6e 2074  a registration t
-0001aae0: 6f20 7468 6520 7365 7276 6572 0a20 2020  o the server.   
-0001aaf0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0001ab00: 2e6d 6f63 6b73 5b27 636c 6965 6e74 275d  .mocks['client']
-0001ab10: 2e43 6c69 656e 7428 292e 6163 6d65 2e75  .Client().acme.u
-0001ab20: 7064 6174 655f 7265 6769 7374 7261 7469  pdate_registrati
-0001ab30: 6f6e 2e63 616c 6c5f 636f 756e 7420 3d3d  on.call_count ==
-0001ab40: 2031 0a20 2020 2020 2020 206d 6f63 6b5f   1.        mock_
-0001ab50: 7265 6772 2e62 6f64 792e 7570 6461 7465  regr.body.update
-0001ab60: 2e61 7373 6572 745f 6361 6c6c 6564 5f77  .assert_called_w
-0001ab70: 6974 6828 636f 6e74 6163 743d 2829 290a  ith(contact=()).
-0001ab80: 2020 2020 2020 2020 2320 5765 2067 6f74          # We got
-0001ab90: 2061 6e20 7570 6461 7465 2066 726f 6d20   an update from 
-0001aba0: 7468 6520 7365 7276 6572 2061 6e64 2070  the server and p
-0001abb0: 6572 7369 7374 6564 2069 740a 2020 2020  ersisted it.    
-0001abc0: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
-0001abd0: 7374 6f72 6167 652e 7570 6461 7465 5f72  storage.update_r
-0001abe0: 6567 722e 6361 6c6c 5f63 6f75 6e74 203d  egr.call_count =
-0001abf0: 3d20 310a 2020 2020 2020 2020 2320 5765  = 1.        # We
-0001ac00: 2073 686f 756c 6420 6861 7665 206e 6f74   should have not
-0001ac10: 6966 6965 6420 7468 6520 7573 6572 0a20  ified the user. 
-0001ac20: 2020 2020 2020 2073 656c 662e 6d6f 636b         self.mock
-0001ac30: 735b 276e 6f74 6966 7927 5d2e 6173 7365  s['notify'].asse
-0001ac40: 7274 5f63 616c 6c65 645f 7769 7468 280a  rt_called_with(.
-0001ac50: 2020 2020 2020 2020 2020 2020 2741 6e79              'Any
-0001ac60: 2063 6f6e 7461 6374 2069 6e66 6f72 6d61   contact informa
-0001ac70: 7469 6f6e 2061 7373 6f63 6961 7465 6420  tion associated 
-0001ac80: 7769 7468 2074 6869 7320 6163 636f 756e  with this accoun
-0001ac90: 7420 6861 7320 6265 656e 2072 656d 6f76  t has been remov
-0001aca0: 6564 2e27 0a20 2020 2020 2020 2029 0a20  ed.'.        ). 
-0001acb0: 2020 2020 2020 2023 2057 6520 7368 6f75         # We shou
-0001acc0: 6c64 206e 6f74 2068 6176 6520 6361 6c6c  ld not have call
-0001acd0: 6564 2073 7562 7363 7269 7074 696f 6e20  ed subscription 
-0001ace0: 6265 6361 7573 6520 7468 6572 6527 7320  because there's 
-0001acf0: 6e6f 2065 6d61 696c 0a20 2020 2020 2020  no email.       
-0001ad00: 2073 656c 662e 6d6f 636b 735b 2770 7265   self.mocks['pre
-0001ad10: 7061 7265 5f73 7562 275d 2e61 7373 6572  pare_sub'].asser
-0001ad20: 745f 6e6f 745f 6361 6c6c 6564 2829 0a0a  t_not_called()..
-0001ad30: 2020 2020 6465 6620 7465 7374 5f6e 6f5f      def test_no_
-0001ad40: 6578 6973 7469 6e67 5f61 6363 6f75 6e74  existing_account
-0001ad50: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0001ad60: 2022 2222 5465 7374 2074 6861 7420 6e6f   """Test that no
-0001ad70: 2065 7869 7374 696e 6720 6163 636f 756e   existing accoun
-0001ad80: 7420 6973 2068 616e 646c 6564 2063 6f72  t is handled cor
-0001ad90: 7265 6374 6c79 2222 220a 2020 2020 2020  rectly""".      
-0001ada0: 2020 6d6f 636b 5f73 746f 7261 6765 203d    mock_storage =
-0001adb0: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
-0001adc0: 290a 2020 2020 2020 2020 6d6f 636b 5f73  ).        mock_s
-0001add0: 746f 7261 6765 2e66 696e 645f 616c 6c2e  torage.find_all.
-0001ade0: 7265 7475 726e 5f76 616c 7565 203d 205b  return_value = [
-0001adf0: 5d0a 2020 2020 2020 2020 7365 6c66 2e6d  ].        self.m
-0001ae00: 6f63 6b73 5b27 6163 636f 756e 7427 5d2e  ocks['account'].
-0001ae10: 4163 636f 756e 7446 696c 6553 746f 7261  AccountFileStora
-0001ae20: 6765 2e72 6574 7572 6e5f 7661 6c75 6520  ge.return_value 
-0001ae30: 3d20 6d6f 636b 5f73 746f 7261 6765 0a20  = mock_storage. 
-0001ae40: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-0001ae50: 6c66 2e5f 6361 6c6c 285b 2775 7064 6174  lf._call(['updat
-0001ae60: 655f 6163 636f 756e 7427 2c20 272d 2d65  e_account', '--e
-0001ae70: 6d61 696c 272c 2027 7573 6572 4065 7861  mail', 'user@exa
-0001ae80: 6d70 6c65 2e6f 7267 275d 2920 3d3d 205c  mple.org']) == \
-0001ae90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001aea0: 2020 2020 2020 2020 2020 2743 6f75 6c64            'Could
-0001aeb0: 206e 6f74 2066 696e 6420 616e 2065 7869   not find an exi
-0001aec0: 7374 696e 6720 6163 636f 756e 7420 666f  sting account fo
-0001aed0: 7220 7365 7276 6572 2720 5c0a 2020 2020  r server' \.    
-0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aef0: 2020 2020 2027 2068 7474 7073 3a2f 2f61       ' https://a
-0001af00: 636d 652d 7630 322e 6170 692e 6c65 7473  cme-v02.api.lets
-0001af10: 656e 6372 7970 742e 6f72 672f 6469 7265  encrypt.org/dire
-0001af20: 6374 6f72 792e 270a 0a20 2020 2064 6566  ctory.'..    def
-0001af30: 2074 6573 745f 7570 6461 7465 5f61 6363   test_update_acc
-0001af40: 6f75 6e74 5f72 656d 6f76 655f 656d 6169  ount_remove_emai
-0001af50: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-0001af60: 2022 2222 5465 7374 2074 6861 7420 2d2d   """Test that --
-0001af70: 7265 6769 7374 6572 2d75 6e73 6166 656c  register-unsafel
-0001af80: 792d 7769 7468 6f75 742d 656d 6169 6c20  y-without-email 
-0001af90: 6973 2068 616e 646c 6564 2061 7320 6e6f  is handled as no
-0001afa0: 2065 6d61 696c 2222 220a 2020 2020 2020   email""".      
-0001afb0: 2020 7365 6c66 2e5f 7465 7374 5f75 7064    self._test_upd
-0001afc0: 6174 655f 6e6f 5f63 6f6e 7461 6374 285b  ate_no_contact([
-0001afd0: 2775 7064 6174 655f 6163 636f 756e 7427  'update_account'
-0001afe0: 2c20 272d 2d72 6567 6973 7465 722d 756e  , '--register-un
-0001aff0: 7361 6665 6c79 2d77 6974 686f 7574 2d65  safely-without-e
-0001b000: 6d61 696c 275d 290a 0a20 2020 2064 6566  mail'])..    def
-0001b010: 2074 6573 745f 7570 6461 7465 5f61 6363   test_update_acc
-0001b020: 6f75 6e74 5f65 6d70 7479 5f65 6d61 696c  ount_empty_email
-0001b030: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001b040: 2222 2254 6573 7420 7468 6174 2070 726f  """Test that pro
-0001b050: 7669 6469 6e67 2061 6e20 656d 7074 7920  viding an empty 
-0001b060: 656d 6169 6c20 6973 2068 616e 646c 6564  email is handled
-0001b070: 2061 7320 6e6f 2065 6d61 696c 2222 220a   as no email""".
-0001b080: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
-0001b090: 7374 5f75 7064 6174 655f 6e6f 5f63 6f6e  st_update_no_con
-0001b0a0: 7461 6374 285b 2775 7064 6174 655f 6163  tact(['update_ac
-0001b0b0: 636f 756e 7427 2c20 272d 6d27 2c20 2727  count', '-m', ''
-0001b0c0: 5d29 0a0a 2020 2020 406d 6f63 6b2e 7061  ])..    @mock.pa
-0001b0d0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
-0001b0e0: 7465 726e 616c 2e6d 6169 6e2e 6469 7370  ternal.main.disp
-0001b0f0: 6c61 795f 6f70 732e 6765 745f 656d 6169  lay_ops.get_emai
-0001b100: 6c27 290a 2020 2020 6465 6620 7465 7374  l').    def test
-0001b110: 5f75 7064 6174 655f 6163 636f 756e 745f  _update_account_
-0001b120: 7769 7468 5f65 6d61 696c 2873 656c 662c  with_email(self,
-0001b130: 206d 6f63 6b5f 656d 6169 6c29 3a0a 2020   mock_email):.  
-0001b140: 2020 2020 2020 2222 2254 6573 7420 7468        """Test th
-0001b150: 6174 2075 7064 6174 696e 6720 7769 7468  at updating with
-0001b160: 2061 2073 696e 6775 6c61 7220 656d 6169   a singular emai
-0001b170: 6c20 6973 2068 616e 646c 6564 2063 6f72  l is handled cor
-0001b180: 7265 6374 6c79 2222 220a 2020 2020 2020  rectly""".      
-0001b190: 2020 6d6f 636b 5f65 6d61 696c 2e72 6574    mock_email.ret
-0001b1a0: 7572 6e5f 7661 6c75 6520 3d20 2775 7365  urn_value = 'use
-0001b1b0: 7240 6578 616d 706c 652e 636f 6d27 0a20  r@example.com'. 
-0001b1c0: 2020 2020 2020 2028 5f2c 206d 6f63 6b5f         (_, mock_
-0001b1d0: 7374 6f72 6167 652c 205f 2920 3d20 7365  storage, _) = se
-0001b1e0: 6c66 2e5f 7072 6570 6172 655f 6d6f 636b  lf._prepare_mock
-0001b1f0: 5f61 6363 6f75 6e74 2829 0a20 2020 2020  _account().     
-0001b200: 2020 206d 6f63 6b5f 636c 6965 6e74 203d     mock_client =
-0001b210: 206d 6f63 6b2e 4d61 6769 634d 6f63 6b28   mock.MagicMock(
-0001b220: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-0001b230: 6f63 6b73 5b27 636c 6965 6e74 275d 2e43  ocks['client'].C
-0001b240: 6c69 656e 742e 7265 7475 726e 5f76 616c  lient.return_val
-0001b250: 7565 203d 206d 6f63 6b5f 636c 6965 6e74  ue = mock_client
-0001b260: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0001b270: 203d 2073 656c 662e 5f63 616c 6c28 5b27   = self._call(['
-0001b280: 7570 6461 7465 5f61 6363 6f75 6e74 275d  update_account']
-0001b290: 290a 2020 2020 2020 2020 2320 4e6f 6e65  ).        # None
-0001b2a0: 2069 6620 7265 6769 7374 7261 7469 6f6e   if registration
-0001b2b0: 2073 7563 6365 6564 730a 2020 2020 2020   succeeds.      
-0001b2c0: 2020 6173 7365 7274 2072 6573 756c 7420    assert result 
-0001b2d0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
-0001b2e0: 2320 5765 2073 686f 756c 6420 6861 7665  # We should have
-0001b2f0: 2075 7064 6174 6564 2074 6865 2073 6572   updated the ser
-0001b300: 7665 720a 2020 2020 2020 2020 6173 7365  ver.        asse
-0001b310: 7274 206d 6f63 6b5f 636c 6965 6e74 2e61  rt mock_client.a
-0001b320: 636d 652e 7570 6461 7465 5f72 6567 6973  cme.update_regis
-0001b330: 7472 6174 696f 6e2e 6361 6c6c 5f63 6f75  tration.call_cou
-0001b340: 6e74 203d 3d20 310a 2020 2020 2020 2020  nt == 1.        
-0001b350: 2320 5765 2073 686f 756c 6420 6861 7665  # We should have
-0001b360: 2075 7064 6174 6564 2074 6865 2061 6363   updated the acc
-0001b370: 6f75 6e74 206f 6e20 6469 736b 0a20 2020  ount on disk.   
-0001b380: 2020 2020 2061 7373 6572 7420 6d6f 636b       assert mock
-0001b390: 5f73 746f 7261 6765 2e75 7064 6174 655f  _storage.update_
-0001b3a0: 7265 6772 2e63 616c 6c5f 636f 756e 7420  regr.call_count 
-0001b3b0: 3d3d 2031 0a20 2020 2020 2020 2023 2053  == 1.        # S
-0001b3c0: 7562 7363 7269 7074 696f 6e20 7368 6f75  ubscription shou
-0001b3d0: 6c64 2068 6176 6520 6265 656e 2070 726f  ld have been pro
-0001b3e0: 6d70 7465 640a 2020 2020 2020 2020 6173  mpted.        as
-0001b3f0: 7365 7274 2073 656c 662e 6d6f 636b 735b  sert self.mocks[
-0001b400: 2770 7265 7061 7265 5f73 7562 275d 2e63  'prepare_sub'].c
-0001b410: 616c 6c5f 636f 756e 7420 3d3d 2031 0a20  all_count == 1. 
-0001b420: 2020 2020 2020 2023 2053 686f 756c 6420         # Should 
-0001b430: 6861 7665 2070 7269 6e74 6564 2074 6865  have printed the
-0001b440: 2065 6d61 696c 0a20 2020 2020 2020 2073   email.        s
-0001b450: 656c 662e 6d6f 636b 735b 276e 6f74 6966  elf.mocks['notif
-0001b460: 7927 5d2e 6173 7365 7274 5f63 616c 6c65  y'].assert_calle
-0001b470: 645f 7769 7468 280a 2020 2020 2020 2020  d_with(.        
-0001b480: 2020 2020 2759 6f75 7220 652d 6d61 696c      'Your e-mail
-0001b490: 2061 6464 7265 7373 2077 6173 2075 7064   address was upd
-0001b4a0: 6174 6564 2074 6f20 7573 6572 4065 7861  ated to user@exa
-0001b4b0: 6d70 6c65 2e63 6f6d 2e27 290a 0a20 2020  mple.com.')..   
-0001b4c0: 2064 6566 2074 6573 745f 7570 6461 7465   def test_update
-0001b4d0: 5f61 6363 6f75 6e74 5f77 6974 685f 6d75  _account_with_mu
-0001b4e0: 6c74 6970 6c65 5f65 6d61 696c 7328 7365  ltiple_emails(se
-0001b4f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0001b500: 5465 7374 2074 6861 7420 6d75 6c74 6970  Test that multip
-0001b510: 6c65 2065 6d61 696c 2061 6464 7265 7373  le email address
-0001b520: 6573 2061 7265 2068 616e 646c 6564 2063  es are handled c
-0001b530: 6f72 7265 6374 6c79 2222 220a 2020 2020  orrectly""".    
-0001b540: 2020 2020 285f 2c20 6d6f 636b 5f73 746f      (_, mock_sto
-0001b550: 7261 6765 2c20 6d6f 636b 5f72 6567 7229  rage, mock_regr)
-0001b560: 203d 2073 656c 662e 5f70 7265 7061 7265   = self._prepare
-0001b570: 5f6d 6f63 6b5f 6163 636f 756e 7428 290a  _mock_account().
-0001b580: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-0001b590: 656c 662e 5f63 616c 6c28 5b27 7570 6461  elf._call(['upda
-0001b5a0: 7465 5f61 6363 6f75 6e74 272c 2027 2d6d  te_account', '-m
-0001b5b0: 272c 2027 7573 6572 4065 7861 6d70 6c65  ', 'user@example
-0001b5c0: 2e63 6f6d 2c75 7365 7240 6578 616d 706c  .com,user@exampl
-0001b5d0: 652e 6f72 6727 5d29 2069 7320 4e6f 6e65  e.org']) is None
-0001b5e0: 0a20 2020 2020 2020 206d 6f63 6b5f 7265  .        mock_re
-0001b5f0: 6772 2e62 6f64 792e 7570 6461 7465 2e61  gr.body.update.a
-0001b600: 7373 6572 745f 6361 6c6c 6564 5f77 6974  ssert_called_wit
-0001b610: 6828 0a20 2020 2020 2020 2020 2020 2063  h(.            c
-0001b620: 6f6e 7461 6374 3d5b 276d 6169 6c74 6f3a  ontact=['mailto:
-0001b630: 7573 6572 4065 7861 6d70 6c65 2e63 6f6d  user@example.com
-0001b640: 272c 2027 6d61 696c 746f 3a75 7365 7240  ', 'mailto:user@
-0001b650: 6578 616d 706c 652e 6f72 6727 5d0a 2020  example.org'].  
-0001b660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001b670: 6173 7365 7274 206d 6f63 6b5f 7374 6f72  assert mock_stor
-0001b680: 6167 652e 7570 6461 7465 5f72 6567 722e  age.update_regr.
-0001b690: 6361 6c6c 5f63 6f75 6e74 203d 3d20 310a  call_count == 1.
-0001b6a0: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
-0001b6b0: 6b73 5b27 6e6f 7469 6679 275d 2e61 7373  ks['notify'].ass
-0001b6c0: 6572 745f 6361 6c6c 6564 5f77 6974 6828  ert_called_with(
-0001b6d0: 0a20 2020 2020 2020 2020 2020 2027 596f  .            'Yo
-0001b6e0: 7572 2065 2d6d 6169 6c20 6164 6472 6573  ur e-mail addres
-0001b6f0: 7320 7761 7320 7570 6461 7465 6420 746f  s was updated to
-0001b700: 2075 7365 7240 6578 616d 706c 652e 636f   user@example.co
-0001b710: 6d2c 7573 6572 4065 7861 6d70 6c65 2e6f  m,user@example.o
-0001b720: 7267 2e27 290a 0a0a 636c 6173 7320 5368  rg.')...class Sh
-0001b730: 6f77 4163 636f 756e 7454 6573 7428 7465  owAccountTest(te
-0001b740: 7374 5f75 7469 6c2e 436f 6e66 6967 5465  st_util.ConfigTe
-0001b750: 7374 4361 7365 293a 0a20 2020 2022 2222  stCase):.    """
-0001b760: 5465 7374 7320 666f 7220 6365 7274 626f  Tests for certbo
-0001b770: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
-0001b780: 2e73 686f 775f 6163 636f 756e 7422 2222  .show_account"""
-0001b790: 0a0a 2020 2020 6465 6620 7365 7455 7028  ..    def setUp(
-0001b7a0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0001b7b0: 6174 6368 6573 203d 207b 0a20 2020 2020  atches = {.     
-0001b7c0: 2020 2020 2020 2027 6163 636f 756e 7427         'account'
-0001b7d0: 3a20 6d6f 636b 2e70 6174 6368 2827 6365  : mock.patch('ce
-0001b7e0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
-0001b7f0: 6d61 696e 2e61 6363 6f75 6e74 2729 2c0a  main.account'),.
-0001b800: 2020 2020 2020 2020 2020 2020 2761 7465              'ate
-0001b810: 7869 7427 3a20 6d6f 636b 2e70 6174 6368  xit': mock.patch
-0001b820: 2827 6365 7274 626f 742e 7574 696c 2e61  ('certbot.util.a
-0001b830: 7465 7869 7427 292c 0a20 2020 2020 2020  texit'),.       
-0001b840: 2020 2020 2027 636c 6965 6e74 273a 206d       'client': m
-0001b850: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0001b860: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
-0001b870: 6e2e 636c 6965 6e74 2729 2c0a 2020 2020  n.client'),.    
-0001b880: 2020 2020 2020 2020 2764 6574 6572 6d69          'determi
-0001b890: 6e65 5f61 6363 6f75 6e74 273a 206d 6f63  ne_account': moc
-0001b8a0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
-0001b8b0: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
-0001b8c0: 5f64 6574 6572 6d69 6e65 5f61 6363 6f75  _determine_accou
-0001b8d0: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
-0001b8e0: 2020 276e 6f74 6966 7927 3a20 6d6f 636b    'notify': mock
-0001b8f0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
-0001b900: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e64  _internal.main.d
-0001b910: 6973 706c 6179 5f75 7469 6c2e 6e6f 7469  isplay_util.noti
-0001b920: 6679 2729 2c0a 2020 2020 2020 2020 2020  fy'),.          
-0001b930: 2020 2775 7469 6c27 3a20 7465 7374 5f75    'util': test_u
-0001b940: 7469 6c2e 7061 7463 685f 6469 7370 6c61  til.patch_displa
-0001b950: 795f 7574 696c 2829 0a20 2020 2020 2020  y_util().       
-0001b960: 207d 0a20 2020 2020 2020 2073 656c 662e   }.        self.
-0001b970: 6d6f 636b 7320 3d20 7b20 6b3a 2070 6174  mocks = { k: pat
-0001b980: 6368 6573 5b6b 5d2e 7374 6172 7428 2920  ches[k].start() 
-0001b990: 666f 7220 6b20 696e 2070 6174 6368 6573  for k in patches
-0001b9a0: 207d 0a20 2020 2020 2020 2066 6f72 2070   }.        for p
-0001b9b0: 6174 6368 2069 6e20 7061 7463 6865 732e  atch in patches.
-0001b9c0: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
-0001b9d0: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
-0001b9e0: 6561 6e75 7028 7061 7463 682e 7374 6f70  eanup(patch.stop
-0001b9f0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001ba00: 6e20 7375 7065 7228 292e 7365 7455 7028  n super().setUp(
-0001ba10: 290a 0a20 2020 2064 6566 205f 6361 6c6c  )..    def _call
-0001ba20: 2873 656c 662c 2061 7267 7329 3a0a 2020  (self, args):.  
-0001ba30: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
-0001ba40: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-0001ba50: 696e 7465 726e 616c 2e6d 6169 6e2e 7379  internal.main.sy
-0001ba60: 732e 7374 646f 7574 2729 2c20 5c0a 2020  s.stdout'), \.  
-0001ba70: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
-0001ba80: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
-0001ba90: 696e 7465 726e 616c 2e6d 6169 6e2e 7379  internal.main.sy
-0001baa0: 732e 7374 6465 7272 2729 3a0a 2020 2020  s.stderr'):.    
-0001bab0: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
-0001bac0: 272d 2d63 6f6e 6669 672d 6469 7227 2c20  '--config-dir', 
-0001bad0: 7365 6c66 2e63 6f6e 6669 672e 636f 6e66  self.config.conf
-0001bae0: 6967 5f64 6972 2c0a 2020 2020 2020 2020  ig_dir,.        
-0001baf0: 2020 2020 2020 2020 2020 2020 272d 2d77              '--w
-0001bb00: 6f72 6b2d 6469 7227 2c20 7365 6c66 2e63  ork-dir', self.c
-0001bb10: 6f6e 6669 672e 776f 726b 5f64 6972 2c0a  onfig.work_dir,.
-0001bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb30: 2020 2020 272d 2d6c 6f67 732d 6469 7227      '--logs-dir'
-0001bb40: 2c20 7365 6c66 2e63 6f6e 6669 672e 6c6f  , self.config.lo
-0001bb50: 6773 5f64 6972 2c20 272d 2d74 6578 7427  gs_dir, '--text'
-0001bb60: 5d20 2b20 6172 6773 0a20 2020 2020 2020  ] + args.       
-0001bb70: 2020 2020 2072 6574 7572 6e20 6d61 696e       return main
-0001bb80: 2e6d 6169 6e28 6172 6773 5b3a 5d29 2023  .main(args[:]) #
-0001bb90: 204e 4f54 453a 2070 6172 7365 7220 6361   NOTE: parser ca
-0001bba0: 6e20 616c 7465 7220 6974 7320 6172 6773  n alter its args
-0001bbb0: 210a 0a20 2020 2064 6566 205f 7072 6570  !..    def _prep
-0001bbc0: 6172 655f 6d6f 636b 5f61 6363 6f75 6e74  are_mock_account
-0001bbd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001bbe0: 6d6f 636b 5f73 746f 7261 6765 203d 206d  mock_storage = m
-0001bbf0: 6f63 6b2e 4d61 6769 634d 6f63 6b28 290a  ock.MagicMock().
-0001bc00: 2020 2020 2020 2020 6d6f 636b 5f61 6363          mock_acc
-0001bc10: 6f75 6e74 203d 206d 6f63 6b2e 4d61 6769  ount = mock.Magi
-0001bc20: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
-0001bc30: 6d6f 636b 5f72 6567 7220 3d20 6d6f 636b  mock_regr = mock
-0001bc40: 2e4d 6167 6963 4d6f 636b 2829 0a20 2020  .MagicMock().   
-0001bc50: 2020 2020 206d 6f63 6b5f 7374 6f72 6167       mock_storag
-0001bc60: 652e 6669 6e64 5f61 6c6c 2e72 6574 7572  e.find_all.retur
-0001bc70: 6e5f 7661 6c75 6520 3d20 5b6d 6f63 6b5f  n_value = [mock_
-0001bc80: 6163 636f 756e 745d 0a20 2020 2020 2020  account].       
-0001bc90: 2073 656c 662e 6d6f 636b 735b 2761 6363   self.mocks['acc
-0001bca0: 6f75 6e74 275d 2e41 6363 6f75 6e74 4669  ount'].AccountFi
-0001bcb0: 6c65 5374 6f72 6167 652e 7265 7475 726e  leStorage.return
-0001bcc0: 5f76 616c 7565 203d 206d 6f63 6b5f 7374  _value = mock_st
-0001bcd0: 6f72 6167 650a 2020 2020 2020 2020 6d6f  orage.        mo
-0001bce0: 636b 5f61 6363 6f75 6e74 2e72 6567 722e  ck_account.regr.
-0001bcf0: 626f 6479 203d 206d 6f63 6b5f 7265 6772  body = mock_regr
-0001bd00: 2e62 6f64 790a 2020 2020 2020 2020 6d6f  .body.        mo
-0001bd10: 636b 5f61 6363 6f75 6e74 2e6b 6579 2e74  ck_account.key.t
-0001bd20: 6875 6d62 7072 696e 742e 7265 7475 726e  humbprint.return
-0001bd30: 5f76 616c 7565 203d 2062 2766 6f6f 6261  _value = b'fooba
-0001bd40: 7262 617a 270a 2020 2020 2020 2020 7365  rbaz'.        se
-0001bd50: 6c66 2e6d 6f63 6b73 5b27 6465 7465 726d  lf.mocks['determ
-0001bd60: 696e 655f 6163 636f 756e 7427 5d2e 7265  ine_account'].re
-0001bd70: 7475 726e 5f76 616c 7565 203d 2028 6d6f  turn_value = (mo
-0001bd80: 636b 5f61 6363 6f75 6e74 2c20 6d6f 636b  ck_account, mock
-0001bd90: 2e4d 6167 6963 4d6f 636b 2829 290a 0a20  .MagicMock()).. 
-0001bda0: 2020 2064 6566 205f 7465 7374 5f73 686f     def _test_sho
-0001bdb0: 775f 6163 636f 756e 7428 7365 6c66 2c20  w_account(self, 
-0001bdc0: 636f 6e74 6163 7429 3a0a 2020 2020 2020  contact):.      
-0001bdd0: 2020 7365 6c66 2e5f 7072 6570 6172 655f    self._prepare_
-0001bde0: 6d6f 636b 5f61 6363 6f75 6e74 2829 0a20  mock_account(). 
-0001bdf0: 2020 2020 2020 206d 6f63 6b5f 636c 6965         mock_clie
-0001be00: 6e74 203d 206d 6f63 6b2e 4d61 6769 634d  nt = mock.MagicM
-0001be10: 6f63 6b28 290a 2020 2020 2020 2020 6d6f  ock().        mo
-0001be20: 636b 5f72 6567 7220 3d20 6d6f 636b 2e4d  ck_regr = mock.M
-0001be30: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
-0001be40: 2020 206d 6f63 6b5f 7265 6772 2e62 6f64     mock_regr.bod
-0001be50: 792e 636f 6e74 6163 7420 3d20 636f 6e74  y.contact = cont
-0001be60: 6163 740a 2020 2020 2020 2020 6d6f 636b  act.        mock
-0001be70: 5f72 6567 722e 7572 6920 3d20 2768 7474  _regr.uri = 'htt
-0001be80: 7073 3a2f 2f77 7777 2e6c 6574 7365 6e63  ps://www.letsenc
-0001be90: 7279 7074 2d64 656d 6f2e 6f72 672f 6163  rypt-demo.org/ac
-0001bea0: 6d65 2f72 6567 2f31 270a 2020 2020 2020  me/reg/1'.      
-0001beb0: 2020 6d6f 636b 5f63 6c69 656e 742e 6163    mock_client.ac
-0001bec0: 6d65 2e71 7565 7279 5f72 6567 6973 7472  me.query_registr
-0001bed0: 6174 696f 6e2e 7265 7475 726e 5f76 616c  ation.return_val
-0001bee0: 7565 203d 206d 6f63 6b5f 7265 6772 0a20  ue = mock_regr. 
-0001bef0: 2020 2020 2020 2073 656c 662e 6d6f 636b         self.mock
-0001bf00: 735b 2763 6c69 656e 7427 5d2e 436c 6965  s['client'].Clie
-0001bf10: 6e74 2e72 6574 7572 6e5f 7661 6c75 6520  nt.return_value 
-0001bf20: 3d20 6d6f 636b 5f63 6c69 656e 740a 0a20  = mock_client.. 
-0001bf30: 2020 2020 2020 2061 7267 7320 3d20 5b27         args = ['
-0001bf40: 7368 6f77 5f61 6363 6f75 6e74 275d 0a0a  show_account']..
-0001bf50: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-0001bf60: 6c6c 2861 7267 7329 0a0a 2020 2020 2020  ll(args)..      
-0001bf70: 2020 6173 7365 7274 206d 6f63 6b5f 636c    assert mock_cl
-0001bf80: 6965 6e74 2e61 636d 652e 7175 6572 795f  ient.acme.query_
-0001bf90: 7265 6769 7374 7261 7469 6f6e 2e63 616c  registration.cal
-0001bfa0: 6c5f 636f 756e 7420 3d3d 2031 0a0a 2020  l_count == 1..  
-0001bfb0: 2020 6465 6620 7465 7374 5f6e 6f5f 6578    def test_no_ex
-0001bfc0: 6973 7469 6e67 5f61 6363 6f75 6e74 7328  isting_accounts(
-0001bfd0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0001bfe0: 2222 5465 7374 2074 6861 7420 6e6f 2065  ""Test that no e
-0001bff0: 7869 7374 696e 6720 6163 636f 756e 7420  xisting account 
-0001c000: 6973 2068 616e 646c 6564 2063 6f72 7265  is handled corre
-0001c010: 6374 6c79 2222 220a 2020 2020 2020 2020  ctly""".        
-0001c020: 6d6f 636b 5f73 746f 7261 6765 203d 206d  mock_storage = m
-0001c030: 6f63 6b2e 4d61 6769 634d 6f63 6b28 290a  ock.MagicMock().
-0001c040: 2020 2020 2020 2020 6d6f 636b 5f73 746f          mock_sto
-0001c050: 7261 6765 2e66 696e 645f 616c 6c2e 7265  rage.find_all.re
-0001c060: 7475 726e 5f76 616c 7565 203d 205b 5d0a  turn_value = [].
-0001c070: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
-0001c080: 6b73 5b27 6163 636f 756e 7427 5d2e 4163  ks['account'].Ac
-0001c090: 636f 756e 7446 696c 6553 746f 7261 6765  countFileStorage
-0001c0a0: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
-0001c0b0: 6d6f 636b 5f73 746f 7261 6765 0a20 2020  mock_storage.   
-0001c0c0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0001c0d0: 2e5f 6361 6c6c 285b 2773 686f 775f 6163  ._call(['show_ac
-0001c0e0: 636f 756e 7427 5d29 203d 3d20 5c0a 2020  count']) == \.  
-0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c100: 2020 2020 2020 2027 436f 756c 6420 6e6f         'Could no
-0001c110: 7420 6669 6e64 2061 6e20 6578 6973 7469  t find an existi
-0001c120: 6e67 2061 6363 6f75 6e74 2066 6f72 2073  ng account for s
-0001c130: 6572 7665 7227 205c 0a20 2020 2020 2020  erver' \.       
-0001c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c150: 2020 2720 6874 7470 733a 2f2f 6163 6d65    ' https://acme
-0001c160: 2d76 3032 2e61 7069 2e6c 6574 7365 6e63  -v02.api.letsenc
-0001c170: 7279 7074 2e6f 7267 2f64 6972 6563 746f  rypt.org/directo
-0001c180: 7279 2e27 0a0a 2020 2020 6465 6620 7465  ry.'..    def te
-0001c190: 7374 5f6e 6f5f 6578 6973 7469 6e67 5f63  st_no_existing_c
-0001c1a0: 6c69 656e 7428 7365 6c66 293a 0a20 2020  lient(self):.   
-0001c1b0: 2020 2020 2022 2222 5465 7374 2074 6861       """Test tha
-0001c1c0: 7420 6973 7375 6573 2077 6974 6820 7468  t issues with th
-0001c1d0: 6520 4143 4d45 2063 6c69 656e 7420 6172  e ACME client ar
-0001c1e0: 6520 6861 6e64 6c65 6420 636f 7272 6563  e handled correc
-0001c1f0: 746c 7922 2222 0a20 2020 2020 2020 2073  tly""".        s
-0001c200: 656c 662e 5f70 7265 7061 7265 5f6d 6f63  elf._prepare_moc
-0001c210: 6b5f 6163 636f 756e 7428 290a 2020 2020  k_account().    
-0001c220: 2020 2020 6d6f 636b 5f63 6c69 656e 7420      mock_client 
-0001c230: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
-0001c240: 2829 0a20 2020 2020 2020 206d 6f63 6b5f  ().        mock_
-0001c250: 636c 6965 6e74 2e61 636d 6520 3d20 4e6f  client.acme = No
-0001c260: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-0001c270: 6d6f 636b 735b 2763 6c69 656e 7427 5d2e  mocks['client'].
-0001c280: 436c 6965 6e74 2e72 6574 7572 6e5f 7661  Client.return_va
-0001c290: 6c75 6520 3d20 6d6f 636b 5f63 6c69 656e  lue = mock_clien
-0001c2a0: 740a 2020 2020 2020 2020 7472 793a 0a20  t.        try:. 
-0001c2b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c2c0: 5f63 616c 6c28 5b27 7368 6f77 5f61 6363  _call(['show_acc
-0001c2d0: 6f75 6e74 275d 290a 2020 2020 2020 2020  ount']).        
-0001c2e0: 6578 6365 7074 2065 7272 6f72 732e 4572  except errors.Er
-0001c2f0: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-0001c300: 2020 2020 2020 6173 7365 7274 2027 4143        assert 'AC
-0001c310: 4d45 2063 6c69 656e 7420 6973 206e 6f74  ME client is not
-0001c320: 2073 6574 2e27 203d 3d20 7374 7228 6529   set.' == str(e)
-0001c330: 0a0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
-0001c340: 6f5f 636f 6e74 6163 7473 2873 656c 6629  o_contacts(self)
-0001c350: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-0001c360: 7465 7374 5f73 686f 775f 6163 636f 756e  test_show_accoun
-0001c370: 7428 2829 290a 0a20 2020 2020 2020 2061  t(())..        a
-0001c380: 7373 6572 7420 7365 6c66 2e6d 6f63 6b73  ssert self.mocks
-0001c390: 5b27 6e6f 7469 6679 275d 2e63 616c 6c5f  ['notify'].call_
-0001c3a0: 636f 756e 7420 3d3d 2031 0a20 2020 2020  count == 1.     
-0001c3b0: 2020 2073 656c 662e 6d6f 636b 735b 276e     self.mocks['n
-0001c3c0: 6f74 6966 7927 5d2e 6173 7365 7274 5f68  otify'].assert_h
-0001c3d0: 6173 5f63 616c 6c73 285b 0a20 2020 2020  as_calls([.     
-0001c3e0: 2020 2020 2020 206d 6f63 6b2e 6361 6c6c         mock.call
-0001c3f0: 2827 4163 636f 756e 7420 6465 7461 696c  ('Account detail
-0001c400: 7320 666f 7220 7365 7276 6572 2068 7474  s for server htt
-0001c410: 7073 3a2f 2f61 636d 652d 7630 322e 6170  ps://acme-v02.ap
-0001c420: 692e 6c65 7473 656e 6372 270a 2020 2020  i.letsencr'.    
-0001c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c440: 2020 2779 7074 2e6f 7267 2f64 6972 6563    'ypt.org/direc
-0001c450: 746f 7279 3a5c 6e20 2041 6363 6f75 6e74  tory:\n  Account
-0001c460: 2055 524c 3a20 6874 7470 733a 2f2f 7777   URL: https://ww
-0001c470: 772e 6c65 7473 656e 6372 7927 0a20 2020  w.letsencry'.   
-0001c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c490: 2020 2027 7074 2d64 656d 6f2e 6f72 672f     'pt-demo.org/
-0001c4a0: 6163 6d65 2f72 6567 2f31 5c6e 2020 4163  acme/reg/1\n  Ac
-0001c4b0: 636f 756e 7420 5468 756d 6270 7269 6e74  count Thumbprint
-0001c4c0: 3a20 5a6d 3976 596d 4679 596d 4636 5c6e  : Zm9vYmFyYmF6\n
-0001c4d0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001c4e0: 2020 2020 2020 2020 2720 2045 6d61 696c          '  Email
-0001c4f0: 2063 6f6e 7461 6374 3a20 6e6f 6e65 2729   contact: none')
-0001c500: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
-0001c510: 5f73 696e 676c 655f 656d 6169 6c28 7365  _single_email(se
-0001c520: 6c66 293a 0a20 2020 2020 2020 2063 6f6e  lf):.        con
-0001c530: 7461 6374 203d 2028 276d 6169 6c74 6f3a  tact = ('mailto:
-0001c540: 666f 6f40 6578 616d 706c 652e 636f 6d27  foo@example.com'
-0001c550: 2c29 0a20 2020 2020 2020 2073 656c 662e  ,).        self.
-0001c560: 5f74 6573 745f 7368 6f77 5f61 6363 6f75  _test_show_accou
-0001c570: 6e74 2863 6f6e 7461 6374 290a 0a20 2020  nt(contact)..   
-0001c580: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0001c590: 2e6d 6f63 6b73 5b27 6e6f 7469 6679 275d  .mocks['notify']
-0001c5a0: 2e63 616c 6c5f 636f 756e 7420 3d3d 2031  .call_count == 1
-0001c5b0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-0001c5c0: 636b 735b 276e 6f74 6966 7927 5d2e 6173  cks['notify'].as
-0001c5d0: 7365 7274 5f68 6173 5f63 616c 6c73 285b  sert_has_calls([
-0001c5e0: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
-0001c5f0: 6b2e 6361 6c6c 2827 4163 636f 756e 7420  k.call('Account 
-0001c600: 6465 7461 696c 7320 666f 7220 7365 7276  details for serv
-0001c610: 6572 2068 7474 7073 3a2f 2f61 636d 652d  er https://acme-
-0001c620: 7630 322e 6170 692e 6c65 7473 656e 6372  v02.api.letsencr
-0001c630: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001c640: 2020 2020 2020 2020 2779 7074 2e6f 7267          'ypt.org
-0001c650: 2f64 6972 6563 746f 7279 3a5c 6e20 2041  /directory:\n  A
-0001c660: 6363 6f75 6e74 2055 524c 3a20 6874 7470  ccount URL: http
-0001c670: 733a 2f2f 7777 772e 6c65 7473 656e 6372  s://www.letsencr
-0001c680: 7927 0a20 2020 2020 2020 2020 2020 2020  y'.             
-0001c690: 2020 2020 2020 2020 2027 7074 2d64 656d           'pt-dem
-0001c6a0: 6f2e 6f72 672f 6163 6d65 2f72 6567 2f31  o.org/acme/reg/1
-0001c6b0: 5c6e 2020 4163 636f 756e 7420 5468 756d  \n  Account Thum
-0001c6c0: 6270 7269 6e74 3a20 5a6d 3976 596d 4679  bprint: Zm9vYmFy
-0001c6d0: 596d 4636 270a 2020 2020 2020 2020 2020  YmF6'.          
-0001c6e0: 2020 2020 2020 2020 2020 2020 275c 6e20              '\n 
-0001c6f0: 2045 6d61 696c 2063 6f6e 7461 6374 3a20   Email contact: 
-0001c700: 666f 6f40 6578 616d 706c 652e 636f 6d27  foo@example.com'
-0001c710: 295d 290a 0a20 2020 2064 6566 2074 6573  )])..    def tes
-0001c720: 745f 646f 7562 6c65 5f65 6d61 696c 2873  t_double_email(s
-0001c730: 656c 6629 3a0a 2020 2020 2020 2020 636f  elf):.        co
-0001c740: 6e74 6163 7420 3d20 2827 6d61 696c 746f  ntact = ('mailto
-0001c750: 3a66 6f6f 4065 7861 6d70 6c65 2e63 6f6d  :foo@example.com
-0001c760: 272c 2027 6d61 696c 746f 3a62 6172 4065  ', 'mailto:bar@e
-0001c770: 7861 6d70 6c65 2e63 6f6d 2729 0a20 2020  xample.com').   
-0001c780: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-0001c790: 7368 6f77 5f61 6363 6f75 6e74 2863 6f6e  show_account(con
-0001c7a0: 7461 6374 290a 0a20 2020 2020 2020 2061  tact)..        a
-0001c7b0: 7373 6572 7420 7365 6c66 2e6d 6f63 6b73  ssert self.mocks
-0001c7c0: 5b27 6e6f 7469 6679 275d 2e63 616c 6c5f  ['notify'].call_
-0001c7d0: 636f 756e 7420 3d3d 2031 0a20 2020 2020  count == 1.     
-0001c7e0: 2020 2073 656c 662e 6d6f 636b 735b 276e     self.mocks['n
-0001c7f0: 6f74 6966 7927 5d2e 6173 7365 7274 5f68  otify'].assert_h
-0001c800: 6173 5f63 616c 6c73 285b 0a20 2020 2020  as_calls([.     
-0001c810: 2020 2020 2020 206d 6f63 6b2e 6361 6c6c         mock.call
-0001c820: 2827 4163 636f 756e 7420 6465 7461 696c  ('Account detail
-0001c830: 7320 666f 7220 7365 7276 6572 2068 7474  s for server htt
-0001c840: 7073 3a2f 2f61 636d 652d 7630 322e 6170  ps://acme-v02.ap
-0001c850: 692e 6c65 7473 656e 6372 270a 2020 2020  i.letsencr'.    
-0001c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c870: 2020 2779 7074 2e6f 7267 2f64 6972 6563    'ypt.org/direc
-0001c880: 746f 7279 3a5c 6e20 2041 6363 6f75 6e74  tory:\n  Account
-0001c890: 2055 524c 3a20 6874 7470 733a 2f2f 7777   URL: https://ww
-0001c8a0: 772e 6c65 7473 656e 6372 7927 0a20 2020  w.letsencry'.   
-0001c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c8c0: 2020 2027 7074 2d64 656d 6f2e 6f72 672f     'pt-demo.org/
-0001c8d0: 6163 6d65 2f72 6567 2f31 5c6e 2020 4163  acme/reg/1\n  Ac
-0001c8e0: 636f 756e 7420 5468 756d 6270 7269 6e74  count Thumbprint
-0001c8f0: 3a20 5a6d 3976 596d 4679 596d 4636 5c6e  : Zm9vYmFyYmF6\n
-0001c900: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0001c910: 2020 2020 2020 2020 2720 2045 6d61 696c          '  Email
-0001c920: 2063 6f6e 7461 6374 733a 2066 6f6f 4065   contacts: foo@e
-0001c930: 7861 6d70 6c65 2e63 6f6d 2c20 6261 7240  xample.com, bar@
-0001c940: 6578 616d 706c 652e 636f 6d27 295d 290a  example.com')]).
-0001c950: 0a0a 636c 6173 7320 5465 7374 4c6f 636b  ..class TestLock
-0001c960: 4f72 6465 723a 0a20 2020 2022 2222 5465  Order:.    """Te
-0001c970: 7374 7320 7468 6174 2043 6572 7462 6f74  sts that Certbot
-0001c980: 2773 2064 6972 6563 746f 7279 206c 6f63  's directory loc
-0001c990: 6b73 2077 6572 6520 6163 7175 6972 6564  ks were acquired
-0001c9a0: 2069 6e20 7468 6520 7269 6768 7420 6f72   in the right or
-0001c9b0: 6465 722e 2222 220a 2020 2020 4558 5045  der.""".    EXPE
-0001c9c0: 4354 4544 5f45 5252 4f52 5f54 5950 4520  CTED_ERROR_TYPE 
-0001c9d0: 3d20 6572 726f 7273 2e45 7272 6f72 0a20  = errors.Error. 
-0001c9e0: 2020 2045 5850 4543 5445 445f 4552 524f     EXPECTED_ERRO
-0001c9f0: 525f 5354 5220 3d20 2745 7870 6563 7465  R_STR = 'Expecte
-0001ca00: 6420 5465 7374 4c6f 636b 4f72 6465 7220  d TestLockOrder 
-0001ca10: 6572 726f 7227 0a20 2020 2023 2054 6869  error'.    # Thi
-0001ca20: 7320 7265 6765 7820 6973 206e 6565 6465  s regex is neede
-0001ca30: 6420 6265 6361 7573 6520 6365 7274 626f  d because certbo
-0001ca40: 7420 7265 6e65 7720 6361 7074 7572 6573  t renew captures
-0001ca50: 2072 6169 7365 6420 6572 726f 7273 2061   raised errors a
-0001ca60: 6e64 0a20 2020 2023 2072 6169 7365 7320  nd.    # raises 
-0001ca70: 6974 7320 6f77 6e2e 0a20 2020 2045 5850  its own..    EXP
-0001ca80: 4543 5445 445f 4552 524f 525f 5354 525f  ECTED_ERROR_STR_
-0001ca90: 5245 4745 5820 3d20 6627 7b45 5850 4543  REGEX = f'{EXPEC
-0001caa0: 5445 445f 4552 524f 525f 5354 527d 7c31  TED_ERROR_STR}|1
-0001cab0: 2072 656e 6577 2066 6169 6c75 7265 270a   renew failure'.
-0001cac0: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-0001cad0: 7475 7265 0a20 2020 2064 6566 206d 6f63  ture.    def moc
-0001cae0: 6b5f 6c6f 636b 5f64 6972 2873 656c 6629  k_lock_dir(self)
-0001caf0: 3a0a 2020 2020 2020 2020 7769 7468 206d  :.        with m
-0001cb00: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
-0001cb10: 6f74 2e5f 696e 7465 726e 616c 2e6c 6f63  ot._internal.loc
-0001cb20: 6b2e 6c6f 636b 5f64 6972 2729 2061 7320  k.lock_dir') as 
-0001cb30: 6d6f 636b 5f6c 6f63 6b5f 6469 723a 0a20  mock_lock_dir:. 
-0001cb40: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-0001cb50: 206d 6f63 6b5f 6c6f 636b 5f64 6972 0a0a   mock_lock_dir..
-0001cb60: 2020 2020 4063 6f6e 7465 7874 6c69 622e      @contextlib.
-0001cb70: 636f 6e74 6578 746d 616e 6167 6572 0a20  contextmanager. 
-0001cb80: 2020 2064 6566 206d 6f63 6b5f 706c 7567     def mock_plug
-0001cb90: 696e 5f70 7265 7061 7265 2873 656c 662c  in_prepare(self,
-0001cba0: 2061 7574 6865 6e74 6963 6174 6f72 5f64   authenticator_d
-0001cbb0: 6972 2c20 696e 7374 616c 6c65 725f 6469  ir, installer_di
-0001cbc0: 722c 206d 6f63 6b5f 6c6f 636b 5f64 6972  r, mock_lock_dir
-0001cbd0: 2c20 7375 6263 6f6d 6d61 6e64 293a 0a20  , subcommand):. 
-0001cbe0: 2020 2020 2020 2022 2222 5061 7463 6865         """Patche
-0001cbf0: 7320 706c 7567 696e 2070 7265 7061 7265  s plugin prepare
-0001cc00: 2074 6f20 6361 6c6c 206d 6f63 6b5f 6c6f   to call mock_lo
-0001cc10: 636b 5f64 6972 2061 6e64 2072 6169 7365  ck_dir and raise
-0001cc20: 2074 6865 2065 7870 6563 7465 6420 6572   the expected er
-0001cc30: 726f 722e 2222 220a 2020 2020 2020 2020  ror.""".        
-0001cc40: 6465 6620 6175 7468 656e 7469 6361 746f  def authenticato
-0001cc50: 725f 6c6f 636b 2875 6e75 7365 645f 7365  r_lock(unused_se
-0001cc60: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
-0001cc70: 206d 6f63 6b5f 6c6f 636b 5f64 6972 2861   mock_lock_dir(a
-0001cc80: 7574 6865 6e74 6963 6174 6f72 5f64 6972  uthenticator_dir
-0001cc90: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
-0001cca0: 6973 6520 7365 6c66 2e45 5850 4543 5445  ise self.EXPECTE
-0001ccb0: 445f 4552 524f 525f 5459 5045 2873 656c  D_ERROR_TYPE(sel
-0001ccc0: 662e 4558 5045 4354 4544 5f45 5252 4f52  f.EXPECTED_ERROR
-0001ccd0: 5f53 5452 290a 0a20 2020 2020 2020 2064  _STR)..        d
-0001cce0: 6566 2069 6e73 7461 6c6c 6572 5f6c 6f63  ef installer_loc
-0001ccf0: 6b28 756e 7573 6564 5f73 656c 6629 3a0a  k(unused_self):.
-0001cd00: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-0001cd10: 5f6c 6f63 6b5f 6469 7228 696e 7374 616c  _lock_dir(instal
-0001cd20: 6c65 725f 6469 7229 0a20 2020 2020 2020  ler_dir).       
-0001cd30: 2020 2020 2023 2055 6e6c 6573 7320 616e       # Unless an
-0001cd40: 2069 6e73 7461 6c6c 6572 2069 736e 2774   installer isn't
-0001cd50: 206e 6565 6465 6420 2865 2e67 2e20 6365   needed (e.g. ce
-0001cd60: 7274 626f 7420 696e 7374 616c 6c29 2c20  rtbot install), 
-0001cd70: 7765 0a20 2020 2020 2020 2020 2020 2023  we.            #
-0001cd80: 2065 7870 6563 7420 7468 6520 6175 7468   expect the auth
-0001cd90: 656e 7469 6361 746f 7220 746f 2072 6169  enticator to rai
-0001cda0: 7365 2074 6865 2065 7870 6563 7465 6420  se the expected 
-0001cdb0: 6572 726f 7220 6265 6361 7573 6520 6974  error because it
-0001cdc0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0001cdd0: 7320 7072 6570 6172 6564 206c 6173 742e  s prepared last.
-0001cde0: 2053 6565 0a20 2020 2020 2020 2020 2020   See.           
-0001cdf0: 2023 2068 7474 7073 3a2f 2f67 6974 6875   # https://githu
-0001ce00: 622e 636f 6d2f 6365 7274 626f 742f 6365  b.com/certbot/ce
-0001ce10: 7274 626f 742f 626c 6f62 2f37 6136 3735  rtbot/blob/7a675
-0001ce20: 3261 3638 6564 3737 6537 3363 3262 3239  2a68ed77e73c2b29
-0001ce30: 6162 3230 6433 6361 3839 3237 6634 6661  ab20d3ca8927f4fa
-0001ce40: 3762 302f 6365 7274 626f 742f 6365 7274  7b0/certbot/cert
-0001ce50: 626f 742f 5f69 6e74 6572 6e61 6c2f 706c  bot/_internal/pl
-0001ce60: 7567 696e 732f 7365 6c65 6374 696f 6e2e  ugins/selection.
-0001ce70: 7079 234c 3234 362d 4c32 3439 0a20 2020  py#L246-L249.   
-0001ce80: 2020 2020 2020 2020 2069 6620 7375 6263           if subc
-0001ce90: 6f6d 6d61 6e64 203d 3d20 2769 6e73 7461  ommand == 'insta
-0001cea0: 6c6c 273a 0a20 2020 2020 2020 2020 2020  ll':.           
-0001ceb0: 2020 2020 2072 6169 7365 2073 656c 662e       raise self.
-0001cec0: 4558 5045 4354 4544 5f45 5252 4f52 5f54  EXPECTED_ERROR_T
-0001ced0: 5950 4528 7365 6c66 2e45 5850 4543 5445  YPE(self.EXPECTE
-0001cee0: 445f 4552 524f 525f 5354 5229 0a0a 2020  D_ERROR_STR)..  
-0001cef0: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
-0001cf00: 7061 7463 682e 6f62 6a65 6374 2873 7461  patch.object(sta
-0001cf10: 6e64 616c 6f6e 652e 4175 7468 656e 7469  ndalone.Authenti
-0001cf20: 6361 746f 722c 2027 7072 6570 6172 6527  cator, 'prepare'
-0001cf30: 2c20 6175 7468 656e 7469 6361 746f 725f  , authenticator_
-0001cf40: 6c6f 636b 293a 0a20 2020 2020 2020 2020  lock):.         
-0001cf50: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
-0001cf60: 6368 2e6f 626a 6563 7428 6e75 6c6c 2e49  ch.object(null.I
-0001cf70: 6e73 7461 6c6c 6572 2c20 2770 7265 7061  nstaller, 'prepa
-0001cf80: 7265 272c 2069 6e73 7461 6c6c 6572 5f6c  re', installer_l
-0001cf90: 6f63 6b29 3a0a 2020 2020 2020 2020 2020  ock):.          
-0001cfa0: 2020 2020 2020 7969 656c 640a 0a20 2020        yield..   
-0001cfb0: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
-0001cfc0: 2870 6172 616d 733d 2763 6572 746f 6e6c  (params='certonl
-0001cfd0: 7920 696e 7374 616c 6c20 7265 6e65 7720  y install renew 
-0001cfe0: 7275 6e27 2e73 706c 6974 2829 290a 2020  run'.split()).  
-0001cff0: 2020 6465 6620 6172 6773 5f61 6e64 5f6c    def args_and_l
-0001d000: 6f63 6b5f 6f72 6465 7228 7365 6c66 2c20  ock_order(self, 
-0001d010: 6d6f 636b 5f6c 6f63 6b5f 6469 722c 2072  mock_lock_dir, r
-0001d020: 6571 7565 7374 2c20 746d 705f 7061 7468  equest, tmp_path
-0001d030: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-0001d040: 7473 2075 7020 4365 7274 626f 7420 7769  ts up Certbot wi
-0001d050: 7468 2061 7267 7320 616e 6420 6d6f 636b  th args and mock
-0001d060: 7320 746f 2065 7272 6f72 2061 6674 6572  s to error after
-0001d070: 2061 6371 7569 7269 6e67 2074 6865 206c   acquiring the l
-0001d080: 6173 7420 6c6f 636b 2e0a 0a20 2020 2020  ast lock...     
-0001d090: 2020 2054 6869 7320 6669 7874 7572 6520     This fixture 
-0001d0a0: 7969 656c 6473 2074 6865 2043 4c49 2061  yields the CLI a
-0001d0b0: 7267 756d 656e 7473 2074 6861 7420 7368  rguments that sh
-0001d0c0: 6f75 6c64 2062 6520 6769 7665 6e20 746f  ould be given to
-0001d0d0: 2043 6572 7462 6f74 0a20 2020 2020 2020   Certbot.       
-0001d0e0: 2061 6e64 2074 6865 2065 7870 6563 7465   and the expecte
-0001d0f0: 6420 6f72 6465 7220 6f66 2064 6972 6563  d order of direc
-0001d100: 746f 7269 6573 2074 6f20 6265 206c 6f63  tories to be loc
-0001d110: 6b65 642e 2041 6e20 6572 726f 7220 6973  ked. An error is
-0001d120: 2072 6169 7365 640a 2020 2020 2020 2020   raised.        
-0001d130: 6166 7465 7220 6163 7175 6972 696e 6720  after acquiring 
-0001d140: 7468 6520 6c61 7374 206c 6f63 6b20 6a75  the last lock ju
-0001d150: 7374 2061 7320 6120 6d65 616e 7320 6f66  st as a means of
-0001d160: 2073 746f 7070 696e 6720 4365 7274 626f   stopping Certbo
-0001d170: 7427 730a 2020 2020 2020 2020 6578 6563  t's.        exec
-0001d180: 7574 696f 6e2e 0a0a 2020 2020 2020 2020  ution...        
-0001d190: 2222 220a 2020 2020 2020 2020 2320 7365  """.        # se
-0001d1a0: 6c65 6374 2064 6972 6563 746f 7269 6573  lect directories
-0001d1b0: 0a20 2020 2020 2020 2061 7574 6865 6e74  .        authent
-0001d1c0: 6963 6174 6f72 5f64 6972 203d 2073 7472  icator_dir = str
-0001d1d0: 2874 6d70 5f70 6174 6820 2f20 2761 7574  (tmp_path / 'aut
-0001d1e0: 6865 6e74 6963 6174 6f72 2729 0a20 2020  henticator').   
-0001d1f0: 2020 2020 2063 6f6e 6669 675f 6469 7220       config_dir 
-0001d200: 3d20 7374 7228 746d 705f 7061 7468 202f  = str(tmp_path /
-0001d210: 2027 636f 6e66 6967 2729 0a20 2020 2020   'config').     
-0001d220: 2020 2069 6e73 7461 6c6c 6572 5f64 6972     installer_dir
-0001d230: 203d 2073 7472 2874 6d70 5f70 6174 6820   = str(tmp_path 
-0001d240: 2f20 2769 6e73 7461 6c6c 6572 2729 0a20  / 'installer'). 
-0001d250: 2020 2020 2020 206c 6f67 735f 6469 7220         logs_dir 
-0001d260: 3d20 7374 7228 746d 705f 7061 7468 202f  = str(tmp_path /
-0001d270: 2027 6c6f 6773 2729 0a20 2020 2020 2020   'logs').       
-0001d280: 2077 6f72 6b5f 6469 7220 3d20 7374 7228   work_dir = str(
-0001d290: 746d 705f 7061 7468 202f 2027 776f 726b  tmp_path / 'work
-0001d2a0: 2729 0a0a 2020 2020 2020 2020 2320 7072  ')..        # pr
-0001d2b0: 6570 6172 6520 6172 6773 2061 6e64 206c  epare args and l
-0001d2c0: 696e 6561 6765 0a20 2020 2020 2020 2073  ineage.        s
-0001d2d0: 7562 636f 6d6d 616e 6420 3d20 7265 7175  ubcommand = requ
-0001d2e0: 6573 742e 7061 7261 6d0a 2020 2020 2020  est.param.      
-0001d2f0: 2020 6172 6773 203d 205b 7375 6263 6f6d    args = [subcom
-0001d300: 6d61 6e64 2c20 272d 6127 2c20 2773 7461  mand, '-a', 'sta
-0001d310: 6e64 616c 6f6e 6527 2c20 272d 6927 2c20  ndalone', '-i', 
-0001d320: 276e 756c 6c27 2c20 272d 2d6e 6f2d 7261  'null', '--no-ra
-0001d330: 6e64 6f6d 2d73 6c65 6570 2d6f 6e2d 7265  ndom-sleep-on-re
-0001d340: 6e65 7727 2c0a 2020 2020 2020 2020 2020  new',.          
-0001d350: 2020 2020 2020 272d 2d63 6f6e 6669 672d        '--config-
-0001d360: 6469 7227 2c20 636f 6e66 6967 5f64 6972  dir', config_dir
-0001d370: 2c20 272d 2d6c 6f67 732d 6469 7227 2c20  , '--logs-dir', 
-0001d380: 6c6f 6773 5f64 6972 2c20 272d 2d77 6f72  logs_dir, '--wor
-0001d390: 6b2d 6469 7227 2c0a 2020 2020 2020 2020  k-dir',.        
-0001d3a0: 2020 2020 2020 2020 776f 726b 5f64 6972          work_dir
-0001d3b0: 5d0a 2020 2020 2020 2020 7465 7374 5f75  ].        test_u
-0001d3c0: 7469 6c2e 6d61 6b65 5f6c 696e 6561 6765  til.make_lineage
-0001d3d0: 2863 6f6e 6669 675f 6469 722c 2027 7361  (config_dir, 'sa
-0001d3e0: 6d70 6c65 2d72 656e 6577 616c 2e63 6f6e  mple-renewal.con
-0001d3f0: 6627 290a 0a20 2020 2020 2020 2077 6974  f')..        wit
-0001d400: 6820 7365 6c66 2e6d 6f63 6b5f 706c 7567  h self.mock_plug
-0001d410: 696e 5f70 7265 7061 7265 2861 7574 6865  in_prepare(authe
-0001d420: 6e74 6963 6174 6f72 5f64 6972 2c20 696e  nticator_dir, in
-0001d430: 7374 616c 6c65 725f 6469 722c 206d 6f63  staller_dir, moc
-0001d440: 6b5f 6c6f 636b 5f64 6972 2c20 7375 6263  k_lock_dir, subc
-0001d450: 6f6d 6d61 6e64 293a 0a20 2020 2020 2020  ommand):.       
-0001d460: 2020 2020 206c 6f63 6b5f 6f72 6465 7220       lock_order 
-0001d470: 3d20 5b6c 6f67 735f 6469 722c 2063 6f6e  = [logs_dir, con
-0001d480: 6669 675f 6469 722c 2077 6f72 6b5f 6469  fig_dir, work_di
-0001d490: 722c 2069 6e73 7461 6c6c 6572 5f64 6972  r, installer_dir
-0001d4a0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-0001d4b0: 2073 7562 636f 6d6d 616e 6420 3d3d 2027   subcommand == '
-0001d4c0: 696e 7374 616c 6c27 3a0a 2020 2020 2020  install':.      
-0001d4d0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-0001d4e0: 6172 6773 2c20 6c6f 636b 5f6f 7264 6572  args, lock_order
-0001d4f0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001d500: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001d510: 2020 2023 2057 6520 6578 7065 6374 2074     # We expect t
-0001d520: 6865 2069 6e73 7461 6c6c 6572 2074 6f20  he installer to 
-0001d530: 6265 2070 7265 7061 7265 6420 6576 656e  be prepared even
-0001d540: 2066 6f72 2063 6572 746f 6e6c 790a 2020   for certonly.  
-0001d550: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001d560: 6265 6361 7573 6520 616e 2069 6e73 7461  because an insta
-0001d570: 6c6c 6572 2077 6173 2072 6571 7565 7374  ller was request
-0001d580: 6564 206f 6e20 7468 6520 636f 6d6d 616e  ed on the comman
-0001d590: 6420 6c69 6e65 2e0a 2020 2020 2020 2020  d line..        
-0001d5a0: 2020 2020 2020 2020 7969 656c 6420 6172          yield ar
-0001d5b0: 6773 2c20 6c6f 636b 5f6f 7264 6572 202b  gs, lock_order +
-0001d5c0: 205b 6175 7468 656e 7469 6361 746f 725f   [authenticator_
-0001d5d0: 6469 725d 0a0a 2020 2020 6465 6620 7465  dir]..    def te
-0001d5e0: 7374 5f6c 6f63 6b5f 6f72 6465 7228 7365  st_lock_order(se
-0001d5f0: 6c66 2c20 6172 6773 5f61 6e64 5f6c 6f63  lf, args_and_loc
-0001d600: 6b5f 6f72 6465 722c 206d 6f63 6b5f 6c6f  k_order, mock_lo
-0001d610: 636b 5f64 6972 293a 0a20 2020 2020 2020  ck_dir):.       
-0001d620: 2061 7267 732c 206c 6f63 6b5f 6f72 6465   args, lock_orde
-0001d630: 7220 3d20 6172 6773 5f61 6e64 5f6c 6f63  r = args_and_loc
-0001d640: 6b5f 6f72 6465 720a 2020 2020 2020 2020  k_order.        
-0001d650: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
-0001d660: 6573 2873 656c 662e 4558 5045 4354 4544  es(self.EXPECTED
-0001d670: 5f45 5252 4f52 5f54 5950 452c 206d 6174  _ERROR_TYPE, mat
-0001d680: 6368 3d73 656c 662e 4558 5045 4354 4544  ch=self.EXPECTED
-0001d690: 5f45 5252 4f52 5f53 5452 5f52 4547 4558  _ERROR_STR_REGEX
-0001d6a0: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
-0001d6b0: 6169 6e2e 6d61 696e 2861 7267 7329 0a20  ain.main(args). 
-0001d6c0: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
-0001d6d0: 636b 5f6c 6f63 6b5f 6469 722e 6361 6c6c  ck_lock_dir.call
-0001d6e0: 5f63 6f75 6e74 203d 3d20 6c65 6e28 6c6f  _count == len(lo
-0001d6f0: 636b 5f6f 7264 6572 290a 2020 2020 2020  ck_order).      
-0001d700: 2020 666f 7220 6361 6c6c 2c20 6c6f 636b    for call, lock
-0001d710: 6564 5f64 6972 2069 6e20 7a69 7028 6d6f  ed_dir in zip(mo
-0001d720: 636b 5f6c 6f63 6b5f 6469 722e 6361 6c6c  ck_lock_dir.call
-0001d730: 5f61 7267 735f 6c69 7374 2c20 6c6f 636b  _args_list, lock
-0001d740: 5f6f 7264 6572 293a 0a20 2020 2020 2020  _order):.       
-0001d750: 2020 2020 2061 7373 6572 7420 6361 6c6c       assert call
-0001d760: 5b30 5d5b 305d 203d 3d20 6c6f 636b 6564  [0][0] == locked
-0001d770: 5f64 6972 0a0a 0a69 6620 5f5f 6e61 6d65  _dir...if __name
-0001d780: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
-0001d790: 3a0a 2020 2020 7379 732e 6578 6974 2870  :.    sys.exit(p
-0001d7a0: 7974 6573 742e 6d61 696e 2873 7973 2e61  ytest.main(sys.a
-0001d7b0: 7267 765b 313a 5d20 2b20 5b5f 5f66 696c  rgv[1:] + [__fil
-0001d7c0: 655f 5f5d 2929 2020 2320 7072 6167 6d61  e__]))  # pragma
-0001d7d0: 3a20 6e6f 2063 6f76 6572 0a              : no cover.
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2020 2020 6572 726f 725f 6578 7065 6374      error_expect
+00012ee0: 6564 3d46 616c 7365 290a 0a20 2020 2064  ed=False)..    d
+00012ef0: 6566 2074 6573 745f 7265 6e65 775f 7665  ef test_renew_ve
+00012f00: 7262 5f65 6d70 7479 5f63 6f6e 6669 6728  rb_empty_config(
+00012f10: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00012f20: 6420 3d20 6f73 2e70 6174 682e 6a6f 696e  d = os.path.join
+00012f30: 2873 656c 662e 636f 6e66 6967 2e63 6f6e  (self.config.con
+00012f40: 6669 675f 6469 722c 2027 7265 6e65 7761  fig_dir, 'renewa
+00012f50: 6c27 290a 2020 2020 2020 2020 6966 206e  l').        if n
+00012f60: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+00012f70: 7328 7264 293a 0a20 2020 2020 2020 2020  s(rd):.         
+00012f80: 2020 2066 696c 6573 7973 7465 6d2e 6d61     filesystem.ma
+00012f90: 6b65 6469 7273 2872 6429 0a20 2020 2020  kedirs(rd).     
+00012fa0: 2020 2077 6974 6820 6f70 656e 286f 732e     with open(os.
+00012fb0: 7061 7468 2e6a 6f69 6e28 7264 2c20 2765  path.join(rd, 'e
+00012fc0: 6d70 7479 2e63 6f6e 6627 292c 2027 7727  mpty.conf'), 'w'
+00012fd0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+00012fe0: 6173 7320 2023 206c 6561 7665 2074 6865  ass  # leave the
+00012ff0: 2066 696c 6520 656d 7074 790a 2020 2020   file empty.    
+00013000: 2020 2020 6172 6773 203d 205b 2272 656e      args = ["ren
+00013010: 6577 222c 2022 2d2d 6472 792d 7275 6e22  ew", "--dry-run"
+00013020: 2c20 222d 7476 7622 5d0a 2020 2020 2020  , "-tvv"].      
+00013030: 2020 7365 6c66 2e5f 7465 7374 5f72 656e    self._test_ren
+00013040: 6577 616c 5f63 6f6d 6d6f 6e28 4661 6c73  ewal_common(Fals
+00013050: 652c 205b 5d2c 2061 7267 733d 6172 6773  e, [], args=args
+00013060: 2c20 7368 6f75 6c64 5f72 656e 6577 3d46  , should_renew=F
+00013070: 616c 7365 2c20 6572 726f 725f 6578 7065  alse, error_expe
+00013080: 6374 6564 3d54 7275 6529 0a0a 2020 2020  cted=True)..    
+00013090: 6465 6620 7465 7374 5f72 656e 6577 5f77  def test_renew_w
+000130a0: 6974 685f 6365 7274 6e61 6d65 2873 656c  ith_certname(sel
+000130b0: 6629 3a0a 2020 2020 2020 2020 7465 7374  f):.        test
+000130c0: 5f75 7469 6c2e 6d61 6b65 5f6c 696e 6561  _util.make_linea
+000130d0: 6765 2873 656c 662e 636f 6e66 6967 2e63  ge(self.config.c
+000130e0: 6f6e 6669 675f 6469 722c 2027 7361 6d70  onfig_dir, 'samp
+000130f0: 6c65 2d72 656e 6577 616c 2e63 6f6e 6627  le-renewal.conf'
+00013100: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00013110: 7465 7374 5f72 656e 6577 616c 5f63 6f6d  test_renewal_com
+00013120: 6d6f 6e28 5472 7565 2c20 5b5d 2c20 7368  mon(True, [], sh
+00013130: 6f75 6c64 5f72 656e 6577 3d54 7275 652c  ould_renew=True,
+00013140: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00013150: 733d 5b27 7265 6e65 7727 2c20 272d 2d64  s=['renew', '--d
+00013160: 7279 2d72 756e 272c 2027 2d2d 6365 7274  ry-run', '--cert
+00013170: 2d6e 616d 6527 2c20 2773 616d 706c 652d  -name', 'sample-
+00013180: 7265 6e65 7761 6c27 5d29 0a0a 2020 2020  renewal'])..    
+00013190: 6465 6620 7465 7374 5f72 656e 6577 5f77  def test_renew_w
+000131a0: 6974 685f 6261 645f 6365 7274 6e61 6d65  ith_bad_certname
+000131b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000131c0: 7365 6c66 2e5f 7465 7374 5f72 656e 6577  self._test_renew
+000131d0: 616c 5f63 6f6d 6d6f 6e28 5472 7565 2c20  al_common(True, 
+000131e0: 5b5d 2c20 7368 6f75 6c64 5f72 656e 6577  [], should_renew
+000131f0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00013200: 2020 2020 6172 6773 3d5b 2772 656e 6577      args=['renew
+00013210: 272c 2027 2d2d 6472 792d 7275 6e27 2c20  ', '--dry-run', 
+00013220: 272d 2d63 6572 742d 6e61 6d65 272c 2027  '--cert-name', '
+00013230: 7361 6d70 6c65 2d72 656e 6577 616c 275d  sample-renewal']
+00013240: 2c0a 2020 2020 2020 2020 2020 2020 6572  ,.            er
+00013250: 726f 725f 6578 7065 6374 6564 3d54 7275  ror_expected=Tru
+00013260: 6529 0a0a 2020 2020 6465 6620 5f6d 616b  e)..    def _mak
+00013270: 655f 6475 6d6d 795f 7265 6e65 7761 6c5f  e_dummy_renewal_
+00013280: 636f 6e66 6967 2873 656c 6629 3a0a 2020  config(self):.  
+00013290: 2020 2020 2020 7265 6e65 7765 725f 636f        renewer_co
+000132a0: 6e66 6967 735f 6469 7220 3d20 6f73 2e70  nfigs_dir = os.p
+000132b0: 6174 682e 6a6f 696e 2873 656c 662e 636f  ath.join(self.co
+000132c0: 6e66 6967 2e63 6f6e 6669 675f 6469 722c  nfig.config_dir,
+000132d0: 2027 7265 6e65 7761 6c27 290a 2020 2020   'renewal').    
+000132e0: 2020 2020 6669 6c65 7379 7374 656d 2e6d      filesystem.m
+000132f0: 616b 6564 6972 7328 7265 6e65 7765 725f  akedirs(renewer_
+00013300: 636f 6e66 6967 735f 6469 7229 0a20 2020  configs_dir).   
+00013310: 2020 2020 2077 6974 6820 6f70 656e 286f       with open(o
+00013320: 732e 7061 7468 2e6a 6f69 6e28 7265 6e65  s.path.join(rene
+00013330: 7765 725f 636f 6e66 6967 735f 6469 722c  wer_configs_dir,
+00013340: 2027 7465 7374 2e63 6f6e 6627 292c 2027   'test.conf'), '
+00013350: 7727 2920 6173 2066 3a0a 2020 2020 2020  w') as f:.      
+00013360: 2020 2020 2020 662e 7772 6974 6528 224d        f.write("M
+00013370: 7920 636f 6e74 656e 7473 2064 6f6e 2774  y contents don't
+00013380: 206d 6174 7465 7222 290a 0a20 2020 2064   matter")..    d
+00013390: 6566 205f 7465 7374 5f72 656e 6577 5f63  ef _test_renew_c
+000133a0: 6f6d 6d6f 6e28 7365 6c66 2c20 7265 6e65  ommon(self, rene
+000133b0: 7761 6c70 6172 616d 733d 4e6f 6e65 2c20  walparams=None, 
+000133c0: 6e61 6d65 733d 4e6f 6e65 2c0a 2020 2020  names=None,.    
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133e0: 2020 2020 2020 2061 7373 6572 745f 6f63         assert_oc
+000133f0: 5f63 616c 6c65 643d 4e6f 6e65 2c20 2a2a  _called=None, **
+00013400: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00013410: 2073 656c 662e 5f6d 616b 655f 6475 6d6d   self._make_dumm
+00013420: 795f 7265 6e65 7761 6c5f 636f 6e66 6967  y_renewal_config
+00013430: 2829 0a20 2020 2020 2020 2077 6974 6820  ().        with 
+00013440: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+00013450: 626f 742e 5f69 6e74 6572 6e61 6c2e 7374  bot._internal.st
+00013460: 6f72 6167 652e 5265 6e65 7761 626c 6543  orage.RenewableC
+00013470: 6572 7427 2920 6173 206d 6f63 6b5f 7263  ert') as mock_rc
+00013480: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00013490: 636b 5f6c 696e 6561 6765 203d 206d 6f63  ck_lineage = moc
+000134a0: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
+000134b0: 2020 2020 2020 2020 2020 6d6f 636b 5f6c            mock_l
+000134c0: 696e 6561 6765 2e66 756c 6c63 6861 696e  ineage.fullchain
+000134d0: 203d 2022 736f 6d65 7061 7468 2f66 756c   = "somepath/ful
+000134e0: 6c63 6861 696e 2e70 656d 220a 2020 2020  lchain.pem".    
+000134f0: 2020 2020 2020 2020 6966 2072 656e 6577          if renew
+00013500: 616c 7061 7261 6d73 2069 7320 6e6f 7420  alparams is not 
+00013510: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00013520: 2020 2020 2020 6d6f 636b 5f6c 696e 6561        mock_linea
+00013530: 6765 2e63 6f6e 6669 6775 7261 7469 6f6e  ge.configuration
+00013540: 203d 207b 2772 656e 6577 616c 7061 7261   = {'renewalpara
+00013550: 6d73 273a 2072 656e 6577 616c 7061 7261  ms': renewalpara
+00013560: 6d73 7d0a 2020 2020 2020 2020 2020 2020  ms}.            
+00013570: 6966 206e 616d 6573 2069 7320 6e6f 7420  if names is not 
+00013580: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00013590: 2020 2020 2020 6d6f 636b 5f6c 696e 6561        mock_linea
+000135a0: 6765 2e6e 616d 6573 2e72 6574 7572 6e5f  ge.names.return_
+000135b0: 7661 6c75 6520 3d20 6e61 6d65 730a 2020  value = names.  
+000135c0: 2020 2020 2020 2020 2020 6d6f 636b 5f72            mock_r
+000135d0: 632e 7265 7475 726e 5f76 616c 7565 203d  c.return_value =
+000135e0: 206d 6f63 6b5f 6c69 6e65 6167 650a 2020   mock_lineage.  
+000135f0: 2020 2020 2020 2020 2020 7769 7468 206d            with m
+00013600: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00013610: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+00013620: 6e2e 7265 6e65 775f 6365 7274 2729 2061  n.renew_cert') a
+00013630: 7320 6d6f 636b 5f72 656e 6577 5f63 6572  s mock_renew_cer
+00013640: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00013650: 2020 206b 7761 7267 732e 7365 7464 6566     kwargs.setdef
+00013660: 6175 6c74 2827 6172 6773 272c 205b 2772  ault('args', ['r
+00013670: 656e 6577 275d 290a 2020 2020 2020 2020  enew']).        
+00013680: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00013690: 7374 5f72 656e 6577 616c 5f63 6f6d 6d6f  st_renewal_commo
+000136a0: 6e28 5472 7565 2c20 4e6f 6e65 2c20 7368  n(True, None, sh
+000136b0: 6f75 6c64 5f72 656e 6577 3d46 616c 7365  ould_renew=False
+000136c0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+000136d0: 2020 2020 2020 2020 2069 6620 6173 7365           if asse
+000136e0: 7274 5f6f 635f 6361 6c6c 6564 2069 7320  rt_oc_called is 
+000136f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00013700: 2020 2020 2020 2020 2020 6966 2061 7373            if ass
+00013710: 6572 745f 6f63 5f63 616c 6c65 643a 0a20  ert_oc_called:. 
+00013720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013730: 2020 2061 7373 6572 7420 6d6f 636b 5f72     assert mock_r
+00013740: 656e 6577 5f63 6572 742e 6361 6c6c 6564  enew_cert.called
+00013750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013760: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013770: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00013780: 7420 6d6f 636b 5f72 656e 6577 5f63 6572  t mock_renew_cer
+00013790: 742e 6361 6c6c 6564 2069 7320 4661 6c73  t.called is Fals
+000137a0: 650a 0a20 2020 2064 6566 2074 6573 745f  e..    def test_
+000137b0: 7265 6e65 775f 6e6f 5f72 656e 6577 616c  renew_no_renewal
+000137c0: 7061 7261 6d73 2873 656c 6629 3a0a 2020  params(self):.  
+000137d0: 2020 2020 2020 7365 6c66 2e5f 7465 7374        self._test
+000137e0: 5f72 656e 6577 5f63 6f6d 6d6f 6e28 6173  _renew_common(as
+000137f0: 7365 7274 5f6f 635f 6361 6c6c 6564 3d46  sert_oc_called=F
+00013800: 616c 7365 2c20 6572 726f 725f 6578 7065  alse, error_expe
+00013810: 6374 6564 3d54 7275 6529 0a0a 2020 2020  cted=True)..    
+00013820: 6465 6620 7465 7374 5f72 656e 6577 5f6e  def test_renew_n
+00013830: 6f5f 6175 7468 656e 7469 6361 746f 7228  o_authenticator(
+00013840: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00013850: 656c 662e 5f74 6573 745f 7265 6e65 775f  elf._test_renew_
+00013860: 636f 6d6d 6f6e 2872 656e 6577 616c 7061  common(renewalpa
+00013870: 7261 6d73 3d7b 7d2c 2061 7373 6572 745f  rams={}, assert_
+00013880: 6f63 5f63 616c 6c65 643d 4661 6c73 652c  oc_called=False,
+00013890: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+000138a0: 6f72 5f65 7870 6563 7465 643d 5472 7565  or_expected=True
+000138b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+000138c0: 7265 6e65 775f 7769 7468 5f62 6164 5f69  renew_with_bad_i
+000138d0: 6e74 2873 656c 6629 3a0a 2020 2020 2020  nt(self):.      
+000138e0: 2020 7265 6e65 7761 6c70 6172 616d 7320    renewalparams 
+000138f0: 3d20 7b27 6175 7468 656e 7469 6361 746f  = {'authenticato
+00013900: 7227 3a20 2777 6562 726f 6f74 272c 0a20  r': 'webroot',. 
+00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013920: 2020 2020 2020 2020 2772 7361 5f6b 6579          'rsa_key
+00013930: 5f73 697a 6527 3a20 276f 7665 7220 3930  _size': 'over 90
+00013940: 3030 277d 0a20 2020 2020 2020 2073 656c  00'}.        sel
+00013950: 662e 5f74 6573 745f 7265 6e65 775f 636f  f._test_renew_co
+00013960: 6d6d 6f6e 2872 656e 6577 616c 7061 7261  mmon(renewalpara
+00013970: 6d73 3d72 656e 6577 616c 7061 7261 6d73  ms=renewalparams
+00013980: 2c20 6572 726f 725f 6578 7065 6374 6564  , error_expected
+00013990: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+000139a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139b0: 2020 2020 2020 2061 7373 6572 745f 6f63         assert_oc
+000139c0: 5f63 616c 6c65 643d 4661 6c73 6529 0a0a  _called=False)..
+000139d0: 2020 2020 6465 6620 7465 7374 5f72 656e      def test_ren
+000139e0: 6577 5f77 6974 685f 6e6f 6e65 7479 7065  ew_with_nonetype
+000139f0: 5f68 7474 7030 3128 7365 6c66 293a 0a20  _http01(self):. 
+00013a00: 2020 2020 2020 2072 656e 6577 616c 7061         renewalpa
+00013a10: 7261 6d73 203d 207b 2761 7574 6865 6e74  rams = {'authent
+00013a20: 6963 6174 6f72 273a 2027 7765 6272 6f6f  icator': 'webroo
+00013a30: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00013a40: 2020 2020 2020 2020 2020 2020 2027 6874               'ht
+00013a50: 7470 3031 5f70 6f72 7427 3a20 274e 6f6e  tp01_port': 'Non
+00013a60: 6527 7d0a 2020 2020 2020 2020 7365 6c66  e'}.        self
+00013a70: 2e5f 7465 7374 5f72 656e 6577 5f63 6f6d  ._test_renew_com
+00013a80: 6d6f 6e28 7265 6e65 7761 6c70 6172 616d  mon(renewalparam
+00013a90: 733d 7265 6e65 7761 6c70 6172 616d 732c  s=renewalparams,
+00013aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ac0: 2061 7373 6572 745f 6f63 5f63 616c 6c65   assert_oc_calle
+00013ad0: 643d 5472 7565 290a 0a20 2020 2064 6566  d=True)..    def
+00013ae0: 2074 6573 745f 7265 6e65 775f 7769 7468   test_renew_with
+00013af0: 5f62 6164 5f64 6f6d 6169 6e28 7365 6c66  _bad_domain(self
+00013b00: 293a 0a20 2020 2020 2020 2072 656e 6577  ):.        renew
+00013b10: 616c 7061 7261 6d73 203d 207b 2761 7574  alparams = {'aut
+00013b20: 6865 6e74 6963 6174 6f72 273a 2027 7765  henticator': 'we
+00013b30: 6272 6f6f 7427 7d0a 2020 2020 2020 2020  broot'}.        
+00013b40: 6e61 6d65 7320 3d20 5b27 756e 69c3 a76f  names = ['uni..o
+00013b50: 64c3 a92e 636f 6d27 5d0a 2020 2020 2020  d...com'].      
+00013b60: 2020 7365 6c66 2e5f 7465 7374 5f72 656e    self._test_ren
+00013b70: 6577 5f63 6f6d 6d6f 6e28 7265 6e65 7761  ew_common(renewa
+00013b80: 6c70 6172 616d 733d 7265 6e65 7761 6c70  lparams=renewalp
+00013b90: 6172 616d 732c 2065 7272 6f72 5f65 7870  arams, error_exp
+00013ba0: 6563 7465 643d 5472 7565 2c0a 2020 2020  ected=True,.    
+00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bc0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00013bd0: 733d 6e61 6d65 732c 2061 7373 6572 745f  s=names, assert_
+00013be0: 6f63 5f63 616c 6c65 643d 4661 6c73 6529  oc_called=False)
+00013bf0: 0a0a 2020 2020 406d 6f63 6b2e 7061 7463  ..    @mock.patc
+00013c00: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00013c10: 726e 616c 2e70 6c75 6769 6e73 2e73 656c  rnal.plugins.sel
+00013c20: 6563 7469 6f6e 2e63 686f 6f73 655f 636f  ection.choose_co
+00013c30: 6e66 6967 7572 6174 6f72 5f70 6c75 6769  nfigurator_plugi
+00013c40: 6e73 2729 0a20 2020 2064 6566 2074 6573  ns').    def tes
+00013c50: 745f 7265 6e65 775f 7769 7468 5f63 6f6e  t_renew_with_con
+00013c60: 6669 6775 7261 746f 7228 7365 6c66 2c20  figurator(self, 
+00013c70: 6d6f 636b 5f73 656c 293a 0a20 2020 2020  mock_sel):.     
+00013c80: 2020 206d 6f63 6b5f 7365 6c2e 7265 7475     mock_sel.retu
+00013c90: 726e 5f76 616c 7565 203d 2028 6d6f 636b  rn_value = (mock
+00013ca0: 2e4d 6167 6963 4d6f 636b 2829 2c20 6d6f  .MagicMock(), mo
+00013cb0: 636b 2e4d 6167 6963 4d6f 636b 2829 290a  ck.MagicMock()).
+00013cc0: 2020 2020 2020 2020 7265 6e65 7761 6c70          renewalp
+00013cd0: 6172 616d 7320 3d20 7b27 6175 7468 656e  arams = {'authen
+00013ce0: 7469 6361 746f 7227 3a20 2777 6562 726f  ticator': 'webro
+00013cf0: 6f74 277d 0a20 2020 2020 2020 2073 656c  ot'}.        sel
+00013d00: 662e 5f74 6573 745f 7265 6e65 775f 636f  f._test_renew_co
+00013d10: 6d6d 6f6e 280a 2020 2020 2020 2020 2020  mmon(.          
+00013d20: 2020 7265 6e65 7761 6c70 6172 616d 733d    renewalparams=
+00013d30: 7265 6e65 7761 6c70 6172 616d 732c 2061  renewalparams, a
+00013d40: 7373 6572 745f 6f63 5f63 616c 6c65 643d  ssert_oc_called=
+00013d50: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00013d60: 2020 6172 6773 3d27 7265 6e65 7720 2d2d    args='renew --
+00013d70: 636f 6e66 6967 7572 6174 6f72 2061 7061  configurator apa
+00013d80: 6368 6527 2e73 706c 6974 2829 290a 0a20  che'.split()).. 
+00013d90: 2020 2064 6566 2074 6573 745f 7265 6e65     def test_rene
+00013da0: 775f 706c 7567 696e 5f63 6f6e 6669 675f  w_plugin_config_
+00013db0: 7265 7374 6f72 6174 696f 6e28 7365 6c66  restoration(self
+00013dc0: 293a 0a20 2020 2020 2020 2072 656e 6577  ):.        renew
+00013dd0: 616c 7061 7261 6d73 203d 207b 2761 7574  alparams = {'aut
+00013de0: 6865 6e74 6963 6174 6f72 273a 2027 7765  henticator': 'we
+00013df0: 6272 6f6f 7427 2c0a 2020 2020 2020 2020  broot',.        
+00013e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e10: 2027 7765 6272 6f6f 745f 7061 7468 273a   'webroot_path':
+00013e20: 2027 4e6f 6e65 272c 0a20 2020 2020 2020   'None',.       
+00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e40: 2020 2777 6562 726f 6f74 5f69 6d61 6769    'webroot_imagi
+00013e50: 6e61 7279 5f66 6c61 6727 3a20 2734 3227  nary_flag': '42'
+00013e60: 7d0a 2020 2020 2020 2020 7365 6c66 2e5f  }.        self._
+00013e70: 7465 7374 5f72 656e 6577 5f63 6f6d 6d6f  test_renew_commo
+00013e80: 6e28 7265 6e65 7761 6c70 6172 616d 733d  n(renewalparams=
+00013e90: 7265 6e65 7761 6c70 6172 616d 732c 0a20  renewalparams,. 
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013ec0: 7373 6572 745f 6f63 5f63 616c 6c65 643d  ssert_oc_called=
+00013ed0: 5472 7565 290a 0a20 2020 2064 6566 2074  True)..    def t
+00013ee0: 6573 745f 7265 6e65 775f 7769 7468 5f77  est_renew_with_w
+00013ef0: 6562 726f 6f74 5f6d 6170 2873 656c 6629  ebroot_map(self)
+00013f00: 3a0a 2020 2020 2020 2020 7265 6e65 7761  :.        renewa
+00013f10: 6c70 6172 616d 7320 3d20 7b27 6175 7468  lparams = {'auth
+00013f20: 656e 7469 6361 746f 7227 3a20 2777 6562  enticator': 'web
+00013f30: 726f 6f74 277d 0a20 2020 2020 2020 2073  root'}.        s
+00013f40: 656c 662e 5f74 6573 745f 7265 6e65 775f  elf._test_renew_
+00013f50: 636f 6d6d 6f6e 280a 2020 2020 2020 2020  common(.        
+00013f60: 2020 2020 7265 6e65 7761 6c70 6172 616d      renewalparam
+00013f70: 733d 7265 6e65 7761 6c70 6172 616d 732c  s=renewalparams,
+00013f80: 2061 7373 6572 745f 6f63 5f63 616c 6c65   assert_oc_calle
+00013f90: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
+00013fa0: 2020 2020 6172 6773 3d5b 2772 656e 6577      args=['renew
+00013fb0: 272c 2027 2d2d 7765 6272 6f6f 742d 6d61  ', '--webroot-ma
+00013fc0: 7027 2c20 6a73 6f6e 2e64 756d 7073 287b  p', json.dumps({
+00013fd0: 2765 7861 6d70 6c65 2e63 6f6d 273a 2074  'example.com': t
+00013fe0: 656d 7066 696c 652e 6765 7474 656d 7064  empfile.gettempd
+00013ff0: 6972 2829 7d29 5d29 0a0a 2020 2020 6465  ir()})])..    de
+00014000: 6620 7465 7374 5f72 656e 6577 5f72 6563  f test_renew_rec
+00014010: 6f6e 7374 6974 7574 655f 6572 726f 7228  onstitute_error(
+00014020: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
+00014030: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+00014040: 3d70 726f 7465 6374 6564 2d61 6363 6573  =protected-acces
+00014050: 730a 2020 2020 2020 2020 7769 7468 206d  s.        with m
+00014060: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+00014070: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+00014080: 6e2e 7265 6e65 7761 6c2e 7265 636f 6e73  n.renewal.recons
+00014090: 7469 7475 7465 2729 2061 7320 6d6f 636b  titute') as mock
+000140a0: 5f72 6563 6f6e 7374 6974 7574 653a 0a20  _reconstitute:. 
+000140b0: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
+000140c0: 7265 636f 6e73 7469 7475 7465 2e73 6964  reconstitute.sid
+000140d0: 655f 6566 6665 6374 203d 2045 7863 6570  e_effect = Excep
+000140e0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+000140f0: 2073 656c 662e 5f74 6573 745f 7265 6e65   self._test_rene
+00014100: 775f 636f 6d6d 6f6e 2861 7373 6572 745f  w_common(assert_
+00014110: 6f63 5f63 616c 6c65 643d 4661 6c73 652c  oc_called=False,
+00014120: 2065 7272 6f72 5f65 7870 6563 7465 643d   error_expected=
+00014130: 5472 7565 290a 0a20 2020 2064 6566 2074  True)..    def t
+00014140: 6573 745f 7265 6e65 775f 6f62 7461 696e  est_renew_obtain
+00014150: 5f63 6572 745f 6572 726f 7228 7365 6c66  _cert_error(self
+00014160: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00014170: 5f6d 616b 655f 6475 6d6d 795f 7265 6e65  _make_dummy_rene
+00014180: 7761 6c5f 636f 6e66 6967 2829 0a20 2020  wal_config().   
+00014190: 2020 2020 2077 6974 6820 6d6f 636b 2e70       with mock.p
+000141a0: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+000141b0: 6e74 6572 6e61 6c2e 7374 6f72 6167 652e  nternal.storage.
+000141c0: 5265 6e65 7761 626c 6543 6572 7427 2920  RenewableCert') 
+000141d0: 6173 206d 6f63 6b5f 7263 3a0a 2020 2020  as mock_rc:.    
+000141e0: 2020 2020 2020 2020 6d6f 636b 5f6c 696e          mock_lin
+000141f0: 6561 6765 203d 206d 6f63 6b2e 4d61 6769  eage = mock.Magi
+00014200: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
+00014210: 2020 2020 6d6f 636b 5f6c 696e 6561 6765      mock_lineage
+00014220: 2e66 756c 6c63 6861 696e 203d 2022 736f  .fullchain = "so
+00014230: 6d65 7768 6572 652f 6675 6c6c 6368 6169  mewhere/fullchai
+00014240: 6e2e 7065 6d22 0a20 2020 2020 2020 2020  n.pem".         
+00014250: 2020 206d 6f63 6b5f 7263 2e72 6574 7572     mock_rc.retur
+00014260: 6e5f 7661 6c75 6520 3d20 6d6f 636b 5f6c  n_value = mock_l
+00014270: 696e 6561 6765 0a20 2020 2020 2020 2020  ineage.         
+00014280: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
+00014290: 636f 6e66 6967 7572 6174 696f 6e20 3d20  configuration = 
+000142a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000142b0: 2020 2772 656e 6577 616c 7061 7261 6d73    'renewalparams
+000142c0: 273a 207b 2761 7574 6865 6e74 6963 6174  ': {'authenticat
+000142d0: 6f72 273a 2027 7765 6272 6f6f 7427 7d7d  or': 'webroot'}}
+000142e0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+000142f0: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
+00014300: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00014310: 6d61 696e 2e72 656e 6577 5f63 6572 7427  main.renew_cert'
+00014320: 2920 6173 206d 6f63 6b5f 7265 6e65 775f  ) as mock_renew_
+00014330: 6365 7274 3a0a 2020 2020 2020 2020 2020  cert:.          
+00014340: 2020 2020 2020 6d6f 636b 5f72 656e 6577        mock_renew
+00014350: 5f63 6572 742e 7369 6465 5f65 6666 6563  _cert.side_effec
+00014360: 7420 3d20 4578 6365 7074 696f 6e0a 2020  t = Exception.  
+00014370: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014380: 6c66 2e5f 7465 7374 5f72 656e 6577 616c  lf._test_renewal
+00014390: 5f63 6f6d 6d6f 6e28 5472 7565 2c20 4e6f  _common(True, No
+000143a0: 6e65 2c20 6572 726f 725f 6578 7065 6374  ne, error_expect
+000143b0: 6564 3d54 7275 652c 0a20 2020 2020 2020  ed=True,.       
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143e0: 2020 2061 7267 733d 5b27 7265 6e65 7727     args=['renew'
+000143f0: 5d2c 2073 686f 756c 645f 7265 6e65 773d  ], should_renew=
+00014400: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+00014410: 7465 7374 5f72 656e 6577 5f77 6974 685f  test_renew_with_
+00014420: 6261 645f 636c 695f 6172 6773 2873 656c  bad_cli_args(sel
+00014430: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00014440: 2e5f 7465 7374 5f72 656e 6577 616c 5f63  ._test_renewal_c
+00014450: 6f6d 6d6f 6e28 5472 7565 2c20 4e6f 6e65  ommon(True, None
+00014460: 2c20 6172 6773 3d27 7265 6e65 7720 2d64  , args='renew -d
+00014470: 2065 7861 6d70 6c65 2e63 6f6d 272e 7370   example.com'.sp
+00014480: 6c69 7428 292c 0a20 2020 2020 2020 2020  lit(),.         
+00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144a0: 2020 2020 2020 2020 2073 686f 756c 645f           should_
+000144b0: 7265 6e65 773d 4661 6c73 652c 2065 7272  renew=False, err
+000144c0: 6f72 5f65 7870 6563 7465 643d 5472 7565  or_expected=True
+000144d0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+000144e0: 7465 7374 5f72 656e 6577 616c 5f63 6f6d  test_renewal_com
+000144f0: 6d6f 6e28 5472 7565 2c20 4e6f 6e65 2c20  mon(True, None, 
+00014500: 6172 6773 3d27 7265 6e65 7720 2d2d 6373  args='renew --cs
+00014510: 7220 7b30 7d27 2e66 6f72 6d61 7428 4353  r {0}'.format(CS
+00014520: 5229 2e73 706c 6974 2829 2c0a 2020 2020  R).split(),.    
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00014550: 6f75 6c64 5f72 656e 6577 3d46 616c 7365  ould_renew=False
+00014560: 2c20 6572 726f 725f 6578 7065 6374 6564  , error_expected
+00014570: 3d54 7275 6529 0a0a 2020 2020 6465 6620  =True)..    def 
+00014580: 7465 7374 5f6e 6f5f 7265 6e65 7761 6c5f  test_no_renewal_
+00014590: 7769 7468 5f68 6f6f 6b73 2873 656c 6629  with_hooks(self)
+000145a0: 3a0a 2020 2020 2020 2020 5f2c 205f 2c20  :.        _, _, 
+000145b0: 7374 646f 7574 203d 2073 656c 662e 5f74  stdout = self._t
+000145c0: 6573 745f 7265 6e65 7761 6c5f 636f 6d6d  est_renewal_comm
+000145d0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000145e0: 6475 655f 666f 725f 7265 6e65 7761 6c3d  due_for_renewal=
+000145f0: 4661 6c73 652c 2065 7874 7261 5f61 7267  False, extra_arg
+00014600: 733d 4e6f 6e65 2c20 7368 6f75 6c64 5f72  s=None, should_r
+00014610: 656e 6577 3d46 616c 7365 2c0a 2020 2020  enew=False,.    
+00014620: 2020 2020 2020 2020 6172 6773 3d5b 2772          args=['r
+00014630: 656e 6577 272c 2027 2d2d 706f 7374 2d68  enew', '--post-h
+00014640: 6f6f 6b27 2c0a 2020 2020 2020 2020 2020  ook',.          
+00014650: 2020 2020 2020 2020 277b 307d 202d 6320          '{0} -c 
+00014660: 2270 7269 6e74 285c 2768 656c 6c6f 2077  "print(\'hello w
+00014670: 6f72 6c64 5c27 293b 2227 0a20 2020 2020  orld\');"'.     
+00014680: 2020 2020 2020 2020 2020 2020 202e 666f               .fo
+00014690: 726d 6174 2873 7973 2e65 7865 6375 7461  rmat(sys.executa
+000146a0: 626c 6529 5d29 0a20 2020 2020 2020 2061  ble)]).        a
+000146b0: 7373 6572 7420 274e 6f20 686f 6f6b 7320  ssert 'No hooks 
+000146c0: 7765 7265 2072 756e 2e27 2069 6e20 7374  were run.' in st
+000146d0: 646f 7574 2e67 6574 7661 6c75 6528 290a  dout.getvalue().
+000146e0: 0a20 2020 2040 7465 7374 5f75 7469 6c2e  .    @test_util.
+000146f0: 7061 7463 685f 6469 7370 6c61 795f 7574  patch_display_ut
+00014700: 696c 2829 0a20 2020 2040 6d6f 636b 2e70  il().    @mock.p
+00014710: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+00014720: 6e74 6572 6e61 6c2e 6d61 696e 2e5f 6669  nternal.main._fi
+00014730: 6e64 5f6c 696e 6561 6765 5f66 6f72 5f64  nd_lineage_for_d
+00014740: 6f6d 6169 6e73 5f61 6e64 5f63 6572 746e  omains_and_certn
+00014750: 616d 6527 290a 2020 2020 406d 6f63 6b2e  ame').    @mock.
+00014760: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+00014770: 696e 7465 726e 616c 2e6d 6169 6e2e 5f69  internal.main._i
+00014780: 6e69 745f 6c65 5f63 6c69 656e 7427 290a  nit_le_client').
+00014790: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+000147a0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+000147b0: 616c 2e6d 6169 6e2e 5f72 6570 6f72 745f  al.main._report_
+000147c0: 6e65 775f 6365 7274 2729 0a20 2020 2064  new_cert').    d
+000147d0: 6566 2074 6573 745f 6365 7274 6f6e 6c79  ef test_certonly
+000147e0: 5f72 6569 6e73 7461 6c6c 2873 656c 662c  _reinstall(self,
+000147f0: 206d 6f63 6b5f 7265 706f 7274 5f6e 6577   mock_report_new
+00014800: 5f63 6572 742c 206d 6f63 6b5f 696e 6974  _cert, mock_init
+00014810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014830: 2020 6d6f 636b 5f72 656e 6577 616c 2c20    mock_renewal, 
+00014840: 6d6f 636b 5f67 6574 5f75 7469 6c69 7479  mock_get_utility
+00014850: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
+00014860: 7265 6e65 7761 6c2e 7265 7475 726e 5f76  renewal.return_v
+00014870: 616c 7565 203d 2028 2772 6569 6e73 7461  alue = ('reinsta
+00014880: 6c6c 272c 206d 6f63 6b2e 4d61 6769 634d  ll', mock.MagicM
+00014890: 6f63 6b28 2929 0a20 2020 2020 2020 206d  ock()).        m
+000148a0: 6f63 6b5f 696e 6974 2e72 6574 7572 6e5f  ock_init.return_
+000148b0: 7661 6c75 6520 3d20 6d6f 636b 5f63 6c69  value = mock_cli
+000148c0: 656e 7420 3d20 6d6f 636b 2e4d 6167 6963  ent = mock.Magic
+000148d0: 4d6f 636b 2829 0a20 2020 2020 2020 2073  Mock().        s
+000148e0: 656c 662e 5f63 616c 6c28 5b27 2d64 272c  elf._call(['-d',
+000148f0: 2027 666f 6f2e 6261 7227 2c20 272d 6127   'foo.bar', '-a'
+00014900: 2c20 2773 7461 6e64 616c 6f6e 6527 2c20  , 'standalone', 
+00014910: 2763 6572 746f 6e6c 7927 5d29 0a20 2020  'certonly']).   
+00014920: 2020 2020 2061 7373 6572 7420 6d6f 636b       assert mock
+00014930: 5f63 6c69 656e 742e 6f62 7461 696e 5f63  _client.obtain_c
+00014940: 6572 7469 6669 6361 7465 2e63 616c 6c65  ertificate.calle
+00014950: 6420 6973 2046 616c 7365 0a20 2020 2020  d is False.     
+00014960: 2020 2061 7373 6572 7420 6d6f 636b 5f63     assert mock_c
+00014970: 6c69 656e 742e 6f62 7461 696e 5f61 6e64  lient.obtain_and
+00014980: 5f65 6e72 6f6c 6c5f 6365 7274 6966 6963  _enroll_certific
+00014990: 6174 652e 6361 6c6c 6564 2069 7320 4661  ate.called is Fa
+000149a0: 6c73 650a 2020 2020 2020 2020 6173 7365  lse.        asse
+000149b0: 7274 206d 6f63 6b5f 6765 745f 7574 696c  rt mock_get_util
+000149c0: 6974 7928 292e 6164 645f 6d65 7373 6167  ity().add_messag
+000149d0: 652e 6361 6c6c 5f63 6f75 6e74 203d 3d20  e.call_count == 
+000149e0: 300a 2020 2020 2020 2020 6d6f 636b 5f72  0.        mock_r
+000149f0: 6570 6f72 745f 6e65 775f 6365 7274 2e61  eport_new_cert.a
+00014a00: 7373 6572 745f 6e6f 745f 6361 6c6c 6564  ssert_not_called
+00014a10: 2829 0a20 2020 2020 2020 2023 7365 6c66  ().        #self
+00014a20: 2e61 7373 6572 7454 7275 6528 2764 6f6e  .assertTrue('don
+00014a30: 6174 6527 206e 6f74 2069 6e20 6d6f 636b  ate' not in mock
+00014a40: 5f67 6574 5f75 7469 6c69 7479 2829 2e61  _get_utility().a
+00014a50: 6464 5f6d 6573 7361 6765 2e63 616c 6c5f  dd_message.call_
+00014a60: 6172 6773 5b30 5d5b 305d 290a 0a20 2020  args[0][0])..   
+00014a70: 2064 6566 205f 7465 7374 5f63 6572 746f   def _test_certo
+00014a80: 6e6c 795f 6373 725f 636f 6d6d 6f6e 2873  nly_csr_common(s
+00014a90: 656c 662c 2065 7874 7261 5f61 7267 733d  elf, extra_args=
+00014aa0: 4e6f 6e65 293a 0a20 2020 2020 2020 2063  None):.        c
+00014ab0: 6572 7472 203d 2027 6365 7274 7227 0a20  ertr = 'certr'. 
+00014ac0: 2020 2020 2020 2063 6861 696e 203d 2027         chain = '
+00014ad0: 6368 6169 6e27 0a20 2020 2020 2020 206d  chain'.        m
+00014ae0: 6f63 6b5f 636c 6965 6e74 203d 206d 6f63  ock_client = moc
+00014af0: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
+00014b00: 2020 2020 2020 6d6f 636b 5f63 6c69 656e        mock_clien
+00014b10: 742e 6f62 7461 696e 5f63 6572 7469 6669  t.obtain_certifi
+00014b20: 6361 7465 5f66 726f 6d5f 6373 722e 7265  cate_from_csr.re
+00014b30: 7475 726e 5f76 616c 7565 203d 2028 6365  turn_value = (ce
+00014b40: 7274 722c 2063 6861 696e 290a 2020 2020  rtr, chain).    
+00014b50: 2020 2020 6365 7274 5f70 6174 6820 3d20      cert_path = 
+00014b60: 6f73 2e70 6174 682e 6e6f 726d 7061 7468  os.path.normpath
+00014b70: 286f 732e 7061 7468 2e6a 6f69 6e28 0a20  (os.path.join(. 
+00014b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014b90: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
+00014ba0: 722c 0a20 2020 2020 2020 2020 2020 2027  r,.            '
+00014bb0: 6c69 7665 2f65 7861 6d70 6c65 2e63 6f6d  live/example.com
+00014bc0: 2f63 6572 745f 3531 322e 7065 6d27 2929  /cert_512.pem'))
+00014bd0: 0a20 2020 2020 2020 2066 756c 6c5f 7061  .        full_pa
+00014be0: 7468 203d 206f 732e 7061 7468 2e6e 6f72  th = os.path.nor
+00014bf0: 6d70 6174 6828 6f73 2e70 6174 682e 6a6f  mpath(os.path.jo
+00014c00: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+00014c10: 7365 6c66 2e63 6f6e 6669 672e 636f 6e66  self.config.conf
+00014c20: 6967 5f64 6972 2c0a 2020 2020 2020 2020  ig_dir,.        
+00014c30: 2020 2020 276c 6976 652f 6578 616d 706c      'live/exampl
+00014c40: 652e 636f 6d2f 6675 6c6c 6368 6169 6e2e  e.com/fullchain.
+00014c50: 7065 6d27 2929 0a20 2020 2020 2020 206d  pem')).        m
+00014c60: 6f63 6b5f 636c 6965 6e74 2e73 6176 655f  ock_client.save_
+00014c70: 6365 7274 6966 6963 6174 652e 7265 7475  certificate.retu
+00014c80: 726e 5f76 616c 7565 203d 2063 6572 745f  rn_value = cert_
+00014c90: 7061 7468 2c20 4e6f 6e65 2c20 6675 6c6c  path, None, full
+00014ca0: 5f70 6174 680a 2020 2020 2020 2020 7769  _path.        wi
+00014cb0: 7468 206d 6f63 6b2e 7061 7463 6828 2763  th mock.patch('c
+00014cc0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00014cd0: 2e6d 6169 6e2e 5f69 6e69 745f 6c65 5f63  .main._init_le_c
+00014ce0: 6c69 656e 7427 2920 6173 206d 6f63 6b5f  lient') as mock_
+00014cf0: 696e 6974 3a0a 2020 2020 2020 2020 2020  init:.          
+00014d00: 2020 6d6f 636b 5f69 6e69 742e 7265 7475    mock_init.retu
+00014d10: 726e 5f76 616c 7565 203d 206d 6f63 6b5f  rn_value = mock_
+00014d20: 636c 6965 6e74 0a20 2020 2020 2020 2020  client.         
+00014d30: 2020 2063 6861 696e 5f70 6174 6820 3d20     chain_path = 
+00014d40: 6f73 2e70 6174 682e 6e6f 726d 7061 7468  os.path.normpath
+00014d50: 286f 732e 7061 7468 2e6a 6f69 6e28 0a20  (os.path.join(. 
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014d70: 656c 662e 636f 6e66 6967 2e63 6f6e 6669  elf.config.confi
+00014d80: 675f 6469 722c 0a20 2020 2020 2020 2020  g_dir,.         
+00014d90: 2020 2020 2020 2027 6c69 7665 2f65 7861         'live/exa
+00014da0: 6d70 6c65 2e63 6f6d 2f63 6861 696e 2e70  mple.com/chain.p
+00014db0: 656d 2729 290a 2020 2020 2020 2020 2020  em')).          
+00014dc0: 2020 6172 6773 203d 2028 272d 6120 7374    args = ('-a st
+00014dd0: 616e 6461 6c6f 6e65 2063 6572 746f 6e6c  andalone certonl
+00014de0: 7920 2d2d 6373 7220 7b30 7d20 2d2d 6365  y --csr {0} --ce
+00014df0: 7274 2d70 6174 6820 7b31 7d20 270a 2020  rt-path {1} '.  
+00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e10: 2020 272d 2d63 6861 696e 2d70 6174 6820    '--chain-path 
+00014e20: 7b32 7d20 2d2d 6675 6c6c 6368 6169 6e2d  {2} --fullchain-
+00014e30: 7061 7468 207b 337d 2729 2e66 6f72 6d61  path {3}').forma
+00014e40: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00014e50: 2020 2020 2020 2020 2020 2043 5352 2c20             CSR, 
+00014e60: 6365 7274 5f70 6174 682c 2063 6861 696e  cert_path, chain
+00014e70: 5f70 6174 682c 2066 756c 6c5f 7061 7468  _path, full_path
+00014e80: 292e 7370 6c69 7428 290a 2020 2020 2020  ).split().      
+00014e90: 2020 2020 2020 6966 2065 7874 7261 5f61        if extra_a
+00014ea0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00014eb0: 2020 2020 2061 7267 7320 2b3d 2065 7874       args += ext
+00014ec0: 7261 5f61 7267 730a 2020 2020 2020 2020  ra_args.        
+00014ed0: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
+00014ee0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+00014ef0: 7465 726e 616c 2e6d 6169 6e2e 6372 7970  ternal.main.cryp
+00014f00: 746f 5f75 7469 6c27 293a 0a20 2020 2020  to_util'):.     
+00014f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014f20: 5f63 616c 6c28 6172 6773 290a 0a20 2020  _call(args)..   
+00014f30: 2020 2020 2069 6620 272d 2d64 7279 2d72       if '--dry-r
+00014f40: 756e 2720 696e 2061 7267 733a 0a20 2020  un' in args:.   
+00014f50: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00014f60: 6d6f 636b 5f63 6c69 656e 742e 7361 7665  mock_client.save
+00014f70: 5f63 6572 7469 6669 6361 7465 2e63 616c  _certificate.cal
+00014f80: 6c65 6420 6973 2046 616c 7365 0a20 2020  led is False.   
+00014f90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014fa0: 2020 2020 2020 206d 6f63 6b5f 636c 6965         mock_clie
+00014fb0: 6e74 2e73 6176 655f 6365 7274 6966 6963  nt.save_certific
+00014fc0: 6174 652e 6173 7365 7274 5f63 616c 6c65  ate.assert_calle
+00014fd0: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
+00014fe0: 2020 2020 2020 2020 2020 2020 2063 6572               cer
+00014ff0: 7472 2c20 6368 6169 6e2c 2063 6572 745f  tr, chain, cert_
+00015000: 7061 7468 2c20 6368 6169 6e5f 7061 7468  path, chain_path
+00015010: 2c20 6675 6c6c 5f70 6174 6829 0a0a 2020  , full_path)..  
+00015020: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+00015030: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00015040: 2e6d 6169 6e2e 5f63 7372 5f72 6570 6f72  .main._csr_repor
+00015050: 745f 6e65 775f 6365 7274 2729 0a20 2020  t_new_cert').   
+00015060: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+00015070: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00015080: 6d61 696e 2e75 7469 6c2e 6174 6578 6974  main.util.atexit
+00015090: 5f72 6567 6973 7465 7227 290a 2020 2020  _register').    
+000150a0: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
+000150b0: 7462 6f74 2e5f 696e 7465 726e 616c 2e65  tbot._internal.e
+000150c0: 6666 2e68 616e 646c 655f 7375 6273 6372  ff.handle_subscr
+000150d0: 6970 7469 6f6e 2729 0a20 2020 2064 6566  iption').    def
+000150e0: 2074 6573 745f 6365 7274 6f6e 6c79 5f63   test_certonly_c
+000150f0: 7372 2873 656c 662c 206d 6f63 6b5f 7375  sr(self, mock_su
+00015100: 6273 6372 6970 7469 6f6e 2c20 6d6f 636b  bscription, mock
+00015110: 5f72 6567 6973 7465 722c 206d 6f63 6b5f  _register, mock_
+00015120: 6373 725f 7265 706f 7274 293a 0a20 2020  csr_report):.   
+00015130: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
+00015140: 6365 7274 6f6e 6c79 5f63 7372 5f63 6f6d  certonly_csr_com
+00015150: 6d6f 6e28 290a 2020 2020 2020 2020 6173  mon().        as
+00015160: 7365 7274 206d 6f63 6b5f 6373 725f 7265  sert mock_csr_re
+00015170: 706f 7274 2e63 616c 6c5f 636f 756e 7420  port.call_count 
+00015180: 3d3d 2031 0a20 2020 2020 2020 2061 7373  == 1.        ass
+00015190: 6572 7420 2763 6572 745f 3531 322e 7065  ert 'cert_512.pe
+000151a0: 6d27 2069 6e20 6d6f 636b 5f63 7372 5f72  m' in mock_csr_r
+000151b0: 6570 6f72 742e 6361 6c6c 5f61 7267 735b  eport.call_args[
+000151c0: 305d 5b31 5d0a 2020 2020 2020 2020 6173  0][1].        as
+000151d0: 7365 7274 206d 6f63 6b5f 6373 725f 7265  sert mock_csr_re
+000151e0: 706f 7274 2e63 616c 6c5f 6172 6773 5b30  port.call_args[0
+000151f0: 5d5b 325d 2069 7320 4e6f 6e65 0a20 2020  ][2] is None.   
+00015200: 2020 2020 2061 7373 6572 7420 2766 756c       assert 'ful
+00015210: 6c63 6861 696e 2e70 656d 2720 696e 206d  lchain.pem' in m
+00015220: 6f63 6b5f 6373 725f 7265 706f 7274 2e63  ock_csr_report.c
+00015230: 616c 6c5f 6172 6773 5b30 5d5b 335d 0a20  all_args[0][3]. 
+00015240: 2020 2020 2020 2061 7373 6572 7420 2764         assert 'd
+00015250: 6f6e 6174 6527 2069 6e20 6d6f 636b 5f72  onate' in mock_r
+00015260: 6567 6973 7465 722e 6361 6c6c 5f61 7267  egister.call_arg
+00015270: 735b 305d 5b31 5d0a 2020 2020 2020 2020  s[0][1].        
+00015280: 6173 7365 7274 206d 6f63 6b5f 7375 6273  assert mock_subs
+00015290: 6372 6970 7469 6f6e 2e63 616c 6c65 6420  cription.called 
+000152a0: 6973 2054 7275 650a 0a20 2020 2040 6d6f  is True..    @mo
+000152b0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+000152c0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+000152d0: 2e5f 6373 725f 7265 706f 7274 5f6e 6577  ._csr_report_new
+000152e0: 5f63 6572 7427 290a 2020 2020 6465 6620  _cert').    def 
+000152f0: 7465 7374 5f63 6572 746f 6e6c 795f 6373  test_certonly_cs
+00015300: 725f 6472 795f 7275 6e28 7365 6c66 2c20  r_dry_run(self, 
+00015310: 6d6f 636b 5f63 7372 5f72 6570 6f72 7429  mock_csr_report)
+00015320: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00015330: 7465 7374 5f63 6572 746f 6e6c 795f 6373  test_certonly_cs
+00015340: 725f 636f 6d6d 6f6e 285b 272d 2d64 7279  r_common(['--dry
+00015350: 2d72 756e 275d 290a 2020 2020 2020 2020  -run']).        
+00015360: 6173 7365 7274 206d 6f63 6b5f 6373 725f  assert mock_csr_
+00015370: 7265 706f 7274 2e63 616c 6c5f 636f 756e  report.call_coun
+00015380: 7420 3d3d 2031 0a20 2020 2020 2020 2061  t == 1.        a
+00015390: 7373 6572 7420 6d6f 636b 5f63 7372 5f72  ssert mock_csr_r
+000153a0: 6570 6f72 742e 6361 6c6c 5f61 7267 735b  eport.call_args[
+000153b0: 305d 5b30 5d2e 6472 795f 7275 6e20 6973  0][0].dry_run is
+000153c0: 2054 7275 650a 0a20 2020 2040 6d6f 636b   True..    @mock
+000153d0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+000153e0: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e5f  _internal.main._
+000153f0: 6465 6c65 7465 5f69 665f 6170 7072 6f70  delete_if_approp
+00015400: 7269 6174 6527 290a 2020 2020 406d 6f63  riate').    @moc
+00015410: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00015420: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
+00015430: 636c 6965 6e74 2e61 636d 655f 636c 6965  client.acme_clie
+00015440: 6e74 2729 0a20 2020 2064 6566 2074 6573  nt').    def tes
+00015450: 745f 7265 766f 6b65 5f77 6974 685f 6b65  t_revoke_with_ke
+00015460: 7928 7365 6c66 2c20 6d6f 636b 5f61 636d  y(self, mock_acm
+00015470: 655f 636c 6965 6e74 2c0a 2020 2020 2020  e_client,.      
+00015480: 2020 2020 2020 6d6f 636b 5f64 656c 6574        mock_delet
+00015490: 655f 6966 5f61 7070 726f 7072 6961 7465  e_if_appropriate
+000154a0: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
+000154b0: 6465 6c65 7465 5f69 665f 6170 7072 6f70  delete_if_approp
+000154c0: 7269 6174 652e 7265 7475 726e 5f76 616c  riate.return_val
+000154d0: 7565 203d 2046 616c 7365 0a20 2020 2020  ue = False.     
+000154e0: 2020 2073 6572 7665 7220 3d20 2766 6f6f     server = 'foo
+000154f0: 2e62 6172 270a 2020 2020 2020 2020 7365  .bar'.        se
+00015500: 6c66 2e5f 6361 6c6c 5f6e 6f5f 636c 6965  lf._call_no_clie
+00015510: 6e74 6d6f 636b 285b 272d 2d63 6572 742d  ntmock(['--cert-
+00015520: 7061 7468 272c 2053 535f 4345 5254 5f50  path', SS_CERT_P
+00015530: 4154 482c 2027 2d2d 6b65 792d 7061 7468  ATH, '--key-path
+00015540: 272c 2052 5341 3230 3438 5f4b 4559 5f50  ', RSA2048_KEY_P
+00015550: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 2020 2020 2020 272d 2d73 6572 7665 7227        '--server'
+00015580: 2c20 7365 7276 6572 2c20 2772 6576 6f6b  , server, 'revok
+00015590: 6527 5d29 0a20 2020 2020 2020 2077 6974  e']).        wit
+000155a0: 6820 6f70 656e 2852 5341 3230 3438 5f4b  h open(RSA2048_K
+000155b0: 4559 5f50 4154 482c 2027 7262 2729 2061  EY_PATH, 'rb') a
+000155c0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+000155d0: 2061 7373 6572 7420 6d6f 636b 5f61 636d   assert mock_acm
+000155e0: 655f 636c 6965 6e74 2e43 6c69 656e 7456  e_client.ClientV
+000155f0: 322e 6361 6c6c 5f63 6f75 6e74 203d 3d20  2.call_count == 
+00015600: 310a 2020 2020 2020 2020 2020 2020 6173  1.            as
+00015610: 7365 7274 206d 6f63 6b5f 6163 6d65 5f63  sert mock_acme_c
+00015620: 6c69 656e 742e 436c 6965 6e74 4e65 7477  lient.ClientNetw
+00015630: 6f72 6b2e 6361 6c6c 5f61 7267 735b 305d  ork.call_args[0]
+00015640: 5b30 5d20 3d3d 205c 0a20 2020 2020 2020  [0] == \.       
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2020 2020 2020 6a6f 7365 2e4a 574b 2e6c        jose.JWK.l
+00015670: 6f61 6428 662e 7265 6164 2829 290a 2020  oad(f.read()).  
+00015680: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00015690: 5353 5f43 4552 545f 5041 5448 2c20 2772  SS_CERT_PATH, 'r
+000156a0: 6227 2920 6173 2066 3a0a 2020 2020 2020  b') as f:.      
+000156b0: 2020 2020 2020 6365 7274 203d 2063 7279        cert = cry
+000156c0: 7074 6f5f 7574 696c 2e70 796f 7065 6e73  pto_util.pyopens
+000156d0: 736c 5f6c 6f61 645f 6365 7274 6966 6963  sl_load_certific
+000156e0: 6174 6528 662e 7265 6164 2829 295b 305d  ate(f.read())[0]
+000156f0: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
+00015700: 6b5f 7265 766f 6b65 203d 206d 6f63 6b5f  k_revoke = mock_
+00015710: 6163 6d65 5f63 6c69 656e 742e 436c 6965  acme_client.Clie
+00015720: 6e74 5632 2829 2e72 6576 6f6b 650a 2020  ntV2().revoke.  
+00015730: 2020 2020 2020 2020 2020 6d6f 636b 5f72            mock_r
+00015740: 6576 6f6b 652e 6173 7365 7274 5f63 616c  evoke.assert_cal
+00015750: 6c65 645f 6f6e 6365 5f77 6974 6828 0a20  led_once_with(. 
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 2020 206a 6f73 652e 436f 6d70 6172 6162     jose.Comparab
+00015780: 6c65 5835 3039 2863 6572 7429 2c0a 2020  leX509(cert),.  
+00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157a0: 2020 6d6f 636b 2e41 4e59 290a 0a20 2020    mock.ANY)..   
+000157b0: 2064 6566 2074 6573 745f 7265 766f 6b65   def test_revoke
+000157c0: 5f77 6974 685f 6b65 795f 6d69 736d 6174  _with_key_mismat
+000157d0: 6368 2873 656c 6629 3a0a 2020 2020 2020  ch(self):.      
+000157e0: 2020 7365 7276 6572 203d 2027 666f 6f2e    server = 'foo.
+000157f0: 6261 7227 0a20 2020 2020 2020 2077 6974  bar'.        wit
+00015800: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+00015810: 6572 726f 7273 2e45 7272 6f72 293a 0a20  errors.Error):. 
+00015820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015830: 5f63 616c 6c5f 6e6f 5f63 6c69 656e 746d  _call_no_clientm
+00015840: 6f63 6b28 5b27 2d2d 6365 7274 2d70 6174  ock(['--cert-pat
+00015850: 6827 2c20 4345 5254 2c20 272d 2d6b 6579  h', CERT, '--key
+00015860: 2d70 6174 6827 2c20 4b45 592c 0a20 2020  -path', KEY,.   
+00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015880: 2020 2020 2020 2020 2020 2020 2020 272d                '-
+00015890: 2d73 6572 7665 7227 2c20 7365 7276 6572  -server', server
+000158a0: 2c20 2772 6576 6f6b 6527 5d29 0a0a 2020  , 'revoke'])..  
+000158b0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+000158c0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+000158d0: 2e6d 6169 6e2e 5f64 656c 6574 655f 6966  .main._delete_if
+000158e0: 5f61 7070 726f 7072 6961 7465 2729 0a20  _appropriate'). 
+000158f0: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+00015900: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00015910: 6c2e 6d61 696e 2e5f 6465 7465 726d 696e  l.main._determin
+00015920: 655f 6163 636f 756e 7427 290a 2020 2020  e_account').    
+00015930: 6465 6620 7465 7374 5f72 6576 6f6b 655f  def test_revoke_
+00015940: 7769 7468 6f75 745f 6b65 7928 7365 6c66  without_key(self
+00015950: 2c20 6d6f 636b 5f64 6574 6572 6d69 6e65  , mock_determine
+00015960: 5f61 6363 6f75 6e74 2c0a 2020 2020 2020  _account,.      
+00015970: 2020 2020 2020 6d6f 636b 5f64 656c 6574        mock_delet
+00015980: 655f 6966 5f61 7070 726f 7072 6961 7465  e_if_appropriate
+00015990: 293a 0a20 2020 2020 2020 206d 6f63 6b5f  ):.        mock_
+000159a0: 6465 6c65 7465 5f69 665f 6170 7072 6f70  delete_if_approp
+000159b0: 7269 6174 652e 7265 7475 726e 5f76 616c  riate.return_val
+000159c0: 7565 203d 2046 616c 7365 0a20 2020 2020  ue = False.     
+000159d0: 2020 206d 6f63 6b5f 6465 7465 726d 696e     mock_determin
+000159e0: 655f 6163 636f 756e 742e 7265 7475 726e  e_account.return
+000159f0: 5f76 616c 7565 203d 2028 6d6f 636b 2e4d  _value = (mock.M
+00015a00: 6167 6963 4d6f 636b 2829 2c20 4e6f 6e65  agicMock(), None
+00015a10: 290a 2020 2020 2020 2020 5f2c 205f 2c20  ).        _, _, 
+00015a20: 5f2c 2063 6c69 656e 7420 3d20 7365 6c66  _, client = self
+00015a30: 2e5f 6361 6c6c 285b 272d 2d63 6572 742d  ._call(['--cert-
+00015a40: 7061 7468 272c 2043 4552 542c 2027 7265  path', CERT, 're
+00015a50: 766f 6b65 275d 290a 2020 2020 2020 2020  voke']).        
+00015a60: 7769 7468 206f 7065 6e28 4345 5254 2920  with open(CERT) 
+00015a70: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00015a80: 2020 6365 7274 203d 2063 7279 7074 6f5f    cert = crypto_
+00015a90: 7574 696c 2e70 796f 7065 6e73 736c 5f6c  util.pyopenssl_l
+00015aa0: 6f61 645f 6365 7274 6966 6963 6174 6528  oad_certificate(
+00015ab0: 662e 7265 6164 2829 295b 305d 0a20 2020  f.read())[0].   
+00015ac0: 2020 2020 2020 2020 206d 6f63 6b5f 7265           mock_re
+00015ad0: 766f 6b65 203d 2063 6c69 656e 742e 6163  voke = client.ac
+00015ae0: 6d65 5f66 726f 6d5f 636f 6e66 6967 5f6b  me_from_config_k
+00015af0: 6579 2829 2e72 6576 6f6b 650a 2020 2020  ey().revoke.    
+00015b00: 2020 2020 2020 2020 6d6f 636b 5f72 6576          mock_rev
+00015b10: 6f6b 652e 6173 7365 7274 5f63 616c 6c65  oke.assert_calle
+00015b20: 645f 6f6e 6365 5f77 6974 6828 0a20 2020  d_once_with(.   
+00015b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b40: 206a 6f73 652e 436f 6d70 6172 6162 6c65   jose.Comparable
+00015b50: 5835 3039 2863 6572 7429 2c0a 2020 2020  X509(cert),.    
+00015b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b70: 6d6f 636b 2e41 4e59 290a 0a20 2020 2040  mock.ANY)..    @
+00015b80: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+00015b90: 626f 742e 5f69 6e74 6572 6e61 6c2e 6c6f  bot._internal.lo
+00015ba0: 672e 706f 7374 5f61 7267 5f70 6172 7365  g.post_arg_parse
+00015bb0: 5f73 6574 7570 2729 0a20 2020 2064 6566  _setup').    def
+00015bc0: 2074 6573 745f 7265 6769 7374 6572 2873   test_register(s
+00015bd0: 656c 662c 205f 293a 0a20 2020 2020 2020  elf, _):.       
+00015be0: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+00015bf0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00015c00: 6e61 6c2e 6d61 696e 2e63 6c69 656e 7427  nal.main.client'
+00015c10: 2920 6173 206d 6f63 6b65 645f 636c 6965  ) as mocked_clie
+00015c20: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00015c30: 6163 6320 3d20 6d6f 636b 2e4d 6167 6963  acc = mock.Magic
+00015c40: 4d6f 636b 2829 0a20 2020 2020 2020 2020  Mock().         
+00015c50: 2020 2061 6363 2e69 6420 3d20 2269 6d61     acc.id = "ima
+00015c60: 6769 6e61 7279 5f61 6363 6f75 6e74 220a  ginary_account".
+00015c70: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
+00015c80: 6564 5f63 6c69 656e 742e 7265 6769 7374  ed_client.regist
+00015c90: 6572 2e72 6574 7572 6e5f 7661 6c75 6520  er.return_value 
+00015ca0: 3d20 2861 6363 2c20 2277 6f72 6b65 6422  = (acc, "worked"
+00015cb0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00015cc0: 6c66 2e5f 6361 6c6c 5f6e 6f5f 636c 6965  lf._call_no_clie
+00015cd0: 6e74 6d6f 636b 285b 2272 6567 6973 7465  ntmock(["registe
+00015ce0: 7222 2c20 222d 2d65 6d61 696c 222c 2022  r", "--email", "
+00015cf0: 7573 6572 4065 7861 6d70 6c65 2e6f 7267  user@example.org
+00015d00: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+00015d10: 2320 544f 444f 3a20 4974 2077 6f75 6c64  # TODO: It would
+00015d20: 2062 6520 6d6f 7265 2063 6f72 7265 6374   be more correct
+00015d30: 2074 6f20 6578 706c 6963 6974 6c79 2063   to explicitly c
+00015d40: 6865 636b 2074 6861 740a 2020 2020 2020  heck that.      
+00015d50: 2020 2020 2020 2320 2020 2020 2020 5f64        #       _d
+00015d60: 6574 6572 6d69 6e65 5f61 6363 6f75 6e74  etermine_account
+00015d70: 2829 2067 6574 7320 6361 6c6c 6564 2069  () gets called i
+00015d80: 6e20 7468 6520 6162 6f76 6520 6361 7365  n the above case
+00015d90: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00015da0: 2020 2020 2020 6275 7420 636f 7665 7261        but covera
+00015db0: 6765 2073 7461 7469 7374 6963 7320 7368  ge statistics sh
+00015dc0: 6f75 6c64 2061 6c73 6f20 7368 6f77 2074  ould also show t
+00015dd0: 6861 7420 6974 2064 6964 2e0a 2020 2020  hat it did..    
+00015de0: 2020 2020 2020 2020 7769 7468 206d 6f63          with moc
+00015df0: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00015e00: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
+00015e10: 6163 636f 756e 7427 2920 6173 206d 6f63  account') as moc
+00015e20: 6b65 645f 6163 636f 756e 743a 0a20 2020  ked_account:.   
+00015e30: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
+00015e40: 6b65 645f 7374 6f72 6167 6520 3d20 6d6f  ked_storage = mo
+00015e50: 636b 2e4d 6167 6963 4d6f 636b 2829 0a20  ck.MagicMock(). 
+00015e60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00015e70: 6f63 6b65 645f 6163 636f 756e 742e 4163  ocked_account.Ac
+00015e80: 636f 756e 7446 696c 6553 746f 7261 6765  countFileStorage
+00015e90: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00015ea0: 6d6f 636b 6564 5f73 746f 7261 6765 0a20  mocked_storage. 
+00015eb0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00015ec0: 6f63 6b65 645f 7374 6f72 6167 652e 6669  ocked_storage.fi
+00015ed0: 6e64 5f61 6c6c 2e72 6574 7572 6e5f 7661  nd_all.return_va
+00015ee0: 6c75 6520 3d20 5b22 616e 2061 6363 6f75  lue = ["an accou
+00015ef0: 6e74 225d 0a20 2020 2020 2020 2020 2020  nt"].           
+00015f00: 2020 2020 2078 203d 2073 656c 662e 5f63       x = self._c
+00015f10: 616c 6c5f 6e6f 5f63 6c69 656e 746d 6f63  all_no_clientmoc
+00015f20: 6b28 5b22 7265 6769 7374 6572 222c 2022  k(["register", "
+00015f30: 2d2d 656d 6169 6c22 2c20 2275 7365 7240  --email", "user@
+00015f40: 6578 616d 706c 652e 6f72 6722 5d29 0a20  example.org"]). 
+00015f50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00015f60: 7373 6572 7420 2254 6865 7265 2069 7320  ssert "There is 
+00015f70: 616e 2065 7869 7374 696e 6720 6163 636f  an existing acco
+00015f80: 756e 7422 2069 6e20 785b 305d 0a0a 2020  unt" in x[0]..  
+00015f90: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+00015fa0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00015fb0: 2e70 6c75 6769 6e73 2e73 656c 6563 7469  .plugins.selecti
+00015fc0: 6f6e 2e63 686f 6f73 655f 636f 6e66 6967  on.choose_config
+00015fd0: 7572 6174 6f72 5f70 6c75 6769 6e73 2729  urator_plugins')
+00015fe0: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+00015ff0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00016000: 6e61 6c2e 7570 6461 7465 722e 5f72 756e  nal.updater._run
+00016010: 5f75 7064 6174 6572 7327 290a 2020 2020  _updaters').    
+00016020: 6465 6620 7465 7374 5f70 6c75 6769 6e5f  def test_plugin_
+00016030: 7365 6c65 6374 696f 6e5f 6572 726f 7228  selection_error(
+00016040: 7365 6c66 2c20 6d6f 636b 5f72 756e 2c20  self, mock_run, 
+00016050: 6d6f 636b 5f63 686f 6f73 6529 3a0a 2020  mock_choose):.  
+00016060: 2020 2020 2020 6d6f 636b 5f63 686f 6f73        mock_choos
+00016070: 652e 7369 6465 5f65 6666 6563 7420 3d20  e.side_effect = 
+00016080: 6572 726f 7273 2e50 6c75 6769 6e53 656c  errors.PluginSel
+00016090: 6563 7469 6f6e 4572 726f 720a 2020 2020  ectionError.    
+000160a0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+000160b0: 7261 6973 6573 2865 7272 6f72 732e 506c  raises(errors.Pl
+000160c0: 7567 696e 5365 6c65 6374 696f 6e45 7272  uginSelectionErr
+000160d0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+000160e0: 206d 6169 6e2e 7265 6e65 775f 6365 7274   main.renew_cert
+000160f0: 284e 6f6e 652c 204e 6f6e 652c 204e 6f6e  (None, None, Non
+00016100: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00016110: 2e63 6f6e 6669 672e 6472 795f 7275 6e20  .config.dry_run 
+00016120: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00016130: 7570 6461 7465 722e 7275 6e5f 6765 6e65  updater.run_gene
+00016140: 7269 635f 7570 6461 7465 7273 2873 656c  ric_updaters(sel
+00016150: 662e 636f 6e66 6967 2c20 4e6f 6e65 2c20  f.config, None, 
+00016160: 4e6f 6e65 290a 2020 2020 2020 2020 2320  None).        # 
+00016170: 4d61 6b65 2073 7572 6520 7765 2772 6520  Make sure we're 
+00016180: 7265 7475 726e 696e 6720 4e6f 6e65 2c20  returning None, 
+00016190: 616e 6420 6865 6e63 6520 6e6f 7420 7472  and hence not tr
+000161a0: 7969 6e67 2074 6f20 7275 6e20 7468 650a  ying to run the.
+000161b0: 2020 2020 2020 2020 2320 7769 7468 6f75          # withou
+000161c0: 7420 696e 7374 616c 6c65 720a 2020 2020  t installer.    
+000161d0: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
+000161e0: 7275 6e2e 6361 6c6c 6564 2069 7320 4661  run.called is Fa
+000161f0: 6c73 650a 0a20 2020 2040 6d6f 636b 2e70  lse..    @mock.p
+00016200: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+00016210: 6e74 6572 6e61 6c2e 6d61 696e 2e75 7064  nternal.main.upd
+00016220: 6174 6572 2e72 756e 5f72 656e 6577 616c  ater.run_renewal
+00016230: 5f64 6570 6c6f 7965 7227 290a 2020 2020  _deployer').    
+00016240: 406d 6f63 6b2e 7061 7463 6828 2763 6572  @mock.patch('cer
+00016250: 7462 6f74 2e5f 696e 7465 726e 616c 2e70  tbot._internal.p
+00016260: 6c75 6769 6e73 2e73 656c 6563 7469 6f6e  lugins.selection
+00016270: 2e63 686f 6f73 655f 636f 6e66 6967 7572  .choose_configur
+00016280: 6174 6f72 5f70 6c75 6769 6e73 2729 0a20  ator_plugins'). 
+00016290: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+000162a0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+000162b0: 6c2e 6d61 696e 2e5f 696e 6974 5f6c 655f  l.main._init_le_
+000162c0: 636c 6965 6e74 2729 0a20 2020 2040 6d6f  client').    @mo
+000162d0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+000162e0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+000162f0: 2e5f 6765 745f 616e 645f 7361 7665 5f63  ._get_and_save_c
+00016300: 6572 7427 290a 2020 2020 6465 6620 7465  ert').    def te
+00016310: 7374 5f72 656e 6577 5f64 6f65 736e 745f  st_renew_doesnt_
+00016320: 7265 7374 6172 745f 6f6e 5f64 7279 7275  restart_on_dryru
+00016330: 6e28 7365 6c66 2c20 6d6f 636b 5f67 6574  n(self, mock_get
+00016340: 5f63 6572 742c 206d 6f63 6b5f 696e 6974  _cert, mock_init
+00016350: 2c20 6d6f 636b 5f63 686f 6f73 652c 0a20  , mock_choose,. 
+00016360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016380: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
+00016390: 7275 6e5f 7265 6e65 7761 6c5f 6465 706c  run_renewal_depl
+000163a0: 6f79 6572 293a 0a20 2020 2020 2020 2022  oyer):.        "
+000163b0: 2222 4120 6472 792d 7275 6e20 7265 6e65  ""A dry-run rene
+000163c0: 7761 6c20 7368 6f75 6c64 6e27 7420 7472  wal shouldn't tr
+000163d0: 7920 746f 2072 6573 7461 7274 2074 6865  y to restart the
+000163e0: 2069 6e73 7461 6c6c 6572 2222 220a 2020   installer""".  
+000163f0: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00016400: 672e 6472 795f 7275 6e20 3d20 5472 7565  g.dry_run = True
+00016410: 0a20 2020 2020 2020 2069 6e73 7461 6c6c  .        install
+00016420: 6572 203d 206d 6f63 6b2e 4d61 6769 634d  er = mock.MagicM
+00016430: 6f63 6b28 290a 2020 2020 2020 2020 6d6f  ock().        mo
+00016440: 636b 5f63 686f 6f73 652e 7265 7475 726e  ck_choose.return
+00016450: 5f76 616c 7565 203d 2028 696e 7374 616c  _value = (instal
+00016460: 6c65 722c 206d 6f63 6b2e 4d61 6769 634d  ler, mock.MagicM
+00016470: 6f63 6b28 2929 0a0a 2020 2020 2020 2020  ock())..        
+00016480: 6d61 696e 2e72 656e 6577 5f63 6572 7428  main.renew_cert(
+00016490: 7365 6c66 2e63 6f6e 6669 672c 204e 6f6e  self.config, Non
+000164a0: 652c 204e 6f6e 6529 0a0a 2020 2020 2020  e, None)..      
+000164b0: 2020 6173 7365 7274 206d 6f63 6b5f 696e    assert mock_in
+000164c0: 6974 2e63 616c 6c5f 636f 756e 7420 3d3d  it.call_count ==
+000164d0: 2031 0a20 2020 2020 2020 2061 7373 6572   1.        asser
+000164e0: 7420 6d6f 636b 5f67 6574 5f63 6572 742e  t mock_get_cert.
+000164f0: 6361 6c6c 5f63 6f75 6e74 203d 3d20 310a  call_count == 1.
+00016500: 2020 2020 2020 2020 696e 7374 616c 6c65          installe
+00016510: 722e 7265 7374 6172 742e 6173 7365 7274  r.restart.assert
+00016520: 5f6e 6f74 5f63 616c 6c65 6428 290a 2020  _not_called().  
+00016530: 2020 2020 2020 6d6f 636b 5f72 756e 5f72        mock_run_r
+00016540: 656e 6577 616c 5f64 6570 6c6f 7965 722e  enewal_deployer.
+00016550: 6173 7365 7274 5f6e 6f74 5f63 616c 6c65  assert_not_calle
+00016560: 6428 290a 0a0a 636c 6173 7320 556e 7265  d()...class Unre
+00016570: 6769 7374 6572 5465 7374 2875 6e69 7474  gisterTest(unitt
+00016580: 6573 742e 5465 7374 4361 7365 293a 0a20  est.TestCase):. 
+00016590: 2020 2064 6566 2073 6574 5570 2873 656c     def setUp(sel
+000165a0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000165b0: 2e70 6174 6368 6572 7320 3d20 7b0a 2020  .patchers = {.  
+000165c0: 2020 2020 2020 2020 2020 275f 6465 7465            '_dete
+000165d0: 726d 696e 655f 6163 636f 756e 7427 3a20  rmine_account': 
+000165e0: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+000165f0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+00016600: 696e 2e5f 6465 7465 726d 696e 655f 6163  in._determine_ac
+00016610: 636f 756e 7427 292c 0a20 2020 2020 2020  count'),.       
+00016620: 2020 2020 2027 6163 636f 756e 7427 3a20       'account': 
+00016630: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+00016640: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+00016650: 696e 2e61 6363 6f75 6e74 2729 2c0a 2020  in.account'),.  
+00016660: 2020 2020 2020 2020 2020 2763 6c69 656e            'clien
+00016670: 7427 3a20 6d6f 636b 2e70 6174 6368 2827  t': mock.patch('
+00016680: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00016690: 6c2e 6d61 696e 2e63 6c69 656e 7427 292c  l.main.client'),
+000166a0: 0a20 2020 2020 2020 2020 2020 2027 6765  .            'ge
+000166b0: 745f 7574 696c 6974 7927 3a20 7465 7374  t_utility': test
+000166c0: 5f75 7469 6c2e 7061 7463 685f 6469 7370  _util.patch_disp
+000166d0: 6c61 795f 7574 696c 2829 7d0a 2020 2020  lay_util()}.    
+000166e0: 2020 2020 7365 6c66 2e6d 6f63 6b73 203d      self.mocks =
+000166f0: 207b 6b3a 2076 2e73 7461 7274 2829 2066   {k: v.start() f
+00016700: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
+00016710: 7061 7463 6865 7273 2e69 7465 6d73 2829  patchers.items()
+00016720: 7d0a 0a20 2020 2064 6566 2074 6561 7244  }..    def tearD
+00016730: 6f77 6e28 7365 6c66 293a 0a20 2020 2020  own(self):.     
+00016740: 2020 2066 6f72 2070 6174 6368 2069 6e20     for patch in 
+00016750: 7365 6c66 2e70 6174 6368 6572 732e 7661  self.patchers.va
+00016760: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
+00016770: 2020 2020 7061 7463 682e 7374 6f70 2829      patch.stop()
+00016780: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+00016790: 626f 7274 5f75 6e72 6567 6973 7465 7228  bort_unregister(
+000167a0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+000167b0: 656c 662e 6d6f 636b 735b 2761 6363 6f75  elf.mocks['accou
+000167c0: 6e74 275d 2e41 6363 6f75 6e74 4669 6c65  nt'].AccountFile
+000167d0: 5374 6f72 6167 652e 7265 7475 726e 5f76  Storage.return_v
+000167e0: 616c 7565 203d 206d 6f63 6b2e 4d6f 636b  alue = mock.Mock
+000167f0: 2829 0a0a 2020 2020 2020 2020 7574 696c  ()..        util
+00016800: 5f6d 6f63 6b20 3d20 7365 6c66 2e6d 6f63  _mock = self.moc
+00016810: 6b73 5b27 6765 745f 7574 696c 6974 7927  ks['get_utility'
+00016820: 5d28 290a 2020 2020 2020 2020 7574 696c  ]().        util
+00016830: 5f6d 6f63 6b2e 7965 736e 6f2e 7265 7475  _mock.yesno.retu
+00016840: 726e 5f76 616c 7565 203d 2046 616c 7365  rn_value = False
+00016850: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
+00016860: 203d 206d 6f63 6b2e 4d6f 636b 2829 0a20   = mock.Mock(). 
+00016870: 2020 2020 2020 2075 6e75 7365 645f 706c         unused_pl
+00016880: 7567 696e 7320 3d20 6d6f 636b 2e4d 6f63  ugins = mock.Moc
+00016890: 6b28 290a 0a20 2020 2020 2020 2072 6573  k()..        res
+000168a0: 203d 206d 6169 6e2e 756e 7265 6769 7374   = main.unregist
+000168b0: 6572 2863 6f6e 6669 672c 2075 6e75 7365  er(config, unuse
+000168c0: 645f 706c 7567 696e 7329 0a20 2020 2020  d_plugins).     
+000168d0: 2020 2061 7373 6572 7420 7265 7320 3d3d     assert res ==
+000168e0: 2022 4465 6163 7469 7661 7469 6f6e 2061   "Deactivation a
+000168f0: 626f 7274 6564 2e22 0a0a 2020 2020 406d  borted."..    @m
+00016900: 6f63 6b2e 7061 7463 6828 2263 6572 7462  ock.patch("certb
+00016910: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+00016920: 6e2e 6469 7370 6c61 795f 7574 696c 2e6e  n.display_util.n
+00016930: 6f74 6966 7922 290a 2020 2020 6465 6620  otify").    def 
+00016940: 7465 7374 5f75 6e72 6567 6973 7465 7228  test_unregister(
+00016950: 7365 6c66 2c20 6d6f 636b 5f6e 6f74 6966  self, mock_notif
+00016960: 7929 3a0a 2020 2020 2020 2020 6d6f 636b  y):.        mock
+00016970: 6564 5f73 746f 7261 6765 203d 206d 6f63  ed_storage = moc
+00016980: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
+00016990: 2020 2020 2020 6d6f 636b 6564 5f73 746f        mocked_sto
+000169a0: 7261 6765 2e66 696e 645f 616c 6c2e 7265  rage.find_all.re
+000169b0: 7475 726e 5f76 616c 7565 203d 205b 2261  turn_value = ["a
+000169c0: 6e20 6163 636f 756e 7422 5d0a 0a20 2020  n account"]..   
+000169d0: 2020 2020 2073 656c 662e 6d6f 636b 735b       self.mocks[
+000169e0: 2761 6363 6f75 6e74 275d 2e41 6363 6f75  'account'].Accou
+000169f0: 6e74 4669 6c65 5374 6f72 6167 652e 7265  ntFileStorage.re
+00016a00: 7475 726e 5f76 616c 7565 203d 206d 6f63  turn_value = moc
+00016a10: 6b65 645f 7374 6f72 6167 650a 2020 2020  ked_storage.    
+00016a20: 2020 2020 7365 6c66 2e6d 6f63 6b73 5b27      self.mocks['
+00016a30: 5f64 6574 6572 6d69 6e65 5f61 6363 6f75  _determine_accou
+00016a40: 6e74 275d 2e72 6574 7572 6e5f 7661 6c75  nt'].return_valu
+00016a50: 6520 3d20 286d 6f63 6b2e 4d61 6769 634d  e = (mock.MagicM
+00016a60: 6f63 6b28 292c 2022 666f 6f22 290a 0a20  ock(), "foo").. 
+00016a70: 2020 2020 2020 2063 625f 636c 6965 6e74         cb_client
+00016a80: 203d 206d 6f63 6b2e 4d61 6769 634d 6f63   = mock.MagicMoc
+00016a90: 6b28 290a 2020 2020 2020 2020 7365 6c66  k().        self
+00016aa0: 2e6d 6f63 6b73 5b27 636c 6965 6e74 275d  .mocks['client']
+00016ab0: 2e43 6c69 656e 742e 7265 7475 726e 5f76  .Client.return_v
+00016ac0: 616c 7565 203d 2063 625f 636c 6965 6e74  alue = cb_client
+00016ad0: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
+00016ae0: 203d 206d 6f63 6b2e 4d61 6769 634d 6f63   = mock.MagicMoc
+00016af0: 6b28 290a 2020 2020 2020 2020 756e 7573  k().        unus
+00016b00: 6564 5f70 6c75 6769 6e73 203d 206d 6f63  ed_plugins = moc
+00016b10: 6b2e 4d61 6769 634d 6f63 6b28 290a 0a20  k.MagicMock().. 
+00016b20: 2020 2020 2020 2072 6573 203d 206d 6169         res = mai
+00016b30: 6e2e 756e 7265 6769 7374 6572 2863 6f6e  n.unregister(con
+00016b40: 6669 672c 2075 6e75 7365 645f 706c 7567  fig, unused_plug
+00016b50: 696e 7329 0a0a 2020 2020 2020 2020 6173  ins)..        as
+00016b60: 7365 7274 2072 6573 2069 7320 4e6f 6e65  sert res is None
+00016b70: 0a20 2020 2020 2020 206d 6f63 6b5f 6e6f  .        mock_no
+00016b80: 7469 6679 2e61 7373 6572 745f 6361 6c6c  tify.assert_call
+00016b90: 6564 5f6f 6e63 655f 7769 7468 2822 4163  ed_once_with("Ac
+00016ba0: 636f 756e 7420 6465 6163 7469 7661 7465  count deactivate
+00016bb0: 642e 2229 0a0a 2020 2020 6465 6620 7465  d.")..    def te
+00016bc0: 7374 5f75 6e72 6567 6973 7465 725f 6e6f  st_unregister_no
+00016bd0: 5f61 6363 6f75 6e74 2873 656c 6629 3a0a  _account(self):.
+00016be0: 2020 2020 2020 2020 6d6f 636b 6564 5f73          mocked_s
+00016bf0: 746f 7261 6765 203d 206d 6f63 6b2e 4d61  torage = mock.Ma
+00016c00: 6769 634d 6f63 6b28 290a 2020 2020 2020  gicMock().      
+00016c10: 2020 6d6f 636b 6564 5f73 746f 7261 6765    mocked_storage
+00016c20: 2e66 696e 645f 616c 6c2e 7265 7475 726e  .find_all.return
+00016c30: 5f76 616c 7565 203d 205b 5d0a 2020 2020  _value = [].    
+00016c40: 2020 2020 7365 6c66 2e6d 6f63 6b73 5b27      self.mocks['
+00016c50: 6163 636f 756e 7427 5d2e 4163 636f 756e  account'].Accoun
+00016c60: 7446 696c 6553 746f 7261 6765 2e72 6574  tFileStorage.ret
+00016c70: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
+00016c80: 6564 5f73 746f 7261 6765 0a0a 2020 2020  ed_storage..    
+00016c90: 2020 2020 6362 5f63 6c69 656e 7420 3d20      cb_client = 
+00016ca0: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
+00016cb0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+00016cc0: 636b 735b 2763 6c69 656e 7427 5d2e 436c  cks['client'].Cl
+00016cd0: 6965 6e74 2e72 6574 7572 6e5f 7661 6c75  ient.return_valu
+00016ce0: 6520 3d20 6362 5f63 6c69 656e 740a 0a20  e = cb_client.. 
+00016cf0: 2020 2020 2020 2063 6f6e 6669 6720 3d20         config = 
+00016d00: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2829  mock.MagicMock()
+00016d10: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00016d20: 7365 7276 6572 203d 2022 6874 7470 733a  server = "https:
+00016d30: 2f2f 6163 6d65 2e65 7861 6d70 6c65 2e63  //acme.example.c
+00016d40: 6f6d 2f64 6972 6563 746f 7279 220a 2020  om/directory".  
+00016d50: 2020 2020 2020 756e 7573 6564 5f70 6c75        unused_plu
+00016d60: 6769 6e73 203d 206d 6f63 6b2e 4d61 6769  gins = mock.Magi
+00016d70: 634d 6f63 6b28 290a 0a20 2020 2020 2020  cMock()..       
+00016d80: 2072 6573 203d 206d 6169 6e2e 756e 7265   res = main.unre
+00016d90: 6769 7374 6572 2863 6f6e 6669 672c 2075  gister(config, u
+00016da0: 6e75 7365 645f 706c 7567 696e 7329 0a20  nused_plugins). 
+00016db0: 2020 2020 2020 206d 203d 2022 436f 756c         m = "Coul
+00016dc0: 6420 6e6f 7420 6669 6e64 2065 7869 7374  d not find exist
+00016dd0: 696e 6720 6163 636f 756e 7420 666f 7220  ing account for 
+00016de0: 7365 7276 6572 2068 7474 7073 3a2f 2f61  server https://a
+00016df0: 636d 652e 6578 616d 706c 652e 636f 6d2f  cme.example.com/
+00016e00: 6469 7265 6374 6f72 792e 220a 2020 2020  directory.".    
+00016e10: 2020 2020 6173 7365 7274 2072 6573 203d      assert res =
+00016e20: 3d20 6d0a 2020 2020 2020 2020 6173 7365  = m.        asse
+00016e30: 7274 2063 625f 636c 6965 6e74 2e61 636d  rt cb_client.acm
+00016e40: 652e 6465 6163 7469 7661 7465 5f72 6567  e.deactivate_reg
+00016e50: 6973 7472 6174 696f 6e2e 6361 6c6c 6564  istration.called
+00016e60: 2069 7320 4661 6c73 650a 0a0a 636c 6173   is False...clas
+00016e70: 7320 4d61 6b65 4f72 5665 7269 6679 4e65  s MakeOrVerifyNe
+00016e80: 6564 6564 4469 7273 2874 6573 745f 7574  ededDirs(test_ut
+00016e90: 696c 2e43 6f6e 6669 6754 6573 7443 6173  il.ConfigTestCas
+00016ea0: 6529 3a0a 2020 2020 2222 2254 6573 7473  e):.    """Tests
+00016eb0: 2066 6f72 2063 6572 7462 6f74 2e5f 696e   for certbot._in
+00016ec0: 7465 726e 616c 2e6d 6169 6e2e 6d61 6b65  ternal.main.make
+00016ed0: 5f6f 725f 7665 7269 6679 5f6e 6565 6465  _or_verify_neede
+00016ee0: 645f 6469 7273 2e22 2222 0a0a 2020 2020  d_dirs."""..    
+00016ef0: 406d 6f63 6b2e 7061 7463 6828 2263 6572  @mock.patch("cer
+00016f00: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+00016f10: 6169 6e2e 7574 696c 2229 0a20 2020 2064  ain.util").    d
+00016f20: 6566 2074 6573 745f 6974 2873 656c 662c  ef test_it(self,
+00016f30: 206d 6f63 6b5f 7574 696c 293a 0a20 2020   mock_util):.   
+00016f40: 2020 2020 206d 6169 6e2e 6d61 6b65 5f6f       main.make_o
+00016f50: 725f 7665 7269 6679 5f6e 6565 6465 645f  r_verify_needed_
+00016f60: 6469 7273 2873 656c 662e 636f 6e66 6967  dirs(self.config
+00016f70: 290a 2020 2020 2020 2020 666f 7220 636f  ).        for co
+00016f80: 7265 5f64 6972 2069 6e20 2873 656c 662e  re_dir in (self.
+00016f90: 636f 6e66 6967 2e63 6f6e 6669 675f 6469  config.config_di
+00016fa0: 722c 2073 656c 662e 636f 6e66 6967 2e77  r, self.config.w
+00016fb0: 6f72 6b5f 6469 722c 293a 0a20 2020 2020  ork_dir,):.     
+00016fc0: 2020 2020 2020 206d 6f63 6b5f 7574 696c         mock_util
+00016fd0: 2e73 6574 5f75 705f 636f 7265 5f64 6972  .set_up_core_dir
+00016fe0: 2e61 7373 6572 745f 616e 795f 6361 6c6c  .assert_any_call
+00016ff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00017000: 2020 636f 7265 5f64 6972 2c20 636f 6e73    core_dir, cons
+00017010: 7461 6e74 732e 434f 4e46 4947 5f44 4952  tants.CONFIG_DIR
+00017020: 535f 4d4f 4445 2c0a 2020 2020 2020 2020  S_MODE,.        
+00017030: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00017040: 6669 672e 7374 7269 6374 5f70 6572 6d69  fig.strict_permi
+00017050: 7373 696f 6e73 0a20 2020 2020 2020 2020  ssions.         
+00017060: 2020 2029 0a0a 2020 2020 2020 2020 686f     )..        ho
+00017070: 6f6b 5f64 6972 7320 3d20 2873 656c 662e  ok_dirs = (self.
+00017080: 636f 6e66 6967 2e72 656e 6577 616c 5f70  config.renewal_p
+00017090: 7265 5f68 6f6f 6b73 5f64 6972 2c0a 2020  re_hooks_dir,.  
+000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170b0: 2020 2073 656c 662e 636f 6e66 6967 2e72     self.config.r
+000170c0: 656e 6577 616c 5f64 6570 6c6f 795f 686f  enewal_deploy_ho
+000170d0: 6f6b 735f 6469 722c 0a20 2020 2020 2020  oks_dir,.       
+000170e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000170f0: 6c66 2e63 6f6e 6669 672e 7265 6e65 7761  lf.config.renewa
+00017100: 6c5f 706f 7374 5f68 6f6f 6b73 5f64 6972  l_post_hooks_dir
+00017110: 2c29 0a20 2020 2020 2020 2066 6f72 2068  ,).        for h
+00017120: 6f6f 6b5f 6469 7220 696e 2068 6f6f 6b5f  ook_dir in hook_
+00017130: 6469 7273 3a0a 2020 2020 2020 2020 2020  dirs:.          
+00017140: 2020 2320 6465 6661 756c 7420 6d6f 6465    # default mode
+00017150: 206f 6620 3735 3520 6973 2075 7365 640a   of 755 is used.
+00017160: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
+00017170: 5f75 7469 6c2e 6d61 6b65 5f6f 725f 7665  _util.make_or_ve
+00017180: 7269 6679 5f64 6972 2e61 7373 6572 745f  rify_dir.assert_
+00017190: 616e 795f 6361 6c6c 280a 2020 2020 2020  any_call(.      
+000171a0: 2020 2020 2020 2020 2020 686f 6f6b 5f64            hook_d
+000171b0: 6972 2c20 7374 7269 6374 3d73 656c 662e  ir, strict=self.
+000171c0: 636f 6e66 6967 2e73 7472 6963 745f 7065  config.strict_pe
+000171d0: 726d 6973 7369 6f6e 7329 0a0a 0a63 6c61  rmissions)...cla
+000171e0: 7373 2045 6e68 616e 6365 5465 7374 2874  ss EnhanceTest(t
+000171f0: 6573 745f 7574 696c 2e43 6f6e 6669 6754  est_util.ConfigT
+00017200: 6573 7443 6173 6529 3a0a 2020 2020 2222  estCase):.    ""
+00017210: 2254 6573 7473 2066 6f72 2063 6572 7462  "Tests for certb
+00017220: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+00017230: 6e2e 656e 6861 6e63 652e 2222 220a 0a20  n.enhance.""".. 
+00017240: 2020 2064 6566 2073 6574 5570 2873 656c     def setUp(sel
+00017250: 6629 3a0a 2020 2020 2020 2020 7375 7065  f):.        supe
+00017260: 7228 292e 7365 7455 7028 290a 2020 2020  r().setUp().    
+00017270: 2020 2020 7365 6c66 2e67 6574 5f75 7469      self.get_uti
+00017280: 6c69 7479 5f70 6174 6368 203d 2074 6573  lity_patch = tes
+00017290: 745f 7574 696c 2e70 6174 6368 5f64 6973  t_util.patch_dis
+000172a0: 706c 6179 5f75 7469 6c28 290a 2020 2020  play_util().    
+000172b0: 2020 2020 7365 6c66 2e6d 6f63 6b5f 6765      self.mock_ge
+000172c0: 745f 7574 696c 6974 7920 3d20 7365 6c66  t_utility = self
+000172d0: 2e67 6574 5f75 7469 6c69 7479 5f70 6174  .get_utility_pat
+000172e0: 6368 2e73 7461 7274 2829 0a20 2020 2020  ch.start().     
+000172f0: 2020 2073 656c 662e 6d6f 636b 696e 7374     self.mockinst
+00017300: 616c 6c65 7220 3d20 6d6f 636b 2e4d 6167  aller = mock.Mag
+00017310: 6963 4d6f 636b 2873 7065 633d 656e 6861  icMock(spec=enha
+00017320: 6e63 656d 656e 7473 2e41 7574 6f48 5354  ncements.AutoHST
+00017330: 5345 6e68 616e 6365 6d65 6e74 290a 0a20  SEnhancement).. 
+00017340: 2020 2064 6566 2074 6561 7244 6f77 6e28     def tearDown(
+00017350: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00017360: 656c 662e 6765 745f 7574 696c 6974 795f  elf.get_utility_
+00017370: 7061 7463 682e 7374 6f70 2829 0a0a 2020  patch.stop()..  
+00017380: 2020 6465 6620 5f63 616c 6c28 7365 6c66    def _call(self
+00017390: 2c20 6172 6773 293a 0a20 2020 2020 2020  , args):.       
+000173a0: 2070 6c75 6769 6e73 203d 2064 6973 636f   plugins = disco
+000173b0: 2e50 6c75 6769 6e73 5265 6769 7374 7279  .PluginsRegistry
+000173c0: 2e66 696e 645f 616c 6c28 290a 2020 2020  .find_all().    
+000173d0: 2020 2020 636f 6e66 6967 203d 2063 6c69      config = cli
+000173e0: 2e70 7265 7061 7265 5f61 6e64 5f70 6172  .prepare_and_par
+000173f0: 7365 5f61 7267 7328 706c 7567 696e 732c  se_args(plugins,
+00017400: 2061 7267 7329 0a0a 2020 2020 2020 2020   args)..        
+00017410: 7769 7468 206d 6f63 6b2e 7061 7463 6828  with mock.patch(
+00017420: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00017430: 616c 2e63 6572 745f 6d61 6e61 6765 722e  al.cert_manager.
+00017440: 6765 745f 6365 7274 6e61 6d65 7327 2920  get_certnames') 
+00017450: 6173 206d 6f63 6b5f 6365 7274 733a 0a20  as mock_certs:. 
+00017460: 2020 2020 2020 2020 2020 206d 6f63 6b5f             mock_
+00017470: 6365 7274 732e 7265 7475 726e 5f76 616c  certs.return_val
+00017480: 7565 203d 205b 2765 7861 6d70 6c65 2e63  ue = ['example.c
+00017490: 6f6d 275d 0a20 2020 2020 2020 2020 2020  om'].           
+000174a0: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+000174b0: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+000174c0: 6e61 6c2e 6365 7274 5f6d 616e 6167 6572  nal.cert_manager
+000174d0: 2e64 6f6d 6169 6e73 5f66 6f72 5f63 6572  .domains_for_cer
+000174e0: 746e 616d 6527 2920 6173 206d 6f63 6b5f  tname') as mock_
+000174f0: 646f 6d3a 0a20 2020 2020 2020 2020 2020  dom:.           
+00017500: 2020 2020 206d 6f63 6b5f 646f 6d2e 7265       mock_dom.re
+00017510: 7475 726e 5f76 616c 7565 203d 205b 2765  turn_value = ['e
+00017520: 7861 6d70 6c65 2e63 6f6d 275d 0a20 2020  xample.com'].   
+00017530: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00017540: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
+00017550: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00017560: 6d61 696e 2e5f 696e 6974 5f6c 655f 636c  main._init_le_cl
+00017570: 6965 6e74 2729 2061 7320 6d6f 636b 5f69  ient') as mock_i
+00017580: 6e69 743a 0a20 2020 2020 2020 2020 2020  nit:.           
+00017590: 2020 2020 2020 2020 206d 6f63 6b5f 636c           mock_cl
+000175a0: 6965 6e74 203d 206d 6f63 6b2e 4d61 6769  ient = mock.Magi
+000175b0: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
+000175c0: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
+000175d0: 5f63 6c69 656e 742e 636f 6e66 6967 203d  _client.config =
+000175e0: 2063 6f6e 6669 670a 2020 2020 2020 2020   config.        
+000175f0: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
+00017600: 5f69 6e69 742e 7265 7475 726e 5f76 616c  _init.return_val
+00017610: 7565 203d 206d 6f63 6b5f 636c 6965 6e74  ue = mock_client
+00017620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017630: 2020 2020 206d 6169 6e2e 656e 6861 6e63       main.enhanc
+00017640: 6528 636f 6e66 6967 2c20 706c 7567 696e  e(config, plugin
+00017650: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00017660: 2020 2020 2020 2072 6574 7572 6e20 6d6f         return mo
+00017670: 636b 5f63 6c69 656e 7420 2320 7265 7475  ck_client # retu
+00017680: 726e 7320 7468 6520 636c 6965 6e74 0a0a  rns the client..
+00017690: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+000176a0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+000176b0: 616c 2e6d 6169 6e2e 706c 7567 5f73 656c  al.main.plug_sel
+000176c0: 2e72 6563 6f72 645f 6368 6f73 656e 5f70  .record_chosen_p
+000176d0: 6c75 6769 6e73 2729 0a20 2020 2040 6d6f  lugins').    @mo
+000176e0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+000176f0: 742e 5f69 6e74 6572 6e61 6c2e 6365 7274  t._internal.cert
+00017700: 5f6d 616e 6167 6572 2e6c 696e 6561 6765  _manager.lineage
+00017710: 5f66 6f72 5f63 6572 746e 616d 6527 290a  _for_certname').
+00017720: 2020 2020 406d 6f63 6b2e 7061 7463 6828      @mock.patch(
+00017730: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+00017740: 616c 2e6d 6169 6e2e 6469 7370 6c61 795f  al.main.display_
+00017750: 6f70 732e 6368 6f6f 7365 5f76 616c 7565  ops.choose_value
+00017760: 7327 290a 2020 2020 406d 6f63 6b2e 7061  s').    @mock.pa
+00017770: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+00017780: 7465 726e 616c 2e6d 6169 6e2e 5f66 696e  ternal.main._fin
+00017790: 645f 646f 6d61 696e 735f 6f72 5f63 6572  d_domains_or_cer
+000177a0: 746e 616d 6527 290a 2020 2020 6465 6620  tname').    def 
+000177b0: 7465 7374 5f73 656c 6563 7469 6f6e 5f71  test_selection_q
+000177c0: 7565 7374 696f 6e28 7365 6c66 2c20 6d6f  uestion(self, mo
+000177d0: 636b 5f66 696e 642c 206d 6f63 6b5f 6368  ck_find, mock_ch
+000177e0: 6f6f 7365 2c20 6d6f 636b 5f6c 696e 6561  oose, mock_linea
+000177f0: 6765 2c20 5f72 6563 293a 0a20 2020 2020  ge, _rec):.     
+00017800: 2020 206d 6f63 6b5f 6c69 6e65 6167 652e     mock_lineage.
+00017810: 7265 7475 726e 5f76 616c 7565 203d 206d  return_value = m
+00017820: 6f63 6b2e 4d61 6769 634d 6f63 6b28 6368  ock.MagicMock(ch
+00017830: 6169 6e5f 7061 7468 3d22 2f74 6d70 2f6e  ain_path="/tmp/n
+00017840: 6f6e 6578 6973 7465 6e74 2229 0a20 2020  onexistent").   
+00017850: 2020 2020 206d 6f63 6b5f 6368 6f6f 7365       mock_choose
+00017860: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00017870: 5b27 6578 616d 706c 652e 636f 6d27 5d0a  ['example.com'].
+00017880: 2020 2020 2020 2020 6d6f 636b 5f66 696e          mock_fin
+00017890: 642e 7265 7475 726e 5f76 616c 7565 203d  d.return_value =
+000178a0: 2028 4e6f 6e65 2c20 4e6f 6e65 290a 2020   (None, None).  
+000178b0: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
+000178c0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+000178d0: 696e 7465 726e 616c 2e6d 6169 6e2e 706c  internal.main.pl
+000178e0: 7567 5f73 656c 2e70 6963 6b5f 696e 7374  ug_sel.pick_inst
+000178f0: 616c 6c65 7227 2920 6173 206d 6f63 6b5f  aller') as mock_
+00017900: 7069 636b 3a0a 2020 2020 2020 2020 2020  pick:.          
+00017910: 2020 7365 6c66 2e5f 6361 6c6c 285b 2765    self._call(['e
+00017920: 6e68 616e 6365 272c 2027 2d2d 7265 6469  nhance', '--redi
+00017930: 7265 6374 275d 290a 2020 2020 2020 2020  rect']).        
+00017940: 2020 2020 6173 7365 7274 206d 6f63 6b5f      assert mock_
+00017950: 7069 636b 2e63 616c 6c65 640a 2020 2020  pick.called.    
+00017960: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00017970: 7468 6174 2074 6865 206d 6573 7361 6765  that the message
+00017980: 2069 6e63 6c75 6465 7320 2265 6e68 616e   includes "enhan
+00017990: 6365 6d65 6e74 7322 0a20 2020 2020 2020  cements".       
+000179a0: 2020 2020 2061 7373 6572 7420 2265 6e68       assert "enh
+000179b0: 616e 6365 6d65 6e74 7322 2069 6e20 6d6f  ancements" in mo
+000179c0: 636b 5f70 6963 6b2e 6361 6c6c 5f61 7267  ck_pick.call_arg
+000179d0: 735b 305d 5b33 5d0a 0a20 2020 2040 6d6f  s[0][3]..    @mo
+000179e0: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+000179f0: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+00017a00: 2e70 6c75 675f 7365 6c2e 7265 636f 7264  .plug_sel.record
+00017a10: 5f63 686f 7365 6e5f 706c 7567 696e 7327  _chosen_plugins'
+00017a20: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00017a30: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00017a40: 726e 616c 2e63 6572 745f 6d61 6e61 6765  rnal.cert_manage
+00017a50: 722e 6c69 6e65 6167 655f 666f 725f 6365  r.lineage_for_ce
+00017a60: 7274 6e61 6d65 2729 0a20 2020 2040 6d6f  rtname').    @mo
+00017a70: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+00017a80: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+00017a90: 2e64 6973 706c 6179 5f6f 7073 2e63 686f  .display_ops.cho
+00017aa0: 6f73 655f 7661 6c75 6573 2729 0a20 2020  ose_values').   
+00017ab0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+00017ac0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00017ad0: 6d61 696e 2e5f 6669 6e64 5f64 6f6d 6169  main._find_domai
+00017ae0: 6e73 5f6f 725f 6365 7274 6e61 6d65 2729  ns_or_certname')
+00017af0: 0a20 2020 2064 6566 2074 6573 745f 7365  .    def test_se
+00017b00: 6c65 6374 696f 6e5f 6175 7468 5f77 6172  lection_auth_war
+00017b10: 6e69 6e67 2873 656c 662c 206d 6f63 6b5f  ning(self, mock_
+00017b20: 6669 6e64 2c20 6d6f 636b 5f63 686f 6f73  find, mock_choos
+00017b30: 652c 206d 6f63 6b5f 6c69 6e65 6167 652c  e, mock_lineage,
+00017b40: 205f 7265 6329 3a0a 2020 2020 2020 2020   _rec):.        
+00017b50: 6d6f 636b 5f6c 696e 6561 6765 2e72 6574  mock_lineage.ret
+00017b60: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
+00017b70: 2e4d 6167 6963 4d6f 636b 2863 6861 696e  .MagicMock(chain
+00017b80: 5f70 6174 683d 222f 746d 702f 6e6f 6e65  _path="/tmp/none
+00017b90: 7869 7374 656e 7422 290a 2020 2020 2020  xistent").      
+00017ba0: 2020 6d6f 636b 5f63 686f 6f73 652e 7265    mock_choose.re
+00017bb0: 7475 726e 5f76 616c 7565 203d 205b 2265  turn_value = ["e
+00017bc0: 7861 6d70 6c65 2e63 6f6d 225d 0a20 2020  xample.com"].   
+00017bd0: 2020 2020 206d 6f63 6b5f 6669 6e64 2e72       mock_find.r
+00017be0: 6574 7572 6e5f 7661 6c75 6520 3d20 284e  eturn_value = (N
+00017bf0: 6f6e 652c 204e 6f6e 6529 0a20 2020 2020  one, None).     
+00017c00: 2020 2077 6974 6820 6d6f 636b 2e70 6174     with mock.pat
+00017c10: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+00017c20: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
+00017c30: 7365 6c2e 7069 636b 5f69 6e73 7461 6c6c  sel.pick_install
+00017c40: 6572 2729 3a0a 2020 2020 2020 2020 2020  er'):.          
+00017c50: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+00017c60: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00017c70: 726e 616c 2e6d 6169 6e2e 706c 7567 5f73  rnal.main.plug_s
+00017c80: 656c 2e6c 6f67 6765 722e 7761 726e 696e  el.logger.warnin
+00017c90: 6727 2920 6173 206d 6f63 6b5f 6c6f 673a  g') as mock_log:
+00017ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017cb0: 206d 6f63 6b5f 636c 6965 6e74 203d 2073   mock_client = s
+00017cc0: 656c 662e 5f63 616c 6c28 5b27 656e 6861  elf._call(['enha
+00017cd0: 6e63 6527 2c20 272d 6127 2c20 2777 6562  nce', '-a', 'web
+00017ce0: 726f 6f74 272c 2027 2d2d 7265 6469 7265  root', '--redire
+00017cf0: 6374 275d 290a 2020 2020 2020 2020 2020  ct']).          
+00017d00: 2020 2020 2020 6173 7365 7274 206d 6f63        assert moc
+00017d10: 6b5f 6c6f 672e 6361 6c6c 6564 0a20 2020  k_log.called.   
+00017d20: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00017d30: 6572 7420 226d 616b 6520 7365 6e73 6522  ert "make sense"
+00017d40: 2069 6e20 6d6f 636b 5f6c 6f67 2e63 616c   in mock_log.cal
+00017d50: 6c5f 6172 6773 5b30 5d5b 305d 0a20 2020  l_args[0][0].   
+00017d60: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00017d70: 6572 7420 6d6f 636b 5f63 6c69 656e 742e  ert mock_client.
+00017d80: 656e 6861 6e63 655f 636f 6e66 6967 2e63  enhance_config.c
+00017d90: 616c 6c65 640a 0a20 2020 2040 6d6f 636b  alled..    @mock
+00017da0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+00017db0: 5f69 6e74 6572 6e61 6c2e 6365 7274 5f6d  _internal.cert_m
+00017dc0: 616e 6167 6572 2e6c 696e 6561 6765 5f66  anager.lineage_f
+00017dd0: 6f72 5f63 6572 746e 616d 6527 290a 2020  or_certname').  
+00017de0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+00017df0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00017e00: 2e6d 6169 6e2e 6469 7370 6c61 795f 6f70  .main.display_op
+00017e10: 732e 6368 6f6f 7365 5f76 616c 7565 7327  s.choose_values'
+00017e20: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00017e30: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00017e40: 726e 616c 2e6d 6169 6e2e 706c 7567 5f73  rnal.main.plug_s
+00017e50: 656c 2e72 6563 6f72 645f 6368 6f73 656e  el.record_chosen
+00017e60: 5f70 6c75 6769 6e73 2729 0a20 2020 2064  _plugins').    d
+00017e70: 6566 2074 6573 745f 656e 6861 6e63 655f  ef test_enhance_
+00017e80: 636f 6e66 6967 5f63 616c 6c28 7365 6c66  config_call(self
+00017e90: 2c20 5f72 6563 2c20 6d6f 636b 5f63 686f  , _rec, mock_cho
+00017ea0: 6f73 652c 206d 6f63 6b5f 6c69 6e65 6167  ose, mock_lineag
+00017eb0: 6529 3a0a 2020 2020 2020 2020 6d6f 636b  e):.        mock
+00017ec0: 5f6c 696e 6561 6765 2e72 6574 7572 6e5f  _lineage.return_
+00017ed0: 7661 6c75 6520 3d20 6d6f 636b 2e4d 6167  value = mock.Mag
+00017ee0: 6963 4d6f 636b 2863 6861 696e 5f70 6174  icMock(chain_pat
+00017ef0: 683d 222f 746d 702f 6e6f 6e65 7869 7374  h="/tmp/nonexist
+00017f00: 656e 7422 290a 2020 2020 2020 2020 6d6f  ent").        mo
+00017f10: 636b 5f63 686f 6f73 652e 7265 7475 726e  ck_choose.return
+00017f20: 5f76 616c 7565 203d 205b 2265 7861 6d70  _value = ["examp
+00017f30: 6c65 2e63 6f6d 225d 0a20 2020 2020 2020  le.com"].       
+00017f40: 2077 6974 6820 6d6f 636b 2e70 6174 6368   with mock.patch
+00017f50: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00017f60: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
+00017f70: 6c2e 7069 636b 5f69 6e73 7461 6c6c 6572  l.pick_installer
+00017f80: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00017f90: 6d6f 636b 5f63 6c69 656e 7420 3d20 7365  mock_client = se
+00017fa0: 6c66 2e5f 6361 6c6c 285b 2765 6e68 616e  lf._call(['enhan
+00017fb0: 6365 272c 2027 2d2d 7265 6469 7265 6374  ce', '--redirect
+00017fc0: 272c 2027 2d2d 6873 7473 275d 290a 2020  ', '--hsts']).  
+00017fd0: 2020 2020 2020 2020 2020 7265 715f 656e            req_en
+00017fe0: 6820 3d20 5b22 7265 6469 7265 6374 222c  h = ["redirect",
+00017ff0: 2022 6873 7473 225d 0a20 2020 2020 2020   "hsts"].       
+00018000: 2020 2020 206e 6f74 5f72 6571 5f65 6e68       not_req_enh
+00018010: 203d 205b 2275 6972 225d 0a20 2020 2020   = ["uir"].     
+00018020: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
+00018030: 636b 5f63 6c69 656e 742e 656e 6861 6e63  ck_client.enhanc
+00018040: 655f 636f 6e66 6967 2e63 616c 6c65 640a  e_config.called.
+00018050: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00018060: 7274 2061 6c6c 2867 6574 6174 7472 286d  rt all(getattr(m
+00018070: 6f63 6b5f 636c 6965 6e74 2e63 6f6e 6669  ock_client.confi
+00018080: 672c 2065 2920 666f 7220 6520 696e 2072  g, e) for e in r
+00018090: 6571 5f65 6e68 290a 2020 2020 2020 2020  eq_enh).        
+000180a0: 2020 2020 6173 7365 7274 206e 6f74 2061      assert not a
+000180b0: 6e79 2867 6574 6174 7472 286d 6f63 6b5f  ny(getattr(mock_
+000180c0: 636c 6965 6e74 2e63 6f6e 6669 672c 2065  client.config, e
+000180d0: 2920 666f 7220 6520 696e 206e 6f74 5f72  ) for e in not_r
+000180e0: 6571 5f65 6e68 290a 2020 2020 2020 2020  eq_enh).        
+000180f0: 2020 2020 6173 7365 7274 2022 6578 616d      assert "exam
+00018100: 706c 652e 636f 6d22 2069 6e20 6d6f 636b  ple.com" in mock
+00018110: 5f63 6c69 656e 742e 656e 6861 6e63 655f  _client.enhance_
+00018120: 636f 6e66 6967 2e63 616c 6c5f 6172 6773  config.call_args
+00018130: 5b30 5d5b 305d 0a0a 2020 2020 406d 6f63  [0][0]..    @moc
+00018140: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+00018150: 2e5f 696e 7465 726e 616c 2e63 6572 745f  ._internal.cert_
+00018160: 6d61 6e61 6765 722e 6c69 6e65 6167 655f  manager.lineage_
+00018170: 666f 725f 6365 7274 6e61 6d65 2729 0a20  for_certname'). 
+00018180: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+00018190: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+000181a0: 6c2e 6d61 696e 2e64 6973 706c 6179 5f6f  l.main.display_o
+000181b0: 7073 2e63 686f 6f73 655f 7661 6c75 6573  ps.choose_values
+000181c0: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
+000181d0: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+000181e0: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
+000181f0: 7365 6c2e 7265 636f 7264 5f63 686f 7365  sel.record_chose
+00018200: 6e5f 706c 7567 696e 7327 290a 2020 2020  n_plugins').    
+00018210: 6465 6620 7465 7374 5f65 6e68 616e 6365  def test_enhance
+00018220: 5f6e 6f6e 696e 7465 7261 6374 6976 6528  _noninteractive(
+00018230: 7365 6c66 2c20 5f72 6563 2c20 6d6f 636b  self, _rec, mock
+00018240: 5f63 686f 6f73 652c 206d 6f63 6b5f 6c69  _choose, mock_li
+00018250: 6e65 6167 6529 3a0a 2020 2020 2020 2020  neage):.        
+00018260: 6d6f 636b 5f6c 696e 6561 6765 2e72 6574  mock_lineage.ret
+00018270: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
+00018280: 2e4d 6167 6963 4d6f 636b 280a 2020 2020  .MagicMock(.    
+00018290: 2020 2020 2020 2020 6368 6169 6e5f 7061          chain_pa
+000182a0: 7468 3d22 2f74 6d70 2f6e 6f6e 6578 6973  th="/tmp/nonexis
+000182b0: 7465 6e74 2229 0a20 2020 2020 2020 206d  tent").        m
+000182c0: 6f63 6b5f 6368 6f6f 7365 2e72 6574 7572  ock_choose.retur
+000182d0: 6e5f 7661 6c75 6520 3d20 5b22 6578 616d  n_value = ["exam
+000182e0: 706c 652e 636f 6d22 5d0a 2020 2020 2020  ple.com"].      
+000182f0: 2020 7769 7468 206d 6f63 6b2e 7061 7463    with mock.patc
+00018300: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00018310: 726e 616c 2e6d 6169 6e2e 706c 7567 5f73  rnal.main.plug_s
+00018320: 656c 2e70 6963 6b5f 696e 7374 616c 6c65  el.pick_installe
+00018330: 7227 293a 0a20 2020 2020 2020 2020 2020  r'):.           
+00018340: 206d 6f63 6b5f 636c 6965 6e74 203d 2073   mock_client = s
+00018350: 656c 662e 5f63 616c 6c28 5b27 656e 6861  elf._call(['enha
+00018360: 6e63 6527 2c20 272d 2d72 6564 6972 6563  nce', '--redirec
+00018370: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018390: 2020 2020 2020 2020 2020 272d 2d68 7374            '--hst
+000183a0: 7327 2c20 272d 2d6e 6f6e 2d69 6e74 6572  s', '--non-inter
+000183b0: 6163 7469 7665 275d 290a 2020 2020 2020  active']).      
+000183c0: 2020 2020 2020 6173 7365 7274 206d 6f63        assert moc
+000183d0: 6b5f 636c 6965 6e74 2e65 6e68 616e 6365  k_client.enhance
+000183e0: 5f63 6f6e 6669 672e 6361 6c6c 6564 0a20  _config.called. 
+000183f0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00018400: 7420 6d6f 636b 5f63 686f 6f73 652e 6361  t mock_choose.ca
+00018410: 6c6c 6564 2069 7320 4661 6c73 650a 0a20  lled is False.. 
+00018420: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+00018430: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00018440: 6c2e 6d61 696e 2e64 6973 706c 6179 5f6f  l.main.display_o
+00018450: 7073 2e63 686f 6f73 655f 7661 6c75 6573  ps.choose_values
+00018460: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
+00018470: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+00018480: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
+00018490: 7365 6c2e 7265 636f 7264 5f63 686f 7365  sel.record_chose
+000184a0: 6e5f 706c 7567 696e 7327 290a 2020 2020  n_plugins').    
+000184b0: 6465 6620 7465 7374 5f75 7365 725f 6162  def test_user_ab
+000184c0: 6f72 745f 646f 6d61 696e 7328 7365 6c66  ort_domains(self
+000184d0: 2c20 5f72 6563 2c20 6d6f 636b 5f63 686f  , _rec, mock_cho
+000184e0: 6f73 6529 3a0a 2020 2020 2020 2020 6d6f  ose):.        mo
+000184f0: 636b 5f63 686f 6f73 652e 7265 7475 726e  ck_choose.return
+00018500: 5f76 616c 7565 203d 205b 5d0a 2020 2020  _value = [].    
+00018510: 2020 2020 7769 7468 206d 6f63 6b2e 7061      with mock.pa
+00018520: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+00018530: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
+00018540: 5f73 656c 2e70 6963 6b5f 696e 7374 616c  _sel.pick_instal
+00018550: 6c65 7227 293a 0a20 2020 2020 2020 2020  ler'):.         
+00018560: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+00018570: 6169 7365 7328 6572 726f 7273 2e45 7272  aises(errors.Err
+00018580: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00018590: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
+000185a0: 5b27 656e 6861 6e63 6527 2c20 272d 2d72  ['enhance', '--r
+000185b0: 6564 6972 6563 7427 2c20 272d 2d68 7374  edirect', '--hst
+000185c0: 7327 5d29 0a0a 2020 2020 6465 6620 7465  s'])..    def te
+000185d0: 7374 5f6e 6f5f 656e 6861 6e63 656d 656e  st_no_enhancemen
+000185e0: 7473 5f64 6566 696e 6564 2873 656c 6629  ts_defined(self)
+000185f0: 3a0a 2020 2020 2020 2020 7769 7468 2070  :.        with p
+00018600: 7974 6573 742e 7261 6973 6573 2865 7272  ytest.raises(err
+00018610: 6f72 732e 4d69 7363 6f6e 6669 6775 7261  ors.Misconfigura
+00018620: 7469 6f6e 4572 726f 7229 3a0a 2020 2020  tionError):.    
+00018630: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+00018640: 6c6c 285b 2765 6e68 616e 6365 272c 2027  ll(['enhance', '
+00018650: 2d61 272c 2027 6e75 6c6c 275d 290a 0a20  -a', 'null']).. 
+00018660: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+00018670: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+00018680: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
+00018690: 6368 6f6f 7365 5f63 6f6e 6669 6775 7261  choose_configura
+000186a0: 746f 725f 706c 7567 696e 7327 290a 2020  tor_plugins').  
+000186b0: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+000186c0: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+000186d0: 2e6d 6169 6e2e 6469 7370 6c61 795f 6f70  .main.display_op
+000186e0: 732e 6368 6f6f 7365 5f76 616c 7565 7327  s.choose_values'
+000186f0: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00018700: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00018710: 726e 616c 2e6d 6169 6e2e 706c 7567 5f73  rnal.main.plug_s
+00018720: 656c 2e72 6563 6f72 645f 6368 6f73 656e  el.record_chosen
+00018730: 5f70 6c75 6769 6e73 2729 0a20 2020 2064  _plugins').    d
+00018740: 6566 2074 6573 745f 706c 7567 696e 5f73  ef test_plugin_s
+00018750: 656c 6563 7469 6f6e 5f65 7272 6f72 2873  election_error(s
+00018760: 656c 662c 205f 7265 632c 206d 6f63 6b5f  elf, _rec, mock_
+00018770: 6368 6f6f 7365 2c20 6d6f 636b 5f70 6963  choose, mock_pic
+00018780: 6b29 3a0a 2020 2020 2020 2020 6d6f 636b  k):.        mock
+00018790: 5f63 686f 6f73 652e 7265 7475 726e 5f76  _choose.return_v
+000187a0: 616c 7565 203d 205b 2265 7861 6d70 6c65  alue = ["example
+000187b0: 2e63 6f6d 225d 0a20 2020 2020 2020 206d  .com"].        m
+000187c0: 6f63 6b5f 7069 636b 2e72 6574 7572 6e5f  ock_pick.return_
+000187d0: 7661 6c75 6520 3d20 284e 6f6e 652c 204e  value = (None, N
+000187e0: 6f6e 6529 0a20 2020 2020 2020 206d 6f63  one).        moc
+000187f0: 6b5f 7069 636b 2e73 6964 655f 6566 6665  k_pick.side_effe
+00018800: 6374 203d 2065 7272 6f72 732e 506c 7567  ct = errors.Plug
+00018810: 696e 5365 6c65 6374 696f 6e45 7272 6f72  inSelectionError
+00018820: 2829 0a20 2020 2020 2020 206d 6f63 6b5f  ().        mock_
+00018830: 636c 6965 6e74 203d 2073 656c 662e 5f63  client = self._c
+00018840: 616c 6c28 5b27 656e 6861 6e63 6527 2c20  all(['enhance', 
+00018850: 272d 2d68 7374 7327 5d29 0a20 2020 2020  '--hsts']).     
+00018860: 2020 2061 7373 6572 7420 6d6f 636b 5f63     assert mock_c
+00018870: 6c69 656e 742e 656e 6861 6e63 655f 636f  lient.enhance_co
+00018880: 6e66 6967 2e63 616c 6c65 6420 6973 2046  nfig.called is F
+00018890: 616c 7365 0a0a 2020 2020 406d 6f63 6b2e  alse..    @mock.
+000188a0: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+000188b0: 696e 7465 726e 616c 2e63 6572 745f 6d61  internal.cert_ma
+000188c0: 6e61 6765 722e 6c69 6e65 6167 655f 666f  nager.lineage_fo
+000188d0: 725f 6365 7274 6e61 6d65 2729 0a20 2020  r_certname').   
+000188e0: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+000188f0: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+00018900: 6d61 696e 2e64 6973 706c 6179 5f6f 7073  main.display_ops
+00018910: 2e63 686f 6f73 655f 7661 6c75 6573 2729  .choose_values')
+00018920: 0a20 2020 2040 6d6f 636b 2e70 6174 6368  .    @mock.patch
+00018930: 2827 6365 7274 626f 742e 5f69 6e74 6572  ('certbot._inter
+00018940: 6e61 6c2e 6d61 696e 2e70 6c75 675f 7365  nal.main.plug_se
+00018950: 6c2e 7069 636b 5f69 6e73 7461 6c6c 6572  l.pick_installer
+00018960: 2729 0a20 2020 2040 6d6f 636b 2e70 6174  ').    @mock.pat
+00018970: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+00018980: 6572 6e61 6c2e 6d61 696e 2e70 6c75 675f  ernal.main.plug_
+00018990: 7365 6c2e 7265 636f 7264 5f63 686f 7365  sel.record_chose
+000189a0: 6e5f 706c 7567 696e 7327 290a 2020 2020  n_plugins').    
+000189b0: 4074 6573 745f 7574 696c 2e70 6174 6368  @test_util.patch
+000189c0: 5f64 6973 706c 6179 5f75 7469 6c28 290a  _display_util().
+000189d0: 2020 2020 6465 6620 7465 7374 5f65 6e68      def test_enh
+000189e0: 616e 6365 6d65 6e74 5f65 6e61 626c 6528  ancement_enable(
+000189f0: 7365 6c66 2c20 5f2c 205f 7265 632c 206d  self, _, _rec, m
+00018a00: 6f63 6b5f 696e 7374 2c20 6d6f 636b 5f63  ock_inst, mock_c
+00018a10: 686f 6f73 652c 206d 6f63 6b5f 6c69 6e65  hoose, mock_line
+00018a20: 6167 6529 3a0a 2020 2020 2020 2020 6d6f  age):.        mo
+00018a30: 636b 5f69 6e73 742e 7265 7475 726e 5f76  ck_inst.return_v
+00018a40: 616c 7565 203d 2073 656c 662e 6d6f 636b  alue = self.mock
+00018a50: 696e 7374 616c 6c65 720a 2020 2020 2020  installer.      
+00018a60: 2020 6d6f 636b 5f63 686f 6f73 652e 7265    mock_choose.re
+00018a70: 7475 726e 5f76 616c 7565 203d 205b 2265  turn_value = ["e
+00018a80: 7861 6d70 6c65 2e63 6f6d 222c 2022 616e  xample.com", "an
+00018a90: 6f74 6865 722e 746c 6422 5d0a 2020 2020  other.tld"].    
+00018aa0: 2020 2020 6d6f 636b 5f6c 696e 6561 6765      mock_lineage
+00018ab0: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00018ac0: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2863  mock.MagicMock(c
+00018ad0: 6861 696e 5f70 6174 683d 222f 746d 702f  hain_path="/tmp/
+00018ae0: 6e6f 6e65 7869 7374 656e 7422 290a 2020  nonexistent").  
+00018af0: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
+00018b00: 285b 2765 6e68 616e 6365 272c 2027 2d2d  (['enhance', '--
+00018b10: 6175 746f 2d68 7374 7327 5d29 0a20 2020  auto-hsts']).   
+00018b20: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+00018b30: 2e6d 6f63 6b69 6e73 7461 6c6c 6572 2e65  .mockinstaller.e
+00018b40: 6e61 626c 655f 6175 746f 6873 7473 2e63  nable_autohsts.c
+00018b50: 616c 6c65 640a 2020 2020 2020 2020 6173  alled.        as
+00018b60: 7365 7274 2073 656c 662e 6d6f 636b 696e  sert self.mockin
+00018b70: 7374 616c 6c65 722e 656e 6162 6c65 5f61  staller.enable_a
+00018b80: 7574 6f68 7374 732e 6361 6c6c 5f61 7267  utohsts.call_arg
+00018b90: 735b 305d 5b31 5d20 3d3d 205c 0a20 2020  s[0][1] == \.   
+00018ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bb0: 2020 2020 2020 205b 2265 7861 6d70 6c65         ["example
+00018bc0: 2e63 6f6d 222c 2022 616e 6f74 6865 722e  .com", "another.
+00018bd0: 746c 6422 5d0a 0a20 2020 2040 6d6f 636b  tld"]..    @mock
+00018be0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+00018bf0: 5f69 6e74 6572 6e61 6c2e 6365 7274 5f6d  _internal.cert_m
+00018c00: 616e 6167 6572 2e6c 696e 6561 6765 5f66  anager.lineage_f
+00018c10: 6f72 5f63 6572 746e 616d 6527 290a 2020  or_certname').  
+00018c20: 2020 406d 6f63 6b2e 7061 7463 6828 2763    @mock.patch('c
+00018c30: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00018c40: 2e6d 6169 6e2e 6469 7370 6c61 795f 6f70  .main.display_op
+00018c50: 732e 6368 6f6f 7365 5f76 616c 7565 7327  s.choose_values'
+00018c60: 290a 2020 2020 406d 6f63 6b2e 7061 7463  ).    @mock.patc
+00018c70: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00018c80: 726e 616c 2e6d 6169 6e2e 706c 7567 5f73  rnal.main.plug_s
+00018c90: 656c 2e70 6963 6b5f 696e 7374 616c 6c65  el.pick_installe
+00018ca0: 7227 290a 2020 2020 406d 6f63 6b2e 7061  r').    @mock.pa
+00018cb0: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+00018cc0: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
+00018cd0: 5f73 656c 2e72 6563 6f72 645f 6368 6f73  _sel.record_chos
+00018ce0: 656e 5f70 6c75 6769 6e73 2729 0a20 2020  en_plugins').   
+00018cf0: 2040 7465 7374 5f75 7469 6c2e 7061 7463   @test_util.patc
+00018d00: 685f 6469 7370 6c61 795f 7574 696c 2829  h_display_util()
+00018d10: 0a20 2020 2064 6566 2074 6573 745f 656e  .    def test_en
+00018d20: 6861 6e63 656d 656e 745f 656e 6162 6c65  hancement_enable
+00018d30: 5f6e 6f74 5f73 7570 706f 7274 6564 2873  _not_supported(s
+00018d40: 656c 662c 205f 2c20 5f72 6563 2c20 6d6f  elf, _, _rec, mo
+00018d50: 636b 5f69 6e73 742c 206d 6f63 6b5f 6368  ck_inst, mock_ch
+00018d60: 6f6f 7365 2c20 6d6f 636b 5f6c 696e 6561  oose, mock_linea
+00018d70: 6765 293a 0a20 2020 2020 2020 206d 6f63  ge):.        moc
+00018d80: 6b5f 696e 7374 2e72 6574 7572 6e5f 7661  k_inst.return_va
+00018d90: 6c75 6520 3d20 6e75 6c6c 2e49 6e73 7461  lue = null.Insta
+00018da0: 6c6c 6572 2873 656c 662e 636f 6e66 6967  ller(self.config
+00018db0: 2c20 226e 756c 6c22 290a 2020 2020 2020  , "null").      
+00018dc0: 2020 6d6f 636b 5f63 686f 6f73 652e 7265    mock_choose.re
+00018dd0: 7475 726e 5f76 616c 7565 203d 205b 2265  turn_value = ["e
+00018de0: 7861 6d70 6c65 2e63 6f6d 222c 2022 616e  xample.com", "an
+00018df0: 6f74 6865 722e 746c 6422 5d0a 2020 2020  other.tld"].    
+00018e00: 2020 2020 6d6f 636b 5f6c 696e 6561 6765      mock_lineage
+00018e10: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+00018e20: 6d6f 636b 2e4d 6167 6963 4d6f 636b 2863  mock.MagicMock(c
+00018e30: 6861 696e 5f70 6174 683d 222f 746d 702f  hain_path="/tmp/
+00018e40: 6e6f 6e65 7869 7374 656e 7422 290a 2020  nonexistent").  
+00018e50: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
+00018e60: 742e 7261 6973 6573 2865 7272 6f72 732e  t.raises(errors.
+00018e70: 4e6f 7453 7570 706f 7274 6564 4572 726f  NotSupportedErro
+00018e80: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00018e90: 7365 6c66 2e5f 6361 6c6c 285b 2765 6e68  self._call(['enh
+00018ea0: 616e 6365 272c 2027 2d2d 6175 746f 2d68  ance', '--auto-h
+00018eb0: 7374 7327 5d29 0a0a 2020 2020 6465 6620  sts'])..    def 
+00018ec0: 7465 7374 5f65 6e68 616e 6365 6d65 6e74  test_enhancement
+00018ed0: 5f65 6e61 626c 655f 636f 6e66 6c69 6374  _enable_conflict
+00018ee0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00018ef0: 7769 7468 2070 7974 6573 742e 7261 6973  with pytest.rais
+00018f00: 6573 2865 7272 6f72 732e 4572 726f 7229  es(errors.Error)
+00018f10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018f20: 6c66 2e5f 6361 6c6c 285b 2765 6e68 616e  lf._call(['enhan
+00018f30: 6365 272c 2027 2d2d 6175 746f 2d68 7374  ce', '--auto-hst
+00018f40: 7327 2c20 272d 2d68 7374 7327 5d29 0a0a  s', '--hsts'])..
+00018f50: 0a63 6c61 7373 2049 6e73 7461 6c6c 5465  .class InstallTe
+00018f60: 7374 2874 6573 745f 7574 696c 2e43 6f6e  st(test_util.Con
+00018f70: 6669 6754 6573 7443 6173 6529 3a0a 2020  figTestCase):.  
+00018f80: 2020 2222 2254 6573 7473 2066 6f72 2063    """Tests for c
+00018f90: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+00018fa0: 2e6d 6169 6e2e 696e 7374 616c 6c2e 2222  .main.install.""
+00018fb0: 220a 0a20 2020 2064 6566 2073 6574 5570  "..    def setUp
+00018fc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00018fd0: 7375 7065 7228 292e 7365 7455 7028 290a  super().setUp().
+00018fe0: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
+00018ff0: 6b69 6e73 7461 6c6c 6572 203d 206d 6f63  kinstaller = moc
+00019000: 6b2e 4d61 6769 634d 6f63 6b28 7370 6563  k.MagicMock(spec
+00019010: 3d65 6e68 616e 6365 6d65 6e74 732e 4175  =enhancements.Au
+00019020: 746f 4853 5453 456e 6861 6e63 656d 656e  toHSTSEnhancemen
+00019030: 7429 0a0a 2020 2020 406d 6f63 6b2e 7061  t)..    @mock.pa
+00019040: 7463 6828 2763 6572 7462 6f74 2e5f 696e  tch('certbot._in
+00019050: 7465 726e 616c 2e6d 6169 6e2e 706c 7567  ternal.main.plug
+00019060: 5f73 656c 2e72 6563 6f72 645f 6368 6f73  _sel.record_chos
+00019070: 656e 5f70 6c75 6769 6e73 2729 0a20 2020  en_plugins').   
+00019080: 2040 6d6f 636b 2e70 6174 6368 2827 6365   @mock.patch('ce
+00019090: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+000190a0: 6d61 696e 2e70 6c75 675f 7365 6c2e 7069  main.plug_sel.pi
+000190b0: 636b 5f69 6e73 7461 6c6c 6572 2729 0a20  ck_installer'). 
+000190c0: 2020 2064 6566 2074 6573 745f 696e 7374     def test_inst
+000190d0: 616c 6c5f 656e 6861 6e63 656d 656e 745f  all_enhancement_
+000190e0: 6e6f 745f 7375 7070 6f72 7465 6428 7365  not_supported(se
+000190f0: 6c66 2c20 6d6f 636b 5f69 6e73 742c 205f  lf, mock_inst, _
+00019100: 7265 6329 3a0a 2020 2020 2020 2020 6d6f  rec):.        mo
+00019110: 636b 5f69 6e73 742e 7265 7475 726e 5f76  ck_inst.return_v
+00019120: 616c 7565 203d 206e 756c 6c2e 496e 7374  alue = null.Inst
+00019130: 616c 6c65 7228 7365 6c66 2e63 6f6e 6669  aller(self.confi
+00019140: 672c 2022 6e75 6c6c 2229 0a20 2020 2020  g, "null").     
+00019150: 2020 2070 6c75 6769 6e73 203d 2064 6973     plugins = dis
+00019160: 636f 2e50 6c75 6769 6e73 5265 6769 7374  co.PluginsRegist
+00019170: 7279 2e66 696e 645f 616c 6c28 290a 2020  ry.find_all().  
+00019180: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00019190: 672e 6175 746f 5f68 7374 7320 3d20 5472  g.auto_hsts = Tr
+000191a0: 7565 0a20 2020 2020 2020 2073 656c 662e  ue.        self.
+000191b0: 636f 6e66 6967 2e63 6572 746e 616d 6520  config.certname 
+000191c0: 3d20 226e 6f6e 6578 6973 7465 6e74 220a  = "nonexistent".
+000191d0: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+000191e0: 6573 742e 7261 6973 6573 2865 7272 6f72  est.raises(error
+000191f0: 732e 4e6f 7453 7570 706f 7274 6564 4572  s.NotSupportedEr
+00019200: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00019210: 2020 6d61 696e 2e69 6e73 7461 6c6c 2873    main.install(s
+00019220: 656c 662e 636f 6e66 6967 2c20 706c 7567  elf.config, plug
+00019230: 696e 7329 0a0a 2020 2020 406d 6f63 6b2e  ins)..    @mock.
+00019240: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+00019250: 696e 7465 726e 616c 2e6d 6169 6e2e 706c  internal.main.pl
+00019260: 7567 5f73 656c 2e72 6563 6f72 645f 6368  ug_sel.record_ch
+00019270: 6f73 656e 5f70 6c75 6769 6e73 2729 0a20  osen_plugins'). 
+00019280: 2020 2040 6d6f 636b 2e70 6174 6368 2827     @mock.patch('
+00019290: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+000192a0: 6c2e 6d61 696e 2e70 6c75 675f 7365 6c2e  l.main.plug_sel.
+000192b0: 7069 636b 5f69 6e73 7461 6c6c 6572 2729  pick_installer')
+000192c0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
+000192d0: 7374 616c 6c5f 656e 6861 6e63 656d 656e  stall_enhancemen
+000192e0: 745f 6e6f 5f63 6572 746e 616d 6528 7365  t_no_certname(se
+000192f0: 6c66 2c20 6d6f 636b 5f69 6e73 742c 205f  lf, mock_inst, _
+00019300: 7265 6329 3a0a 2020 2020 2020 2020 6d6f  rec):.        mo
+00019310: 636b 5f69 6e73 742e 7265 7475 726e 5f76  ck_inst.return_v
+00019320: 616c 7565 203d 2073 656c 662e 6d6f 636b  alue = self.mock
+00019330: 696e 7374 616c 6c65 720a 2020 2020 2020  installer.      
+00019340: 2020 706c 7567 696e 7320 3d20 6469 7363    plugins = disc
+00019350: 6f2e 506c 7567 696e 7352 6567 6973 7472  o.PluginsRegistr
+00019360: 792e 6669 6e64 5f61 6c6c 2829 0a20 2020  y.find_all().   
+00019370: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
+00019380: 2e61 7574 6f5f 6873 7473 203d 2054 7275  .auto_hsts = Tru
+00019390: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
+000193a0: 6f6e 6669 672e 6365 7274 6e61 6d65 203d  onfig.certname =
+000193b0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+000193c0: 6c66 2e63 6f6e 6669 672e 6b65 795f 7061  lf.config.key_pa
+000193d0: 7468 203d 2022 2f74 6d70 2f6e 6f6e 6578  th = "/tmp/nonex
+000193e0: 6973 7465 6e74 220a 2020 2020 2020 2020  istent".        
+000193f0: 7365 6c66 2e63 6f6e 6669 672e 6365 7274  self.config.cert
+00019400: 5f70 6174 6820 3d20 222f 746d 702f 6e6f  _path = "/tmp/no
+00019410: 6e65 7869 7374 656e 7422 0a20 2020 2020  nexistent".     
+00019420: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+00019430: 6169 7365 7328 6572 726f 7273 2e43 6f6e  aises(errors.Con
+00019440: 6669 6775 7261 7469 6f6e 4572 726f 7229  figurationError)
+00019450: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+00019460: 696e 2e69 6e73 7461 6c6c 2873 656c 662e  in.install(self.
+00019470: 636f 6e66 6967 2c20 706c 7567 696e 7329  config, plugins)
+00019480: 0a0a 0a63 6c61 7373 2052 6570 6f72 744e  ...class ReportN
+00019490: 6577 4365 7274 5465 7374 2875 6e69 7474  ewCertTest(unitt
+000194a0: 6573 742e 5465 7374 4361 7365 293a 0a20  est.TestCase):. 
+000194b0: 2020 2022 2222 5465 7374 7320 666f 7220     """Tests for 
+000194c0: 6365 7274 626f 742e 5f69 6e74 6572 6e61  certbot._interna
+000194d0: 6c2e 6d61 696e 2e5f 7265 706f 7274 5f6e  l.main._report_n
+000194e0: 6577 5f63 6572 7420 616e 640a 2020 2020  ew_cert and.    
+000194f0: 2020 2063 6572 7462 6f74 2e5f 696e 7465     certbot._inte
+00019500: 726e 616c 2e6d 6169 6e2e 5f63 7372 5f72  rnal.main._csr_r
+00019510: 6570 6f72 745f 6e65 775f 6365 7274 2e0a  eport_new_cert..
+00019520: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+00019530: 2073 6574 5570 2873 656c 6629 3a0a 2020   setUp(self):.  
+00019540: 2020 2020 2020 7365 6c66 2e6e 6f74 6966        self.notif
+00019550: 795f 7061 7463 6820 3d20 6d6f 636b 2e70  y_patch = mock.p
+00019560: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+00019570: 6e74 6572 6e61 6c2e 6d61 696e 2e64 6973  nternal.main.dis
+00019580: 706c 6179 5f75 7469 6c2e 6e6f 7469 6679  play_util.notify
+00019590: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+000195a0: 6d6f 636b 5f6e 6f74 6966 7920 3d20 7365  mock_notify = se
+000195b0: 6c66 2e6e 6f74 6966 795f 7061 7463 682e  lf.notify_patch.
+000195c0: 7374 6172 7428 290a 0a20 2020 2020 2020  start()..       
+000195d0: 2073 656c 662e 6e6f 7461 6674 6572 5f70   self.notafter_p
+000195e0: 6174 6368 203d 206d 6f63 6b2e 7061 7463  atch = mock.patc
+000195f0: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+00019600: 726e 616c 2e6d 6169 6e2e 6372 7970 746f  rnal.main.crypto
+00019610: 5f75 7469 6c2e 6e6f 7441 6674 6572 2729  _util.notAfter')
+00019620: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+00019630: 636b 5f6e 6f74 6166 7465 7220 3d20 7365  ck_notafter = se
+00019640: 6c66 2e6e 6f74 6166 7465 725f 7061 7463  lf.notafter_patc
+00019650: 682e 7374 6172 7428 290a 2020 2020 2020  h.start().      
+00019660: 2020 7365 6c66 2e6d 6f63 6b5f 6e6f 7461    self.mock_nota
+00019670: 6674 6572 2e72 6574 7572 6e5f 7661 6c75  fter.return_valu
+00019680: 6520 3d20 6461 7465 7469 6d65 2e64 6174  e = datetime.dat
+00019690: 6574 696d 6528 3139 3730 2c20 312c 2031  etime(1970, 1, 1
+000196a0: 2c20 302c 2030 290a 0a20 2020 2064 6566  , 0, 0)..    def
+000196b0: 2074 6561 7244 6f77 6e28 7365 6c66 293a   tearDown(self):
+000196c0: 0a20 2020 2020 2020 2073 656c 662e 6e6f  .        self.no
+000196d0: 7469 6679 5f70 6174 6368 2e73 746f 7028  tify_patch.stop(
+000196e0: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+000196f0: 6f74 6166 7465 725f 7061 7463 682e 7374  otafter_patch.st
+00019700: 6f70 2829 0a0a 2020 2020 4063 6c61 7373  op()..    @class
+00019710: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
+00019720: 6361 6c6c 2863 6c73 2c20 2a61 7267 732c  call(cls, *args,
+00019730: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00019740: 2020 2020 6672 6f6d 2063 6572 7462 6f74      from certbot
+00019750: 2e5f 696e 7465 726e 616c 2e6d 6169 6e20  ._internal.main 
+00019760: 696d 706f 7274 205f 7265 706f 7274 5f6e  import _report_n
+00019770: 6577 5f63 6572 740a 2020 2020 2020 2020  ew_cert.        
+00019780: 7265 7475 726e 205f 7265 706f 7274 5f6e  return _report_n
+00019790: 6577 5f63 6572 7428 2a61 7267 732c 202a  ew_cert(*args, *
+000197a0: 2a6b 7761 7267 7329 0a0a 2020 2020 4063  *kwargs)..    @c
+000197b0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+000197c0: 6566 205f 6361 6c6c 5f63 7372 2863 6c73  ef _call_csr(cls
+000197d0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+000197e0: 7329 3a0a 2020 2020 2020 2020 6672 6f6d  s):.        from
+000197f0: 2063 6572 7462 6f74 2e5f 696e 7465 726e   certbot._intern
+00019800: 616c 2e6d 6169 6e20 696d 706f 7274 205f  al.main import _
+00019810: 6373 725f 7265 706f 7274 5f6e 6577 5f63  csr_report_new_c
+00019820: 6572 740a 2020 2020 2020 2020 7265 7475  ert.        retu
+00019830: 726e 205f 6373 725f 7265 706f 7274 5f6e  rn _csr_report_n
+00019840: 6577 5f63 6572 7428 2a61 7267 732c 202a  ew_cert(*args, *
+00019850: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00019860: 6620 7465 7374 5f72 6570 6f72 745f 6472  f test_report_dr
+00019870: 795f 7275 6e28 7365 6c66 293a 0a20 2020  y_run(self):.   
+00019880: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
+00019890: 6d6f 636b 2e4d 6f63 6b28 6472 795f 7275  mock.Mock(dry_ru
+000198a0: 6e3d 5472 7565 292c 204e 6f6e 652c 204e  n=True), None, N
+000198b0: 6f6e 652c 204e 6f6e 6529 0a20 2020 2020  one, None).     
+000198c0: 2020 2073 656c 662e 6d6f 636b 5f6e 6f74     self.mock_not
+000198d0: 6966 792e 6173 7365 7274 5f63 616c 6c65  ify.assert_calle
+000198e0: 645f 7769 7468 2822 5468 6520 6472 7920  d_with("The dry 
+000198f0: 7275 6e20 7761 7320 7375 6363 6573 7366  run was successf
+00019900: 756c 2e22 290a 0a20 2020 2064 6566 2074  ul.")..    def t
+00019910: 6573 745f 6373 725f 7265 706f 7274 5f64  est_csr_report_d
+00019920: 7279 5f72 756e 2873 656c 6629 3a0a 2020  ry_run(self):.  
+00019930: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
+00019940: 5f63 7372 286d 6f63 6b2e 4d6f 636b 2864  _csr(mock.Mock(d
+00019950: 7279 5f72 756e 3d54 7275 6529 2c20 4e6f  ry_run=True), No
+00019960: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 290a  ne, None, None).
+00019970: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
+00019980: 6b5f 6e6f 7469 6679 2e61 7373 6572 745f  k_notify.assert_
+00019990: 6361 6c6c 6564 5f77 6974 6828 2254 6865  called_with("The
+000199a0: 2064 7279 2072 756e 2077 6173 2073 7563   dry run was suc
+000199b0: 6365 7373 6675 6c2e 2229 0a0a 2020 2020  cessful.")..    
+000199c0: 6465 6620 7465 7374 5f72 6570 6f72 745f  def test_report_
+000199d0: 6e6f 5f70 6174 6873 2873 656c 6629 3a0a  no_paths(self):.
+000199e0: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+000199f0: 6573 742e 7261 6973 6573 2841 7373 6572  est.raises(Asser
+00019a00: 7469 6f6e 4572 726f 7229 3a0a 2020 2020  tionError):.    
+00019a10: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+00019a20: 6c6c 286d 6f63 6b2e 4d6f 636b 2864 7279  ll(mock.Mock(dry
+00019a30: 5f72 756e 3d46 616c 7365 292c 204e 6f6e  _run=False), Non
+00019a40: 652c 204e 6f6e 652c 204e 6f6e 6529 0a0a  e, None, None)..
+00019a50: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
+00019a60: 6573 742e 7261 6973 6573 2841 7373 6572  est.raises(Asser
+00019a70: 7469 6f6e 4572 726f 7229 3a0a 2020 2020  tionError):.    
+00019a80: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+00019a90: 6c6c 5f63 7372 286d 6f63 6b2e 4d6f 636b  ll_csr(mock.Mock
+00019aa0: 2864 7279 5f72 756e 3d46 616c 7365 292c  (dry_run=False),
+00019ab0: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
+00019ac0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
+00019ad0: 5f72 6570 6f72 7428 7365 6c66 293a 0a20  _report(self):. 
+00019ae0: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
+00019af0: 6c28 6d6f 636b 2e4d 6f63 6b28 6472 795f  l(mock.Mock(dry_
+00019b00: 7275 6e3d 4661 6c73 6529 2c0a 2020 2020  run=False),.    
+00019b10: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+00019b20: 7061 7468 2f74 6f2f 6365 7274 2e70 656d  path/to/cert.pem
+00019b30: 272c 2027 2f70 6174 682f 746f 2f66 756c  ', '/path/to/ful
+00019b40: 6c63 6861 696e 2e70 656d 272c 0a20 2020  lchain.pem',.   
+00019b50: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00019b60: 2f70 6174 682f 746f 2f70 7269 766b 6579  /path/to/privkey
+00019b70: 2e70 656d 2729 0a0a 2020 2020 2020 2020  .pem')..        
+00019b80: 7365 6c66 2e6d 6f63 6b5f 6e6f 7469 6679  self.mock_notify
+00019b90: 2e61 7373 6572 745f 6361 6c6c 6564 5f77  .assert_called_w
+00019ba0: 6974 6828 0a20 2020 2020 2020 2020 2020  ith(.           
+00019bb0: 2027 5c6e 5375 6363 6573 7366 756c 6c79   '\nSuccessfully
+00019bc0: 2072 6563 6569 7665 6420 6365 7274 6966   received certif
+00019bd0: 6963 6174 652e 5c6e 270a 2020 2020 2020  icate.\n'.      
+00019be0: 2020 2020 2020 2743 6572 7469 6669 6361        'Certifica
+00019bf0: 7465 2069 7320 7361 7665 6420 6174 3a20  te is saved at: 
+00019c00: 2f70 6174 682f 746f 2f66 756c 6c63 6861  /path/to/fullcha
+00019c10: 696e 2e70 656d 5c6e 270a 2020 2020 2020  in.pem\n'.      
+00019c20: 2020 2020 2020 274b 6579 2069 7320 7361        'Key is sa
+00019c30: 7665 6420 6174 3a20 2020 2020 2020 2020  ved at:         
+00019c40: 2f70 6174 682f 746f 2f70 7269 766b 6579  /path/to/privkey
+00019c50: 2e70 656d 5c6e 270a 2020 2020 2020 2020  .pem\n'.        
+00019c60: 2020 2020 2754 6869 7320 6365 7274 6966      'This certif
+00019c70: 6963 6174 6520 6578 7069 7265 7320 6f6e  icate expires on
+00019c80: 2031 3937 302d 3031 2d30 312e 5c6e 270a   1970-01-01.\n'.
+00019c90: 2020 2020 2020 2020 2020 2020 2754 6865              'The
+00019ca0: 7365 2066 696c 6573 2077 696c 6c20 6265  se files will be
+00019cb0: 2075 7064 6174 6564 2077 6865 6e20 7468   updated when th
+00019cc0: 6520 6365 7274 6966 6963 6174 6520 7265  e certificate re
+00019cd0: 6e65 7773 2e5c 6e27 0a20 2020 2020 2020  news.\n'.       
+00019ce0: 2020 2020 2027 4365 7274 626f 7420 6861       'Certbot ha
+00019cf0: 7320 7365 7420 7570 2061 2073 6368 6564  s set up a sched
+00019d00: 756c 6564 2074 6173 6b20 746f 2061 7574  uled task to aut
+00019d10: 6f6d 6174 6963 616c 6c79 2072 656e 6577  omatically renew
+00019d20: 2074 6869 7320 270a 2020 2020 2020 2020   this '.        
+00019d30: 2020 2020 2763 6572 7469 6669 6361 7465      'certificate
+00019d40: 2069 6e20 7468 6520 6261 636b 6772 6f75   in the backgrou
+00019d50: 6e64 2e27 0a20 2020 2020 2020 2029 0a0a  nd.'.        )..
+00019d60: 2020 2020 6465 6620 7465 7374 5f72 6570      def test_rep
+00019d70: 6f72 745f 6e6f 5f6b 6579 2873 656c 6629  ort_no_key(self)
+00019d80: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00019d90: 6361 6c6c 286d 6f63 6b2e 4d6f 636b 2864  call(mock.Mock(d
+00019da0: 7279 5f72 756e 3d46 616c 7365 292c 0a20  ry_run=False),. 
+00019db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dc0: 2027 2f70 6174 682f 746f 2f63 6572 742e   '/path/to/cert.
+00019dd0: 7065 6d27 2c20 272f 7061 7468 2f74 6f2f  pem', '/path/to/
+00019de0: 6675 6c6c 6368 6169 6e2e 7065 6d27 2c0a  fullchain.pem',.
+00019df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e00: 2020 4e6f 6e65 290a 0a20 2020 2020 2020    None)..       
+00019e10: 2073 656c 662e 6d6f 636b 5f6e 6f74 6966   self.mock_notif
+00019e20: 792e 6173 7365 7274 5f63 616c 6c65 645f  y.assert_called_
+00019e30: 7769 7468 280a 2020 2020 2020 2020 2020  with(.          
+00019e40: 2020 275c 6e53 7563 6365 7373 6675 6c6c    '\nSuccessfull
+00019e50: 7920 7265 6365 6976 6564 2063 6572 7469  y received certi
+00019e60: 6669 6361 7465 2e5c 6e27 0a20 2020 2020  ficate.\n'.     
+00019e70: 2020 2020 2020 2027 4365 7274 6966 6963         'Certific
+00019e80: 6174 6520 6973 2073 6176 6564 2061 743a  ate is saved at:
+00019e90: 202f 7061 7468 2f74 6f2f 6675 6c6c 6368   /path/to/fullch
+00019ea0: 6169 6e2e 7065 6d5c 6e27 0a20 2020 2020  ain.pem\n'.     
+00019eb0: 2020 2020 2020 2027 5468 6973 2063 6572         'This cer
+00019ec0: 7469 6669 6361 7465 2065 7870 6972 6573  tificate expires
+00019ed0: 206f 6e20 3139 3730 2d30 312d 3031 2e5c   on 1970-01-01.\
+00019ee0: 6e27 0a20 2020 2020 2020 2020 2020 2027  n'.            '
+00019ef0: 5468 6573 6520 6669 6c65 7320 7769 6c6c  These files will
+00019f00: 2062 6520 7570 6461 7465 6420 7768 656e   be updated when
+00019f10: 2074 6865 2063 6572 7469 6669 6361 7465   the certificate
+00019f20: 2072 656e 6577 732e 5c6e 270a 2020 2020   renews.\n'.    
+00019f30: 2020 2020 2020 2020 2743 6572 7462 6f74          'Certbot
+00019f40: 2068 6173 2073 6574 2075 7020 6120 7363   has set up a sc
+00019f50: 6865 6475 6c65 6420 7461 736b 2074 6f20  heduled task to 
+00019f60: 6175 746f 6d61 7469 6361 6c6c 7920 7265  automatically re
+00019f70: 6e65 7720 7468 6973 2027 0a20 2020 2020  new this '.     
+00019f80: 2020 2020 2020 2027 6365 7274 6966 6963         'certific
+00019f90: 6174 6520 696e 2074 6865 2062 6163 6b67  ate in the backg
+00019fa0: 726f 756e 642e 270a 2020 2020 2020 2020  round.'.        
+00019fb0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00019fc0: 7265 706f 7274 5f6e 6f5f 7072 6563 6f6e  report_no_precon
+00019fd0: 6669 6775 7265 645f 7265 6e65 7761 6c28  figured_renewal(
+00019fe0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00019ff0: 656c 662e 5f63 616c 6c28 6d6f 636b 2e4d  elf._call(mock.M
+0001a000: 6f63 6b28 6472 795f 7275 6e3d 4661 6c73  ock(dry_run=Fals
+0001a010: 652c 2070 7265 636f 6e66 6967 7572 6564  e, preconfigured
+0001a020: 5f72 656e 6577 616c 3d46 616c 7365 292c  _renewal=False),
+0001a030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a040: 2020 2027 2f70 6174 682f 746f 2f63 6572     '/path/to/cer
+0001a050: 742e 7065 6d27 2c20 272f 7061 7468 2f74  t.pem', '/path/t
+0001a060: 6f2f 6675 6c6c 6368 6169 6e2e 7065 6d27  o/fullchain.pem'
+0001a070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001a080: 2020 2020 272f 7061 7468 2f74 6f2f 7072      '/path/to/pr
+0001a090: 6976 6b65 792e 7065 6d27 290a 0a20 2020  ivkey.pem')..   
+0001a0a0: 2020 2020 2073 656c 662e 6d6f 636b 5f6e       self.mock_n
+0001a0b0: 6f74 6966 792e 6173 7365 7274 5f63 616c  otify.assert_cal
+0001a0c0: 6c65 645f 7769 7468 280a 2020 2020 2020  led_with(.      
+0001a0d0: 2020 2020 2020 275c 6e53 7563 6365 7373        '\nSuccess
+0001a0e0: 6675 6c6c 7920 7265 6365 6976 6564 2063  fully received c
+0001a0f0: 6572 7469 6669 6361 7465 2e5c 6e27 0a20  ertificate.\n'. 
+0001a100: 2020 2020 2020 2020 2020 2027 4365 7274             'Cert
+0001a110: 6966 6963 6174 6520 6973 2073 6176 6564  ificate is saved
+0001a120: 2061 743a 202f 7061 7468 2f74 6f2f 6675   at: /path/to/fu
+0001a130: 6c6c 6368 6169 6e2e 7065 6d5c 6e27 0a20  llchain.pem\n'. 
+0001a140: 2020 2020 2020 2020 2020 2027 4b65 7920             'Key 
+0001a150: 6973 2073 6176 6564 2061 743a 2020 2020  is saved at:    
+0001a160: 2020 2020 202f 7061 7468 2f74 6f2f 7072       /path/to/pr
+0001a170: 6976 6b65 792e 7065 6d5c 6e27 0a20 2020  ivkey.pem\n'.   
+0001a180: 2020 2020 2020 2020 2027 5468 6973 2063           'This c
+0001a190: 6572 7469 6669 6361 7465 2065 7870 6972  ertificate expir
+0001a1a0: 6573 206f 6e20 3139 3730 2d30 312d 3031  es on 1970-01-01
+0001a1b0: 2e5c 6e27 0a20 2020 2020 2020 2020 2020  .\n'.           
+0001a1c0: 2027 5468 6573 6520 6669 6c65 7320 7769   'These files wi
+0001a1d0: 6c6c 2062 6520 7570 6461 7465 6420 7768  ll be updated wh
+0001a1e0: 656e 2074 6865 2063 6572 7469 6669 6361  en the certifica
+0001a1f0: 7465 2072 656e 6577 732e 270a 2020 2020  te renews.'.    
+0001a200: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
+0001a210: 6573 745f 6373 725f 7265 706f 7274 2873  est_csr_report(s
+0001a220: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0001a230: 6c66 2e5f 6361 6c6c 5f63 7372 286d 6f63  lf._call_csr(moc
+0001a240: 6b2e 4d6f 636b 2864 7279 5f72 756e 3d46  k.Mock(dry_run=F
+0001a250: 616c 7365 292c 2027 2f70 6174 682f 746f  alse), '/path/to
+0001a260: 2f63 6572 742e 7065 6d27 2c0a 2020 2020  /cert.pem',.    
+0001a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a280: 2020 272f 7061 7468 2f74 6f2f 6368 6169    '/path/to/chai
+0001a290: 6e2e 7065 6d27 2c20 272f 7061 7468 2f74  n.pem', '/path/t
+0001a2a0: 6f2f 6675 6c6c 6368 6169 6e2e 7065 6d27  o/fullchain.pem'
+0001a2b0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0001a2c0: 6d6f 636b 5f6e 6f74 6966 792e 6173 7365  mock_notify.asse
+0001a2d0: 7274 5f63 616c 6c65 645f 7769 7468 280a  rt_called_with(.
+0001a2e0: 2020 2020 2020 2020 2020 2020 275c 6e53              '\nS
+0001a2f0: 7563 6365 7373 6675 6c6c 7920 7265 6365  uccessfully rece
+0001a300: 6976 6564 2063 6572 7469 6669 6361 7465  ived certificate
+0001a310: 2e5c 6e27 0a20 2020 2020 2020 2020 2020  .\n'.           
+0001a320: 2027 4365 7274 6966 6963 6174 6520 6973   'Certificate is
+0001a330: 2073 6176 6564 2061 743a 2020 2020 2020   saved at:      
+0001a340: 2020 2020 2020 2f70 6174 682f 746f 2f63        /path/to/c
+0001a350: 6572 742e 7065 6d5c 6e27 0a20 2020 2020  ert.pem\n'.     
+0001a360: 2020 2020 2020 2027 496e 7465 726d 6564         'Intermed
+0001a370: 6961 7465 2043 4120 6368 6169 6e20 6973  iate CA chain is
+0001a380: 2073 6176 6564 2061 743a 2020 2f70 6174   saved at:  /pat
+0001a390: 682f 746f 2f63 6861 696e 2e70 656d 5c6e  h/to/chain.pem\n
+0001a3a0: 270a 2020 2020 2020 2020 2020 2020 2746  '.            'F
+0001a3b0: 756c 6c20 6365 7274 6966 6963 6174 6520  ull certificate 
+0001a3c0: 6368 6169 6e20 6973 2073 6176 6564 2061  chain is saved a
+0001a3d0: 743a 202f 7061 7468 2f74 6f2f 6675 6c6c  t: /path/to/full
+0001a3e0: 6368 6169 6e2e 7065 6d5c 6e27 0a20 2020  chain.pem\n'.   
+0001a3f0: 2020 2020 2020 2020 2027 5468 6973 2063           'This c
+0001a400: 6572 7469 6669 6361 7465 2065 7870 6972  ertificate expir
+0001a410: 6573 206f 6e20 3139 3730 2d30 312d 3031  es on 1970-01-01
+0001a420: 2e27 0a20 2020 2020 2020 2029 0a0a 2020  .'.        )..  
+0001a430: 2020 6465 6620 7465 7374 5f6d 616e 7561    def test_manua
+0001a440: 6c5f 6e6f 5f68 6f6f 6b73 5f72 6570 6f72  l_no_hooks_repor
+0001a450: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001a460: 2022 2222 5368 6f75 6c64 6e27 7420 6765   """Shouldn't ge
+0001a470: 7420 6120 6d65 7373 6167 6520 6162 6f75  t a message abou
+0001a480: 7420 6175 746f 7265 6e65 7761 6c20 6966  t autorenewal if
+0001a490: 206e 6f20 2d2d 6d61 6e75 616c 2d61 7574   no --manual-aut
+0001a4a0: 682d 686f 6f6b 2222 220a 2020 2020 2020  h-hook""".      
+0001a4b0: 2020 7365 6c66 2e5f 6361 6c6c 286d 6f63    self._call(moc
+0001a4c0: 6b2e 4d6f 636b 2864 7279 5f72 756e 3d46  k.Mock(dry_run=F
+0001a4d0: 616c 7365 2c20 6175 7468 656e 7469 6361  alse, authentica
+0001a4e0: 746f 723d 276d 616e 7561 6c27 2c20 6d61  tor='manual', ma
+0001a4f0: 6e75 616c 5f61 7574 685f 686f 6f6b 3d4e  nual_auth_hook=N
+0001a500: 6f6e 6529 2c0a 2020 2020 2020 2020 2020  one),.          
+0001a510: 2020 2020 2020 2020 272f 7061 7468 2f74          '/path/t
+0001a520: 6f2f 6365 7274 2e70 656d 272c 2027 2f70  o/cert.pem', '/p
+0001a530: 6174 682f 746f 2f66 756c 6c63 6861 696e  ath/to/fullchain
+0001a540: 2e70 656d 272c 0a20 2020 2020 2020 2020  .pem',.         
+0001a550: 2020 2020 2020 2020 2027 2f70 6174 682f           '/path/
+0001a560: 746f 2f70 7269 766b 6579 2e70 656d 2729  to/privkey.pem')
+0001a570: 0a0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+0001a580: 6f63 6b5f 6e6f 7469 6679 2e61 7373 6572  ock_notify.asser
+0001a590: 745f 6361 6c6c 6564 5f77 6974 6828 0a20  t_called_with(. 
+0001a5a0: 2020 2020 2020 2020 2020 2027 5c6e 5375             '\nSu
+0001a5b0: 6363 6573 7366 756c 6c79 2072 6563 6569  ccessfully recei
+0001a5c0: 7665 6420 6365 7274 6966 6963 6174 652e  ved certificate.
+0001a5d0: 5c6e 270a 2020 2020 2020 2020 2020 2020  \n'.            
+0001a5e0: 2743 6572 7469 6669 6361 7465 2069 7320  'Certificate is 
+0001a5f0: 7361 7665 6420 6174 3a20 2f70 6174 682f  saved at: /path/
+0001a600: 746f 2f66 756c 6c63 6861 696e 2e70 656d  to/fullchain.pem
+0001a610: 5c6e 270a 2020 2020 2020 2020 2020 2020  \n'.            
+0001a620: 274b 6579 2069 7320 7361 7665 6420 6174  'Key is saved at
+0001a630: 3a20 2020 2020 2020 2020 2f70 6174 682f  :         /path/
+0001a640: 746f 2f70 7269 766b 6579 2e70 656d 5c6e  to/privkey.pem\n
+0001a650: 270a 2020 2020 2020 2020 2020 2020 2754  '.            'T
+0001a660: 6869 7320 6365 7274 6966 6963 6174 6520  his certificate 
+0001a670: 6578 7069 7265 7320 6f6e 2031 3937 302d  expires on 1970-
+0001a680: 3031 2d30 312e 5c6e 270a 2020 2020 2020  01-01.\n'.      
+0001a690: 2020 2020 2020 2754 6865 7365 2066 696c        'These fil
+0001a6a0: 6573 2077 696c 6c20 6265 2075 7064 6174  es will be updat
+0001a6b0: 6564 2077 6865 6e20 7468 6520 6365 7274  ed when the cert
+0001a6c0: 6966 6963 6174 6520 7265 6e65 7773 2e27  ificate renews.'
+0001a6d0: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+0001a6e0: 7373 2052 6570 6f72 744e 6578 7453 7465  ss ReportNextSte
+0001a6f0: 7073 5465 7374 2875 6e69 7474 6573 742e  psTest(unittest.
+0001a700: 5465 7374 4361 7365 293a 0a20 2020 2022  TestCase):.    "
+0001a710: 2222 5465 7374 7320 666f 7220 6365 7274  ""Tests for cert
+0001a720: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0001a730: 696e 2e5f 7265 706f 7274 5f6e 6578 745f  in._report_next_
+0001a740: 7374 6570 7322 2222 0a0a 2020 2020 6465  steps"""..    de
+0001a750: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
+0001a760: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
+0001a770: 6967 203d 206d 6f63 6b2e 4d61 6769 634d  ig = mock.MagicM
+0001a780: 6f63 6b28 0a20 2020 2020 2020 2020 2020  ock(.           
+0001a790: 2063 6572 745f 6e61 6d65 3d22 6578 616d   cert_name="exam
+0001a7a0: 706c 652e 636f 6d22 2c20 7072 6563 6f6e  ple.com", precon
+0001a7b0: 6669 6775 7265 645f 7265 6e65 7761 6c3d  figured_renewal=
+0001a7c0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0001a7d0: 2020 6373 723d 4e6f 6e65 2c20 6175 7468    csr=None, auth
+0001a7e0: 656e 7469 6361 746f 723d 226e 6769 6e78  enticator="nginx
+0001a7f0: 222c 206d 616e 7561 6c5f 6175 7468 5f68  ", manual_auth_h
+0001a800: 6f6f 6b3d 4e6f 6e65 290a 2020 2020 2020  ook=None).      
+0001a810: 2020 6e6f 7469 6679 5f70 6174 6368 203d    notify_patch =
+0001a820: 206d 6f63 6b2e 7061 7463 6828 2763 6572   mock.patch('cer
+0001a830: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+0001a840: 6169 6e2e 6469 7370 6c61 795f 7574 696c  ain.display_util
+0001a850: 2e6e 6f74 6966 7927 290a 2020 2020 2020  .notify').      
+0001a860: 2020 7365 6c66 2e6d 6f63 6b5f 6e6f 7469    self.mock_noti
+0001a870: 6679 203d 206e 6f74 6966 795f 7061 7463  fy = notify_patc
+0001a880: 682e 7374 6172 7428 290a 2020 2020 2020  h.start().      
+0001a890: 2020 7365 6c66 2e61 6464 436c 6561 6e75    self.addCleanu
+0001a8a0: 7028 6e6f 7469 6679 5f70 6174 6368 2e73  p(notify_patch.s
+0001a8b0: 746f 7029 0a20 2020 2020 2020 2073 656c  top).        sel
+0001a8c0: 662e 6f6c 645f 7374 646f 7574 203d 2073  f.old_stdout = s
+0001a8d0: 7973 2e73 7464 6f75 740a 2020 2020 2020  ys.stdout.      
+0001a8e0: 2020 7379 732e 7374 646f 7574 203d 2069    sys.stdout = i
+0001a8f0: 6f2e 5374 7269 6e67 494f 2829 0a0a 2020  o.StringIO()..  
+0001a900: 2020 6465 6620 7465 6172 446f 776e 2873    def tearDown(s
+0001a910: 656c 6629 3a0a 2020 2020 2020 2020 7379  elf):.        sy
+0001a920: 732e 7374 646f 7574 203d 2073 656c 662e  s.stdout = self.
+0001a930: 6f6c 645f 7374 646f 7574 0a0a 2020 2020  old_stdout..    
+0001a940: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+0001a950: 2064 6566 205f 6361 6c6c 2863 6c73 2c20   def _call(cls, 
+0001a960: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0001a970: 3a0a 2020 2020 2020 2020 6672 6f6d 2063  :.        from c
+0001a980: 6572 7462 6f74 2e5f 696e 7465 726e 616c  ertbot._internal
+0001a990: 2e6d 6169 6e20 696d 706f 7274 205f 7265  .main import _re
+0001a9a0: 706f 7274 5f6e 6578 745f 7374 6570 730a  port_next_steps.
+0001a9b0: 2020 2020 2020 2020 5f72 6570 6f72 745f          _report_
+0001a9c0: 6e65 7874 5f73 7465 7073 282a 6172 6773  next_steps(*args
+0001a9d0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+0001a9e0: 2064 6566 205f 6f75 7470 7574 2873 656c   def _output(sel
+0001a9f0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+0001aa00: 2020 2061 7373 6572 7420 7365 6c66 2e6d     assert self.m
+0001aa10: 6f63 6b5f 6e6f 7469 6679 2e63 616c 6c5f  ock_notify.call_
+0001aa20: 636f 756e 7420 3d3d 2032 0a20 2020 2020  count == 2.     
+0001aa30: 2020 2061 7373 6572 7420 7365 6c66 2e6d     assert self.m
+0001aa40: 6f63 6b5f 6e6f 7469 6679 2e63 616c 6c5f  ock_notify.call_
+0001aa50: 6172 6773 5f6c 6973 745b 305d 5b30 5d5b  args_list[0][0][
+0001aa60: 305d 203d 3d20 274e 4558 5420 5354 4550  0] == 'NEXT STEP
+0001aa70: 533a 270a 2020 2020 2020 2020 7265 7475  S:'.        retu
+0001aa80: 726e 2073 656c 662e 6d6f 636b 5f6e 6f74  rn self.mock_not
+0001aa90: 6966 792e 6361 6c6c 5f61 7267 735f 6c69  ify.call_args_li
+0001aaa0: 7374 5b31 5d5b 305d 5b30 5d0a 0a20 2020  st[1][0][0]..   
+0001aab0: 2064 6566 2074 6573 745f 7265 706f 7274   def test_report
+0001aac0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001aad0: 2222 224e 6f20 7374 6570 7320 666f 7220  """No steps for 
+0001aae0: 6120 6e6f 726d 616c 2072 656e 6577 616c  a normal renewal
+0001aaf0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0001ab00: 2e63 6f6e 6669 672e 6175 7468 656e 7469  .config.authenti
+0001ab10: 6361 746f 7220 3d20 226d 616e 7561 6c22  cator = "manual"
+0001ab20: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0001ab30: 6e66 6967 2e6d 616e 7561 6c5f 6175 7468  nfig.manual_auth
+0001ab40: 5f68 6f6f 6b20 3d20 222f 6269 6e2f 7472  _hook = "/bin/tr
+0001ab50: 7565 220a 2020 2020 2020 2020 7365 6c66  ue".        self
+0001ab60: 2e5f 6361 6c6c 2873 656c 662e 636f 6e66  ._call(self.conf
+0001ab70: 6967 2c20 4e6f 6e65 2c20 4e6f 6e65 290a  ig, None, None).
+0001ab80: 2020 2020 2020 2020 7365 6c66 2e6d 6f63          self.moc
+0001ab90: 6b5f 6e6f 7469 6679 2e61 7373 6572 745f  k_notify.assert_
+0001aba0: 6e6f 745f 6361 6c6c 6564 2829 0a0a 2020  not_called()..  
+0001abb0: 2020 6465 6620 7465 7374 5f63 7372 5f72    def test_csr_r
+0001abc0: 6570 6f72 7428 7365 6c66 293a 0a20 2020  eport(self):.   
+0001abd0: 2020 2020 2022 2222 2d2d 6373 7220 7265       """--csr re
+0001abe0: 7175 6972 6573 206d 616e 7561 6c20 7265  quires manual re
+0001abf0: 6e65 7761 6c22 2222 0a20 2020 2020 2020  newal""".       
+0001ac00: 2073 656c 662e 636f 6e66 6967 2e63 7372   self.config.csr
+0001ac10: 203d 2022 666f 6f2e 6373 7222 0a20 2020   = "foo.csr".   
+0001ac20: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
+0001ac30: 7365 6c66 2e63 6f6e 6669 672c 204e 6f6e  self.config, Non
+0001ac40: 652c 204e 6f6e 6529 0a20 2020 2020 2020  e, None).       
+0001ac50: 2061 7373 6572 7420 222d 2d63 7372 2077   assert "--csr w
+0001ac60: 696c 6c20 6e6f 7420 6265 2072 656e 6577  ill not be renew
+0001ac70: 6564 2220 696e 2073 656c 662e 5f6f 7574  ed" in self._out
+0001ac80: 7075 7428 290a 0a20 2020 2064 6566 2074  put()..    def t
+0001ac90: 6573 745f 6d61 6e75 616c 5f6e 6f5f 686f  est_manual_no_ho
+0001aca0: 6f6b 5f72 656e 6577 616c 2873 656c 6629  ok_renewal(self)
+0001acb0: 3a0a 2020 2020 2020 2020 2222 222d 2d6d  :.        """--m
+0001acc0: 616e 7561 6c20 7769 7468 6f75 7420 6120  anual without a 
+0001acd0: 686f 6f6b 2072 6571 7569 7265 7320 6d61  hook requires ma
+0001ace0: 6e75 616c 2072 656e 6577 616c 2222 220a  nual renewal""".
+0001acf0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0001ad00: 6669 672e 6175 7468 656e 7469 6361 746f  fig.authenticato
+0001ad10: 7220 3d20 226d 616e 7561 6c22 0a20 2020  r = "manual".   
+0001ad20: 2020 2020 2073 656c 662e 5f63 616c 6c28       self._call(
+0001ad30: 7365 6c66 2e63 6f6e 6669 672c 204e 6f6e  self.config, Non
+0001ad40: 652c 204e 6f6e 6529 0a20 2020 2020 2020  e, None).       
+0001ad50: 2061 7373 6572 7420 222d 2d6d 616e 7561   assert "--manua
+0001ad60: 6c20 6365 7274 6966 6963 6174 6573 2072  l certificates r
+0001ad70: 6571 7569 7265 7322 2069 6e20 7365 6c66  equires" in self
+0001ad80: 2e5f 6f75 7470 7574 2829 0a0a 2020 2020  ._output()..    
+0001ad90: 6465 6620 7465 7374 5f6e 6f5f 7072 6563  def test_no_prec
+0001ada0: 6f6e 6669 6775 7265 645f 7265 6e65 7761  onfigured_renewa
+0001adb0: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
+0001adc0: 2022 2222 4e6f 202d 2d70 7265 636f 6e66   """No --preconf
+0001add0: 6967 7572 6564 2d72 656e 6577 616c 206e  igured-renewal n
+0001ade0: 6565 6473 206d 616e 7561 6c20 6372 6f6e  eeds manual cron
+0001adf0: 2073 6574 7570 2222 220a 2020 2020 2020   setup""".      
+0001ae00: 2020 7365 6c66 2e63 6f6e 6669 672e 7072    self.config.pr
+0001ae10: 6563 6f6e 6669 6775 7265 645f 7265 6e65  econfigured_rene
+0001ae20: 7761 6c20 3d20 4661 6c73 650a 2020 2020  wal = False.    
+0001ae30: 2020 2020 7365 6c66 2e5f 6361 6c6c 2873      self._call(s
+0001ae40: 656c 662e 636f 6e66 6967 2c20 4e6f 6e65  elf.config, None
+0001ae50: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0001ae60: 6173 7365 7274 2022 6874 7470 733a 2f2f  assert "https://
+0001ae70: 6365 7274 626f 742e 6f72 672f 7265 6e65  certbot.org/rene
+0001ae80: 7761 6c2d 7365 7475 7022 2069 6e20 7365  wal-setup" in se
+0001ae90: 6c66 2e5f 6f75 7470 7574 2829 0a0a 0a63  lf._output()...c
+0001aea0: 6c61 7373 2055 7064 6174 6541 6363 6f75  lass UpdateAccou
+0001aeb0: 6e74 5465 7374 2874 6573 745f 7574 696c  ntTest(test_util
+0001aec0: 2e43 6f6e 6669 6754 6573 7443 6173 6529  .ConfigTestCase)
+0001aed0: 3a0a 2020 2020 2222 2254 6573 7473 2066  :.    """Tests f
+0001aee0: 6f72 2063 6572 7462 6f74 2e5f 696e 7465  or certbot._inte
+0001aef0: 726e 616c 2e6d 6169 6e2e 7570 6461 7465  rnal.main.update
+0001af00: 5f61 6363 6f75 6e74 2222 220a 0a20 2020  _account"""..   
+0001af10: 2064 6566 2073 6574 5570 2873 656c 6629   def setUp(self)
+0001af20: 3a0a 2020 2020 2020 2020 7061 7463 6865  :.        patche
+0001af30: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+0001af40: 2020 2761 6363 6f75 6e74 273a 206d 6f63    'account': moc
+0001af50: 6b2e 7061 7463 6828 2763 6572 7462 6f74  k.patch('certbot
+0001af60: 2e5f 696e 7465 726e 616c 2e6d 6169 6e2e  ._internal.main.
+0001af70: 6163 636f 756e 7427 292c 0a20 2020 2020  account'),.     
+0001af80: 2020 2020 2020 2027 6174 6578 6974 273a         'atexit':
+0001af90: 206d 6f63 6b2e 7061 7463 6828 2763 6572   mock.patch('cer
+0001afa0: 7462 6f74 2e75 7469 6c2e 6174 6578 6974  tbot.util.atexit
+0001afb0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0001afc0: 2763 6c69 656e 7427 3a20 6d6f 636b 2e70  'client': mock.p
+0001afd0: 6174 6368 2827 6365 7274 626f 742e 5f69  atch('certbot._i
+0001afe0: 6e74 6572 6e61 6c2e 6d61 696e 2e63 6c69  nternal.main.cli
+0001aff0: 656e 7427 292c 0a20 2020 2020 2020 2020  ent'),.         
+0001b000: 2020 2027 6465 7465 726d 696e 655f 6163     'determine_ac
+0001b010: 636f 756e 7427 3a20 6d6f 636b 2e70 6174  count': mock.pat
+0001b020: 6368 2827 6365 7274 626f 742e 5f69 6e74  ch('certbot._int
+0001b030: 6572 6e61 6c2e 6d61 696e 2e5f 6465 7465  ernal.main._dete
+0001b040: 726d 696e 655f 6163 636f 756e 7427 292c  rmine_account'),
+0001b050: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
+0001b060: 7469 6679 273a 206d 6f63 6b2e 7061 7463  tify': mock.patc
+0001b070: 6828 2763 6572 7462 6f74 2e5f 696e 7465  h('certbot._inte
+0001b080: 726e 616c 2e6d 6169 6e2e 6469 7370 6c61  rnal.main.displa
+0001b090: 795f 7574 696c 2e6e 6f74 6966 7927 292c  y_util.notify'),
+0001b0a0: 0a20 2020 2020 2020 2020 2020 2027 7072  .            'pr
+0001b0b0: 6570 6172 655f 7375 6227 3a20 6d6f 636b  epare_sub': mock
+0001b0c0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0001b0d0: 5f69 6e74 6572 6e61 6c2e 6566 662e 7072  _internal.eff.pr
+0001b0e0: 6570 6172 655f 7375 6273 6372 6970 7469  epare_subscripti
+0001b0f0: 6f6e 2729 2c0a 2020 2020 2020 2020 2020  on'),.          
+0001b100: 2020 2775 7469 6c27 3a20 7465 7374 5f75    'util': test_u
+0001b110: 7469 6c2e 7061 7463 685f 6469 7370 6c61  til.patch_displa
+0001b120: 795f 7574 696c 2829 0a20 2020 2020 2020  y_util().       
+0001b130: 207d 0a20 2020 2020 2020 2073 656c 662e   }.        self.
+0001b140: 6d6f 636b 7320 3d20 7b20 6b3a 2070 6174  mocks = { k: pat
+0001b150: 6368 6573 5b6b 5d2e 7374 6172 7428 2920  ches[k].start() 
+0001b160: 666f 7220 6b20 696e 2070 6174 6368 6573  for k in patches
+0001b170: 207d 0a20 2020 2020 2020 2066 6f72 2070   }.        for p
+0001b180: 6174 6368 2069 6e20 7061 7463 6865 732e  atch in patches.
+0001b190: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
+0001b1a0: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
+0001b1b0: 6561 6e75 7028 7061 7463 682e 7374 6f70  eanup(patch.stop
+0001b1c0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0001b1d0: 6e20 7375 7065 7228 292e 7365 7455 7028  n super().setUp(
+0001b1e0: 290a 0a20 2020 2064 6566 205f 6361 6c6c  )..    def _call
+0001b1f0: 2873 656c 662c 2061 7267 7329 3a0a 2020  (self, args):.  
+0001b200: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
+0001b210: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0001b220: 696e 7465 726e 616c 2e6d 6169 6e2e 7379  internal.main.sy
+0001b230: 732e 7374 646f 7574 2729 2c20 5c0a 2020  s.stdout'), \.  
+0001b240: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
+0001b250: 7061 7463 6828 2763 6572 7462 6f74 2e5f  patch('certbot._
+0001b260: 696e 7465 726e 616c 2e6d 6169 6e2e 7379  internal.main.sy
+0001b270: 732e 7374 6465 7272 2729 3a0a 2020 2020  s.stderr'):.    
+0001b280: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
+0001b290: 272d 2d63 6f6e 6669 672d 6469 7227 2c20  '--config-dir', 
+0001b2a0: 7365 6c66 2e63 6f6e 6669 672e 636f 6e66  self.config.conf
+0001b2b0: 6967 5f64 6972 2c0a 2020 2020 2020 2020  ig_dir,.        
+0001b2c0: 2020 2020 2020 2020 2020 2020 272d 2d77              '--w
+0001b2d0: 6f72 6b2d 6469 7227 2c20 7365 6c66 2e63  ork-dir', self.c
+0001b2e0: 6f6e 6669 672e 776f 726b 5f64 6972 2c0a  onfig.work_dir,.
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b300: 2020 2020 272d 2d6c 6f67 732d 6469 7227      '--logs-dir'
+0001b310: 2c20 7365 6c66 2e63 6f6e 6669 672e 6c6f  , self.config.lo
+0001b320: 6773 5f64 6972 2c20 272d 2d74 6578 7427  gs_dir, '--text'
+0001b330: 5d20 2b20 6172 6773 0a20 2020 2020 2020  ] + args.       
+0001b340: 2020 2020 2072 6574 7572 6e20 6d61 696e       return main
+0001b350: 2e6d 6169 6e28 6172 6773 5b3a 5d29 2023  .main(args[:]) #
+0001b360: 204e 4f54 453a 2070 6172 7365 7220 6361   NOTE: parser ca
+0001b370: 6e20 616c 7465 7220 6974 7320 6172 6773  n alter its args
+0001b380: 210a 0a20 2020 2064 6566 205f 7072 6570  !..    def _prep
+0001b390: 6172 655f 6d6f 636b 5f61 6363 6f75 6e74  are_mock_account
+0001b3a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001b3b0: 6d6f 636b 5f73 746f 7261 6765 203d 206d  mock_storage = m
+0001b3c0: 6f63 6b2e 4d61 6769 634d 6f63 6b28 290a  ock.MagicMock().
+0001b3d0: 2020 2020 2020 2020 6d6f 636b 5f61 6363          mock_acc
+0001b3e0: 6f75 6e74 203d 206d 6f63 6b2e 4d61 6769  ount = mock.Magi
+0001b3f0: 634d 6f63 6b28 290a 2020 2020 2020 2020  cMock().        
+0001b400: 6d6f 636b 5f72 6567 7220 3d20 6d6f 636b  mock_regr = mock
+0001b410: 2e4d 6167 6963 4d6f 636b 2829 0a20 2020  .MagicMock().   
+0001b420: 2020 2020 206d 6f63 6b5f 7374 6f72 6167       mock_storag
+0001b430: 652e 6669 6e64 5f61 6c6c 2e72 6574 7572  e.find_all.retur
+0001b440: 6e5f 7661 6c75 6520 3d20 5b6d 6f63 6b5f  n_value = [mock_
+0001b450: 6163 636f 756e 745d 0a20 2020 2020 2020  account].       
+0001b460: 2073 656c 662e 6d6f 636b 735b 2761 6363   self.mocks['acc
+0001b470: 6f75 6e74 275d 2e41 6363 6f75 6e74 4669  ount'].AccountFi
+0001b480: 6c65 5374 6f72 6167 652e 7265 7475 726e  leStorage.return
+0001b490: 5f76 616c 7565 203d 206d 6f63 6b5f 7374  _value = mock_st
+0001b4a0: 6f72 6167 650a 2020 2020 2020 2020 6d6f  orage.        mo
+0001b4b0: 636b 5f61 6363 6f75 6e74 2e72 6567 722e  ck_account.regr.
+0001b4c0: 626f 6479 203d 206d 6f63 6b5f 7265 6772  body = mock_regr
+0001b4d0: 2e62 6f64 790a 2020 2020 2020 2020 7365  .body.        se
+0001b4e0: 6c66 2e6d 6f63 6b73 5b27 6465 7465 726d  lf.mocks['determ
+0001b4f0: 696e 655f 6163 636f 756e 7427 5d2e 7265  ine_account'].re
+0001b500: 7475 726e 5f76 616c 7565 203d 2028 6d6f  turn_value = (mo
+0001b510: 636b 5f61 6363 6f75 6e74 2c20 6d6f 636b  ck_account, mock
+0001b520: 2e4d 6167 6963 4d6f 636b 2829 290a 2020  .MagicMock()).  
+0001b530: 2020 2020 2020 7265 7475 726e 2028 6d6f        return (mo
+0001b540: 636b 5f61 6363 6f75 6e74 2c20 6d6f 636b  ck_account, mock
+0001b550: 5f73 746f 7261 6765 2c20 6d6f 636b 5f72  _storage, mock_r
+0001b560: 6567 7229 0a0a 2020 2020 6465 6620 5f74  egr)..    def _t
+0001b570: 6573 745f 7570 6461 7465 5f6e 6f5f 636f  est_update_no_co
+0001b580: 6e74 6163 7428 7365 6c66 2c20 6172 6773  ntact(self, args
+0001b590: 293a 0a20 2020 2020 2020 2022 2222 5574  ):.        """Ut
+0001b5a0: 696c 6974 7920 746f 2061 7373 6572 7420  ility to assert 
+0001b5b0: 7468 6174 2065 6d61 696c 2072 656d 6f76  that email remov
+0001b5c0: 616c 2069 7320 6861 6e64 6c65 6420 636f  al is handled co
+0001b5d0: 7272 6563 746c 7922 2222 0a20 2020 2020  rrectly""".     
+0001b5e0: 2020 2028 5f2c 206d 6f63 6b5f 7374 6f72     (_, mock_stor
+0001b5f0: 6167 652c 206d 6f63 6b5f 7265 6772 2920  age, mock_regr) 
+0001b600: 3d20 7365 6c66 2e5f 7072 6570 6172 655f  = self._prepare_
+0001b610: 6d6f 636b 5f61 6363 6f75 6e74 2829 0a20  mock_account(). 
+0001b620: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0001b630: 7365 6c66 2e5f 6361 6c6c 2861 7267 7329  self._call(args)
+0001b640: 0a20 2020 2020 2020 2023 2057 6865 6e20  .        # When 
+0001b650: 7570 6461 7465 2073 7563 6365 6564 732c  update succeeds,
+0001b660: 2074 6865 2072 6574 7572 6e20 7661 6c75   the return valu
+0001b670: 6520 6f66 2075 7064 6174 655f 6163 636f  e of update_acco
+0001b680: 756e 7428 2920 6973 204e 6f6e 650a 2020  unt() is None.  
+0001b690: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+0001b6a0: 756c 7420 6973 204e 6f6e 650a 2020 2020  ult is None.    
+0001b6b0: 2020 2020 2320 5765 2073 7562 6d69 7474      # We submitt
+0001b6c0: 6564 2061 2072 6567 6973 7472 6174 696f  ed a registratio
+0001b6d0: 6e20 746f 2074 6865 2073 6572 7665 720a  n to the server.
+0001b6e0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0001b6f0: 656c 662e 6d6f 636b 735b 2763 6c69 656e  elf.mocks['clien
+0001b700: 7427 5d2e 436c 6965 6e74 2829 2e61 636d  t'].Client().acm
+0001b710: 652e 7570 6461 7465 5f72 6567 6973 7472  e.update_registr
+0001b720: 6174 696f 6e2e 6361 6c6c 5f63 6f75 6e74  ation.call_count
+0001b730: 203d 3d20 310a 2020 2020 2020 2020 6d6f   == 1.        mo
+0001b740: 636b 5f72 6567 722e 626f 6479 2e75 7064  ck_regr.body.upd
+0001b750: 6174 652e 6173 7365 7274 5f63 616c 6c65  ate.assert_calle
+0001b760: 645f 7769 7468 2863 6f6e 7461 6374 3d28  d_with(contact=(
+0001b770: 2929 0a20 2020 2020 2020 2023 2057 6520  )).        # We 
+0001b780: 676f 7420 616e 2075 7064 6174 6520 6672  got an update fr
+0001b790: 6f6d 2074 6865 2073 6572 7665 7220 616e  om the server an
+0001b7a0: 6420 7065 7273 6973 7465 6420 6974 0a20  d persisted it. 
+0001b7b0: 2020 2020 2020 2061 7373 6572 7420 6d6f         assert mo
+0001b7c0: 636b 5f73 746f 7261 6765 2e75 7064 6174  ck_storage.updat
+0001b7d0: 655f 7265 6772 2e63 616c 6c5f 636f 756e  e_regr.call_coun
+0001b7e0: 7420 3d3d 2031 0a20 2020 2020 2020 2023  t == 1.        #
+0001b7f0: 2057 6520 7368 6f75 6c64 2068 6176 6520   We should have 
+0001b800: 6e6f 7469 6669 6564 2074 6865 2075 7365  notified the use
+0001b810: 720a 2020 2020 2020 2020 7365 6c66 2e6d  r.        self.m
+0001b820: 6f63 6b73 5b27 6e6f 7469 6679 275d 2e61  ocks['notify'].a
+0001b830: 7373 6572 745f 6361 6c6c 6564 5f77 6974  ssert_called_wit
+0001b840: 6828 0a20 2020 2020 2020 2020 2020 2027  h(.            '
+0001b850: 416e 7920 636f 6e74 6163 7420 696e 666f  Any contact info
+0001b860: 726d 6174 696f 6e20 6173 736f 6369 6174  rmation associat
+0001b870: 6564 2077 6974 6820 7468 6973 2061 6363  ed with this acc
+0001b880: 6f75 6e74 2068 6173 2062 6565 6e20 7265  ount has been re
+0001b890: 6d6f 7665 642e 270a 2020 2020 2020 2020  moved.'.        
+0001b8a0: 290a 2020 2020 2020 2020 2320 5765 2073  ).        # We s
+0001b8b0: 686f 756c 6420 6e6f 7420 6861 7665 2063  hould not have c
+0001b8c0: 616c 6c65 6420 7375 6273 6372 6970 7469  alled subscripti
+0001b8d0: 6f6e 2062 6563 6175 7365 2074 6865 7265  on because there
+0001b8e0: 2773 206e 6f20 656d 6169 6c0a 2020 2020  's no email.    
+0001b8f0: 2020 2020 7365 6c66 2e6d 6f63 6b73 5b27      self.mocks['
+0001b900: 7072 6570 6172 655f 7375 6227 5d2e 6173  prepare_sub'].as
+0001b910: 7365 7274 5f6e 6f74 5f63 616c 6c65 6428  sert_not_called(
+0001b920: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001b930: 6e6f 5f65 7869 7374 696e 675f 6163 636f  no_existing_acco
+0001b940: 756e 7473 2873 656c 6629 3a0a 2020 2020  unts(self):.    
+0001b950: 2020 2020 2222 2254 6573 7420 7468 6174      """Test that
+0001b960: 206e 6f20 6578 6973 7469 6e67 2061 6363   no existing acc
+0001b970: 6f75 6e74 2069 7320 6861 6e64 6c65 6420  ount is handled 
+0001b980: 636f 7272 6563 746c 7922 2222 0a20 2020  correctly""".   
+0001b990: 2020 2020 206d 6f63 6b5f 7374 6f72 6167       mock_storag
+0001b9a0: 6520 3d20 6d6f 636b 2e4d 6167 6963 4d6f  e = mock.MagicMo
+0001b9b0: 636b 2829 0a20 2020 2020 2020 206d 6f63  ck().        moc
+0001b9c0: 6b5f 7374 6f72 6167 652e 6669 6e64 5f61  k_storage.find_a
+0001b9d0: 6c6c 2e72 6574 7572 6e5f 7661 6c75 6520  ll.return_value 
+0001b9e0: 3d20 5b5d 0a20 2020 2020 2020 2073 656c  = [].        sel
+0001b9f0: 662e 6d6f 636b 735b 2761 6363 6f75 6e74  f.mocks['account
+0001ba00: 275d 2e41 6363 6f75 6e74 4669 6c65 5374  '].AccountFileSt
+0001ba10: 6f72 6167 652e 7265 7475 726e 5f76 616c  orage.return_val
+0001ba20: 7565 203d 206d 6f63 6b5f 7374 6f72 6167  ue = mock_storag
+0001ba30: 650a 2020 2020 2020 2020 6173 7365 7274  e.        assert
+0001ba40: 2073 656c 662e 5f63 616c 6c28 5b27 7570   self._call(['up
+0001ba50: 6461 7465 5f61 6363 6f75 6e74 272c 2027  date_account', '
+0001ba60: 2d2d 656d 6169 6c27 2c20 2775 7365 7240  --email', 'user@
+0001ba70: 6578 616d 706c 652e 6f72 6727 5d29 203d  example.org']) =
+0001ba80: 3d20 5c0a 2020 2020 2020 2020 2020 2020  = \.            
+0001ba90: 2020 2020 2020 2020 2020 2020 2027 436f               'Co
+0001baa0: 756c 6420 6e6f 7420 6669 6e64 2061 6e20  uld not find an 
+0001bab0: 6578 6973 7469 6e67 2061 6363 6f75 6e74  existing account
+0001bac0: 2066 6f72 2073 6572 7665 7227 205c 0a20   for server' \. 
+0001bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bae0: 2020 2020 2020 2020 2720 6874 7470 733a          ' https:
+0001baf0: 2f2f 6163 6d65 2d76 3032 2e61 7069 2e6c  //acme-v02.api.l
+0001bb00: 6574 7365 6e63 7279 7074 2e6f 7267 2f64  etsencrypt.org/d
+0001bb10: 6972 6563 746f 7279 2e27 0a0a 2020 2020  irectory.'..    
+0001bb20: 6465 6620 7465 7374 5f75 7064 6174 655f  def test_update_
+0001bb30: 6163 636f 756e 745f 7265 6d6f 7665 5f65  account_remove_e
+0001bb40: 6d61 696c 2873 656c 6629 3a0a 2020 2020  mail(self):.    
+0001bb50: 2020 2020 2222 2254 6573 7420 7468 6174      """Test that
+0001bb60: 202d 2d72 6567 6973 7465 722d 756e 7361   --register-unsa
+0001bb70: 6665 6c79 2d77 6974 686f 7574 2d65 6d61  fely-without-ema
+0001bb80: 696c 2069 7320 6861 6e64 6c65 6420 6173  il is handled as
+0001bb90: 206e 6f20 656d 6169 6c22 2222 0a20 2020   no email""".   
+0001bba0: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
+0001bbb0: 7570 6461 7465 5f6e 6f5f 636f 6e74 6163  update_no_contac
+0001bbc0: 7428 5b27 7570 6461 7465 5f61 6363 6f75  t(['update_accou
+0001bbd0: 6e74 272c 2027 2d2d 7265 6769 7374 6572  nt', '--register
+0001bbe0: 2d75 6e73 6166 656c 792d 7769 7468 6f75  -unsafely-withou
+0001bbf0: 742d 656d 6169 6c27 5d29 0a0a 2020 2020  t-email'])..    
+0001bc00: 6465 6620 7465 7374 5f75 7064 6174 655f  def test_update_
+0001bc10: 6163 636f 756e 745f 656d 7074 795f 656d  account_empty_em
+0001bc20: 6169 6c28 7365 6c66 293a 0a20 2020 2020  ail(self):.     
+0001bc30: 2020 2022 2222 5465 7374 2074 6861 7420     """Test that 
+0001bc40: 7072 6f76 6964 696e 6720 616e 2065 6d70  providing an emp
+0001bc50: 7479 2065 6d61 696c 2069 7320 6861 6e64  ty email is hand
+0001bc60: 6c65 6420 6173 206e 6f20 656d 6169 6c22  led as no email"
+0001bc70: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0001bc80: 5f74 6573 745f 7570 6461 7465 5f6e 6f5f  _test_update_no_
+0001bc90: 636f 6e74 6163 7428 5b27 7570 6461 7465  contact(['update
+0001bca0: 5f61 6363 6f75 6e74 272c 2027 2d6d 272c  _account', '-m',
+0001bcb0: 2027 275d 290a 0a20 2020 2040 6d6f 636b   ''])..    @mock
+0001bcc0: 2e70 6174 6368 2827 6365 7274 626f 742e  .patch('certbot.
+0001bcd0: 5f69 6e74 6572 6e61 6c2e 6d61 696e 2e64  _internal.main.d
+0001bce0: 6973 706c 6179 5f6f 7073 2e67 6574 5f65  isplay_ops.get_e
+0001bcf0: 6d61 696c 2729 0a20 2020 2064 6566 2074  mail').    def t
+0001bd00: 6573 745f 7570 6461 7465 5f61 6363 6f75  est_update_accou
+0001bd10: 6e74 5f77 6974 685f 656d 6169 6c28 7365  nt_with_email(se
+0001bd20: 6c66 2c20 6d6f 636b 5f65 6d61 696c 293a  lf, mock_email):
+0001bd30: 0a20 2020 2020 2020 2022 2222 5465 7374  .        """Test
+0001bd40: 2074 6861 7420 7570 6461 7469 6e67 2077   that updating w
+0001bd50: 6974 6820 6120 7369 6e67 756c 6172 2065  ith a singular e
+0001bd60: 6d61 696c 2069 7320 6861 6e64 6c65 6420  mail is handled 
+0001bd70: 636f 7272 6563 746c 7922 2222 0a20 2020  correctly""".   
+0001bd80: 2020 2020 206d 6f63 6b5f 656d 6169 6c2e       mock_email.
+0001bd90: 7265 7475 726e 5f76 616c 7565 203d 2027  return_value = '
+0001bda0: 7573 6572 4065 7861 6d70 6c65 2e63 6f6d  user@example.com
+0001bdb0: 270a 2020 2020 2020 2020 285f 2c20 6d6f  '.        (_, mo
+0001bdc0: 636b 5f73 746f 7261 6765 2c20 5f29 203d  ck_storage, _) =
+0001bdd0: 2073 656c 662e 5f70 7265 7061 7265 5f6d   self._prepare_m
+0001bde0: 6f63 6b5f 6163 636f 756e 7428 290a 2020  ock_account().  
+0001bdf0: 2020 2020 2020 6d6f 636b 5f63 6c69 656e        mock_clien
+0001be00: 7420 3d20 6d6f 636b 2e4d 6167 6963 4d6f  t = mock.MagicMo
+0001be10: 636b 2829 0a20 2020 2020 2020 2073 656c  ck().        sel
+0001be20: 662e 6d6f 636b 735b 2763 6c69 656e 7427  f.mocks['client'
+0001be30: 5d2e 436c 6965 6e74 2e72 6574 7572 6e5f  ].Client.return_
+0001be40: 7661 6c75 6520 3d20 6d6f 636b 5f63 6c69  value = mock_cli
+0001be50: 656e 740a 0a20 2020 2020 2020 2072 6573  ent..        res
+0001be60: 756c 7420 3d20 7365 6c66 2e5f 6361 6c6c  ult = self._call
+0001be70: 285b 2775 7064 6174 655f 6163 636f 756e  (['update_accoun
+0001be80: 7427 5d29 0a20 2020 2020 2020 2023 204e  t']).        # N
+0001be90: 6f6e 6520 6966 2072 6567 6973 7472 6174  one if registrat
+0001bea0: 696f 6e20 7375 6363 6565 6473 0a20 2020  ion succeeds.   
+0001beb0: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+0001bec0: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
+0001bed0: 2020 2023 2057 6520 7368 6f75 6c64 2068     # We should h
+0001bee0: 6176 6520 7570 6461 7465 6420 7468 6520  ave updated the 
+0001bef0: 7365 7276 6572 0a20 2020 2020 2020 2061  server.        a
+0001bf00: 7373 6572 7420 6d6f 636b 5f63 6c69 656e  ssert mock_clien
+0001bf10: 742e 6163 6d65 2e75 7064 6174 655f 7265  t.acme.update_re
+0001bf20: 6769 7374 7261 7469 6f6e 2e63 616c 6c5f  gistration.call_
+0001bf30: 636f 756e 7420 3d3d 2031 0a20 2020 2020  count == 1.     
+0001bf40: 2020 2023 2057 6520 7368 6f75 6c64 2068     # We should h
+0001bf50: 6176 6520 7570 6461 7465 6420 7468 6520  ave updated the 
+0001bf60: 6163 636f 756e 7420 6f6e 2064 6973 6b0a  account on disk.
+0001bf70: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
+0001bf80: 6f63 6b5f 7374 6f72 6167 652e 7570 6461  ock_storage.upda
+0001bf90: 7465 5f72 6567 722e 6361 6c6c 5f63 6f75  te_regr.call_cou
+0001bfa0: 6e74 203d 3d20 310a 2020 2020 2020 2020  nt == 1.        
+0001bfb0: 2320 5375 6273 6372 6970 7469 6f6e 2073  # Subscription s
+0001bfc0: 686f 756c 6420 6861 7665 2062 6565 6e20  hould have been 
+0001bfd0: 7072 6f6d 7074 6564 0a20 2020 2020 2020  prompted.       
+0001bfe0: 2061 7373 6572 7420 7365 6c66 2e6d 6f63   assert self.moc
+0001bff0: 6b73 5b27 7072 6570 6172 655f 7375 6227  ks['prepare_sub'
+0001c000: 5d2e 6361 6c6c 5f63 6f75 6e74 203d 3d20  ].call_count == 
+0001c010: 310a 2020 2020 2020 2020 2320 5368 6f75  1.        # Shou
+0001c020: 6c64 2068 6176 6520 7072 696e 7465 6420  ld have printed 
+0001c030: 7468 6520 656d 6169 6c0a 2020 2020 2020  the email.      
+0001c040: 2020 7365 6c66 2e6d 6f63 6b73 5b27 6e6f    self.mocks['no
+0001c050: 7469 6679 275d 2e61 7373 6572 745f 6361  tify'].assert_ca
+0001c060: 6c6c 6564 5f77 6974 6828 0a20 2020 2020  lled_with(.     
+0001c070: 2020 2020 2020 2027 596f 7572 2065 2d6d         'Your e-m
+0001c080: 6169 6c20 6164 6472 6573 7320 7761 7320  ail address was 
+0001c090: 7570 6461 7465 6420 746f 2075 7365 7240  updated to user@
+0001c0a0: 6578 616d 706c 652e 636f 6d2e 2729 0a0a  example.com.')..
+0001c0b0: 2020 2020 6465 6620 7465 7374 5f75 7064      def test_upd
+0001c0c0: 6174 655f 6163 636f 756e 745f 7769 7468  ate_account_with
+0001c0d0: 5f6d 756c 7469 706c 655f 656d 6169 6c73  _multiple_emails
+0001c0e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001c0f0: 2222 2254 6573 7420 7468 6174 206d 756c  """Test that mul
+0001c100: 7469 706c 6520 656d 6169 6c20 6164 6472  tiple email addr
+0001c110: 6573 7365 7320 6172 6520 6861 6e64 6c65  esses are handle
+0001c120: 6420 636f 7272 6563 746c 7922 2222 0a20  d correctly""". 
+0001c130: 2020 2020 2020 2028 5f2c 206d 6f63 6b5f         (_, mock_
+0001c140: 7374 6f72 6167 652c 206d 6f63 6b5f 7265  storage, mock_re
+0001c150: 6772 2920 3d20 7365 6c66 2e5f 7072 6570  gr) = self._prep
+0001c160: 6172 655f 6d6f 636b 5f61 6363 6f75 6e74  are_mock_account
+0001c170: 2829 0a20 2020 2020 2020 2061 7373 6572  ().        asser
+0001c180: 7420 7365 6c66 2e5f 6361 6c6c 285b 2775  t self._call(['u
+0001c190: 7064 6174 655f 6163 636f 756e 7427 2c20  pdate_account', 
+0001c1a0: 272d 6d27 2c20 2775 7365 7240 6578 616d  '-m', 'user@exam
+0001c1b0: 706c 652e 636f 6d2c 7573 6572 4065 7861  ple.com,user@exa
+0001c1c0: 6d70 6c65 2e6f 7267 275d 2920 6973 204e  mple.org']) is N
+0001c1d0: 6f6e 650a 2020 2020 2020 2020 6d6f 636b  one.        mock
+0001c1e0: 5f72 6567 722e 626f 6479 2e75 7064 6174  _regr.body.updat
+0001c1f0: 652e 6173 7365 7274 5f63 616c 6c65 645f  e.assert_called_
+0001c200: 7769 7468 280a 2020 2020 2020 2020 2020  with(.          
+0001c210: 2020 636f 6e74 6163 743d 5b27 6d61 696c    contact=['mail
+0001c220: 746f 3a75 7365 7240 6578 616d 706c 652e  to:user@example.
+0001c230: 636f 6d27 2c20 276d 6169 6c74 6f3a 7573  com', 'mailto:us
+0001c240: 6572 4065 7861 6d70 6c65 2e6f 7267 275d  er@example.org']
+0001c250: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001c260: 2020 2061 7373 6572 7420 6d6f 636b 5f73     assert mock_s
+0001c270: 746f 7261 6765 2e75 7064 6174 655f 7265  torage.update_re
+0001c280: 6772 2e63 616c 6c5f 636f 756e 7420 3d3d  gr.call_count ==
+0001c290: 2031 0a20 2020 2020 2020 2073 656c 662e   1.        self.
+0001c2a0: 6d6f 636b 735b 276e 6f74 6966 7927 5d2e  mocks['notify'].
+0001c2b0: 6173 7365 7274 5f63 616c 6c65 645f 7769  assert_called_wi
+0001c2c0: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+0001c2d0: 2759 6f75 7220 652d 6d61 696c 2061 6464  'Your e-mail add
+0001c2e0: 7265 7373 2077 6173 2075 7064 6174 6564  ress was updated
+0001c2f0: 2074 6f20 7573 6572 4065 7861 6d70 6c65   to user@example
+0001c300: 2e63 6f6d 2c75 7365 7240 6578 616d 706c  .com,user@exampl
+0001c310: 652e 6f72 672e 2729 0a0a 0a63 6c61 7373  e.org.')...class
+0001c320: 2053 686f 7741 6363 6f75 6e74 5465 7374   ShowAccountTest
+0001c330: 2874 6573 745f 7574 696c 2e43 6f6e 6669  (test_util.Confi
+0001c340: 6754 6573 7443 6173 6529 3a0a 2020 2020  gTestCase):.    
+0001c350: 2222 2254 6573 7473 2066 6f72 2063 6572  """Tests for cer
+0001c360: 7462 6f74 2e5f 696e 7465 726e 616c 2e6d  tbot._internal.m
+0001c370: 6169 6e2e 7368 6f77 5f61 6363 6f75 6e74  ain.show_account
+0001c380: 2222 220a 0a20 2020 2064 6566 2073 6574  """..    def set
+0001c390: 5570 2873 656c 6629 3a0a 2020 2020 2020  Up(self):.      
+0001c3a0: 2020 7061 7463 6865 7320 3d20 7b0a 2020    patches = {.  
+0001c3b0: 2020 2020 2020 2020 2020 2761 6363 6f75            'accou
+0001c3c0: 6e74 273a 206d 6f63 6b2e 7061 7463 6828  nt': mock.patch(
+0001c3d0: 2763 6572 7462 6f74 2e5f 696e 7465 726e  'certbot._intern
+0001c3e0: 616c 2e6d 6169 6e2e 6163 636f 756e 7427  al.main.account'
+0001c3f0: 292c 0a20 2020 2020 2020 2020 2020 2027  ),.            '
+0001c400: 6174 6578 6974 273a 206d 6f63 6b2e 7061  atexit': mock.pa
+0001c410: 7463 6828 2763 6572 7462 6f74 2e75 7469  tch('certbot.uti
+0001c420: 6c2e 6174 6578 6974 2729 2c0a 2020 2020  l.atexit'),.    
+0001c430: 2020 2020 2020 2020 2763 6c69 656e 7427          'client'
+0001c440: 3a20 6d6f 636b 2e70 6174 6368 2827 6365  : mock.patch('ce
+0001c450: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0001c460: 6d61 696e 2e63 6c69 656e 7427 292c 0a20  main.client'),. 
+0001c470: 2020 2020 2020 2020 2020 2027 6465 7465             'dete
+0001c480: 726d 696e 655f 6163 636f 756e 7427 3a20  rmine_account': 
+0001c490: 6d6f 636b 2e70 6174 6368 2827 6365 7274  mock.patch('cert
+0001c4a0: 626f 742e 5f69 6e74 6572 6e61 6c2e 6d61  bot._internal.ma
+0001c4b0: 696e 2e5f 6465 7465 726d 696e 655f 6163  in._determine_ac
+0001c4c0: 636f 756e 7427 292c 0a20 2020 2020 2020  count'),.       
+0001c4d0: 2020 2020 2027 6e6f 7469 6679 273a 206d       'notify': m
+0001c4e0: 6f63 6b2e 7061 7463 6828 2763 6572 7462  ock.patch('certb
+0001c4f0: 6f74 2e5f 696e 7465 726e 616c 2e6d 6169  ot._internal.mai
+0001c500: 6e2e 6469 7370 6c61 795f 7574 696c 2e6e  n.display_util.n
+0001c510: 6f74 6966 7927 292c 0a20 2020 2020 2020  otify'),.       
+0001c520: 2020 2020 2027 7574 696c 273a 2074 6573       'util': tes
+0001c530: 745f 7574 696c 2e70 6174 6368 5f64 6973  t_util.patch_dis
+0001c540: 706c 6179 5f75 7469 6c28 290a 2020 2020  play_util().    
+0001c550: 2020 2020 7d0a 2020 2020 2020 2020 7365      }.        se
+0001c560: 6c66 2e6d 6f63 6b73 203d 207b 206b 3a20  lf.mocks = { k: 
+0001c570: 7061 7463 6865 735b 6b5d 2e73 7461 7274  patches[k].start
+0001c580: 2829 2066 6f72 206b 2069 6e20 7061 7463  () for k in patc
+0001c590: 6865 7320 7d0a 2020 2020 2020 2020 666f  hes }.        fo
+0001c5a0: 7220 7061 7463 6820 696e 2070 6174 6368  r patch in patch
+0001c5b0: 6573 2e76 616c 7565 7328 293a 0a20 2020  es.values():.   
+0001c5c0: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+0001c5d0: 6443 6c65 616e 7570 2870 6174 6368 2e73  dCleanup(patch.s
+0001c5e0: 746f 7029 0a0a 2020 2020 2020 2020 7265  top)..        re
+0001c5f0: 7475 726e 2073 7570 6572 2829 2e73 6574  turn super().set
+0001c600: 5570 2829 0a0a 2020 2020 6465 6620 5f63  Up()..    def _c
+0001c610: 616c 6c28 7365 6c66 2c20 6172 6773 293a  all(self, args):
+0001c620: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
+0001c630: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+0001c640: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+0001c650: 2e73 7973 2e73 7464 6f75 7427 292c 205c  .sys.stdout'), \
+0001c660: 0a20 2020 2020 2020 2020 2020 2020 6d6f  .             mo
+0001c670: 636b 2e70 6174 6368 2827 6365 7274 626f  ck.patch('certbo
+0001c680: 742e 5f69 6e74 6572 6e61 6c2e 6d61 696e  t._internal.main
+0001c690: 2e73 7973 2e73 7464 6572 7227 293a 0a20  .sys.stderr'):. 
+0001c6a0: 2020 2020 2020 2020 2020 2061 7267 7320             args 
+0001c6b0: 3d20 5b27 2d2d 636f 6e66 6967 2d64 6972  = ['--config-dir
+0001c6c0: 272c 2073 656c 662e 636f 6e66 6967 2e63  ', self.config.c
+0001c6d0: 6f6e 6669 675f 6469 722c 0a20 2020 2020  onfig_dir,.     
+0001c6e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001c6f0: 2d2d 776f 726b 2d64 6972 272c 2073 656c  --work-dir', sel
+0001c700: 662e 636f 6e66 6967 2e77 6f72 6b5f 6469  f.config.work_di
+0001c710: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0001c720: 2020 2020 2020 2027 2d2d 6c6f 6773 2d64         '--logs-d
+0001c730: 6972 272c 2073 656c 662e 636f 6e66 6967  ir', self.config
+0001c740: 2e6c 6f67 735f 6469 722c 2027 2d2d 7465  .logs_dir, '--te
+0001c750: 7874 275d 202b 2061 7267 730a 2020 2020  xt'] + args.    
+0001c760: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+0001c770: 6169 6e2e 6d61 696e 2861 7267 735b 3a5d  ain.main(args[:]
+0001c780: 2920 2320 4e4f 5445 3a20 7061 7273 6572  ) # NOTE: parser
+0001c790: 2063 616e 2061 6c74 6572 2069 7473 2061   can alter its a
+0001c7a0: 7267 7321 0a0a 2020 2020 6465 6620 5f70  rgs!..    def _p
+0001c7b0: 7265 7061 7265 5f6d 6f63 6b5f 6163 636f  repare_mock_acco
+0001c7c0: 756e 7428 7365 6c66 293a 0a20 2020 2020  unt(self):.     
+0001c7d0: 2020 206d 6f63 6b5f 7374 6f72 6167 6520     mock_storage 
+0001c7e0: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
+0001c7f0: 2829 0a20 2020 2020 2020 206d 6f63 6b5f  ().        mock_
+0001c800: 6163 636f 756e 7420 3d20 6d6f 636b 2e4d  account = mock.M
+0001c810: 6167 6963 4d6f 636b 2829 0a20 2020 2020  agicMock().     
+0001c820: 2020 206d 6f63 6b5f 7265 6772 203d 206d     mock_regr = m
+0001c830: 6f63 6b2e 4d61 6769 634d 6f63 6b28 290a  ock.MagicMock().
+0001c840: 2020 2020 2020 2020 6d6f 636b 5f73 746f          mock_sto
+0001c850: 7261 6765 2e66 696e 645f 616c 6c2e 7265  rage.find_all.re
+0001c860: 7475 726e 5f76 616c 7565 203d 205b 6d6f  turn_value = [mo
+0001c870: 636b 5f61 6363 6f75 6e74 5d0a 2020 2020  ck_account].    
+0001c880: 2020 2020 7365 6c66 2e6d 6f63 6b73 5b27      self.mocks['
+0001c890: 6163 636f 756e 7427 5d2e 4163 636f 756e  account'].Accoun
+0001c8a0: 7446 696c 6553 746f 7261 6765 2e72 6574  tFileStorage.ret
+0001c8b0: 7572 6e5f 7661 6c75 6520 3d20 6d6f 636b  urn_value = mock
+0001c8c0: 5f73 746f 7261 6765 0a20 2020 2020 2020  _storage.       
+0001c8d0: 206d 6f63 6b5f 6163 636f 756e 742e 7265   mock_account.re
+0001c8e0: 6772 2e62 6f64 7920 3d20 6d6f 636b 5f72  gr.body = mock_r
+0001c8f0: 6567 722e 626f 6479 0a20 2020 2020 2020  egr.body.       
+0001c900: 206d 6f63 6b5f 6163 636f 756e 742e 6b65   mock_account.ke
+0001c910: 792e 7468 756d 6270 7269 6e74 2e72 6574  y.thumbprint.ret
+0001c920: 7572 6e5f 7661 6c75 6520 3d20 6227 666f  urn_value = b'fo
+0001c930: 6f62 6172 6261 7a27 0a20 2020 2020 2020  obarbaz'.       
+0001c940: 2073 656c 662e 6d6f 636b 735b 2764 6574   self.mocks['det
+0001c950: 6572 6d69 6e65 5f61 6363 6f75 6e74 275d  ermine_account']
+0001c960: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+0001c970: 286d 6f63 6b5f 6163 636f 756e 742c 206d  (mock_account, m
+0001c980: 6f63 6b2e 4d61 6769 634d 6f63 6b28 2929  ock.MagicMock())
+0001c990: 0a0a 2020 2020 6465 6620 5f74 6573 745f  ..    def _test_
+0001c9a0: 7368 6f77 5f61 6363 6f75 6e74 2873 656c  show_account(sel
+0001c9b0: 662c 2063 6f6e 7461 6374 293a 0a20 2020  f, contact):.   
+0001c9c0: 2020 2020 2073 656c 662e 5f70 7265 7061       self._prepa
+0001c9d0: 7265 5f6d 6f63 6b5f 6163 636f 756e 7428  re_mock_account(
+0001c9e0: 290a 2020 2020 2020 2020 6d6f 636b 5f63  ).        mock_c
+0001c9f0: 6c69 656e 7420 3d20 6d6f 636b 2e4d 6167  lient = mock.Mag
+0001ca00: 6963 4d6f 636b 2829 0a20 2020 2020 2020  icMock().       
+0001ca10: 206d 6f63 6b5f 7265 6772 203d 206d 6f63   mock_regr = moc
+0001ca20: 6b2e 4d61 6769 634d 6f63 6b28 290a 2020  k.MagicMock().  
+0001ca30: 2020 2020 2020 6d6f 636b 5f72 6567 722e        mock_regr.
+0001ca40: 626f 6479 2e63 6f6e 7461 6374 203d 2063  body.contact = c
+0001ca50: 6f6e 7461 6374 0a20 2020 2020 2020 206d  ontact.        m
+0001ca60: 6f63 6b5f 7265 6772 2e75 7269 203d 2027  ock_regr.uri = '
+0001ca70: 6874 7470 733a 2f2f 7777 772e 6c65 7473  https://www.lets
+0001ca80: 656e 6372 7970 742d 6465 6d6f 2e6f 7267  encrypt-demo.org
+0001ca90: 2f61 636d 652f 7265 672f 3127 0a20 2020  /acme/reg/1'.   
+0001caa0: 2020 2020 206d 6f63 6b5f 636c 6965 6e74       mock_client
+0001cab0: 2e61 636d 652e 7175 6572 795f 7265 6769  .acme.query_regi
+0001cac0: 7374 7261 7469 6f6e 2e72 6574 7572 6e5f  stration.return_
+0001cad0: 7661 6c75 6520 3d20 6d6f 636b 5f72 6567  value = mock_reg
+0001cae0: 720a 2020 2020 2020 2020 7365 6c66 2e6d  r.        self.m
+0001caf0: 6f63 6b73 5b27 636c 6965 6e74 275d 2e43  ocks['client'].C
+0001cb00: 6c69 656e 742e 7265 7475 726e 5f76 616c  lient.return_val
+0001cb10: 7565 203d 206d 6f63 6b5f 636c 6965 6e74  ue = mock_client
+0001cb20: 0a0a 2020 2020 2020 2020 6172 6773 203d  ..        args =
+0001cb30: 205b 2773 686f 775f 6163 636f 756e 7427   ['show_account'
+0001cb40: 5d0a 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+0001cb50: 5f63 616c 6c28 6172 6773 290a 0a20 2020  _call(args)..   
+0001cb60: 2020 2020 2061 7373 6572 7420 6d6f 636b       assert mock
+0001cb70: 5f63 6c69 656e 742e 6163 6d65 2e71 7565  _client.acme.que
+0001cb80: 7279 5f72 6567 6973 7472 6174 696f 6e2e  ry_registration.
+0001cb90: 6361 6c6c 5f63 6f75 6e74 203d 3d20 310a  call_count == 1.
+0001cba0: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
+0001cbb0: 5f65 7869 7374 696e 675f 6163 636f 756e  _existing_accoun
+0001cbc0: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+0001cbd0: 2020 2222 2254 6573 7420 7468 6174 206e    """Test that n
+0001cbe0: 6f20 6578 6973 7469 6e67 2061 6363 6f75  o existing accou
+0001cbf0: 6e74 2069 7320 6861 6e64 6c65 6420 636f  nt is handled co
+0001cc00: 7272 6563 746c 7922 2222 0a20 2020 2020  rrectly""".     
+0001cc10: 2020 206d 6f63 6b5f 7374 6f72 6167 6520     mock_storage 
+0001cc20: 3d20 6d6f 636b 2e4d 6167 6963 4d6f 636b  = mock.MagicMock
+0001cc30: 2829 0a20 2020 2020 2020 206d 6f63 6b5f  ().        mock_
+0001cc40: 7374 6f72 6167 652e 6669 6e64 5f61 6c6c  storage.find_all
+0001cc50: 2e72 6574 7572 6e5f 7661 6c75 6520 3d20  .return_value = 
+0001cc60: 5b5d 0a20 2020 2020 2020 2073 656c 662e  [].        self.
+0001cc70: 6d6f 636b 735b 2761 6363 6f75 6e74 275d  mocks['account']
+0001cc80: 2e41 6363 6f75 6e74 4669 6c65 5374 6f72  .AccountFileStor
+0001cc90: 6167 652e 7265 7475 726e 5f76 616c 7565  age.return_value
+0001cca0: 203d 206d 6f63 6b5f 7374 6f72 6167 650a   = mock_storage.
+0001ccb0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0001ccc0: 656c 662e 5f63 616c 6c28 5b27 7368 6f77  elf._call(['show
+0001ccd0: 5f61 6363 6f75 6e74 275d 2920 3d3d 205c  _account']) == \
+0001cce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ccf0: 2020 2020 2020 2020 2020 2743 6f75 6c64            'Could
+0001cd00: 206e 6f74 2066 696e 6420 616e 2065 7869   not find an exi
+0001cd10: 7374 696e 6720 6163 636f 756e 7420 666f  sting account fo
+0001cd20: 7220 7365 7276 6572 2720 5c0a 2020 2020  r server' \.    
+0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd40: 2020 2020 2027 2068 7474 7073 3a2f 2f61       ' https://a
+0001cd50: 636d 652d 7630 322e 6170 692e 6c65 7473  cme-v02.api.lets
+0001cd60: 656e 6372 7970 742e 6f72 672f 6469 7265  encrypt.org/dire
+0001cd70: 6374 6f72 792e 270a 0a20 2020 2064 6566  ctory.'..    def
+0001cd80: 2074 6573 745f 6e6f 5f65 7869 7374 696e   test_no_existin
+0001cd90: 675f 636c 6965 6e74 2873 656c 6629 3a0a  g_client(self):.
+0001cda0: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
+0001cdb0: 7468 6174 2069 7373 7565 7320 7769 7468  that issues with
+0001cdc0: 2074 6865 2041 434d 4520 636c 6965 6e74   the ACME client
+0001cdd0: 2061 7265 2068 616e 646c 6564 2063 6f72   are handled cor
+0001cde0: 7265 6374 6c79 2222 220a 2020 2020 2020  rectly""".      
+0001cdf0: 2020 7365 6c66 2e5f 7072 6570 6172 655f    self._prepare_
+0001ce00: 6d6f 636b 5f61 6363 6f75 6e74 2829 0a20  mock_account(). 
+0001ce10: 2020 2020 2020 206d 6f63 6b5f 636c 6965         mock_clie
+0001ce20: 6e74 203d 206d 6f63 6b2e 4d61 6769 634d  nt = mock.MagicM
+0001ce30: 6f63 6b28 290a 2020 2020 2020 2020 6d6f  ock().        mo
+0001ce40: 636b 5f63 6c69 656e 742e 6163 6d65 203d  ck_client.acme =
+0001ce50: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0001ce60: 6c66 2e6d 6f63 6b73 5b27 636c 6965 6e74  lf.mocks['client
+0001ce70: 275d 2e43 6c69 656e 742e 7265 7475 726e  '].Client.return
+0001ce80: 5f76 616c 7565 203d 206d 6f63 6b5f 636c  _value = mock_cl
+0001ce90: 6965 6e74 0a20 2020 2020 2020 2074 7279  ient.        try
+0001cea0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001ceb0: 6c66 2e5f 6361 6c6c 285b 2773 686f 775f  lf._call(['show_
+0001cec0: 6163 636f 756e 7427 5d29 0a20 2020 2020  account']).     
+0001ced0: 2020 2065 7863 6570 7420 6572 726f 7273     except errors
+0001cee0: 2e45 7272 6f72 2061 7320 653a 0a20 2020  .Error as e:.   
+0001cef0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0001cf00: 2741 434d 4520 636c 6965 6e74 2069 7320  'ACME client is 
+0001cf10: 6e6f 7420 7365 742e 2720 3d3d 2073 7472  not set.' == str
+0001cf20: 2865 290a 0a20 2020 2064 6566 2074 6573  (e)..    def tes
+0001cf30: 745f 6e6f 5f63 6f6e 7461 6374 7328 7365  t_no_contacts(se
+0001cf40: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0001cf50: 662e 5f74 6573 745f 7368 6f77 5f61 6363  f._test_show_acc
+0001cf60: 6f75 6e74 2828 2929 0a0a 2020 2020 2020  ount(())..      
+0001cf70: 2020 6173 7365 7274 2073 656c 662e 6d6f    assert self.mo
+0001cf80: 636b 735b 276e 6f74 6966 7927 5d2e 6361  cks['notify'].ca
+0001cf90: 6c6c 5f63 6f75 6e74 203d 3d20 310a 2020  ll_count == 1.  
+0001cfa0: 2020 2020 2020 7365 6c66 2e6d 6f63 6b73        self.mocks
+0001cfb0: 5b27 6e6f 7469 6679 275d 2e61 7373 6572  ['notify'].asser
+0001cfc0: 745f 6861 735f 6361 6c6c 7328 5b0a 2020  t_has_calls([.  
+0001cfd0: 2020 2020 2020 2020 2020 6d6f 636b 2e63            mock.c
+0001cfe0: 616c 6c28 2741 6363 6f75 6e74 2064 6574  all('Account det
+0001cff0: 6169 6c73 2066 6f72 2073 6572 7665 7220  ails for server 
+0001d000: 6874 7470 733a 2f2f 6163 6d65 2d76 3032  https://acme-v02
+0001d010: 2e61 7069 2e6c 6574 7365 6e63 7227 0a20  .api.letsencr'. 
+0001d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d030: 2020 2020 2027 7970 742e 6f72 672f 6469       'ypt.org/di
+0001d040: 7265 6374 6f72 793a 5c6e 2020 4163 636f  rectory:\n  Acco
+0001d050: 756e 7420 5552 4c3a 2068 7474 7073 3a2f  unt URL: https:/
+0001d060: 2f77 7777 2e6c 6574 7365 6e63 7279 270a  /www.letsencry'.
+0001d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d080: 2020 2020 2020 2770 742d 6465 6d6f 2e6f        'pt-demo.o
+0001d090: 7267 2f61 636d 652f 7265 672f 315c 6e20  rg/acme/reg/1\n 
+0001d0a0: 2041 6363 6f75 6e74 2054 6875 6d62 7072   Account Thumbpr
+0001d0b0: 696e 743a 205a 6d39 7659 6d46 7959 6d46  int: Zm9vYmFyYmF
+0001d0c0: 365c 6e27 0a20 2020 2020 2020 2020 2020  6\n'.           
+0001d0d0: 2020 2020 2020 2020 2020 2027 2020 456d             '  Em
+0001d0e0: 6169 6c20 636f 6e74 6163 743a 206e 6f6e  ail contact: non
+0001d0f0: 6527 295d 290a 0a20 2020 2064 6566 2074  e')])..    def t
+0001d100: 6573 745f 7369 6e67 6c65 5f65 6d61 696c  est_single_email
+0001d110: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001d120: 636f 6e74 6163 7420 3d20 2827 6d61 696c  contact = ('mail
+0001d130: 746f 3a66 6f6f 4065 7861 6d70 6c65 2e63  to:foo@example.c
+0001d140: 6f6d 272c 290a 2020 2020 2020 2020 7365  om',).        se
+0001d150: 6c66 2e5f 7465 7374 5f73 686f 775f 6163  lf._test_show_ac
+0001d160: 636f 756e 7428 636f 6e74 6163 7429 0a0a  count(contact)..
+0001d170: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0001d180: 656c 662e 6d6f 636b 735b 276e 6f74 6966  elf.mocks['notif
+0001d190: 7927 5d2e 6361 6c6c 5f63 6f75 6e74 203d  y'].call_count =
+0001d1a0: 3d20 310a 2020 2020 2020 2020 7365 6c66  = 1.        self
+0001d1b0: 2e6d 6f63 6b73 5b27 6e6f 7469 6679 275d  .mocks['notify']
+0001d1c0: 2e61 7373 6572 745f 6861 735f 6361 6c6c  .assert_has_call
+0001d1d0: 7328 5b0a 2020 2020 2020 2020 2020 2020  s([.            
+0001d1e0: 6d6f 636b 2e63 616c 6c28 2741 6363 6f75  mock.call('Accou
+0001d1f0: 6e74 2064 6574 6169 6c73 2066 6f72 2073  nt details for s
+0001d200: 6572 7665 7220 6874 7470 733a 2f2f 6163  erver https://ac
+0001d210: 6d65 2d76 3032 2e61 7069 2e6c 6574 7365  me-v02.api.letse
+0001d220: 6e63 7227 0a20 2020 2020 2020 2020 2020  ncr'.           
+0001d230: 2020 2020 2020 2020 2020 2027 7970 742e             'ypt.
+0001d240: 6f72 672f 6469 7265 6374 6f72 793a 5c6e  org/directory:\n
+0001d250: 2020 4163 636f 756e 7420 5552 4c3a 2068    Account URL: h
+0001d260: 7474 7073 3a2f 2f77 7777 2e6c 6574 7365  ttps://www.letse
+0001d270: 6e63 7279 270a 2020 2020 2020 2020 2020  ncry'.          
+0001d280: 2020 2020 2020 2020 2020 2020 2770 742d              'pt-
+0001d290: 6465 6d6f 2e6f 7267 2f61 636d 652f 7265  demo.org/acme/re
+0001d2a0: 672f 315c 6e20 2041 6363 6f75 6e74 2054  g/1\n  Account T
+0001d2b0: 6875 6d62 7072 696e 743a 205a 6d39 7659  humbprint: Zm9vY
+0001d2c0: 6d46 7959 6d46 3627 0a20 2020 2020 2020  mFyYmF6'.       
+0001d2d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001d2e0: 5c6e 2020 456d 6169 6c20 636f 6e74 6163  \n  Email contac
+0001d2f0: 743a 2066 6f6f 4065 7861 6d70 6c65 2e63  t: foo@example.c
+0001d300: 6f6d 2729 5d29 0a0a 2020 2020 6465 6620  om')])..    def 
+0001d310: 7465 7374 5f64 6f75 626c 655f 656d 6169  test_double_emai
+0001d320: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
+0001d330: 2063 6f6e 7461 6374 203d 2028 276d 6169   contact = ('mai
+0001d340: 6c74 6f3a 666f 6f40 6578 616d 706c 652e  lto:foo@example.
+0001d350: 636f 6d27 2c20 276d 6169 6c74 6f3a 6261  com', 'mailto:ba
+0001d360: 7240 6578 616d 706c 652e 636f 6d27 290a  r@example.com').
+0001d370: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0001d380: 7374 5f73 686f 775f 6163 636f 756e 7428  st_show_account(
+0001d390: 636f 6e74 6163 7429 0a0a 2020 2020 2020  contact)..      
+0001d3a0: 2020 6173 7365 7274 2073 656c 662e 6d6f    assert self.mo
+0001d3b0: 636b 735b 276e 6f74 6966 7927 5d2e 6361  cks['notify'].ca
+0001d3c0: 6c6c 5f63 6f75 6e74 203d 3d20 310a 2020  ll_count == 1.  
+0001d3d0: 2020 2020 2020 7365 6c66 2e6d 6f63 6b73        self.mocks
+0001d3e0: 5b27 6e6f 7469 6679 275d 2e61 7373 6572  ['notify'].asser
+0001d3f0: 745f 6861 735f 6361 6c6c 7328 5b0a 2020  t_has_calls([.  
+0001d400: 2020 2020 2020 2020 2020 6d6f 636b 2e63            mock.c
+0001d410: 616c 6c28 2741 6363 6f75 6e74 2064 6574  all('Account det
+0001d420: 6169 6c73 2066 6f72 2073 6572 7665 7220  ails for server 
+0001d430: 6874 7470 733a 2f2f 6163 6d65 2d76 3032  https://acme-v02
+0001d440: 2e61 7069 2e6c 6574 7365 6e63 7227 0a20  .api.letsencr'. 
+0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d460: 2020 2020 2027 7970 742e 6f72 672f 6469       'ypt.org/di
+0001d470: 7265 6374 6f72 793a 5c6e 2020 4163 636f  rectory:\n  Acco
+0001d480: 756e 7420 5552 4c3a 2068 7474 7073 3a2f  unt URL: https:/
+0001d490: 2f77 7777 2e6c 6574 7365 6e63 7279 270a  /www.letsencry'.
+0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4b0: 2020 2020 2020 2770 742d 6465 6d6f 2e6f        'pt-demo.o
+0001d4c0: 7267 2f61 636d 652f 7265 672f 315c 6e20  rg/acme/reg/1\n 
+0001d4d0: 2041 6363 6f75 6e74 2054 6875 6d62 7072   Account Thumbpr
+0001d4e0: 696e 743a 205a 6d39 7659 6d46 7959 6d46  int: Zm9vYmFyYmF
+0001d4f0: 365c 6e27 0a20 2020 2020 2020 2020 2020  6\n'.           
+0001d500: 2020 2020 2020 2020 2020 2027 2020 456d             '  Em
+0001d510: 6169 6c20 636f 6e74 6163 7473 3a20 666f  ail contacts: fo
+0001d520: 6f40 6578 616d 706c 652e 636f 6d2c 2062  o@example.com, b
+0001d530: 6172 4065 7861 6d70 6c65 2e63 6f6d 2729  ar@example.com')
+0001d540: 5d29 0a0a 0a63 6c61 7373 2054 6573 744c  ])...class TestL
+0001d550: 6f63 6b4f 7264 6572 3a0a 2020 2020 2222  ockOrder:.    ""
+0001d560: 2254 6573 7473 2074 6861 7420 4365 7274  "Tests that Cert
+0001d570: 626f 7427 7320 6469 7265 6374 6f72 7920  bot's directory 
+0001d580: 6c6f 636b 7320 7765 7265 2061 6371 7569  locks were acqui
+0001d590: 7265 6420 696e 2074 6865 2072 6967 6874  red in the right
+0001d5a0: 206f 7264 6572 2e22 2222 0a20 2020 2045   order.""".    E
+0001d5b0: 5850 4543 5445 445f 4552 524f 525f 5459  XPECTED_ERROR_TY
+0001d5c0: 5045 203d 2065 7272 6f72 732e 4572 726f  PE = errors.Erro
+0001d5d0: 720a 2020 2020 4558 5045 4354 4544 5f45  r.    EXPECTED_E
+0001d5e0: 5252 4f52 5f53 5452 203d 2027 4578 7065  RROR_STR = 'Expe
+0001d5f0: 6374 6564 2054 6573 744c 6f63 6b4f 7264  cted TestLockOrd
+0001d600: 6572 2065 7272 6f72 270a 2020 2020 2320  er error'.    # 
+0001d610: 5468 6973 2072 6567 6578 2069 7320 6e65  This regex is ne
+0001d620: 6564 6564 2062 6563 6175 7365 2063 6572  eded because cer
+0001d630: 7462 6f74 2072 656e 6577 2063 6170 7475  tbot renew captu
+0001d640: 7265 7320 7261 6973 6564 2065 7272 6f72  res raised error
+0001d650: 7320 616e 640a 2020 2020 2320 7261 6973  s and.    # rais
+0001d660: 6573 2069 7473 206f 776e 2e0a 2020 2020  es its own..    
+0001d670: 4558 5045 4354 4544 5f45 5252 4f52 5f53  EXPECTED_ERROR_S
+0001d680: 5452 5f52 4547 4558 203d 2066 277b 4558  TR_REGEX = f'{EX
+0001d690: 5045 4354 4544 5f45 5252 4f52 5f53 5452  PECTED_ERROR_STR
+0001d6a0: 7d7c 3120 7265 6e65 7720 6661 696c 7572  }|1 renew failur
+0001d6b0: 6527 0a0a 2020 2020 4070 7974 6573 742e  e'..    @pytest.
+0001d6c0: 6669 7874 7572 650a 2020 2020 6465 6620  fixture.    def 
+0001d6d0: 6d6f 636b 5f6c 6f63 6b5f 6469 7228 7365  mock_lock_dir(se
+0001d6e0: 6c66 293a 0a20 2020 2020 2020 2077 6974  lf):.        wit
+0001d6f0: 6820 6d6f 636b 2e70 6174 6368 2827 6365  h mock.patch('ce
+0001d700: 7274 626f 742e 5f69 6e74 6572 6e61 6c2e  rtbot._internal.
+0001d710: 6c6f 636b 2e6c 6f63 6b5f 6469 7227 2920  lock.lock_dir') 
+0001d720: 6173 206d 6f63 6b5f 6c6f 636b 5f64 6972  as mock_lock_dir
+0001d730: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
+0001d740: 656c 6420 6d6f 636b 5f6c 6f63 6b5f 6469  eld mock_lock_di
+0001d750: 720a 0a20 2020 2040 636f 6e74 6578 746c  r..    @contextl
+0001d760: 6962 2e63 6f6e 7465 7874 6d61 6e61 6765  ib.contextmanage
+0001d770: 720a 2020 2020 6465 6620 6d6f 636b 5f70  r.    def mock_p
+0001d780: 6c75 6769 6e5f 7072 6570 6172 6528 7365  lugin_prepare(se
+0001d790: 6c66 2c20 6175 7468 656e 7469 6361 746f  lf, authenticato
+0001d7a0: 725f 6469 722c 2069 6e73 7461 6c6c 6572  r_dir, installer
+0001d7b0: 5f64 6972 2c20 6d6f 636b 5f6c 6f63 6b5f  _dir, mock_lock_
+0001d7c0: 6469 722c 2073 7562 636f 6d6d 616e 6429  dir, subcommand)
+0001d7d0: 3a0a 2020 2020 2020 2020 2222 2250 6174  :.        """Pat
+0001d7e0: 6368 6573 2070 6c75 6769 6e20 7072 6570  ches plugin prep
+0001d7f0: 6172 6520 746f 2063 616c 6c20 6d6f 636b  are to call mock
+0001d800: 5f6c 6f63 6b5f 6469 7220 616e 6420 7261  _lock_dir and ra
+0001d810: 6973 6520 7468 6520 6578 7065 6374 6564  ise the expected
+0001d820: 2065 7272 6f72 2e22 2222 0a20 2020 2020   error.""".     
+0001d830: 2020 2064 6566 2061 7574 6865 6e74 6963     def authentic
+0001d840: 6174 6f72 5f6c 6f63 6b28 756e 7573 6564  ator_lock(unused
+0001d850: 5f73 656c 6629 3a0a 2020 2020 2020 2020  _self):.        
+0001d860: 2020 2020 6d6f 636b 5f6c 6f63 6b5f 6469      mock_lock_di
+0001d870: 7228 6175 7468 656e 7469 6361 746f 725f  r(authenticator_
+0001d880: 6469 7229 0a20 2020 2020 2020 2020 2020  dir).           
+0001d890: 2072 6169 7365 2073 656c 662e 4558 5045   raise self.EXPE
+0001d8a0: 4354 4544 5f45 5252 4f52 5f54 5950 4528  CTED_ERROR_TYPE(
+0001d8b0: 7365 6c66 2e45 5850 4543 5445 445f 4552  self.EXPECTED_ER
+0001d8c0: 524f 525f 5354 5229 0a0a 2020 2020 2020  ROR_STR)..      
+0001d8d0: 2020 6465 6620 696e 7374 616c 6c65 725f    def installer_
+0001d8e0: 6c6f 636b 2875 6e75 7365 645f 7365 6c66  lock(unused_self
+0001d8f0: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
+0001d900: 6f63 6b5f 6c6f 636b 5f64 6972 2869 6e73  ock_lock_dir(ins
+0001d910: 7461 6c6c 6572 5f64 6972 290a 2020 2020  taller_dir).    
+0001d920: 2020 2020 2020 2020 2320 556e 6c65 7373          # Unless
+0001d930: 2061 6e20 696e 7374 616c 6c65 7220 6973   an installer is
+0001d940: 6e27 7420 6e65 6564 6564 2028 652e 672e  n't needed (e.g.
+0001d950: 2063 6572 7462 6f74 2069 6e73 7461 6c6c   certbot install
+0001d960: 292c 2077 650a 2020 2020 2020 2020 2020  ), we.          
+0001d970: 2020 2320 6578 7065 6374 2074 6865 2061    # expect the a
+0001d980: 7574 6865 6e74 6963 6174 6f72 2074 6f20  uthenticator to 
+0001d990: 7261 6973 6520 7468 6520 6578 7065 6374  raise the expect
+0001d9a0: 6564 2065 7272 6f72 2062 6563 6175 7365  ed error because
+0001d9b0: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+0001d9c0: 2320 6973 2070 7265 7061 7265 6420 6c61  # is prepared la
+0001d9d0: 7374 2e20 5365 650a 2020 2020 2020 2020  st. See.        
+0001d9e0: 2020 2020 2320 6874 7470 733a 2f2f 6769      # https://gi
+0001d9f0: 7468 7562 2e63 6f6d 2f63 6572 7462 6f74  thub.com/certbot
+0001da00: 2f63 6572 7462 6f74 2f62 6c6f 622f 3761  /certbot/blob/7a
+0001da10: 3637 3532 6136 3865 6437 3765 3733 6332  6752a68ed77e73c2
+0001da20: 6232 3961 6232 3064 3363 6138 3932 3766  b29ab20d3ca8927f
+0001da30: 3466 6137 6230 2f63 6572 7462 6f74 2f63  4fa7b0/certbot/c
+0001da40: 6572 7462 6f74 2f5f 696e 7465 726e 616c  ertbot/_internal
+0001da50: 2f70 6c75 6769 6e73 2f73 656c 6563 7469  /plugins/selecti
+0001da60: 6f6e 2e70 7923 4c32 3436 2d4c 3234 390a  on.py#L246-L249.
+0001da70: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001da80: 7562 636f 6d6d 616e 6420 3d3d 2027 696e  ubcommand == 'in
+0001da90: 7374 616c 6c27 3a0a 2020 2020 2020 2020  stall':.        
+0001daa0: 2020 2020 2020 2020 7261 6973 6520 7365          raise se
+0001dab0: 6c66 2e45 5850 4543 5445 445f 4552 524f  lf.EXPECTED_ERRO
+0001dac0: 525f 5459 5045 2873 656c 662e 4558 5045  R_TYPE(self.EXPE
+0001dad0: 4354 4544 5f45 5252 4f52 5f53 5452 290a  CTED_ERROR_STR).
+0001dae0: 0a20 2020 2020 2020 2077 6974 6820 6d6f  .        with mo
+0001daf0: 636b 2e70 6174 6368 2e6f 626a 6563 7428  ck.patch.object(
+0001db00: 7374 616e 6461 6c6f 6e65 2e41 7574 6865  standalone.Authe
+0001db10: 6e74 6963 6174 6f72 2c20 2770 7265 7061  nticator, 'prepa
+0001db20: 7265 272c 2061 7574 6865 6e74 6963 6174  re', authenticat
+0001db30: 6f72 5f6c 6f63 6b29 3a0a 2020 2020 2020  or_lock):.      
+0001db40: 2020 2020 2020 7769 7468 206d 6f63 6b2e        with mock.
+0001db50: 7061 7463 682e 6f62 6a65 6374 286e 756c  patch.object(nul
+0001db60: 6c2e 496e 7374 616c 6c65 722c 2027 7072  l.Installer, 'pr
+0001db70: 6570 6172 6527 2c20 696e 7374 616c 6c65  epare', installe
+0001db80: 725f 6c6f 636b 293a 0a20 2020 2020 2020  r_lock):.       
+0001db90: 2020 2020 2020 2020 2079 6965 6c64 0a0a           yield..
+0001dba0: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+0001dbb0: 7572 6528 7061 7261 6d73 3d27 6365 7274  ure(params='cert
+0001dbc0: 6f6e 6c79 2069 6e73 7461 6c6c 2072 656e  only install ren
+0001dbd0: 6577 2072 756e 272e 7370 6c69 7428 2929  ew run'.split())
+0001dbe0: 0a20 2020 2064 6566 2061 7267 735f 616e  .    def args_an
+0001dbf0: 645f 6c6f 636b 5f6f 7264 6572 2873 656c  d_lock_order(sel
+0001dc00: 662c 206d 6f63 6b5f 6c6f 636b 5f64 6972  f, mock_lock_dir
+0001dc10: 2c20 7265 7175 6573 742c 2074 6d70 5f70  , request, tmp_p
+0001dc20: 6174 6829 3a0a 2020 2020 2020 2020 2222  ath):.        ""
+0001dc30: 2253 6574 7320 7570 2043 6572 7462 6f74  "Sets up Certbot
+0001dc40: 2077 6974 6820 6172 6773 2061 6e64 206d   with args and m
+0001dc50: 6f63 6b73 2074 6f20 6572 726f 7220 6166  ocks to error af
+0001dc60: 7465 7220 6163 7175 6972 696e 6720 7468  ter acquiring th
+0001dc70: 6520 6c61 7374 206c 6f63 6b2e 0a0a 2020  e last lock...  
+0001dc80: 2020 2020 2020 5468 6973 2066 6978 7475        This fixtu
+0001dc90: 7265 2079 6965 6c64 7320 7468 6520 434c  re yields the CL
+0001dca0: 4920 6172 6775 6d65 6e74 7320 7468 6174  I arguments that
+0001dcb0: 2073 686f 756c 6420 6265 2067 6976 656e   should be given
+0001dcc0: 2074 6f20 4365 7274 626f 740a 2020 2020   to Certbot.    
+0001dcd0: 2020 2020 616e 6420 7468 6520 6578 7065      and the expe
+0001dce0: 6374 6564 206f 7264 6572 206f 6620 6469  cted order of di
+0001dcf0: 7265 6374 6f72 6965 7320 746f 2062 6520  rectories to be 
+0001dd00: 6c6f 636b 6564 2e20 416e 2065 7272 6f72  locked. An error
+0001dd10: 2069 7320 7261 6973 6564 0a20 2020 2020   is raised.     
+0001dd20: 2020 2061 6674 6572 2061 6371 7569 7269     after acquiri
+0001dd30: 6e67 2074 6865 206c 6173 7420 6c6f 636b  ng the last lock
+0001dd40: 206a 7573 7420 6173 2061 206d 6561 6e73   just as a means
+0001dd50: 206f 6620 7374 6f70 7069 6e67 2043 6572   of stopping Cer
+0001dd60: 7462 6f74 2773 0a20 2020 2020 2020 2065  tbot's.        e
+0001dd70: 7865 6375 7469 6f6e 2e0a 0a20 2020 2020  xecution...     
+0001dd80: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+0001dd90: 2073 656c 6563 7420 6469 7265 6374 6f72   select director
+0001dda0: 6965 730a 2020 2020 2020 2020 6175 7468  ies.        auth
+0001ddb0: 656e 7469 6361 746f 725f 6469 7220 3d20  enticator_dir = 
+0001ddc0: 7374 7228 746d 705f 7061 7468 202f 2027  str(tmp_path / '
+0001ddd0: 6175 7468 656e 7469 6361 746f 7227 290a  authenticator').
+0001dde0: 2020 2020 2020 2020 636f 6e66 6967 5f64          config_d
+0001ddf0: 6972 203d 2073 7472 2874 6d70 5f70 6174  ir = str(tmp_pat
+0001de00: 6820 2f20 2763 6f6e 6669 6727 290a 2020  h / 'config').  
+0001de10: 2020 2020 2020 696e 7374 616c 6c65 725f        installer_
+0001de20: 6469 7220 3d20 7374 7228 746d 705f 7061  dir = str(tmp_pa
+0001de30: 7468 202f 2027 696e 7374 616c 6c65 7227  th / 'installer'
+0001de40: 290a 2020 2020 2020 2020 6c6f 6773 5f64  ).        logs_d
+0001de50: 6972 203d 2073 7472 2874 6d70 5f70 6174  ir = str(tmp_pat
+0001de60: 6820 2f20 276c 6f67 7327 290a 2020 2020  h / 'logs').    
+0001de70: 2020 2020 776f 726b 5f64 6972 203d 2073      work_dir = s
+0001de80: 7472 2874 6d70 5f70 6174 6820 2f20 2777  tr(tmp_path / 'w
+0001de90: 6f72 6b27 290a 0a20 2020 2020 2020 2023  ork')..        #
+0001dea0: 2070 7265 7061 7265 2061 7267 7320 616e   prepare args an
+0001deb0: 6420 6c69 6e65 6167 650a 2020 2020 2020  d lineage.      
+0001dec0: 2020 7375 6263 6f6d 6d61 6e64 203d 2072    subcommand = r
+0001ded0: 6571 7565 7374 2e70 6172 616d 0a20 2020  equest.param.   
+0001dee0: 2020 2020 2061 7267 7320 3d20 5b73 7562       args = [sub
+0001def0: 636f 6d6d 616e 642c 2027 2d61 272c 2027  command, '-a', '
+0001df00: 7374 616e 6461 6c6f 6e65 272c 2027 2d69  standalone', '-i
+0001df10: 272c 2027 6e75 6c6c 272c 2027 2d2d 6e6f  ', 'null', '--no
+0001df20: 2d72 616e 646f 6d2d 736c 6565 702d 6f6e  -random-sleep-on
+0001df30: 2d72 656e 6577 272c 0a20 2020 2020 2020  -renew',.       
+0001df40: 2020 2020 2020 2020 2027 2d2d 636f 6e66           '--conf
+0001df50: 6967 2d64 6972 272c 2063 6f6e 6669 675f  ig-dir', config_
+0001df60: 6469 722c 2027 2d2d 6c6f 6773 2d64 6972  dir, '--logs-dir
+0001df70: 272c 206c 6f67 735f 6469 722c 2027 2d2d  ', logs_dir, '--
+0001df80: 776f 726b 2d64 6972 272c 0a20 2020 2020  work-dir',.     
+0001df90: 2020 2020 2020 2020 2020 2077 6f72 6b5f             work_
+0001dfa0: 6469 725d 0a20 2020 2020 2020 2074 6573  dir].        tes
+0001dfb0: 745f 7574 696c 2e6d 616b 655f 6c69 6e65  t_util.make_line
+0001dfc0: 6167 6528 636f 6e66 6967 5f64 6972 2c20  age(config_dir, 
+0001dfd0: 2773 616d 706c 652d 7265 6e65 7761 6c2e  'sample-renewal.
+0001dfe0: 636f 6e66 2729 0a0a 2020 2020 2020 2020  conf')..        
+0001dff0: 7769 7468 2073 656c 662e 6d6f 636b 5f70  with self.mock_p
+0001e000: 6c75 6769 6e5f 7072 6570 6172 6528 6175  lugin_prepare(au
+0001e010: 7468 656e 7469 6361 746f 725f 6469 722c  thenticator_dir,
+0001e020: 2069 6e73 7461 6c6c 6572 5f64 6972 2c20   installer_dir, 
+0001e030: 6d6f 636b 5f6c 6f63 6b5f 6469 722c 2073  mock_lock_dir, s
+0001e040: 7562 636f 6d6d 616e 6429 3a0a 2020 2020  ubcommand):.    
+0001e050: 2020 2020 2020 2020 6c6f 636b 5f6f 7264          lock_ord
+0001e060: 6572 203d 205b 6c6f 6773 5f64 6972 2c20  er = [logs_dir, 
+0001e070: 636f 6e66 6967 5f64 6972 2c20 776f 726b  config_dir, work
+0001e080: 5f64 6972 2c20 696e 7374 616c 6c65 725f  _dir, installer_
+0001e090: 6469 725d 0a20 2020 2020 2020 2020 2020  dir].           
+0001e0a0: 2069 6620 7375 6263 6f6d 6d61 6e64 203d   if subcommand =
+0001e0b0: 3d20 2769 6e73 7461 6c6c 273a 0a20 2020  = 'install':.   
+0001e0c0: 2020 2020 2020 2020 2020 2020 2079 6965               yie
+0001e0d0: 6c64 2061 7267 732c 206c 6f63 6b5f 6f72  ld args, lock_or
+0001e0e0: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
+0001e0f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001e100: 2020 2020 2020 2320 5765 2065 7870 6563        # We expec
+0001e110: 7420 7468 6520 696e 7374 616c 6c65 7220  t the installer 
+0001e120: 746f 2062 6520 7072 6570 6172 6564 2065  to be prepared e
+0001e130: 7665 6e20 666f 7220 6365 7274 6f6e 6c79  ven for certonly
+0001e140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e150: 2023 2062 6563 6175 7365 2061 6e20 696e   # because an in
+0001e160: 7374 616c 6c65 7220 7761 7320 7265 7175  staller was requ
+0001e170: 6573 7465 6420 6f6e 2074 6865 2063 6f6d  ested on the com
+0001e180: 6d61 6e64 206c 696e 652e 0a20 2020 2020  mand line..     
+0001e190: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0001e1a0: 2061 7267 732c 206c 6f63 6b5f 6f72 6465   args, lock_orde
+0001e1b0: 7220 2b20 5b61 7574 6865 6e74 6963 6174  r + [authenticat
+0001e1c0: 6f72 5f64 6972 5d0a 0a20 2020 2064 6566  or_dir]..    def
+0001e1d0: 2074 6573 745f 6c6f 636b 5f6f 7264 6572   test_lock_order
+0001e1e0: 2873 656c 662c 2061 7267 735f 616e 645f  (self, args_and_
+0001e1f0: 6c6f 636b 5f6f 7264 6572 2c20 6d6f 636b  lock_order, mock
+0001e200: 5f6c 6f63 6b5f 6469 7229 3a0a 2020 2020  _lock_dir):.    
+0001e210: 2020 2020 6172 6773 2c20 6c6f 636b 5f6f      args, lock_o
+0001e220: 7264 6572 203d 2061 7267 735f 616e 645f  rder = args_and_
+0001e230: 6c6f 636b 5f6f 7264 6572 0a20 2020 2020  lock_order.     
+0001e240: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+0001e250: 6169 7365 7328 7365 6c66 2e45 5850 4543  aises(self.EXPEC
+0001e260: 5445 445f 4552 524f 525f 5459 5045 2c20  TED_ERROR_TYPE, 
+0001e270: 6d61 7463 683d 7365 6c66 2e45 5850 4543  match=self.EXPEC
+0001e280: 5445 445f 4552 524f 525f 5354 525f 5245  TED_ERROR_STR_RE
+0001e290: 4745 5829 3a0a 2020 2020 2020 2020 2020  GEX):.          
+0001e2a0: 2020 6d61 696e 2e6d 6169 6e28 6172 6773    main.main(args
+0001e2b0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+0001e2c0: 206d 6f63 6b5f 6c6f 636b 5f64 6972 2e63   mock_lock_dir.c
+0001e2d0: 616c 6c5f 636f 756e 7420 3d3d 206c 656e  all_count == len
+0001e2e0: 286c 6f63 6b5f 6f72 6465 7229 0a20 2020  (lock_order).   
+0001e2f0: 2020 2020 2066 6f72 2063 616c 6c2c 206c       for call, l
+0001e300: 6f63 6b65 645f 6469 7220 696e 207a 6970  ocked_dir in zip
+0001e310: 286d 6f63 6b5f 6c6f 636b 5f64 6972 2e63  (mock_lock_dir.c
+0001e320: 616c 6c5f 6172 6773 5f6c 6973 742c 206c  all_args_list, l
+0001e330: 6f63 6b5f 6f72 6465 7229 3a0a 2020 2020  ock_order):.    
+0001e340: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
+0001e350: 616c 6c5b 305d 5b30 5d20 3d3d 206c 6f63  all[0][0] == loc
+0001e360: 6b65 645f 6469 720a 0a0a 6966 205f 5f6e  ked_dir...if __n
+0001e370: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+0001e380: 5f5f 273a 0a20 2020 2073 7973 2e65 7869  __':.    sys.exi
+0001e390: 7428 7079 7465 7374 2e6d 6169 6e28 7379  t(pytest.main(sy
+0001e3a0: 732e 6172 6776 5b31 3a5d 202b 205b 5f5f  s.argv[1:] + [__
+0001e3b0: 6669 6c65 5f5f 5d29 2920 2023 2070 7261  file__]))  # pra
+0001e3c0: 676d 613a 206e 6f20 636f 7665 720a       gma: no cover.
```

### Comparing `certbot-2.8.0/certbot/_internal/tests/ocsp_test.py` & `certbot-2.9.0/certbot/_internal/tests/ocsp_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/common_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/common_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/disco_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/disco_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/dns_common_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/dns_common_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/enhancements_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/enhancements_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/manual_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/manual_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/null_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/null_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/selection_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/selection_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/standalone_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/standalone_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/storage_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/storage_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/util_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/plugins/webroot_test.py` & `certbot-2.9.0/certbot/_internal/tests/plugins/webroot_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/renewal_test.py` & `certbot-2.9.0/certbot/_internal/tests/renewal_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/renewupdater_test.py` & `certbot-2.9.0/certbot/_internal/tests/renewupdater_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/reverter_test.py` & `certbot-2.9.0/certbot/_internal/tests/reverter_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/storage_test.py` & `certbot-2.9.0/certbot/_internal/tests/storage_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/tests/util_test.py` & `certbot-2.9.0/certbot/_internal/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/_internal/updater.py` & `certbot-2.9.0/certbot/_internal/updater.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/achallenges.py` & `certbot-2.9.0/certbot/achallenges.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/compat/_path.py` & `certbot-2.9.0/certbot/compat/_path.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/compat/filesystem.py` & `certbot-2.9.0/certbot/compat/filesystem.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/compat/misc.py` & `certbot-2.9.0/certbot/compat/misc.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/compat/os.py` & `certbot-2.9.0/certbot/compat/os.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/configuration.py` & `certbot-2.9.0/certbot/configuration.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/crypto_util.py` & `certbot-2.9.0/certbot/crypto_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,28 +204,28 @@
 
     domains = _get_names_from_loaded_cert_or_req(csr)
     # Internally we always use PEM, so re-encode as PEM before returning.
     data_pem = crypto.dump_certificate_request(PEM, csr)
     return PEM, util.CSR(file=csrfile, data=data_pem, form="pem"), domains
 
 
-def make_key(bits: int = 1024, key_type: str = "rsa",
+def make_key(bits: int = 2048, key_type: str = "rsa",
              elliptic_curve: Optional[str] = None) -> bytes:
     """Generate PEM encoded RSA|EC key.
 
-    :param int bits: Number of bits if key_type=rsa. At least 1024 for RSA.
+    :param int bits: Number of bits if key_type=rsa. At least 2048 for RSA.
     :param str key_type: The type of key to generate, but be rsa or ecdsa
     :param str elliptic_curve: The elliptic curve to use.
 
     :returns: new RSA or ECDSA key in PEM form with specified number of bits
               or of type ec_curve when key_type ecdsa is used.
     :rtype: str
     """
     if key_type == 'rsa':
-        if bits < 1024:
+        if bits < 2048:
             raise errors.Error("Unsupported RSA key length: {}".format(bits))
 
         key = crypto.PKey()
         key.generate_key(crypto.TYPE_RSA, bits)
     elif key_type == 'ecdsa':
         if not elliptic_curve:
             raise errors.Error("When key_type == ecdsa, elliptic_curve must be set.")
```

### Comparing `certbot-2.8.0/certbot/display/ops.py` & `certbot-2.9.0/certbot/display/ops.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/display/util.py` & `certbot-2.9.0/certbot/display/util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/errors.py` & `certbot-2.9.0/certbot/errors.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/interfaces.py` & `certbot-2.9.0/certbot/interfaces.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/main.py` & `certbot-2.9.0/certbot/main.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/ocsp.py` & `certbot-2.9.0/certbot/ocsp.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/common.py` & `certbot-2.9.0/certbot/plugins/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,13 +461,13 @@
     config_dir = expanded_tempdir("config")
     work_dir = expanded_tempdir("work")
 
     filesystem.chmod(temp_dir, constants.CONFIG_DIRS_MODE)
     filesystem.chmod(config_dir, constants.CONFIG_DIRS_MODE)
     filesystem.chmod(work_dir, constants.CONFIG_DIRS_MODE)
 
-    test_dir_ref = importlib_resources.files(pkg).joinpath("testdata", test_dir)
+    test_dir_ref = importlib_resources.files(pkg).joinpath("testdata").joinpath(test_dir)
     with importlib_resources.as_file(test_dir_ref) as path:
         shutil.copytree(
             path, os.path.join(temp_dir, test_dir), symlinks=True)
 
     return temp_dir, config_dir, work_dir
```

### Comparing `certbot-2.8.0/certbot/plugins/dns_common.py` & `certbot-2.9.0/certbot/plugins/dns_common.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/dns_common_lexicon.py` & `certbot-2.9.0/certbot/plugins/dns_common_lexicon.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/dns_test_common.py` & `certbot-2.9.0/certbot/plugins/dns_test_common.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/dns_test_common_lexicon.py` & `certbot-2.9.0/certbot/plugins/dns_test_common_lexicon.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/enhancements.py` & `certbot-2.9.0/certbot/plugins/enhancements.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/storage.py` & `certbot-2.9.0/certbot/plugins/storage.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/plugins/util.py` & `certbot-2.9.0/certbot/plugins/util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/reverter.py` & `certbot-2.9.0/certbot/reverter.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/acme_util.py` & `certbot-2.9.0/certbot/tests/acme_util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/README` & `certbot-2.9.0/certbot/tests/testdata/README`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert-5sans_512.pem` & `certbot-2.9.0/certbot/tests/testdata/cert-5sans_512.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert-nosans_nistp256.pem` & `certbot-2.9.0/certbot/tests/testdata/cert-nosans_nistp256.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert-san_512.pem` & `certbot-2.9.0/certbot/tests/testdata/cert-san_512.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_2048.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_2048.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_512.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_512.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_512_bad.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_512_bad.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_fullchain_2048.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_fullchain_2048.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_intermediate_1.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_intermediate_1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_intermediate_2.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_intermediate_2.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/cert_leaf.pem` & `certbot-2.9.0/certbot/tests/testdata/cert_leaf.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/csr-6sans_512.pem` & `certbot-2.9.0/certbot/tests/testdata/csr-6sans_512.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/csr-san_512.pem` & `certbot-2.9.0/certbot/tests/testdata/csr-san_512.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/ocsp_certificate.pem` & `certbot-2.9.0/certbot/tests/testdata/ocsp_certificate.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/ocsp_issuer_certificate.pem` & `certbot-2.9.0/certbot/tests/testdata/ocsp_issuer_certificate.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/ocsp_responder_certificate.pem` & `certbot-2.9.0/certbot/tests/testdata/ocsp_responder_certificate.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/rsa2048_key.pem` & `certbot-2.9.0/certbot/tests/testdata/rsa2048_key.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive/cert1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive/cert1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive/chain1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive/chain1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive/fullchain1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive/fullchain1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive/privkey1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive/privkey1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/cert1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/cert1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/chain1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/chain1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-archive-ec/fullchain1.pem` & `certbot-2.9.0/certbot/tests/testdata/sample-archive-ec/fullchain1.pem`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-renewal-ancient.conf` & `certbot-2.9.0/certbot/tests/testdata/sample-renewal-ancient.conf`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-renewal-deprecated-option.conf` & `certbot-2.9.0/certbot/tests/testdata/sample-renewal-deprecated-option.conf`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-renewal-ec.conf` & `certbot-2.9.0/certbot/tests/testdata/sample-renewal-ec.conf`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/testdata/sample-renewal.conf` & `certbot-2.9.0/certbot/tests/testdata/sample-renewal.conf`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/tests/util.py` & `certbot-2.9.0/certbot/tests/util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot/util.py` & `certbot-2.9.0/certbot/util.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot.egg-info/PKG-INFO` & `certbot-2.9.0/certbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot
-Version: 2.8.0
+Version: 2.9.0
 Summary: ACME client
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,23 +14,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: acme>=2.8.0
+Requires-Dist: acme>=2.9.0
 Requires-Dist: ConfigArgParse>=1.5.3
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: cryptography>=3.2.1
 Requires-Dist: distro>=1.0.1
 Requires-Dist: importlib_resources>=1.3.1; python_version < "3.9"
 Requires-Dist: importlib_metadata>=4.6; python_version < "3.10"
 Requires-Dist: josepy>=1.13.0
```

### Comparing `certbot-2.8.0/certbot.egg-info/SOURCES.txt` & `certbot-2.9.0/certbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/certbot.egg-info/requires.txt` & `certbot-2.9.0/certbot.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-acme>=2.8.0
+acme>=2.9.0
 ConfigArgParse>=1.5.3
 configobj>=5.0.6
 cryptography>=3.2.1
 distro>=1.0.1
 josepy>=1.13.0
 parsedatetime>=2.4
 pyrfc3339
```

### Comparing `certbot-2.8.0/docs/Makefile` & `certbot-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/_templates/footer.html` & `certbot-2.9.0/docs/_templates/footer.html`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/challenges.rst` & `certbot-2.9.0/docs/challenges.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/ciphers.rst` & `certbot-2.9.0/docs/ciphers.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/cli-help.txt` & `certbot-2.9.0/docs/cli-help.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-usage:
+usage: 
   certbot [SUBCOMMAND] [options] [-d DOMAIN] [-d DOMAIN] ...
 
 Certbot can obtain and install HTTPS/TLS/SSL certificates.  By default,
 it will attempt to use a webserver both for obtaining and installing the
 certificate. The most common SUBCOMMANDS and flags are:
 
 obtain, install, and renew certificates:
@@ -118,15 +118,15 @@
   --user-agent USER_AGENT
                         Set a custom user agent string for the client. User
                         agent strings allow the CA to collect high level
                         statistics about success rates by OS, plugin and use
                         case, and to know when to deprecate support for past
                         Python versions and flags. If you wish to hide this
                         information from the Let's Encrypt server, set this to
-                        "". (default: CertbotACMEClient/2.7.4 (certbot;
+                        "". (default: CertbotACMEClient/2.8.0 (certbot;
                         OS_NAME OS_VERSION) Authenticator/XXX Installer/YYY
                         (SUBCOMMAND; flags: FLAGS) Py/major.minor.patchlevel).
                         The flags encoded in the user agent are: --duplicate,
                         --force-renew, --allow-subset-of-names, -n, and
                         whether any hooks are set.
   --user-agent-comment USER_AGENT_COMMENT
                         Add a comment to the default user agent string. May be
```

### Comparing `certbot-2.8.0/docs/compatibility.rst` & `certbot-2.9.0/docs/compatibility.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/conf.py` & `certbot-2.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'Certbot'
 # this is now overridden by the footer.html template
-#copyright = u'2014-2018 - The Certbot software and documentation are licensed under the Apache 2.0 license as described at https://eff.org/cb-license.'
+copyright = u'2014-2018 - The Certbot software and documentation are licensed under the Apache 2.0 license as described at https://eff.org/cb-license.'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '.'.join(meta['version'].split('.')[:2])
```

### Comparing `certbot-2.8.0/docs/contributing.rst` & `certbot-2.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/install.rst` & `certbot-2.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/make.bat` & `certbot-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/man/certbot.rst` & `certbot-2.9.0/docs/man/certbot.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/packaging.rst` & `certbot-2.9.0/docs/packaging.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/docs/using.rst` & `certbot-2.9.0/docs/using.rst`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,15 @@
 DuckDNS_           Y    N    DNS Authentication for DuckDNS
 Porkbun_           Y    N    DNS Authentication for Porkbun
 Infomaniak_        Y    N    DNS Authentication using Infomaniak Domains API
 dns-multi_         Y    N    DNS authentication of 100+ providers using go-acme/lego
 dns-dnsmanager_    Y    N    DNS Authentication for dnsmanager.io
 standalone-nfq_    Y    N    HTTP Authentication that works with any webserver (Linux only)
 dns-solidserver_   Y    N    DNS Authentication using SOLIDserver (EfficientIP)
+dns-stackit_       Y    N    DNS Authentication using STACKIT DNS
 ================== ==== ==== ===============================================================
 
 .. _haproxy: https://github.com/greenhost/certbot-haproxy
 .. _s3front: https://github.com/dlapiduz/letsencrypt-s3front
 .. _gandi: https://github.com/obynio/certbot-plugin-gandi
 .. _varnish: https://git.sesse.net/?p=letsencrypt-varnish-plugin
 .. _pritunl: https://github.com/kharkevich/letsencrypt-pritunl
@@ -347,14 +348,15 @@
 .. _DuckDNS: https://github.com/infinityofspace/certbot_dns_duckdns
 .. _Porkbun: https://github.com/infinityofspace/certbot_dns_porkbun
 .. _Infomaniak: https://github.com/Infomaniak/certbot-dns-infomaniak
 .. _dns-multi: https://github.com/alexzorin/certbot-dns-multi
 .. _dns-dnsmanager: https://github.com/stayallive/certbot-dns-dnsmanager
 .. _standalone-nfq: https://github.com/alexzorin/certbot-standalone-nfq
 .. _dns-solidserver: https://gitlab.com/charlyhong/certbot-dns-solidserver
+.. _dns-stackit: https://github.com/stackitcloud/certbot-dns-stackit
 
 If you're interested, you can also :ref:`write your own plugin <dev-plugin>`.
 
 .. _managing-certs:
 
 Managing certificates
 =====================
```

### Comparing `certbot-2.8.0/docs/what.rst` & `certbot-2.9.0/docs/what.rst`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/examples/cli.ini` & `certbot-2.9.0/examples/cli.ini`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/examples/generate-csr.sh` & `certbot-2.9.0/examples/generate-csr.sh`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/examples/plugins/certbot_example_plugins.py` & `certbot-2.9.0/examples/plugins/certbot_example_plugins.py`

 * *Files identical despite different names*

### Comparing `certbot-2.8.0/setup.py` & `certbot-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Networking',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
```

