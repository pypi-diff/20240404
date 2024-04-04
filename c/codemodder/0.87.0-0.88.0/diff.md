# Comparing `tmp/codemodder-0.87.0.tar.gz` & `tmp/codemodder-0.88.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemodder-0.87.0.tar", last modified: Tue Apr  2 14:47:54 2024, max compression
+gzip compressed data, was "codemodder-0.88.0.tar", last modified: Thu Apr  4 17:49:16 2024, max compression
```

## Comparing `codemodder-0.87.0.tar` & `codemodder-0.88.0.tar`

### file list

```diff
@@ -1,463 +1,485 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 14:47:41.000000 codemodder-0.87.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.174824 codemodder-0.87.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/pixeebot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/autoformat-pixeebot-prs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/codemod_pygoat.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/sonar_pixee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 14:47:41.000000 codemodder-0.87.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 14:47:41.000000 codemodder-0.87.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-02 14:47:41.000000 codemodder-0.87.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 14:47:41.000000 codemodder-0.87.0/.semgrepignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 14:47:41.000000 codemodder-0.87.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-02 14:47:41.000000 codemodder-0.87.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 14:47:41.000000 codemodder-0.87.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 14:47:41.000000 codemodder-0.87.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 14:47:41.000000 codemodder-0.87.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 14:47:41.000000 codemodder-0.87.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 14:47:41.000000 codemodder-0.87.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-02 14:47:54.246827 codemodder-0.87.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-02 14:47:41.000000 codemodder-0.87.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/ci_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-02 14:47:41.000000 codemodder-0.87.0/ci_tests/test_pygoat_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 14:47:41.000000 codemodder-0.87.0/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.178824 codemodder-0.87.0/img/
--rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/base-codemod.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-02 14:47:41.000000 codemodder-0.87.0/img/codemodder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.190825 codemodder-0.87.0/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_add_requests_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_process_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_str_concat_in_seq_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_defusedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 14:47:41.000000 codemodder-0.87.0/integration_tests/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-02 14:47:41.000000 codemodder-0.87.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 14:47:41.000000 codemodder-0.87.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:47:54.246827 codemodder-0.87.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.170824 codemodder-0.87.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.194825 codemodder-0.87.0/src/codemodder/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemodder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.194825 codemodder-0.87.0/src/codemodder/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/check_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/import_modifier_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/imported_call_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/sonar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/codemods/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12544 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/test/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/codemods/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/clean_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/transformations/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codemods/utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/codemod_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/dependency_management/setupcfg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.198825 codemodder-0.87.0/src/codemodder/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/project_analysis/python_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/sarifs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/scripts/get_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/sonar_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.202825 codemodder-0.87.0/src/codemodder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/abc_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/codemodder/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/src/codemodder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 14:47:54.000000 codemodder-0.87.0/src/codemodder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.210826 codemodder-0.87.0/src/core_codemods/
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/add_requests_timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.214826 codemodder-0.87.0/src/core_codemods/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/api/core_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/django_session_cookie_secure_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_https-connection.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_lazy-logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_limit-readline.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-module-global.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_requests-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_unused-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_url-sandbox.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-generator.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-set-literal.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_async_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/process_creation_sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/refactor/refactor_new_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/requests_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/secure_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.222826 codemodder-0.87.0/src/core_codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-02 14:47:41.000000 codemodder-0.87.0/src/core_codemods/with_threading_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.226826 codemodder-0.87.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_add_requests_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_async_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_include_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lxml_safe_parameter_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_process_creation_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/codemods/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/dependency_management/test_setupcfgt_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.238826 codemodder-0.87.0/tests/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.242827 codemodder-0.87.0/tests/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/project_analysis/test_python_repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.242827 codemodder-0.87.0/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/make_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/semgrep.sarif
--rw-r--r--   0 runner    (1001) docker     (127)    77614 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/sonar_issues.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/samples/webgoat_v8.2.0_codeql.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_ancestorpatterns_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_basetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codemod_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codemodder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_nameresolution_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_sarif_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:54.246827 codemodder-0.87.0/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 14:47:41.000000 codemodder-0.87.0/tests/transformations/test_remove_unused_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.993865 codemodder-0.88.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 17:49:07.000000 codemodder-0.88.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.913864 codemodder-0.88.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/pixeebot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/autoformat-pixeebot-prs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/codemod_pygoat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/sonar_pixee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-04 17:49:07.000000 codemodder-0.88.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 17:49:07.000000 codemodder-0.88.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 17:49:07.000000 codemodder-0.88.0/.semgrepignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 17:49:07.000000 codemodder-0.88.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-04 17:49:07.000000 codemodder-0.88.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 17:49:07.000000 codemodder-0.88.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 17:49:07.000000 codemodder-0.88.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-04 17:49:07.000000 codemodder-0.88.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 17:49:07.000000 codemodder-0.88.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 17:49:07.000000 codemodder-0.88.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-04 17:49:16.993865 codemodder-0.88.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 17:49:07.000000 codemodder-0.88.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/ci_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 17:49:07.000000 codemodder-0.88.0/ci_tests/test_pygoat_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 17:49:07.000000 codemodder-0.88.0/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/base-codemod.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.929865 codemodder-0.88.0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_add_requests_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_process_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_str_concat_in_seq_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_defusedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-04 17:49:07.000000 codemodder-0.88.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 17:49:07.000000 codemodder-0.88.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:49:16.993865 codemodder-0.88.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.909865 codemodder-0.88.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.933865 codemodder-0.88.0/src/codemodder/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemodder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/import_modifier_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/imported_call_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/sonar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/clean_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/codemod_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/setupcfg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/python_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/sarifs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/get_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/sonar_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/abc_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/src/codemodder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/add_requests_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/api/core_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/combine_startswith_endswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/defectdojo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_session_cookie_secure_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.965865 codemodder-0.88.0/src/core_codemods/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_https-connection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_lazy-logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_limit-readline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-module-global.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_requests-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_unused-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_url-sandbox.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-set-literal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_async_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/process_creation_sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.965865 codemodder-0.88.0/src/core_codemods/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/refactor/refactor_new_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/requests_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_cookie_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.969865 codemodder-0.88.0/src/core_codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/with_threading_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.969865 codemodder-0.88.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/tests/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.909865 codemodder-0.88.0/tests/codemods/defectdojo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_add_requests_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_async_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_include_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lxml_safe_parameter_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_process_creation_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_setupcfgt_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/test_python_repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/tests/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/make_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/semgrep.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/sonar_hotspots.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77614 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/sonar_issues.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/webgoat_v8.2.0_codeql.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_ancestorpatterns_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_basetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codemod_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codemodder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_nameresolution_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_sarif_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.87.0/.github/workflows/autoformat-pixeebot-prs.yaml` & `codemodder-0.88.0/.github/workflows/autoformat-pixeebot-prs.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/codemod_pygoat.yml` & `codemodder-0.88.0/.github/workflows/codemod_pygoat.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/deploy_to_pypi.yml` & `codemodder-0.88.0/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/integration_test.yml` & `codemodder-0.88.0/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/lint.yml` & `codemodder-0.88.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/pre-commit-autoupdate.yml` & `codemodder-0.88.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/sonar_pixee.yml` & `codemodder-0.88.0/.github/workflows/sonar_pixee.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.github/workflows/test.yml` & `codemodder-0.88.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.gitignore` & `codemodder-0.88.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/.pre-commit-config.yaml` & `codemodder-0.88.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/CHANGELOG.md` & `codemodder-0.88.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/CONTRIBUTING.md` & `codemodder-0.88.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/LICENSE` & `codemodder-0.88.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/Makefile` & `codemodder-0.88.0/Makefile`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/PKG-INFO` & `codemodder-0.88.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.87.0
+Version: 0.88.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,31 +677,31 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Security
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython<4
 Requires-Dist: isort<5.14,>=5.12
-Requires-Dist: libcst<1.3,>=1.1
+Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.6.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.67,>=1.50
+Requires-Dist: semgrep<1.68,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.5,>=7.3; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
 Requires-Dist: jsonschema~=4.21.0; extra == "test"
-Requires-Dist: lxml<5.2.0,>=4.9.3; extra == "test"
+Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
 Requires-Dist: pytest<8.2,>=7.4; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
 Requires-Dist: pytest-randomly==3.*; extra == "test"
```

### Comparing `codemodder-0.87.0/README.md` & `codemodder-0.88.0/README.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/ci_tests/test_pygoat_findings.py` & `codemodder-0.88.0/ci_tests/test_pygoat_findings.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/img/base-codemod.jpg` & `codemodder-0.88.0/img/base-codemod.jpg`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/img/codemodder-dark.png` & `codemodder-0.88.0/img/codemodder-dark.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/img/codemodder-light.png` & `codemodder-0.88.0/img/codemodder-light.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/img/codemodder.png` & `codemodder-0.88.0/img/codemodder.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_add_requests_timeout.py` & `codemodder-0.88.0/integration_tests/test_add_requests_timeout.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_combine_startswith_endswith.py` & `codemodder-0.88.0/integration_tests/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_dependency_manager.py` & `codemodder-0.88.0/integration_tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_django_debug_flag_on.py` & `codemodder-0.88.0/integration_tests/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_django_json_response_type.py` & `codemodder-0.88.0/integration_tests/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_django_model_without_dunder_str.py` & `codemodder-0.88.0/integration_tests/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_django_receiver_on_top.py` & `codemodder-0.88.0/integration_tests/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_django_session_cookie_secure_off.py` & `codemodder-0.88.0/integration_tests/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_exception_without_raise.py` & `codemodder-0.88.0/integration_tests/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_file_resource_leak.py` & `codemodder-0.88.0/integration_tests/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_assert_tuple.py` & `codemodder-0.88.0/integration_tests/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_dataclass_defaults.py` & `codemodder-0.88.0/integration_tests/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_deprecated_abstractproperty.py` & `codemodder-0.88.0/integration_tests/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_deprecated_logging_warn.py` & `codemodder-0.88.0/integration_tests/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_empty_sequence_comparison.py` & `codemodder-0.88.0/integration_tests/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_hasattr_call.py` & `codemodder-0.88.0/integration_tests/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_missing_self_or_cls.py` & `codemodder-0.88.0/integration_tests/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_mutable_params.py` & `codemodder-0.88.0/integration_tests/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_fix_task_instantiation.py` & `codemodder-0.88.0/integration_tests/test_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_flask_enable_csrf_protection.py` & `codemodder-0.88.0/integration_tests/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_flask_json_response_type.py` & `codemodder-0.88.0/integration_tests/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_harden_pickle_load.py` & `codemodder-0.88.0/integration_tests/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_harden_pyyaml.py` & `codemodder-0.88.0/integration_tests/test_harden_pyyaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import yaml
 
 from codemodder.codemods.test import BaseIntegrationTest
-from core_codemods.harden_pyyaml import HardenPyyaml
+from core_codemods.harden_pyyaml import HardenPyyaml, HardenPyyamlTransformer
 
 
 class TestHardenPyyaml(BaseIntegrationTest):
     codemod = HardenPyyaml
     original_code = """
     import yaml
 
@@ -13,10 +13,10 @@
     deserialized_data = yaml.load(data, Loader=yaml.Loader)
     """
     replacement_lines = [
         (4, "deserialized_data = yaml.load(data, Loader=yaml.SafeLoader)\n")
     ]
     expected_diff = '--- \n+++ \n@@ -1,4 +1,4 @@\n import yaml\n \n data = b"!!python/object/apply:subprocess.Popen \\\\n- ls"\n-deserialized_data = yaml.load(data, Loader=yaml.Loader)\n+deserialized_data = yaml.load(data, Loader=yaml.SafeLoader)\n'
     expected_line_change = "4"
-    change_description = HardenPyyaml.change_description
+    change_description = HardenPyyamlTransformer.change_description
     # expected exception because the yaml.SafeLoader protects against unsafe code
     allowed_exceptions = (yaml.constructor.ConstructorError,)
```

### Comparing `codemodder-0.87.0/integration_tests/test_harden_ruamel.py` & `codemodder-0.88.0/integration_tests/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_https_connection.py` & `codemodder-0.88.0/integration_tests/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_jinja2_autoescape.py` & `codemodder-0.88.0/integration_tests/test_jinja2_autoescape.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from codemodder.codemods.test import BaseIntegrationTest
-from core_codemods.enable_jinja2_autoescape import EnableJinja2Autoescape
+from core_codemods.enable_jinja2_autoescape import (
+    EnableJinja2Autoescape,
+    EnableJinja2AutoescapeTransformer,
+)
 
 
 class TestEnableJinja2Autoescape(BaseIntegrationTest):
     codemod = EnableJinja2Autoescape
     original_code = """
     from jinja2 import Environment
 
@@ -13,8 +16,8 @@
     replacement_lines = [
         (3, "env = Environment(autoescape=True)\n"),
         (4, "env = Environment(autoescape=True)\n"),
     ]
     expected_diff = "--- \n+++ \n@@ -1,4 +1,4 @@\n from jinja2 import Environment\n \n-env = Environment()\n-env = Environment(autoescape=False)\n+env = Environment(autoescape=True)\n+env = Environment(autoescape=True)\n"
     expected_line_change = "3"
     num_changes = 2
-    change_description = EnableJinja2Autoescape.change_description
+    change_description = EnableJinja2AutoescapeTransformer.change_description
```

### Comparing `codemodder-0.87.0/integration_tests/test_jwt_decode_verify.py` & `codemodder-0.88.0/integration_tests/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_lazy_logging.py` & `codemodder-0.88.0/integration_tests/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_limit_readline.py` & `codemodder-0.88.0/integration_tests/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_literal_or_new_object_identity.py` & `codemodder-0.88.0/integration_tests/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_lxml_safe_parser_defaults.py` & `codemodder-0.88.0/integration_tests/test_lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_lxml_safe_parsing.py` & `codemodder-0.88.0/integration_tests/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_multiple_codemods.py` & `codemodder-0.88.0/integration_tests/test_multiple_codemods.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_numpy_nan_equality.py` & `codemodder-0.88.0/integration_tests/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_order_imports.py` & `codemodder-0.88.0/integration_tests/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_process_sandbox.py` & `codemodder-0.88.0/integration_tests/test_process_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_program.py` & `codemodder-0.88.0/integration_tests/test_program.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         completed_process = subprocess.run(["codemodder"], check=False)
         assert completed_process.returncode == 3
 
     def test_codemods_include_exclude_conflict(self):
         completed_process = subprocess.run(
             [
                 "codemodder",
-                "tests/samples/",
+                "some/path",
                 "--output",
                 "doesntmatter.txt",
                 "--codemod-exclude",
                 "secure-random",
                 "--codemod-include",
                 "secure-random",
             ],
```

### Comparing `codemodder-0.87.0/integration_tests/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.88.0/integration_tests/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_remove_debug_breakpoint.py` & `codemodder-0.88.0/integration_tests/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_remove_future_imports.py` & `codemodder-0.88.0/integration_tests/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_remove_module_global.py` & `codemodder-0.88.0/integration_tests/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_remove_unused_imports.py` & `codemodder-0.88.0/integration_tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_replace_flask_send_file.py` & `codemodder-0.88.0/integration_tests/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_request_verify.py` & `codemodder-0.88.0/integration_tests/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_secure_flask_cookie.py` & `codemodder-0.88.0/integration_tests/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_secure_flask_session_config.py` & `codemodder-0.88.0/integration_tests/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_secure_random.py` & `codemodder-0.88.0/integration_tests/test_secure_random.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from codemodder.codemods.test import BaseIntegrationTest
-from core_codemods.secure_random import SecureRandom
+from core_codemods.secure_random import SecureRandom, SecureRandomTransformer
 
 
 class TestSecureRandom(BaseIntegrationTest):
     codemod = SecureRandom
     original_code = """
     import random
     random.random()
@@ -22,8 +22,8 @@
         """-random.random()\n"""
         """+import secrets\n"""
         """+\n"""
         """+secrets.SystemRandom().random()\n"""
         """ var = "hello"\n""")
     # fmt: on
     expected_line_change = "2"
-    change_description = SecureRandom.change_description
+    change_description = SecureRandomTransformer.change_description
```

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_django_json_response_type.py` & `codemodder-0.88.0/integration_tests/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_django_receiver_on_top.py` & `codemodder-0.88.0/integration_tests/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_exception_without_raise.py` & `codemodder-0.88.0/integration_tests/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_fix_assert_tuple.py` & `codemodder-0.88.0/integration_tests/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.88.0/integration_tests/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_flask_json_response_type.py` & `codemodder-0.88.0/integration_tests/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_jwt_decode_verify.py` & `codemodder-0.88.0/integration_tests/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.88.0/integration_tests/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_numpy_nan_equality.py` & `codemodder-0.88.0/integration_tests/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.88.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sonar_tempfile_mktemp.py` & `codemodder-0.88.0/integration_tests/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_sql_parameterization.py` & `codemodder-0.88.0/integration_tests/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_str_concat_in_seq_literals.py` & `codemodder-0.88.0/integration_tests/test_str_concat_in_seq_literals.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_subprocess_shell_false.py` & `codemodder-0.88.0/integration_tests/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_tempfile_mktemp.py` & `codemodder-0.88.0/integration_tests/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_unnecessary_f_str.py` & `codemodder-0.88.0/integration_tests/test_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_upgrade_sslcontext_tls.py` & `codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_url_sandbox.py` & `codemodder-0.88.0/integration_tests/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_use_defusedxml.py` & `codemodder-0.88.0/integration_tests/test_use_defusedxml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_use_generator.py` & `codemodder-0.88.0/integration_tests/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_use_set_literal.py` & `codemodder-0.88.0/integration_tests/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_use_walrus_if.py` & `codemodder-0.88.0/integration_tests/test_use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/integration_tests/test_with_threading_lock.py` & `codemodder-0.88.0/integration_tests/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/pyproject.toml` & `codemodder-0.88.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 requires-python = ">=3.10.0"
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A pluggable framework for building codemods in Python"
 dependencies = [
     "GitPython<4",
     "isort>=5.12,<5.14",
-    "libcst>=1.1,<1.3",
+    "libcst>=1.1,<1.4",
     "packaging>=23.2,<25.0",
     "pydantic~=2.6.0",
     "pylint>=3.0,<3.2",
     "python-json-logger~=2.0.0",
     "PyYAML~=6.0.0",
-    "semgrep>=1.50,<1.67",
+    "semgrep>=1.50,<1.68",
     "toml~=0.10.2",
     "tomlkit~=0.12.0",
     "wrapt~=1.16.0",
     "chardet~=5.2.0",
 ]
 keywords = ["codemod", "codemods", "security", "fix", "fixes"]
 classifiers = [
@@ -48,15 +48,15 @@
 
 [project.optional-dependencies]
 test = [
     "coverage>=7.3,<7.5",
     "Flask<4",
     "Jinja2~=3.1.2",
     "jsonschema~=4.21.0",
-    "lxml>=4.9.3,<5.2.0",
+    "lxml>=4.9.3,<5.3.0",
     "mock==5.1.*",
     "pre-commit<4",
     "Pyjwt~=2.8.0",
     "pytest>=7.4,<8.2",
     "pytest-cov>=4.1,<5.1",
     "pytest-mock>=3.12,<3.15",
     "pytest-randomly==3.*",
@@ -77,14 +77,15 @@
     "codemodder[test]",
     "codemodder[complexity]",
 ]
 
 [project.entry-points.codemods]
 core = "core_codemods:registry"
 sonar = "core_codemods:sonar_registry"
+defectdojo = "core_codemods:defectdojo_registry"
 
 [tool.setuptools]
 
 [tool.setuptools.package-data]
 "core_codemods.semgrep" = ["src/core_codemods/semgrep/*.yaml"]
 "core_codemods.docs" = ["src/core_codemods/docs/*.md"]
```

### Comparing `codemodder-0.87.0/src/codemodder/cli.py` & `codemodder-0.88.0/src/codemodder/cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/code_directory.py` & `codemodder-0.88.0/src/codemodder/code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemodder.py` & `codemodder-0.88.0/src/codemodder/codemodder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import itertools
 import logging
 import os
 import sys
 from pathlib import Path
-from typing import Sequence
+from typing import DefaultDict, Sequence
 
 from codemodder import __version__, registry
 from codemodder.cli import parse_args
 from codemodder.code_directory import match_files
 from codemodder.codemods.api import BaseCodemod
 from codemodder.codemods.semgrep import SemgrepRuleDetector
 from codemodder.codetf import CodeTF
@@ -152,20 +152,21 @@
 
     configure_logger(argv.verbose, argv.log_format, argv.project_name)
 
     log_section("startup")
     logger.info("codemodder: python/%s", __version__)
     logger.info("command: %s %s", Path(sys.argv[0]).name, " ".join(original_args))
 
-    # TODO: sonar files should be _parsed_ here as well
     # TODO: this should be dict[str, list[Path]]
-    tool_result_files_map: dict[str, list[str]] = detect_sarif_tools(
+    tool_result_files_map: DefaultDict[str, list[str]] = detect_sarif_tools(
         [Path(name) for name in argv.sarif or []]
     )
-    tool_result_files_map["sonar"] = argv.sonar_issues_json
+    tool_result_files_map["sonar"].extend(argv.sonar_issues_json or [])
+    tool_result_files_map["sonar"].extend(argv.sonar_hotspots_json or [])
+    tool_result_files_map["defectdojo"] = argv.defectdojo_findings_json or []
 
     repo_manager = PythonRepoManager(Path(argv.directory))
     context = CodemodExecutionContext(
         Path(argv.directory),
         argv.dry_run,
         argv.verbose,
         codemod_registry,
```

### Comparing `codemodder-0.87.0/src/codemodder/codemods/api.py` & `codemodder-0.88.0/src/codemodder/codemods/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/base_codemod.py` & `codemodder-0.88.0/src/codemodder/codemods/base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/base_transformer.py` & `codemodder-0.88.0/src/codemodder/codemods/base_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/base_visitor.py` & `codemodder-0.88.0/src/codemodder/codemods/base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/check_annotations.py` & `codemodder-0.88.0/src/codemodder/codemods/check_annotations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/import_modifier_codemod.py` & `codemodder-0.88.0/src/codemodder/codemods/import_modifier_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/imported_call_modifier.py` & `codemodder-0.88.0/src/codemodder/codemods/imported_call_modifier.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/libcst_transformer.py` & `codemodder-0.88.0/src/codemodder/codemods/libcst_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,18 +114,21 @@
 
     def lineno_for_node(self, node):
         return self.node_position(node).start.line
 
     def add_dependency(self, dependency: Dependency):
         self.file_context.add_dependency(dependency)
 
-    def report_change(self, original_node):
+    def report_change(self, original_node, description: str | None = None):
         line_number = self.lineno_for_node(original_node)
         self.file_context.codemod_changes.append(
-            Change(lineNumber=line_number, description=self.change_description)
+            Change(
+                lineNumber=line_number,
+                description=description or self.change_description,
+            )
         )
 
     def remove_unused_import(self, original_node):
         RemoveImportsVisitor.remove_unused_import_by_node(self.context, original_node)
 
     def add_needed_import(self, module, obj=None):
         # TODO: do we need to check if this import already exists?
```

### Comparing `codemodder-0.87.0/src/codemodder/codemods/semgrep.py` & `codemodder-0.88.0/src/codemodder/codemods/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/sonar.py` & `codemodder-0.88.0/src/codemodder/codemods/sonar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import cache
 from pathlib import Path
 
 from codemodder.codemods.base_codemod import Metadata, Reference, ToolMetadata
 from codemodder.codemods.base_detector import BaseDetector
 from codemodder.codemods.base_transformer import BaseTransformerPipeline
 from codemodder.context import CodemodExecutionContext
 from codemodder.result import ResultSet
@@ -48,26 +49,27 @@
             transformer=transformer if transformer else other.transformer,
             detector=SonarDetector(),
             requested_rules=[rule_id],
         )
 
 
 class SonarDetector(BaseDetector):
-    _lazy_cache = None
-
-    def _process_sonar_findings(self, sonar_json_files: list[str]) -> SonarResultSet:
-        combined_result_set = SonarResultSet()
-        for file in sonar_json_files or []:
-            combined_result_set |= SonarResultSet.from_json(file)
-        return combined_result_set
-
     def apply(
         self,
         codemod_id: str,
         context: CodemodExecutionContext,
         files_to_analyze: list[Path],
     ) -> ResultSet:
-        if not self._lazy_cache:
-            self._lazy_cache = self._process_sonar_findings(
-                context.tool_result_files_map.get("sonar", [])
-            )
-        return self._lazy_cache
+        sonar_findings = process_sonar_findings(
+            tuple(
+                context.tool_result_files_map.get("sonar", ())
+            )  # Convert list to tuple for cache hashability
+        )
+        return sonar_findings
+
+
+@cache
+def process_sonar_findings(sonar_json_files: tuple[str]) -> SonarResultSet:
+    combined_result_set = SonarResultSet()
+    for file in sonar_json_files or ():
+        combined_result_set |= SonarResultSet.from_json(file)
+    return combined_result_set
```

### Comparing `codemodder-0.87.0/src/codemodder/codemods/test/integration_utils.py` & `codemodder-0.88.0/src/codemodder/codemods/test/integration_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pathlib import Path
 from textwrap import dedent
 from types import ModuleType
 
 import jsonschema
 
 from codemodder import __version__, registry
-from codemodder.sonar_results import SonarResultSet
 
 from .validations import execute_code
 
 
 class DependencyTestMixin:
     # Only for codemods that modify requirements should these be overridden
     requirements_file_name = ""
@@ -39,14 +38,15 @@
     original_code = NotImplementedError
     replacement_lines = NotImplementedError
     num_changes = 1
     _lines: list = []
     num_changed_files = 1
     allowed_exceptions = ()
     sonar_issues_json: str | None = None
+    sonar_hotspots_json: str | None = None
 
     @classmethod
     def setup_class(cls):
         cls.codemod_registry = registry.load_registered_codemods()
         cls.output_path = tempfile.mkstemp()[1]
         cls.code_dir = tempfile.mkdtemp()
 
@@ -108,33 +108,38 @@
         assert run["elapsed"] != ""
         assert run[
             "commandLine"
         ] == f'codemodder {self.code_dir} --output {output_path} --codemod-include={self.codemod_instance.name} --path-include={self.code_filename} --path-exclude=""' + (
             f" --sonar-issues-json={self.sonar_issues_json}"
             if self.sonar_issues_json
             else ""
+        ) + (
+            f" --sonar-hotspots-json={self.sonar_hotspots_json}"
+            if self.sonar_hotspots_json
+            else ""
         )
         assert run["directory"] == os.path.abspath(self.code_dir)
         assert run["sarifs"] == []
 
     def _assert_results_fields(self, results, output_path):
         assert len(results) == 1
         result = results[0]
         assert result["codemod"] == self.codemod_instance.id
         assert result["references"] == [
             ref.model_dump(exclude_none=True)
             for ref in self.codemod_instance.references
         ]
 
         assert ("detectionTool" in result) == bool(self.sonar_issues_json)
+        assert ("detectionTool" in result) == bool(self.sonar_hotspots_json)
 
         # TODO: if/when we add description for each url
         for reference in result["references"][
             # Last reference for Sonar has a different description
-            : (-1 if self.sonar_issues_json else None)
+            : (-1 if self.sonar_issues_json or self.sonar_hotspots_json else None)
         ]:
             assert reference["url"] == reference["description"]
 
         self._assert_sonar_fields(result)
 
         assert len(result["changeset"]) == self.num_changed_files
 
@@ -195,14 +200,16 @@
             f"--codemod-include={self.codemod_instance.name}",
             f"--path-include={self.code_filename}",
             '--path-exclude=""',
         ]
 
         if self.sonar_issues_json:
             command.append(f"--sonar-issues-json={self.sonar_issues_json}")
+        if self.sonar_hotspots_json:
+            command.append(f"--sonar-hotspots-json={self.sonar_hotspots_json}")
 
         self.write_original_code()
         self.write_original_dependencies()
 
         completed_process = subprocess.run(
             command,
             check=False,
@@ -241,14 +248,15 @@
     """
     Sonar integration tests must use code from a file in tests/samples
     because those files are what appears in sonar_issues.json
     """
 
     code_path = NotImplementedError
     sonar_issues_json = "tests/samples/sonar_issues.json"
+    sonar_hotspots_json = "tests/samples/sonar_hotspots.json"
 
     @classmethod
     def setup_class(cls):
         cls.codemod_registry = registry.load_registered_codemods()
         cls.original_code, cls.expected_new_code = original_and_expected_from_code_path(
             cls.code_path, cls.replacement_lines
         )
@@ -270,24 +278,28 @@
         pathlib.Path(cls.output_path).unlink(missing_ok=True)
         # Revert code file
         with open(cls.code_path, mode="w", encoding="utf-8") as f:
             f.write(cls.original_code)
 
     @classmethod
     def check_sonar_issues(cls):
-        sonar_results = SonarResultSet.from_json(cls.sonar_issues_json)
+        from codemodder.codemods.sonar import process_sonar_findings
+
+        sonar_results = process_sonar_findings(
+            (cls.sonar_issues_json, cls.sonar_hotspots_json)
+        )
 
         assert (
             cls.codemod.rule_id in sonar_results
-        ), f"Make sure to add a sonar issue for {cls.codemod.rule_id} in {cls.sonar_issues_json}"
+        ), f"Make sure to add a sonar issue/hotspot for {cls.codemod.rule_id} in {cls.sonar_issues_json} or {cls.sonar_hotspots_json}"
         results_for_codemod = sonar_results[cls.codemod.rule_id]
         file_path = pathlib.Path(cls.code_filename)
         assert (
             file_path in results_for_codemod
-        ), f"Make sure to add a sonar issue for file `{cls.code_filename}` under rule `{cls.codemod.rule_id}` in {cls.sonar_issues_json}"
+        ), f"Make sure to add a sonar issue/hotspot for file `{cls.code_filename}` under rule `{cls.codemod.rule_id}`in {cls.sonar_issues_json} or {cls.sonar_hotspots_json}"
 
     def _assert_sonar_fields(self, result):
         assert self.codemod_instance._metadata.tool is not None
         assert (
             result["references"][-1]["description"]
             == self.codemod_instance._metadata.tool.rule_name
         )
```

### Comparing `codemodder-0.87.0/src/codemodder/codemods/test/utils.py` & `codemodder-0.88.0/src/codemodder/codemods/test/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
         results: str = "",
     ):
         root = root or tmpdir
         tmp_file_path = files[0] if files else Path(tmpdir) / "code.py"
         tmp_file_path.write_text(dedent(input_code))
 
         tmp_results_file_path = Path(tmpdir) / "sast_results"
-
-        with open(tmp_results_file_path, "w", encoding="utf-8") as results_file:
-            results_file.write(results)
+        tmp_results_file_path.write_text(results)
 
         files_to_check = files or [tmp_file_path]
 
         path_exclude = [f"{tmp_file_path}:{line}" for line in lines_to_exclude or []]
 
         self.execution_context = CodemodExecutionContext(
             directory=root,
```

### Comparing `codemodder-0.87.0/src/codemodder/codemods/test/validations.py` & `codemodder-0.88.0/src/codemodder/codemods/test/validations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/transformations/clean_imports.py` & `codemodder-0.88.0/src/codemodder/codemods/transformations/clean_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py` & `codemodder-0.88.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/transformations/remove_unused_imports.py` & `codemodder-0.88.0/src/codemodder/codemods/transformations/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/utils.py` & `codemodder-0.88.0/src/codemodder/codemods/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codemods/utils_mixin.py` & `codemodder-0.88.0/src/codemodder/codemods/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/codetf.py` & `codemodder-0.88.0/src/codemodder/codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/context.py` & `codemodder-0.88.0/src/codemodder/context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency.py` & `codemodder-0.88.0/src/codemodder/dependency.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/base_dependency_writer.py` & `codemodder-0.88.0/src/codemodder/dependency_management/base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/dependency_manager.py` & `codemodder-0.88.0/src/codemodder/dependency_management/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/pyproject_writer.py` & `codemodder-0.88.0/src/codemodder/dependency_management/pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/requirements_txt_writer.py` & `codemodder-0.88.0/src/codemodder/dependency_management/requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/setup_py_writer.py` & `codemodder-0.88.0/src/codemodder/dependency_management/setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/dependency_management/setupcfg_writer.py` & `codemodder-0.88.0/src/codemodder/dependency_management/setupcfg_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/diff.py` & `codemodder-0.88.0/src/codemodder/diff.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/file_context.py` & `codemodder-0.88.0/src/codemodder/file_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/logging.py` & `codemodder-0.88.0/src/codemodder/logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/base_parser.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/package_store.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/package_store.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py` & `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/project_analysis/python_repo_manager.py` & `codemodder-0.88.0/src/codemodder/project_analysis/python_repo_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/registry.py` & `codemodder-0.88.0/src/codemodder/registry.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/result.py` & `codemodder-0.88.0/src/codemodder/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 if TYPE_CHECKING:
     from codemodder.context import CodemodExecutionContext
 
 
 @dataclass
 class LineInfo:
     line: int
-    column: int
-    snippet: str | None
+    column: int = -1
+    snippet: str | None = None
 
 
 @dataclass
 class Location(ABCDataclass):
     file: Path
     start: LineInfo
     end: LineInfo
```

### Comparing `codemodder-0.87.0/src/codemodder/sarifs.py` & `codemodder-0.88.0/src/codemodder/sarifs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from abc import ABCMeta, abstractmethod
+from collections import defaultdict
 from importlib.metadata import entry_points
 from pathlib import Path
-from typing import Optional
+from typing import DefaultDict, Optional
 
 from typing_extensions import Self
 
 from codemodder.logging import logger
 
 from .result import LineInfo, Location, Result, ResultSet
 
@@ -14,30 +15,30 @@
 class AbstractSarifToolDetector(metaclass=ABCMeta):
     @classmethod
     @abstractmethod
     def detect(cls, run_data: dict) -> bool:
         pass
 
 
-def detect_sarif_tools(filenames: list[Path]) -> dict[str, list[str]]:
-    results: dict[str, list[str]] = {}
+def detect_sarif_tools(filenames: list[Path]) -> DefaultDict[str, list[str]]:
+    results: DefaultDict[str, list[str]] = defaultdict(list)
 
     logger.debug("loading registered SARIF tool detectors")
     detectors = {
         ent.name: ent.load() for ent in entry_points().select(group="sarif_detectors")
     }
     for fname in filenames:
         data = json.loads(fname.read_text())
         for name, det in detectors.items():
             # TODO: handle malformed sarif?
             for run in data["runs"]:
                 try:
                     if det.detect(run):
                         logger.debug("detected %s sarif: %s", name, fname)
-                        results.setdefault(name, []).append(str(fname))
+                        results[name].append(str(fname))
                 except (KeyError, AttributeError, ValueError):
                     continue
 
     return results
 
 
 def extract_rule_id(result, sarif_run) -> Optional[str]:
```

### Comparing `codemodder-0.87.0/src/codemodder/scripts/generate_docs.py` & `codemodder-0.88.0/src/codemodder/scripts/generate_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,34 @@
         need_sarif="Yes (Sonar)",
     ),
     "secure-tempfile-S5445": DocMetadata(
         importance=CORE_METADATA["secure-tempfile"].importance,
         guidance_explained=CORE_METADATA["secure-tempfile"].guidance_explained,
         need_sarif="Yes (Sonar)",
     ),
+    "secure-random-S2245": DocMetadata(
+        importance=CORE_METADATA["secure-random"].importance,
+        guidance_explained=CORE_METADATA["secure-random"].guidance_explained,
+        need_sarif="Yes (Sonar)",
+    ),
+    "enable-jinja2-autoescape-S5247": DocMetadata(
+        importance=CORE_METADATA["enable-jinja2-autoescape"].importance,
+        guidance_explained=CORE_METADATA["enable-jinja2-autoescape"].guidance_explained,
+        need_sarif="Yes (Sonar)",
+    ),
+    "django-secure-set-cookie": DocMetadata(
+        importance="Medium",
+        guidance_explained="Our change provides the most secure way to create cookies in Django. However, it's possible you have configured your Django application configurations to use secure cookies. In these cases, using the default parameters for `set_cookie` is safe.",
+        need_sarif="Yes (DefectDojo)",
+    ),
+    "avoid-insecure-deserialization": DocMetadata(
+        importance="High",
+        guidance_explained="This change is generally safe and will prevent deserialization vulnerabilities.",
+        need_sarif="Yes (DefectDojo)",
+    ),
 }
 
 
 def generate_docs(codemod):
     try:
         codemod_data = METADATA[codemod.name]
     except KeyError as exc:
```

### Comparing `codemodder-0.87.0/src/codemodder/scripts/get_hashes.py` & `codemodder-0.88.0/src/codemodder/scripts/get_hashes.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/semgrep.py` & `codemodder-0.88.0/src/codemodder/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/utils/clean_code.py` & `codemodder-0.88.0/src/codemodder/utils/clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/utils/format_string_parser.py` & `codemodder-0.88.0/src/codemodder/utils/format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/utils/linearize_string_expression.py` & `codemodder-0.88.0/src/codemodder/utils/linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/utils/timer.py` & `codemodder-0.88.0/src/codemodder/utils/timer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder/utils/utils.py` & `codemodder-0.88.0/src/codemodder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/codemodder.egg-info/PKG-INFO` & `codemodder-0.88.0/src/codemodder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.87.0
+Version: 0.88.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,31 +677,31 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Security
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython<4
 Requires-Dist: isort<5.14,>=5.12
-Requires-Dist: libcst<1.3,>=1.1
+Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.6.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.67,>=1.50
+Requires-Dist: semgrep<1.68,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.5,>=7.3; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
 Requires-Dist: jsonschema~=4.21.0; extra == "test"
-Requires-Dist: lxml<5.2.0,>=4.9.3; extra == "test"
+Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
 Requires-Dist: pytest<8.2,>=7.4; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
 Requires-Dist: pytest-randomly==3.*; extra == "test"
```

### Comparing `codemodder-0.87.0/src/codemodder.egg-info/SOURCES.txt` & `codemodder-0.88.0/src/codemodder.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -82,18 +82,20 @@
 integration_tests/test_secure_random.py
 integration_tests/test_sonar_django_json_response_type.py
 integration_tests/test_sonar_django_receiver_on_top.py
 integration_tests/test_sonar_exception_without_raise.py
 integration_tests/test_sonar_fix_assert_tuple.py
 integration_tests/test_sonar_fix_missing_self_or_cls.py
 integration_tests/test_sonar_flask_json_response_type.py
+integration_tests/test_sonar_jinja2_autoescape.py
 integration_tests/test_sonar_jwt_decode_verify.py
 integration_tests/test_sonar_literal_or_new_object_identity.py
 integration_tests/test_sonar_numpy_nan_equality.py
 integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
+integration_tests/test_sonar_secure_random.py
 integration_tests/test_sonar_tempfile_mktemp.py
 integration_tests/test_sql_parameterization.py
 integration_tests/test_str_concat_in_seq_literals.py
 integration_tests/test_subprocess_shell_false.py
 integration_tests/test_tempfile_mktemp.py
 integration_tests/test_unnecessary_f_str.py
 integration_tests/test_upgrade_sslcontext_minimum_version.py
@@ -214,14 +216,15 @@
 src/core_codemods/remove_debug_breakpoint.py
 src/core_codemods/remove_future_imports.py
 src/core_codemods/remove_module_global.py
 src/core_codemods/remove_unnecessary_f_str.py
 src/core_codemods/remove_unused_imports.py
 src/core_codemods/replace_flask_send_file.py
 src/core_codemods/requests_verify.py
+src/core_codemods/secure_cookie_mixin.py
 src/core_codemods/secure_flask_cookie.py
 src/core_codemods/secure_flask_session_config.py
 src/core_codemods/secure_random.py
 src/core_codemods/sql_parameterization.py
 src/core_codemods/str_concat_in_seq_literal.py
 src/core_codemods/subprocess_shell_false.py
 src/core_codemods/tempfile_mktemp.py
@@ -231,15 +234,21 @@
 src/core_codemods/use_defused_xml.py
 src/core_codemods/use_generator.py
 src/core_codemods/use_set_literal.py
 src/core_codemods/use_walrus_if.py
 src/core_codemods/with_threading_lock.py
 src/core_codemods/api/__init__.py
 src/core_codemods/api/core_codemod.py
+src/core_codemods/defectdojo/api.py
+src/core_codemods/defectdojo/results.py
+src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
+src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
 src/core_codemods/docs/__init__.py
+src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
+src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
 src/core_codemods/docs/pixee_python_add-requests-timeouts.md
 src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
 src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
 src/core_codemods/docs/pixee_python_django-debug-flag-on.md
 src/core_codemods/docs/pixee_python_django-json-response-type.md
 src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
 src/core_codemods/docs/pixee_python_django-receiver-on-top.md
@@ -292,22 +301,24 @@
 src/core_codemods/docs/pixee_python_use-generator.md
 src/core_codemods/docs/pixee_python_use-set-literal.md
 src/core_codemods/docs/pixee_python_use-walrus-if.md
 src/core_codemods/refactor/__init__.py
 src/core_codemods/refactor/refactor_new_api.py
 src/core_codemods/sonar/sonar_django_json_response_type.py
 src/core_codemods/sonar/sonar_django_receiver_on_top.py
+src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
 src/core_codemods/sonar/sonar_exception_without_raise.py
 src/core_codemods/sonar/sonar_fix_assert_tuple.py
 src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
 src/core_codemods/sonar/sonar_flask_json_response_type.py
 src/core_codemods/sonar/sonar_jwt_decode_verify.py
 src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
 src/core_codemods/sonar/sonar_numpy_nan_equality.py
 src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+src/core_codemods/sonar/sonar_secure_random.py
 src/core_codemods/sonar/sonar_tempfile_mktemp.py
 tests/__init__.py
 tests/conftest.py
 tests/test_ancestorpatterns_mixin.py
 tests/test_basetype.py
 tests/test_cli.py
 tests/test_code_directory.py
@@ -371,35 +382,39 @@
 tests/codemods/test_replace_flask_send_file.py
 tests/codemods/test_request_verify.py
 tests/codemods/test_secure_flask_cookie.py
 tests/codemods/test_secure_flask_session_config.py
 tests/codemods/test_secure_random.py
 tests/codemods/test_sonar_django_json_response_type.py
 tests/codemods/test_sonar_django_receiver_on_top.py
+tests/codemods/test_sonar_enable_jinja2_autoescape.py
 tests/codemods/test_sonar_exception_without_raise.py
 tests/codemods/test_sonar_fix_assert_tuple.py
 tests/codemods/test_sonar_fix_missing_self_or_cls.py
 tests/codemods/test_sonar_flask_json_response_type.py
 tests/codemods/test_sonar_jwt_decode_verify.py
 tests/codemods/test_sonar_literal_or_new_object_identity.py
 tests/codemods/test_sonar_numpy_nan_equality.py
 tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
+tests/codemods/test_sonar_secure_random.py
 tests/codemods/test_sonar_tempfile_mktemp.py
 tests/codemods/test_sql_parameterization.py
 tests/codemods/test_str_concat_in_seq_literal.py
 tests/codemods/test_subprocess_shell_false.py
 tests/codemods/test_tempfile_mktemp.py
 tests/codemods/test_upgrade_sslcontext_minimum_version.py
 tests/codemods/test_upgrade_sslcontext_tls.py
 tests/codemods/test_url_sandbox.py
 tests/codemods/test_use_defused_xml.py
 tests/codemods/test_use_generator.py
 tests/codemods/test_use_set_literal.py
 tests/codemods/test_walrus_if.py
 tests/codemods/test_with_threading_lock.py
+tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
+tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
 tests/dependency_management/__init__.py
 tests/dependency_management/test_base_dependency_writer.py
 tests/dependency_management/test_dependency_manager.py
 tests/dependency_management/test_pyproject_writer.py
 tests/dependency_management/test_requirements_txt_writer.py
 tests/dependency_management/test_setup_py_writer.py
 tests/dependency_management/test_setupcfgt_writer.py
@@ -412,21 +427,24 @@
 tests/project_analysis/file_parsers/test_setup_py_file_parser.py
 tests/samples/django_json_response_type.py
 tests/samples/django_receiver_on_top.py
 tests/samples/exception_without_raise.py
 tests/samples/fix_assert_tuple.py
 tests/samples/fix_missing_self_or_cls.py
 tests/samples/flask_json_response_type.py
+tests/samples/jinja2_autoescape.py
 tests/samples/jwt_decode_verify.py
 tests/samples/literal_or_new_object_identity.py
 tests/samples/make_request.py
 tests/samples/multiple_codemods.py
 tests/samples/numpy_nan_equality.py
 tests/samples/remove_assertion_in_pytest_raises.py
+tests/samples/secure_random.py
 tests/samples/semgrep.sarif
+tests/samples/sonar_hotspots.json
 tests/samples/sonar_issues.json
 tests/samples/tempfile_mktemp.py
 tests/samples/webgoat_v8.2.0_codeql.sarif
 tests/transformations/__init__.py
 tests/transformations/test_clean_code.py
 tests/transformations/test_remove_empty_string_concatenation.py
 tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.87.0/src/codemodder.egg-info/requires.txt` & `codemodder-0.88.0/src/codemodder.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 GitPython<4
 isort<5.14,>=5.12
-libcst<1.3,>=1.1
+libcst<1.4,>=1.1
 packaging<25.0,>=23.2
 pydantic~=2.6.0
 pylint<3.2,>=3.0
 python-json-logger~=2.0.0
 PyYAML~=6.0.0
-semgrep<1.67,>=1.50
+semgrep<1.68,>=1.50
 toml~=0.10.2
 tomlkit~=0.12.0
 wrapt~=1.16.0
 chardet~=5.2.0
 
 [all]
 codemodder[test]
@@ -21,15 +21,15 @@
 xenon==0.9.*
 
 [test]
 coverage<7.5,>=7.3
 Flask<4
 Jinja2~=3.1.2
 jsonschema~=4.21.0
-lxml<5.2.0,>=4.9.3
+lxml<5.3.0,>=4.9.3
 mock==5.1.*
 pre-commit<4
 Pyjwt~=2.8.0
 pytest<8.2,>=7.4
 pytest-cov<5.1,>=4.1
 pytest-mock<3.15,>=3.12
 pytest-randomly==3.*
```

### Comparing `codemodder-0.87.0/src/core_codemods/__init__.py` & `codemodder-0.88.0/src/core_codemods/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from codemodder.registry import CodemodCollection
 
 from .add_requests_timeouts import AddRequestsTimeouts
 from .combine_startswith_endswith import CombineStartswithEndswith
+from .defectdojo.semgrep.avoid_insecure_deserialization import (
+    AvoidInsecureDeserialization,
+)
+from .defectdojo.semgrep.django_secure_set_cookie import DjangoSecureSetCookie
 from .django_debug_flag_on import DjangoDebugFlagOn
 from .django_json_response_type import DjangoJsonResponseType
 from .django_model_without_dunder_str import DjangoModelWithoutDunderStr
 from .django_receiver_on_top import DjangoReceiverOnTop
 from .django_session_cookie_secure_off import DjangoSessionCookieSecureOff
 from .enable_jinja2_autoescape import EnableJinja2Autoescape
 from .exception_without_raise import ExceptionWithoutRaise
@@ -43,24 +47,26 @@
 from .replace_flask_send_file import ReplaceFlaskSendFile
 from .requests_verify import RequestsVerify
 from .secure_flask_cookie import SecureFlaskCookie
 from .secure_flask_session_config import SecureFlaskSessionConfig
 from .secure_random import SecureRandom
 from .sonar.sonar_django_json_response_type import SonarDjangoJsonResponseType
 from .sonar.sonar_django_receiver_on_top import SonarDjangoReceiverOnTop
+from .sonar.sonar_enable_jinja2_autoescape import SonarEnableJinja2Autoescape
 from .sonar.sonar_exception_without_raise import SonarExceptionWithoutRaise
 from .sonar.sonar_fix_assert_tuple import SonarFixAssertTuple
 from .sonar.sonar_fix_missing_self_or_cls import SonarFixMissingSelfOrCls
 from .sonar.sonar_flask_json_response_type import SonarFlaskJsonResponseType
 from .sonar.sonar_jwt_decode_verify import SonarJwtDecodeVerify
 from .sonar.sonar_literal_or_new_object_identity import SonarLiteralOrNewObjectIdentity
 from .sonar.sonar_numpy_nan_equality import SonarNumpyNanEquality
 from .sonar.sonar_remove_assertion_in_pytest_raises import (
     SonarRemoveAssertionInPytestRaises,
 )
+from .sonar.sonar_secure_random import SonarSecureRandom
 from .sonar.sonar_tempfile_mktemp import SonarTempfileMktemp
 from .sql_parameterization import SQLQueryParameterization
 from .str_concat_in_seq_literal import StrConcatInSeqLiteral
 from .subprocess_shell_false import SubprocessShellFalse
 from .tempfile_mktemp import TempfileMktemp
 from .upgrade_sslcontext_minimum_version import UpgradeSSLContextMinimumVersion
 from .upgrade_sslcontext_tls import UpgradeSSLContextTLS
@@ -144,9 +150,19 @@
         SonarFixAssertTuple,
         SonarRemoveAssertionInPytestRaises,
         SonarFlaskJsonResponseType,
         SonarDjangoJsonResponseType,
         SonarJwtDecodeVerify,
         SonarFixMissingSelfOrCls,
         SonarTempfileMktemp,
+        SonarSecureRandom,
+        SonarEnableJinja2Autoescape,
+    ],
+)
+
+defectdojo_registry = CodemodCollection(
+    origin="defectdojo",
+    codemods=[
+        AvoidInsecureDeserialization,
+        DjangoSecureSetCookie,
     ],
 )
```

### Comparing `codemodder-0.87.0/src/core_codemods/add_requests_timeouts.py` & `codemodder-0.88.0/src/core_codemods/add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/api/core_codemod.py` & `codemodder-0.88.0/src/core_codemods/api/core_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/combine_startswith_endswith.py` & `codemodder-0.88.0/src/core_codemods/combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/django_debug_flag_on.py` & `codemodder-0.88.0/src/core_codemods/django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/django_json_response_type.py` & `codemodder-0.88.0/src/core_codemods/django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/django_model_without_dunder_str.py` & `codemodder-0.88.0/src/core_codemods/django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/django_receiver_on_top.py` & `codemodder-0.88.0/src/core_codemods/django_receiver_on_top.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     change_description = "Moved @receiver to the top."
 
     def leave_FunctionDef(
         self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
     ) -> Union[
         cst.BaseStatement, cst.FlattenSentinel[cst.BaseStatement], cst.RemovalSentinel
     ]:
-        # TODO: add filter by include or exclude that works for nodes
-        # that that have different start/end numbers.
         maybe_receiver_with_index = None
         for i, decorator in enumerate(original_node.decorators):
             if self.find_base_name(decorator.decorator) == "django.dispatch.receiver":
                 maybe_receiver_with_index = (i, decorator)
 
         if maybe_receiver_with_index and self.node_is_selected(
             maybe_receiver_with_index[1]
```

### Comparing `codemodder-0.87.0/src/core_codemods/django_session_cookie_secure_off.py` & `codemodder-0.88.0/src/core_codemods/django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-json-response-type.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_harden-ruamel.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-ruamel.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_lazy-logging.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_lazy-logging.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_limit-readline.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_limit-readline.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_remove-future-imports.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-future-imports.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_requests-verify.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_requests-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_secure-random.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-random.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_sql-parameterization.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_sql-parameterization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_url-sandbox.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_url-sandbox.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-defusedxml.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-defusedxml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-generator.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-generator.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/docs/pixee_python_use-walrus-if.md` & `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-walrus-if.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/enable_jinja2_autoescape.py` & `codemodder-0.88.0/src/core_codemods/harden_ruamel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 from codemodder.codemods.libcst_transformer import NewArg
 from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
 
 
-class EnableJinja2Autoescape(SimpleCodemod):
+class HardenRuamel(SimpleCodemod):
     metadata = Metadata(
-        name="enable-jinja2-autoescape",
-        summary="Enable Jinja2 Autoescape",
-        review_guidance=ReviewGuidance.MERGE_AFTER_REVIEW,
+        name="harden-ruamel",
+        summary="Use `typ='safe'` in ruamel.yaml() Calls",
+        review_guidance=ReviewGuidance.MERGE_WITHOUT_REVIEW,
         references=[
-            Reference(url="https://owasp.org/www-community/attacks/xss/"),
             Reference(
-                url="https://jinja.palletsprojects.com/en/3.1.x/api/#autoescaping"
+                url="https://owasp.org/www-community/vulnerabilities/Deserialization_of_untrusted_data"
             ),
         ],
     )
     change_description = (
-        "Sets the `autoescape` parameter in jinja2.Environment to `True`."
+        "Ensures all unsafe calls to ruamel.yaml.YAML use `typ='safe'`."
     )
     detector_pattern = """
             rules:
-              - pattern-either:
-                - patterns:
-                  - pattern: jinja2.Environment(...)
-                  - pattern-not: jinja2.Environment(..., autoescape=True, ...)
-                  - pattern-not: jinja2.Environment(..., autoescape=jinja2.select_autoescape(...), ...)
-                  # Exclude cases where the arguments can't be precisely determined
-                  - pattern-not: jinja2.Environment(**$KWARGS)
-                  - pattern-inside: |
-                      import jinja2
-                      ...
-                - patterns:
-                  - pattern: aiohttp_jinja2.setup(..., autoescape=False, ...)
-                  - pattern-inside: |
-                      import aiohttp_jinja2
-                      ...
+                - pattern-either:
+                  - patterns:
+                    - pattern: ruamel.yaml.YAML(typ="unsafe", ...)
+                    - pattern-inside: |
+                        import ruamel
+                        ...
+                  - patterns:
+                    - pattern: ruamel.yaml.YAML(typ="base", ...)
+                    - pattern-inside: |
+                        import ruamel
+                        ...
+
         """
 
     def on_result_found(self, original_node, updated_node):
         new_args = self.replace_args(
-            original_node,
-            [NewArg(name="autoescape", value="True", add_if_missing=True)],
+            original_node, [NewArg(name="typ", value='"safe"', add_if_missing=False)]
         )
         return self.update_arg_target(updated_node, new_args)
```

### Comparing `codemodder-0.87.0/src/core_codemods/exception_without_raise.py` & `codemodder-0.88.0/src/core_codemods/exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/file_resource_leak.py` & `codemodder-0.88.0/src/core_codemods/file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_assert_tuple.py` & `codemodder-0.88.0/src/core_codemods/fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_async_task_instantiation.py` & `codemodder-0.88.0/src/core_codemods/fix_async_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_dataclass_defaults.py` & `codemodder-0.88.0/src/core_codemods/fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_deprecated_abstractproperty.py` & `codemodder-0.88.0/src/core_codemods/fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_deprecated_logging_warn.py` & `codemodder-0.88.0/src/core_codemods/fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_empty_sequence_comparison.py` & `codemodder-0.88.0/src/core_codemods/fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_hasattr_call.py` & `codemodder-0.88.0/src/core_codemods/fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_missing_self_or_cls.py` & `codemodder-0.88.0/src/core_codemods/fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/fix_mutable_params.py` & `codemodder-0.88.0/src/core_codemods/fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/flask_enable_csrf_protection.py` & `codemodder-0.88.0/src/core_codemods/flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/flask_json_response_type.py` & `codemodder-0.88.0/src/core_codemods/flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/harden_pickle_load.py` & `codemodder-0.88.0/src/core_codemods/harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/harden_pyyaml.py` & `codemodder-0.88.0/src/core_codemods/harden_pyyaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,128 @@
-from typing import Union, cast
+from typing import Protocol, Union, cast
 
 import libcst as cst
 
+from codemodder.codemods.libcst_transformer import (
+    LibcstResultTransformer,
+    LibcstTransformerPipeline,
+)
+from codemodder.codemods.semgrep import SemgrepRuleDetector
 from codemodder.codemods.utils_mixin import NameResolutionMixin
-from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
+from core_codemods.api import CoreCodemod, Metadata, Reference, ReviewGuidance
 
+YAML_MODULE_NAME = "yaml"
 
-class HardenPyyaml(SimpleCodemod, NameResolutionMixin):
-    metadata = Metadata(
+
+class CodemodProtocol(Protocol):
+    def add_needed_import(self, module: str, obj=None): ...
+    def get_aliased_prefix_name(self, node: cst.CSTNode, module: str): ...
+    def parse_expression(self, code: str) -> cst.BaseExpression: ...
+    def update_arg_target(
+        self, node: cst.Call, new_args: list[cst.Arg]
+    ) -> cst.Call: ...
+
+
+class HardenPyyamlCallMixin:
+    def update_call(
+        self: CodemodProtocol, original_node: cst.Call, updated_node: cst.Call
+    ) -> cst.Call:
+        maybe_name = self.get_aliased_prefix_name(original_node, YAML_MODULE_NAME)
+        if (maybe_name := maybe_name or YAML_MODULE_NAME) == YAML_MODULE_NAME:
+            self.add_needed_import(YAML_MODULE_NAME)
+        updated_node = cast(cst.Call, updated_node)  # satisfy the type checker
+        new_args = [
+            *updated_node.args[:1],
+            # This is the case where the arg is present but a bad value
+            (
+                updated_node.args[1].with_changes(
+                    value=self.parse_expression(f"{maybe_name}.SafeLoader")
+                )
+                if len(updated_node.args) > 1
+                # This is the case where the arg is not present
+                # Note that this case is deprecated in PyYAML 5.1 since the default is unsafe
+                else cst.Arg(
+                    keyword=cst.Name("Loader"),
+                    value=self.parse_expression(f"{maybe_name}.SafeLoader"),
+                    equal=cst.AssignEqual(
+                        whitespace_before=cst.SimpleWhitespace(""),
+                        whitespace_after=cst.SimpleWhitespace(""),
+                    ),
+                )
+            ),
+        ]
+        return self.update_arg_target(updated_node, new_args)
+
+
+class HardenPyyamlTransformer(
+    LibcstResultTransformer,
+    NameResolutionMixin,
+    HardenPyyamlCallMixin,
+    CodemodProtocol,
+):
+    change_description = "Replace unsafe `pyyaml` loader with `SafeLoader` in calls to `yaml.load` or custom loader classes."
+
+    def on_result_found(
+        self,
+        original_node: Union[cst.Call, cst.ClassDef],
+        updated_node: Union[cst.Call, cst.ClassDef],
+    ):
+        # TODO: provide different change description for each case.
+        match original_node, updated_node:
+            case cst.Call(), cst.Call():
+                return self.update_call(original_node, updated_node)
+            case cst.ClassDef(), _:
+                return updated_node.with_changes(
+                    bases=self._update_bases(original_node)
+                )
+        return updated_node
+
+    def _update_bases(self, original_node: cst.ClassDef) -> list[cst.Arg]:
+        new = []
+        base_names = [
+            f"yaml.{klas}"
+            for klas in ("UnsafeLoader", "Loader", "BaseLoader", "FullLoader")
+        ]
+        for base_arg in original_node.bases:
+            base_name = self.find_base_name(base_arg.value)
+            if base_name not in base_names:
+                new.append(base_arg)
+                continue
+
+            match base_arg.value:
+                case cst.Name():
+                    self.add_needed_import(YAML_MODULE_NAME, "SafeLoader")
+                    self.remove_unused_import(base_arg.value)
+                    base_arg = base_arg.with_changes(
+                        value=base_arg.value.with_changes(value="SafeLoader")
+                    )
+                case cst.Attribute():
+                    base_arg = base_arg.with_changes(
+                        value=base_arg.value.with_changes(attr=cst.Name("SafeLoader"))
+                    )
+            new.append(base_arg)
+        return new
+
+
+HardenPyyaml = CoreCodemod(
+    metadata=Metadata(
         name="harden-pyyaml",
         summary="Replace unsafe `pyyaml` loader with `SafeLoader`",
         review_guidance=ReviewGuidance.MERGE_WITHOUT_REVIEW,
         references=[
             Reference(
                 url="https://owasp.org/www-community/vulnerabilities/Deserialization_of_untrusted_data"
             ),
             Reference(
                 url="https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation"
             ),
         ],
-    )
-    change_description = "Replace unsafe `pyyaml` loader with `SafeLoader` in calls to `yaml.load` or custom loader classes."
-
-    _module_name = "yaml"
-    detector_pattern = """
+    ),
+    detector=SemgrepRuleDetector(
+        """
         rules:
             - pattern-either:
               - patterns:
                   - pattern: yaml.load(...)
                   - pattern-inside: |
                       import yaml
                       ...
@@ -69,74 +164,10 @@
                       patterns:
                         - pattern-either:
                             - pattern: yaml.Loader
                             - pattern: yaml.BaseLoader
                             - pattern: yaml.FullLoader
                             - pattern: yaml.UnsafeLoader
         """
-
-    def on_result_found(
-        self,
-        original_node: Union[cst.Call, cst.ClassDef],
-        updated_node: Union[cst.Call, cst.ClassDef],
-    ):
-        # TODO: provide different change description for each case.
-        match original_node:
-            case cst.Call():
-                maybe_name = self.get_aliased_prefix_name(
-                    original_node, self._module_name
-                )
-                if (maybe_name := maybe_name or self._module_name) == self._module_name:
-                    self.add_needed_import(self._module_name)
-                updated_node = cast(cst.Call, updated_node)  # satisfy the type checker
-                new_args = [
-                    *updated_node.args[:1],
-                    # This is the case where the arg is present but a bad value
-                    (
-                        updated_node.args[1].with_changes(
-                            value=self.parse_expression(f"{maybe_name}.SafeLoader")
-                        )
-                        if len(updated_node.args) > 1
-                        # This is the case where the arg is not present
-                        # Note that this case is deprecated in PyYAML 5.1 since the default is unsafe
-                        else cst.Arg(
-                            keyword=cst.Name("Loader"),
-                            value=self.parse_expression(f"{maybe_name}.SafeLoader"),
-                            equal=cst.AssignEqual(
-                                whitespace_before=cst.SimpleWhitespace(""),
-                                whitespace_after=cst.SimpleWhitespace(""),
-                            ),
-                        )
-                    ),
-                ]
-                return self.update_arg_target(updated_node, new_args)
-            case cst.ClassDef():
-                return updated_node.with_changes(
-                    bases=self._update_bases(original_node)
-                )
-        return updated_node
-
-    def _update_bases(self, original_node: cst.ClassDef) -> list[cst.Arg]:
-        new = []
-        base_names = [
-            f"yaml.{klas}"
-            for klas in ("UnsafeLoader", "Loader", "BaseLoader", "FullLoader")
-        ]
-        for base_arg in original_node.bases:
-            base_name = self.find_base_name(base_arg.value)
-            if base_name not in base_names:
-                new.append(base_arg)
-                continue
-
-            match base_arg.value:
-                case cst.Name():
-                    self.add_needed_import(self._module_name, "SafeLoader")
-                    self.remove_unused_import(base_arg.value)
-                    base_arg = base_arg.with_changes(
-                        value=base_arg.value.with_changes(value="SafeLoader")
-                    )
-                case cst.Attribute():
-                    base_arg = base_arg.with_changes(
-                        value=base_arg.value.with_changes(attr=cst.Name("SafeLoader"))
-                    )
-            new.append(base_arg)
-        return new
+    ),
+    transformer=LibcstTransformerPipeline(HardenPyyamlTransformer),
+)
```

### Comparing `codemodder-0.87.0/src/core_codemods/https_connection.py` & `codemodder-0.88.0/src/core_codemods/https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/jwt_decode_verify.py` & `codemodder-0.88.0/src/core_codemods/jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/lazy_logging.py` & `codemodder-0.88.0/src/core_codemods/lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/limit_readline.py` & `codemodder-0.88.0/src/core_codemods/limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/literal_or_new_object_identity.py` & `codemodder-0.88.0/src/core_codemods/literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/lxml_safe_parser_defaults.py` & `codemodder-0.88.0/src/core_codemods/lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/lxml_safe_parsing.py` & `codemodder-0.88.0/src/core_codemods/lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/numpy_nan_equality.py` & `codemodder-0.88.0/src/core_codemods/numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/order_imports.py` & `codemodder-0.88.0/src/core_codemods/order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/process_creation_sandbox.py` & `codemodder-0.88.0/src/core_codemods/process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/refactor/refactor_new_api.py` & `codemodder-0.88.0/src/core_codemods/refactor/refactor_new_api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/remove_assertion_in_pytest_raises.py` & `codemodder-0.88.0/src/core_codemods/remove_assertion_in_pytest_raises.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,18 +89,14 @@
         return assert_stmts, assert_position, new_statement_before_asserts
 
     def leave_With(
         self, original_node: cst.With, updated_node: cst.With
     ) -> Union[
         cst.BaseStatement, cst.FlattenSentinel[cst.BaseStatement], cst.RemovalSentinel
     ]:
-        # TODO: add filter by include or exclude that works for nodes
-        # that that have different start/end numbers.
-
-        # Are all items pytest.raises?
         if not self._all_pytest_raises(original_node):
             return updated_node
 
         assert_stmts: list[cst.SimpleStatementLine] = []
         assert_position = len(original_node.body.body)
         new_statement_before_asserts = None
         match original_node.body:
```

### Comparing `codemodder-0.87.0/src/core_codemods/remove_debug_breakpoint.py` & `codemodder-0.88.0/src/core_codemods/remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/remove_future_imports.py` & `codemodder-0.88.0/src/core_codemods/remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/remove_module_global.py` & `codemodder-0.88.0/src/core_codemods/remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/remove_unnecessary_f_str.py` & `codemodder-0.88.0/src/core_codemods/remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/remove_unused_imports.py` & `codemodder-0.88.0/src/core_codemods/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/replace_flask_send_file.py` & `codemodder-0.88.0/src/core_codemods/replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/requests_verify.py` & `codemodder-0.88.0/src/core_codemods/requests_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/secure_flask_cookie.py` & `codemodder-0.88.0/src/core_codemods/secure_flask_cookie.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from libcst import matchers
-
-from codemodder.codemods.libcst_transformer import NewArg
 from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
+from core_codemods.secure_cookie_mixin import SecureCookieMixin
 
 
-class SecureFlaskCookie(SimpleCodemod):
+class SecureFlaskCookie(SimpleCodemod, SecureCookieMixin):
     metadata = Metadata(
         name="secure-flask-cookie",
         summary="Use Safe Parameters in `flask` Response `set_cookie` Call",
         review_guidance=ReviewGuidance.MERGE_AFTER_CURSORY_REVIEW,
         references=[
             Reference(
                 url="https://flask.palletsprojects.com/en/3.0.x/api/#flask.Response.set_cookie"
@@ -38,34 +36,12 @@
             pattern-sinks:
               - patterns:
                 - pattern: $SINK.set_cookie(...)
                 - pattern-not: $SINK.set_cookie(..., secure=True, ..., httponly=True, ..., samesite="Lax", ...)
                 - pattern-not: $SINK.set_cookie(..., secure=True, ..., httponly=True, ..., samesite="Strict", ...)
         """
 
-    def _choose_new_args(self, original_node):
-        new_args = [
-            NewArg(name="secure", value="True", add_if_missing=True),
-            NewArg(name="httponly", value="True", add_if_missing=True),
-        ]
-
-        samesite = matchers.Arg(
-            keyword=matchers.Name(value="samesite"),
-            value=matchers.SimpleString(value="'Strict'"),
-        )
-
-        # samesite=Strict is OK because it's more restrictive than Lax.
-        strict_samesite_defined = any(
-            matchers.matches(arg, samesite) for arg in original_node.args
-        )
-        if not strict_samesite_defined:
-            new_args.append(
-                NewArg(name="samesite", value="'Lax'", add_if_missing=True),
-            )
-
-        return new_args
-
     def on_result_found(self, original_node, updated_node):
         new_args = self.replace_args(
             original_node, self._choose_new_args(original_node)
         )
         return self.update_arg_target(updated_node, new_args)
```

### Comparing `codemodder-0.87.0/src/core_codemods/secure_flask_session_config.py` & `codemodder-0.88.0/src/core_codemods/secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/secure_random.py` & `codemodder-0.88.0/src/core_codemods/secure_random.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,49 @@
-from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
+from codemodder.codemods.libcst_transformer import (
+    LibcstResultTransformer,
+    LibcstTransformerPipeline,
+)
+from codemodder.codemods.semgrep import SemgrepRuleDetector
+from codemodder.codemods.utils_mixin import NameResolutionMixin
+from core_codemods.api import CoreCodemod, Metadata, Reference, ReviewGuidance
 
 
-class SecureRandom(SimpleCodemod):
-    metadata = Metadata(
+class SecureRandomTransformer(LibcstResultTransformer, NameResolutionMixin):
+    change_description = (
+        "Replace random.{func} with more secure secrets library functions."
+    )
+
+    def on_result_found(self, original_node, updated_node):
+        self.remove_unused_import(original_node)
+        self.add_needed_import("secrets")
+
+        if self.find_base_name(original_node.func) == "random.choice":
+            return self.update_call_target(updated_node, "secrets")
+        return self.update_call_target(updated_node, "secrets.SystemRandom()")
+
+
+SecureRandom = CoreCodemod(
+    metadata=Metadata(
         name="secure-random",
         review_guidance=ReviewGuidance.MERGE_AFTER_CURSORY_REVIEW,
         summary="Secure Source of Randomness",
         references=[
             Reference(
                 url="https://owasp.org/www-community/vulnerabilities/Insecure_Randomness",
             ),
             Reference(
                 url="https://docs.python.org/3/library/random.html",
             ),
         ],
-    )
-
-    detector_pattern = """
-        - patterns:
-          - pattern: random.$F(...)
-          - pattern-not: random.SystemRandom()
-          - pattern-inside: |
-              import random
-              ...
-    """
-
-    change_description = (
-        "Replace random.{func} with more secure secrets library functions."
-    )
-
-    def on_result_found(self, original_node, updated_node):
-        self.remove_unused_import(original_node)
-        self.add_needed_import("secrets")
-        return self.update_call_target(updated_node, "secrets.SystemRandom()")
+    ),
+    detector=SemgrepRuleDetector(
+        """
+            - patterns:
+              - pattern: random.$F(...)
+              - pattern-not: random.SystemRandom()
+              - pattern-inside: |
+                  import random
+                  ...
+        """
+    ),
+    transformer=LibcstTransformerPipeline(SecureRandomTransformer),
+)
```

### Comparing `codemodder-0.87.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py` & `codemodder-0.88.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/sql_parameterization.py` & `codemodder-0.88.0/src/core_codemods/sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/str_concat_in_seq_literal.py` & `codemodder-0.88.0/src/core_codemods/str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/subprocess_shell_false.py` & `codemodder-0.88.0/src/core_codemods/subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/tempfile_mktemp.py` & `codemodder-0.88.0/src/core_codemods/tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_minimum_version.py` & `codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/upgrade_sslcontext_tls.py` & `codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/url_sandbox.py` & `codemodder-0.88.0/src/core_codemods/url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/use_defused_xml.py` & `codemodder-0.88.0/src/core_codemods/use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/use_generator.py` & `codemodder-0.88.0/src/core_codemods/use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/use_set_literal.py` & `codemodder-0.88.0/src/core_codemods/use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/use_walrus_if.py` & `codemodder-0.88.0/src/core_codemods/use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/src/core_codemods/with_threading_lock.py` & `codemodder-0.88.0/src/core_codemods/with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_add_requests_timeouts.py` & `codemodder-0.88.0/tests/codemods/test_add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_async_fix_task_instantiation.py` & `codemodder-0.88.0/tests/codemods/test_async_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_base_codemod.py` & `codemodder-0.88.0/tests/codemods/test_base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_base_visitor.py` & `codemodder-0.88.0/tests/codemods/test_base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_combine_startswith_endswith.py` & `codemodder-0.88.0/tests/codemods/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_django_debug_flag_on.py` & `codemodder-0.88.0/tests/codemods/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_django_json_response_type.py` & `codemodder-0.88.0/tests/codemods/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_django_model_without_dunder_str.py` & `codemodder-0.88.0/tests/codemods/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_django_receiver_on_top.py` & `codemodder-0.88.0/tests/codemods/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_django_session_cookie_secure_off.py` & `codemodder-0.88.0/tests/codemods/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_enable_jinja2_autoescape.py` & `codemodder-0.88.0/tests/codemods/test_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_exception_without_raise.py` & `codemodder-0.88.0/tests/codemods/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_file_resource_leak.py` & `codemodder-0.88.0/tests/codemods/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_assert_tuple.py` & `codemodder-0.88.0/tests/codemods/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_dataclass_defaults.py` & `codemodder-0.88.0/tests/codemods/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_deprecated_abstractproperty.py` & `codemodder-0.88.0/tests/codemods/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_deprecated_logging_warn.py` & `codemodder-0.88.0/tests/codemods/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_empty_sequence_comparison.py` & `codemodder-0.88.0/tests/codemods/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_hasattr_call.py` & `codemodder-0.88.0/tests/codemods/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_missing_self_or_cls.py` & `codemodder-0.88.0/tests/codemods/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_fix_mutable_params.py` & `codemodder-0.88.0/tests/codemods/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_flask_enable_csrf_protection.py` & `codemodder-0.88.0/tests/codemods/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_flask_json_response_type.py` & `codemodder-0.88.0/tests/codemods/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_harden_pickle_load.py` & `codemodder-0.88.0/tests/codemods/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_harden_pyyaml.py` & `codemodder-0.88.0/tests/codemods/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_harden_ruamel.py` & `codemodder-0.88.0/tests/codemods/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_https_connection.py` & `codemodder-0.88.0/tests/codemods/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_include_exclude.py` & `codemodder-0.88.0/tests/codemods/test_include_exclude.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_jwt_decode_verify.py` & `codemodder-0.88.0/tests/codemods/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_lazy_logging.py` & `codemodder-0.88.0/tests/codemods/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_limit_readline.py` & `codemodder-0.88.0/tests/codemods/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_literal_or_new_object_identity.py` & `codemodder-0.88.0/tests/codemods/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_lxml_safe_parameter_defaults.py` & `codemodder-0.88.0/tests/codemods/test_lxml_safe_parameter_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_lxml_safe_parsing.py` & `codemodder-0.88.0/tests/codemods/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_numpy_nan_equality.py` & `codemodder-0.88.0/tests/codemods/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_order_imports.py` & `codemodder-0.88.0/tests/codemods/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_process_creation_sandbox.py` & `codemodder-0.88.0/tests/codemods/test_process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.88.0/tests/codemods/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_debug_breakpoint.py` & `codemodder-0.88.0/tests/codemods/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_future_imports.py` & `codemodder-0.88.0/tests/codemods/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_module_global.py` & `codemodder-0.88.0/tests/codemods/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_unnecessary_f_str.py` & `codemodder-0.88.0/tests/codemods/test_remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_remove_unused_imports.py` & `codemodder-0.88.0/tests/codemods/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_replace_flask_send_file.py` & `codemodder-0.88.0/tests/codemods/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_request_verify.py` & `codemodder-0.88.0/tests/codemods/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_secure_flask_cookie.py` & `codemodder-0.88.0/tests/codemods/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_secure_flask_session_config.py` & `codemodder-0.88.0/tests/codemods/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_secure_random.py` & `codemodder-0.88.0/tests/codemods/test_secure_random.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,26 @@
         assert self.codemod.name == "secure-random"
 
     def test_import_random(self, tmpdir):
         input_code = """
         import random
 
         random.random()
+        random.getrandbits(1)
         var = "hello"
         """
         expected_output = """
         import secrets
 
         secrets.SystemRandom().random()
+        secrets.SystemRandom().getrandbits(1)
         var = "hello"
         """
 
-        self.run_and_assert(tmpdir, input_code, expected_output)
+        self.run_and_assert(tmpdir, input_code, expected_output, num_changes=2)
 
     def test_from_random(self, tmpdir):
         input_code = """
         from random import random
 
         random()
         var = "hello"
@@ -195,7 +197,39 @@
     def test_random_systemrandom_import_alias(self, tmpdir):
         input_code = """
         import random as domran
 
         rand = domran.SystemRandom()
         """
         self.run_and_assert(tmpdir, input_code, input_code)
+
+    def test_sampling(self, tmpdir):
+        input_code = """
+        import random
+
+        random.sample(["a", "b"], 1)
+        random.choice(["a", "b"])
+        random.choices(["a", "b"])
+        """
+        expected_output = """
+        import secrets
+
+        secrets.SystemRandom().sample(["a", "b"], 1)
+        secrets.choice(["a", "b"])
+        secrets.SystemRandom().choices(["a", "b"])
+        """
+
+        self.run_and_assert(tmpdir, input_code, expected_output, num_changes=3)
+
+    def test_from_import_choice(self, tmpdir):
+        input_code = """
+        from random import choice
+
+        choice(["a", "b"])
+        """
+        expected_output = """
+        import secrets
+
+        secrets.choice(["a", "b"])
+        """
+
+        self.run_and_assert(tmpdir, input_code, expected_output, num_changes=1)
```

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_django_json_response_type.py` & `codemodder-0.88.0/tests/codemods/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_django_receiver_on_top.py` & `codemodder-0.88.0/tests/codemods/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_exception_without_raise.py` & `codemodder-0.88.0/tests/codemods/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_fix_assert_tuple.py` & `codemodder-0.88.0/tests/codemods/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.88.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_flask_json_response_type.py` & `codemodder-0.88.0/tests/codemods/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_jwt_decode_verify.py` & `codemodder-0.88.0/tests/codemods/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.88.0/tests/codemods/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_numpy_nan_equality.py` & `codemodder-0.88.0/tests/codemods/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.88.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sonar_tempfile_mktemp.py` & `codemodder-0.88.0/tests/codemods/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_sql_parameterization.py` & `codemodder-0.88.0/tests/codemods/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_str_concat_in_seq_literal.py` & `codemodder-0.88.0/tests/codemods/test_str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_subprocess_shell_false.py` & `codemodder-0.88.0/tests/codemods/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_tempfile_mktemp.py` & `codemodder-0.88.0/tests/codemods/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_upgrade_sslcontext_tls.py` & `codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_url_sandbox.py` & `codemodder-0.88.0/tests/codemods/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_use_defused_xml.py` & `codemodder-0.88.0/tests/codemods/test_use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_use_generator.py` & `codemodder-0.88.0/tests/codemods/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_use_set_literal.py` & `codemodder-0.88.0/tests/codemods/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_walrus_if.py` & `codemodder-0.88.0/tests/codemods/test_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/codemods/test_with_threading_lock.py` & `codemodder-0.88.0/tests/codemods/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/conftest.py` & `codemodder-0.88.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_base_dependency_writer.py` & `codemodder-0.88.0/tests/dependency_management/test_base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_dependency_manager.py` & `codemodder-0.88.0/tests/dependency_management/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_pyproject_writer.py` & `codemodder-0.88.0/tests/dependency_management/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_requirements_txt_writer.py` & `codemodder-0.88.0/tests/dependency_management/test_requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_setup_py_writer.py` & `codemodder-0.88.0/tests/dependency_management/test_setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/dependency_management/test_setupcfgt_writer.py` & `codemodder-0.88.0/tests/dependency_management/test_setupcfgt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py` & `codemodder-0.88.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py` & `codemodder-0.88.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py` & `codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py` & `codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/samples/semgrep.sarif` & `codemodder-0.88.0/tests/samples/semgrep.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/samples/sonar_issues.json` & `codemodder-0.88.0/tests/samples/sonar_issues.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/samples/webgoat_v8.2.0_codeql.sarif` & `codemodder-0.88.0/tests/samples/webgoat_v8.2.0_codeql.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_ancestorpatterns_mixin.py` & `codemodder-0.88.0/tests/test_ancestorpatterns_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_basetype.py` & `codemodder-0.88.0/tests/test_basetype.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_cli.py` & `codemodder-0.88.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         )
 
     @pytest.mark.parametrize(
         "cli_args",
         [
             ["--help"],
             [
-                "tests/samples/",
+                "some/path",
                 "--output",
                 "here.txt",
                 "--codemod-include=url-sandbox",
                 "--help",
             ],
         ],
     )
@@ -47,15 +47,15 @@
         assert err.value.args[0] == 0
 
     @pytest.mark.parametrize(
         "cli_args",
         [
             ["--version"],
             [
-                "tests/samples/",
+                "some/path",
                 "--output",
                 "here.txt",
                 "--codemod-include=url-sandbox",
                 "--version",
             ],
         ],
     )
@@ -68,15 +68,15 @@
         assert err.value.args[0] == 0
 
     @pytest.mark.parametrize(
         "cli_args",
         [
             ["--list"],
             [
-                "tests/samples/",
+                "some/path",
                 "--output",
                 "here.txt",
                 "--list",
             ],
         ],
     )
     @mock.patch("builtins.print")
@@ -108,15 +108,15 @@
         )
 
     @mock.patch("codemodder.cli.logger.error")
     def test_bad_output_format(self, error_logger):
         with pytest.raises(SystemExit) as err:
             parse_args(
                 [
-                    "tests/samples/",
+                    "some/path",
                     "--output",
                     "here.txt",
                     "--output-format",
                     "hello",
                 ],
                 self.registry,
             )
@@ -128,15 +128,15 @@
         )
 
     @mock.patch("codemodder.cli.logger.error")
     def test_bad_option(self, error_logger):
         with pytest.raises(SystemExit) as err:
             parse_args(
                 [
-                    "tests/samples/",
+                    "some/path",
                     "--output",
                     "here.txt",
                     "--codemod=url-sandbox",
                     "--path-exclude",
                     "*request.py",
                 ],
                 self.registry,
@@ -148,14 +148,14 @@
             "ambiguous option: --codemod=url-sandbox could match --codemod-exclude, --codemod-include",
         )
 
     @pytest.mark.parametrize("codemod", ["secure-random", "pixee:python/secure-random"])
     def test_codemod_name_or_id(self, codemod):
         parse_args(
             [
-                "tests/samples/",
+                "some/path",
                 "--output",
                 "here.txt",
                 f"--codemod-include={codemod}",
             ],
             self.registry,
         )
```

### Comparing `codemodder-0.87.0/tests/test_code_directory.py` & `codemodder-0.88.0/tests/test_code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_codemod_docs.py` & `codemodder-0.88.0/tests/test_codemod_docs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_codemodder.py` & `codemodder-0.88.0/tests/test_codemodder.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,42 +2,66 @@
 import mock
 import pytest
 
 from codemodder.codemodder import find_semgrep_results, run
 from codemodder.diff import create_diff_from_tree
 from codemodder.registry import load_registered_codemods
 from codemodder.result import ResultSet
-from codemodder.semgrep import run as semgrep_run
 
 
 @pytest.fixture(autouse=True, scope="module")
 def disable_write_report():
     """Override fixture from conftest.py"""
 
 
 @pytest.fixture(autouse=True)
 def disable_codemod_apply(mocker, request):
     """
     The tests in this module are like integration tests in that they  often
     run all of codemodder but we most often don't need to actually apply codemods.
     """
     # Skip mocking only for specific tests that need to apply codemods.
-    if request.function.__name__ == "test_cst_parsing_fails":
+    if request.function.__name__ in (
+        "test_cst_parsing_fails",
+        "test_dry_run",
+        "test_run_codemod_name_or_id",
+    ):
         return
     mocker.patch("codemodder.codemods.base_codemod.BaseCodemod.apply")
 
 
+@pytest.fixture(scope="function")
+def dir_structure(tmp_path_factory):
+    code_dir = tmp_path_factory.mktemp("code")
+    (code_dir / "test_request.py").write_text(
+        """
+    from test_sources import untrusted_data
+    import requests
+
+    url = untrusted_data()
+    requests.get(url)
+    var = "hello"
+    """
+    )
+    (code_dir / "test_random.py").write_text(
+        """
+    import random
+    def func(foo=[]):
+        return random.random()
+    """
+    )
+    codetf = code_dir / "result.codetf"
+    assert not codetf.exists()
+    return code_dir, codetf
+
+
 class TestRun:
     @mock.patch("libcst.parse_module")
-    def test_no_files_matched(self, mock_parse, tmpdir):
-        codetf = tmpdir / "result.codetf"
-        code_dir = tmpdir.mkdir("code")
-        code_dir.join("code.py").write("# anything")
-        assert not codetf.exists()
-
+    def test_no_files_matched(self, mock_parse, dir_structure):
+        code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
             str(codetf),
             "--codemod-include=url-sandbox",
             "--path-exclude",
             "*py",
@@ -46,23 +70,20 @@
         assert res == 0
 
         mock_parse.assert_not_called()
         assert codetf.exists()
 
     @mock.patch("libcst.parse_module", side_effect=Exception)
     @mock.patch("codemodder.codetf.CodeTF.build")
-    def test_cst_parsing_fails(self, build_report, mock_parse, tmpdir):
-        code_dir = tmpdir.mkdir("code")
-        code_file = code_dir.join("test_request.py")
-        code_file.write("# anything")
-
+    def test_cst_parsing_fails(self, build_report, mock_parse, dir_structure):
+        code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
-            str(tmpdir / "result.codetf"),
+            str(codetf),
             "--codemod-include",
             "fix-assert-tuple",
             "--path-include",
             "*request.py",
         ]
 
         res = run(args)
@@ -76,47 +97,52 @@
         _, _, _, results_by_codemod = args_to_reporting
         assert results_by_codemod != []
 
         requests_report = results_by_codemod[0]
         assert requests_report.changeset == []
         assert len(requests_report.failedFiles) == 1
         assert sorted(requests_report.failedFiles) == [
-            str(code_file),
+            str(code_dir / "test_request.py"),
         ]
 
         build_report.return_value.write_report.assert_called_once()
 
     @mock.patch("codemodder.codemods.libcst_transformer.update_code")
-    @mock.patch("codemodder.codemods.semgrep.semgrep_run", side_effect=semgrep_run)
-    def test_dry_run(self, _, mock_update_code, tmpdir):
-        codetf = tmpdir / "result.codetf"
+    @mock.patch(
+        "codemodder.codemods.libcst_transformer.LibcstTransformerPipeline.apply",
+        new_callable=mock.PropertyMock,
+    )
+    @mock.patch("codemodder.context.CodemodExecutionContext.compile_results")
+    def test_dry_run(self, _, transform_apply, mock_update_code, dir_structure):
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
             str(codetf),
             "--dry-run",
             # Make this test faster by restricting the number of codemods
             "--codemod-include=url-sandbox",
         ]
 
         assert not codetf.exists()
 
         res = run(args)
         assert res == 0
         assert codetf.exists()
-
+        transform_apply.assert_called()
         mock_update_code.assert_not_called()
 
     @pytest.mark.parametrize("dry_run", [True, False])
     @mock.patch("codemodder.codetf.CodeTF.build")
-    def test_reporting(self, mock_reporting, dry_run):
+    def test_reporting(self, mock_reporting, dry_run, dir_structure):
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             # Make this test faster by restricting the number of codemods
             "--codemod-include=use-generator,use-defusedxml,use-walrus-if",
         ]
         if dry_run:
             args += ["--dry-run"]
 
         res = run(args)
@@ -128,42 +154,57 @@
         _, _, _, results_by_codemod = args_to_reporting
 
         assert len(results_by_codemod) == 3
 
         mock_reporting.return_value.write_report.assert_called_once()
 
     @pytest.mark.parametrize("codemod", ["secure-random", "pixee:python/secure-random"])
+    @mock.patch(
+        "codemodder.codemods.libcst_transformer.LibcstTransformerPipeline.apply",
+        new_callable=mock.PropertyMock,
+    )
     @mock.patch("codemodder.context.CodemodExecutionContext.compile_results")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_run_codemod_name_or_id(self, write_report, mock_compile_results, codemod):
+    def test_run_codemod_name_or_id(
+        self,
+        write_report,
+        mock_compile_results,
+        transform_apply,
+        codemod,
+        dir_structure,
+    ):
         del write_report
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             f"--codemod-include={codemod}",
         ]
 
         exit_code = run(args)
         assert exit_code == 0
-        # todo: if no codemods run do we still compile results?
         mock_compile_results.assert_called()
+        transform_apply.assert_called()
 
 
 class TestCodemodIncludeExclude:
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_codemod_include_no_match(self, write_report, info_logger, warning_logger):
+    def test_codemod_include_no_match(
+        self, write_report, info_logger, warning_logger, dir_structure
+    ):
         bad_codemod = "doesntexist"
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             f"--codemod-include={bad_codemod}",
         ]
         run(args)
         write_report.assert_called_once()
 
         assert any("no codemods to run" in x[0][0] for x in info_logger.call_args_list)
         assert any(x[0] == ("scanned: %s files", 0) for x in info_logger.call_args_list)
@@ -173,44 +214,46 @@
             for x in warning_logger.call_args_list
         )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     def test_codemod_include_some_match(
-        self, write_report, info_logger, warning_logger
+        self, write_report, info_logger, warning_logger, dir_structure
     ):
         bad_codemod = "doesntexist"
         good_codemod = "secure-random"
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             f"--codemod-include={bad_codemod},{good_codemod}",
         ]
         run(args)
         write_report.assert_called_once()
         assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
         assert any(
             f"Requested codemod to include'{bad_codemod}' does not exist." in x[0][0]
             for x in warning_logger.call_args_list
         )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     def test_codemod_exclude_some_match(
-        self, write_report, info_logger, warning_logger
+        self, write_report, info_logger, warning_logger, dir_structure
     ):
         bad_codemod = "doesntexist"
         good_codemod = "secure-random"
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             f"--codemod-exclude={bad_codemod},{good_codemod}",
         ]
         run(args)
         write_report.assert_called_once()
         codemods_that_ran = [
             x[0][1]
             for x in info_logger.call_args_list
@@ -225,58 +268,60 @@
         )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     @mock.patch("codemodder.codemods.base_codemod.BaseCodemod.apply")
     def test_codemod_exclude_no_match(
-        self, apply, write_report, info_logger, warning_logger
+        self, apply, write_report, info_logger, warning_logger, dir_structure
     ):
         bad_codemod = "doesntexist"
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
-            "here.txt",
+            str(codetf),
             f"--codemod-exclude={bad_codemod}",
         ]
 
         run(args)
         write_report.assert_called_once()
         assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
         assert any(
             f"Requested codemod to exclude'{bad_codemod}' does not exist." in x[0][0]
             for x in warning_logger.call_args_list
         )
 
     @mock.patch("codemodder.codemods.semgrep.semgrep_run")
-    def test_exclude_all_registered_codemods(self, mock_semgrep_run, tmpdir):
-        codetf = tmpdir / "result.codetf"
+    def test_exclude_all_registered_codemods(self, mock_semgrep_run, dir_structure):
+        code_dir, codetf = dir_structure
         assert not codetf.exists()
 
         registry = load_registered_codemods()
         names = ",".join(registry.names)
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
             str(codetf),
             f"--codemod-exclude={names}",
         ]
 
         exit_code = run(args)
         assert exit_code == 0
         mock_semgrep_run.assert_not_called()
         assert codetf.exists()
 
 
 class TestExitCode:
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_success_0(self, mock_report):
+    def test_no_changes_success_0(self, mock_report, dir_structure):
         del mock_report
+        code_dir, codetf = dir_structure
         args = [
-            "tests/samples/",
+            str(code_dir),
             "--output",
             "here.txt",
             "--codemod-include=url-sandbox",
             "--path-exclude",
             "*request.py",
         ]
 
@@ -296,15 +341,15 @@
         exit_code = run(args)
         assert exit_code == 1
 
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     def test_conflicting_include_exclude(self, mock_report):
         del mock_report
         args = [
-            "tests/samples/",
+            "anything",
             "--output",
             "here.txt",
             "--codemod-exclude",
             "secure-random",
             "--codemod-include",
             "secure-random",
         ]
```

### Comparing `codemodder-0.87.0/tests/test_codetf.py` & `codemodder-0.88.0/tests/test_codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_context.py` & `codemodder-0.88.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_format_string_parser.py` & `codemodder-0.88.0/tests/test_format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_linearize_string_expression.py` & `codemodder-0.88.0/tests/test_linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_logging.py` & `codemodder-0.88.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_nameresolution_mixin.py` & `codemodder-0.88.0/tests/test_nameresolution_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_results.py` & `codemodder-0.88.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/test_sarif_processing.py` & `codemodder-0.88.0/tests/test_sarif_processing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/transformations/test_clean_code.py` & `codemodder-0.88.0/tests/transformations/test_clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/transformations/test_remove_empty_string_concatenation.py` & `codemodder-0.88.0/tests/transformations/test_remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.87.0/tests/transformations/test_remove_unused_imports.py` & `codemodder-0.88.0/tests/transformations/test_remove_unused_imports.py`

 * *Files identical despite different names*

