# Comparing `tmp/authx-1.0.1b1.tar.gz` & `tmp/authx-1.1.0.tar.gz`

## Comparing `authx-1.0.1b1.tar` & `authx-1.1.0.tar`

### file list

```diff
@@ -1,81 +1,109 @@
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 authx-1.0.1b1/.all-contributorsrc
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx-1.0.1b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 authx-1.0.1b1/mkdocs.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/FUNDING.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/SECURITY.md
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/dependabot.yml
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.0.1b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/__init__.py
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/config.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/core.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/dependencies.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/exceptions.py
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/py.typed
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/schema.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/token.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/types.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/__init__.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_callback.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_error.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_logger.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_memory.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_signature.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 authx-1.0.1b1/authx/_internal/_utils.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/contributing.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/faq.md
--rw-r--r--   0        0        0    86820 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/favicon.png
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/header.svg
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/help.md
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/index.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/installation.md
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/license.md
--rw-r--r--   0        0        0    65324 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/release.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/css/custom.css
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/css/termynal.css
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Cache.md
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Metrics.md
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/OAuth2.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/Sessions.md
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/extra/profiler.md
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/get-started/basic-usage.md
--rw-r--r--   0        0        0   495130 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/img/install.gif
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.0.1b1/docs/js/termynal.js
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/all.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/docs.in
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/docs.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/linting.in
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/linting.txt
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/pyproject.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/testing.in
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 authx-1.0.1b1/requirements/testing.txt
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/clean.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/docs_build.sh
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/docs_serve.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/format.sh
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/install.sh
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/mypy.sh
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/requirements.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.0.1b1/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/__init__.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_authx.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_callback.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_config.py
--rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_core.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_dependencies.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_errors.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_schema.py
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_logger.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_memory.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_signature.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.0.1b1/tests/internal/test_utils.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.0.1b1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.0.1b1/LICENSE
--rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 authx-1.0.1b1/README.md
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 authx-1.0.1b1/pyproject.toml
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 authx-1.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 authx-1.1.0/.all-contributorsrc
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 authx-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 authx-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 authx-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 authx-1.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 authx-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 authx-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 authx-1.1.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 authx-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 authx-1.1.0/authx/__init__.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 authx-1.1.0/authx/config.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 authx-1.1.0/authx/core.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 authx-1.1.0/authx/dependencies.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 authx-1.1.0/authx/exceptions.py
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 authx-1.1.0/authx/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.0/authx/py.typed
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 authx-1.1.0/authx/schema.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 authx-1.1.0/authx/token.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 authx-1.1.0/authx/types.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/__init__.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_callback.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_error.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_logger.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_memory.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_signature.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 authx-1.1.0/authx/_internal/_utils.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 authx-1.1.0/docs/index.md
+-rw-r--r--   0        0        0    49581 2020-02-02 00:00:00.000000 authx-1.1.0/docs/release.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/config.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/dependencies.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/exceptions.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/main.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/reference.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/request.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/token.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/internal/callback.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/internal/errors.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/internal/memory.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 authx-1.1.0/docs/api/internal/signature.md
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 authx-1.1.0/docs/callbacks/token.md
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 authx-1.1.0/docs/callbacks/user.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 authx-1.1.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 authx-1.1.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 authx-1.1.0/docs/dependencies/aliases.md
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 authx-1.1.0/docs/dependencies/bundle.md
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 authx-1.1.0/docs/dependencies/dependencies.md
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 authx-1.1.0/docs/dependencies/injection.md
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 authx-1.1.0/docs/development/contributing.md
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 authx-1.1.0/docs/extra/Cache.md
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 authx-1.1.0/docs/extra/Metrics.md
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 authx-1.1.0/docs/extra/OAuth2.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 authx-1.1.0/docs/extra/Sessions.md
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 authx-1.1.0/docs/extra/profiler.md
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 authx-1.1.0/docs/faq/code_of_conduct.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 authx-1.1.0/docs/faq/faq.md
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 authx-1.1.0/docs/faq/help.md
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 authx-1.1.0/docs/faq/license.md
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/basic-usage.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/installation.md
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/location.md
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/payload.md
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/refresh.md
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 authx-1.1.0/docs/get-started/token.md
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 authx-1.1.0/docs/img/header.svg
+-rw-r--r--   0        0        0   335246 2020-02-02 00:00:00.000000 authx-1.1.0/docs/img/icon.ico
+-rw-r--r--   0        0        0   112430 2020-02-02 00:00:00.000000 authx-1.1.0/docs/img/logo.png
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 authx-1.1.0/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 authx-1.1.0/docs/js/termynal.js
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/all.txt
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/docs.in
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/docs.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/linting.in
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/linting.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/testing.in
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 authx-1.1.0/requirements/testing.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/clean.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/docs_build.sh
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/docs_serve.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/format.sh
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/mypy.sh
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/requirements.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 authx-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_authx.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_callback.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0    13102 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_core.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_errors.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_schema.py
+-rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 authx-1.1.0/tests/test_token.py
+-rw-r--r--   0        0        0     7660 2020-02-02 00:00:00.000000 authx-1.1.0/tests/utils.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/conftest.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/test_access_location.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/test_blocklist_token.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/test_fresh_token.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/test_get_subject.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 authx-1.1.0/tests/app/test_token_protected_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 authx-1.1.0/tests/internal/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 authx-1.1.0/tests/internal/test_logger.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 authx-1.1.0/tests/internal/test_memory.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 authx-1.1.0/tests/internal/test_signature.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 authx-1.1.0/tests/internal/test_utils.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 authx-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 authx-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 authx-1.1.0/README.md
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 authx-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 authx-1.1.0/PKG-INFO
```

### Comparing `authx-1.0.1b1/.all-contributorsrc` & `authx-1.1.0/.all-contributorsrc`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.90625%*

 * *Differences: {"'commitType'": "'docs'",*

 * * "'contributors'": "{insert: [(9, OrderedDict([('login', 'pinchXOXO'), ('name', 'Devy Santo'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/68501799?v=4'), "*

 * *                   "('profile', 'https://github.com/pinchXOXO'), ('contributions', ['infra'])]))], "*

 * *                   'delete: [4, 3]}'}*

```diff
@@ -1,10 +1,11 @@
 {
     "commit": false,
     "commitConvention": "angular",
+    "commitType": "docs",
     "contributors": [
         {
             "avatar_url": "https://avatars.githubusercontent.com/u/52716203?v=4",
             "contributions": [
                 "code",
                 "doc",
                 "maintenance",
@@ -31,32 +32,14 @@
                 "security"
             ],
             "login": "smakosh",
             "name": "Ismail Ghallou ",
             "profile": "https://smakosh.com"
         },
         {
-            "avatar_url": "https://talentuno.com/assets/img/talentuno/mm/mm-letsdoit_num1.png",
-            "contributions": [
-                "financial"
-            ],
-            "login": "talentuno",
-            "name": "talentuno LLC",
-            "profile": "https://talentuno.com/en/matchmakers"
-        },
-        {
-            "avatar_url": "https://res.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco,dpr_1/v1492757324/sdovorqhcnnkgybhf05h.jpg",
-            "contributions": [
-                "financial"
-            ],
-            "login": "Cactus",
-            "name": "Cactus LLC",
-            "profile": "https://www.stryker.com/us/en/index.html"
-        },
-        {
             "avatar_url": "https://avatars.githubusercontent.com/u/76670309?v=4",
             "contributions": [
                 "code",
                 "bug"
             ],
             "login": "MojixCoder",
             "name": "MojixCoder",
@@ -103,14 +86,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/170559?v=4",
             "contributions": [
                 "doc"
             ],
             "login": "alobbs",
             "name": "Alvaro Lopez Ortega",
             "profile": "https://www.linkedin.com/today/author/alobbs"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/68501799?v=4",
+            "contributions": [
+                "infra"
+            ],
+            "login": "pinchXOXO",
+            "name": "Devy Santo",
+            "profile": "https://github.com/pinchXOXO"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `authx-1.0.1b1/.github/workflows/release.yml` & `authx-1.1.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,14 @@
       - name: check GITHUB_REF matches package version
         uses: samuelcolvin/check-python-version@v4.1
         with:
           version_file_path: authx/__init__.py
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `authx-1.0.1b1/authx/config.py` & `authx-1.1.0/authx/config.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/core.py` & `authx-1.1.0/authx/core.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/dependencies.py` & `authx-1.1.0/authx/dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/exceptions.py` & `authx-1.1.0/authx/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,8 +82,13 @@
     pass
 
 
 class InvalidToken(Exception):
     """When a token is invalid for all identity providers"""
 
     def __init__(self, errors):
+        """Initialize InvalidToken Exception
+
+        Args:
+            errors (List[str]): List of errors
+        """
         self.errors = errors
```

### Comparing `authx-1.0.1b1/authx/main.py` & `authx-1.1.0/authx/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import contextlib
 from typing import Any, Callable, Coroutine, Dict, Literal, Optional, overload
 
-from fastapi import Request, Response
+from fastapi import Depends, Request, Response
 
 from authx._internal._callback import _CallbackHandler
 from authx._internal._error import _ErrorHandler
 from authx._internal._utils import get_uuid
 from authx.config import AuthXConfig
 from authx.core import _get_token_from_request
 from authx.dependencies import AuthXDependency
@@ -268,63 +268,75 @@
                 config=self.config,
             )
         except MissingTokenError as e:
             if optional:
                 return None
             raise e
 
-    async def get_access_token_from_request(self, request: Request) -> RequestToken:
+    async def get_access_token_from_request(
+        self, request: Request, locations: Optional[TokenLocations] = None
+    ) -> RequestToken:
         """Dependency to retrieve access token from request
 
         Args:
             request (Request): Request to retrieve access token from
+            locations (Optional[TokenLocations], optional): Locations to retrieve token from. Defaults to None.
 
         Raises:
             MissingTokenError: When no `access` token is available in request
 
         Returns:
             RequestToken: Request Token instance for `access` token type
         """
-        return await self._get_token_from_request(request, optional=False)
+        return await self._get_token_from_request(
+            request, optional=False, locations=locations
+        )
 
-    async def get_refresh_token_from_request(self, request: Request) -> RequestToken:
+    async def get_refresh_token_from_request(
+        self, request: Request, locations: Optional[TokenLocations] = None
+    ) -> RequestToken:
         """Dependency to retrieve refresh token from request
 
         Args:
             request (Request): Request to retrieve refresh token from
+            locations (Optional[TokenLocations], optional): Locations to retrieve token from. Defaults to None.
 
         Raises:
             MissingTokenError: When no `refresh` token is available in request
 
         Returns:
             RequestToken: Request Token instance for `refresh` token type
         """
-        return await self._get_token_from_request(request, refresh=True, optional=False)
+        return await self._get_token_from_request(
+            request, refresh=True, optional=False, locations=locations
+        )
 
     async def _auth_required(
         self,
         request: Request,
         type: str = "access",
         verify_type: bool = True,
         verify_fresh: bool = False,
         verify_csrf: Optional[bool] = None,
+        locations: Optional[TokenLocations] = None,
     ) -> TokenPayload:
         if type == "access":
             method = self.get_access_token_from_request
         elif type == "refresh":
             method = self.get_refresh_token_from_request
         else:
             ...
         if verify_csrf is None:
             verify_csrf = self.config.JWT_COOKIE_CSRF_PROTECT and (
                 request.method.upper() in self.config.JWT_CSRF_METHODS
             )
 
         request_token = await method(
             request=request,
+            locations=locations,
         )
 
         if self.is_token_in_blocklist(request_token.token):
             raise RevokedTokenError("Token has been revoked")
 
         return self.verify_token(
             request_token,
@@ -485,14 +497,62 @@
 
         Args:
             response (Response): response to remove token cookies from
         """
         self.unset_access_cookies(response)
         self.unset_refresh_cookies(response)
 
+    # Notes:
+    # The AuthXDeps is a utility class, to enable quick token operations
+    # within the route logic. It provides methods to avoid addtional code
+    # in your route that would be outside of the route logic
+
+    # Such methods includes setting and unsetting cookies without the need
+    # to generate a response object beforhand.
+
+    @property
+    def DEPENDENCY(self) -> AuthXDependency:
+        """FastAPI Dependency to return an AuthX sub-object within the route context"""
+        return Depends(self.get_dependency)
+
+    @property
+    def BUNDLE(self) -> AuthXDependency:
+        """FastAPI Dependency to return a AuthX sub-object within the route context"""
+        return self.DEPENDENCY
+
+    @property
+    def FRESH_REQUIRED(self) -> TokenPayload:
+        """FastAPI Dependency to enforce valid token availability in request"""
+        return Depends(self.fresh_token_required)
+
+    @property
+    def ACCESS_REQUIRED(self) -> TokenPayload:
+        """FastAPI Dependency to enforce presence of an `access` token in request"""
+        return Depends(self.access_token_required)
+
+    @property
+    def REFRESH_REQUIRED(self) -> TokenPayload:
+        """FastAPI Dependency to enforce presence of a `refresh` token in request"""
+        return Depends(self.refresh_token_required)
+
+    @property
+    def ACCESS_TOKEN(self) -> RequestToken:
+        """FastAPI Dependency to retrieve access token from request"""
+        return Depends(self.get_token_from_request(type="access"))
+
+    @property
+    def REFRESH_TOKEN(self) -> RequestToken:
+        """FastAPI Dependency to retrieve refresh token from request"""
+        return Depends(self.get_token_from_request(type="refresh"))
+
+    @property
+    def CURRENT_SUBJECT(self) -> T:
+        """FastAPI Dependency to retrieve the current subject from request"""
+        return Depends(self.get_current_subject)
+
     def get_dependency(self, request: Request, response: Response) -> AuthXDependency:
         """FastAPI Dependency to return a AuthX sub-object within the route context
 
         Args:
             request (Request): Request context managed by FastAPI
             response (Response): Response context managed by FastAPI
 
@@ -511,34 +571,37 @@
 
     def token_required(
         self,
         type: str = "access",
         verify_type: bool = True,
         verify_fresh: bool = False,
         verify_csrf: Optional[bool] = None,
+        locations: Optional[TokenLocations] = None,
     ) -> Callable[[Request], TokenPayload]:
         """Dependency to enforce valid token availability in request
 
         Args:
             type (str, optional): Require a given token type. Defaults to "access".
             verify_type (bool, optional): Apply type verification. Defaults to True.
             verify_fresh (bool, optional): Require token freshness. Defaults to False.
             verify_csrf (Optional[bool], optional): Enable CSRF verification. Defaults to None.
+            locations (Optional[TokenLocations], optional): Locations to retrieve token from. Defaults to None.
 
         Returns:
             Callable[[Request], TokenPayload]: Dependency for Valid token Payload retrieval
         """
 
         async def _auth_required(request: Request):
             return await self._auth_required(
                 request=request,
                 type=type,
                 verify_csrf=verify_csrf,
                 verify_type=verify_type,
                 verify_fresh=verify_fresh,
+                locations=locations,
             )
 
         return _auth_required
 
     @property
     def fresh_token_required(self) -> Callable[[Request], TokenPayload]:
         """FastAPI Dependency to enforce presence of a `fresh` `access` token in request"""
```

### Comparing `authx-1.0.1b1/authx/schema.py` & `authx-1.1.0/authx/schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/token.py` & `authx-1.1.0/authx/token.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/types.py` & `authx-1.1.0/authx/types.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/_internal/__init__.py` & `authx-1.1.0/authx/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/_internal/_callback.py` & `authx-1.1.0/authx/_internal/_callback.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,22 @@
         """Set callback for model instance"""
         self.callback_get_model_instance = callback
 
     def set_callback_token_blocklist(self, callback: TokenCallback) -> None:
         """Set callback for token"""
         self.callback_is_token_in_blocklist = callback
 
+    def set_subject_getter(self, callback: ModelCallback[T]) -> None:
+        """Set the callback to run for subject retrieval and serialization"""
+        self.set_callback_get_model_instance(callback)
+
+    def set_token_blocklist(self, callback: TokenCallback) -> None:
+        """Set the callback to run for validation of revoked tokens"""
+        self.set_callback_token_blocklist(callback)
+
     def _get_current_subject(self, uid: str, **kwargs) -> T:
         """Get current model instance from callback"""
         self._check_model_callback_is_set()
         callback: ModelCallback[T] = self.callback_get_model_instance
         return callback(uid, **kwargs)
 
     def is_token_in_blocklist(self, token: str, **kwargs) -> bool:
```

### Comparing `authx-1.0.1b1/authx/_internal/_error.py` & `authx-1.1.0/authx/_internal/_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse
 
 from authx import exceptions
 
 
 class _ErrorHandler:
-    def __init__(self) -> None:
-        """Base Handler for FastAPI handling AuthX exceptions"""
+    """Base Handler for FastAPI handling AuthX exceptions"""
 
-        self.MSG_DEFAULT = "AuthX Error"
-        self.MSG_TOKEN_ERROR = "Token Error"
-        self.MSG_MISSING_TOKEN_ERROR = "Missing JWT in request"
-        self.MSG_MISSING_CSRF_ERROR = "Missing CSRF double submit token in request"
-        self.MSG_TOKEN_TYPE_ERROR = "Bad token type"
-        self.MSG_REVOKED_TOKEN_ERROR = "Invalid token"
-        self.MSG_TOKEN_REQUIRED_ERROR = "Token required"
-        self.MSG_FRESH_TOKEN_REQUIRED_ERROR = "Fresh token required"
-        self.MSG_ACCESS_TOKEN_REQUIRED_ERROR = "Access token required"
-        self.MSG_REFRESH_TOKEN_REQUIRED_ERROR = "Refresh token required"
-        self.MSG_CSRF_ERROR = "CSRF double submit does not match"
-        self.MSG_DECODE_JWT_ERROR = "Invalid Token"
+    MSG_DEFAULT = "AuthX Error"
+    MSG_TOKEN_ERROR = "Token Error"
+    MSG_MISSING_TOKEN_ERROR = "Missing JWT in request"
+    MSG_MISSING_CSRF_ERROR = "Missing CSRF double submit token in request"
+    MSG_TOKEN_TYPE_ERROR = "Bad token type"
+    MSG_REVOKED_TOKEN_ERROR = "Invalid token"
+    MSG_TOKEN_REQUIRED_ERROR = "Token required"
+    MSG_FRESH_TOKEN_REQUIRED_ERROR = "Fresh token required"
+    MSG_ACCESS_TOKEN_REQUIRED_ERROR = "Access token required"
+    MSG_REFRESH_TOKEN_REQUIRED_ERROR = "Refresh token required"
+    MSG_CSRF_ERROR = "CSRF double submit does not match"
+    MSG_DECODE_JWT_ERROR = "Invalid Token"
 
     def _error_handler(
         self,
         exception: Type[exceptions.AuthXException],
         status_code: int,
         message: Optional[str] = None,
     ) -> Coroutine[Any, Any, JSONResponse]:
```

### Comparing `authx-1.0.1b1/authx/_internal/_logger.py` & `authx-1.1.0/authx/_internal/_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/authx/_internal/_memory.py` & `authx-1.1.0/authx/_internal/_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import time
 
 
 class MemoryIO:
+    """
+    MemoryIO is a class that implements the IO interface for the session store.
+
+    It is used to store session data in memory.
+    """
+
     def __init__(self):
         """
         Initialize an instance of MemoryIO.
 
         Creates a dictionary to store the session data.
         """
```

### Comparing `authx-1.0.1b1/authx/_internal/_signature.py` & `authx-1.1.0/authx/_internal/_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from itsdangerous import BadTimeSignature, SignatureExpired, URLSafeTimedSerializer
 
 CASUAL_UT = False
 
 
 class SignatureSerializer:
+    """
+    A class that implements a URL-safe timed serializer.
+    """
+
     def __init__(self, secret_key, expired_in=0):
         """
         Initialize the serializer with a secret key and an optional expiration time.
         """
         self.ser = URLSafeTimedSerializer(secret_key)
         self.expired_in = expired_in
```

### Comparing `authx-1.0.1b1/authx/_internal/_utils.py` & `authx-1.1.0/authx/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/code_of_conduct.md` & `authx-1.1.0/docs/faq/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/contributing.md` & `authx-1.1.0/docs/development/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-# Development - Contributing 🐣
+---
+hide:
+  - navigation
+---
 
 First, you might want to see the basic ways to
-[help AuthX and get help](help.md)
+[help AuthX and get help](../faq/help.md)
 
 ## Developing
 
 If you already cloned the repository and you know that you need to deep dive
 into the code, here is a guideline to set up your environment:
 
 ### Virtual environment with `uv`
@@ -111,15 +114,15 @@
 
 #### Including
 
 The Dependencies file contains all the dependencies that you need to develop
 AuthX, which are:
 
 - The Base Dependencies - the ones that are needed to run AuthX.
-  [See Installation](installation.md).
+  [See Installation](../get-started/installation.md).
 
 ### Format
 
 For Providing a good and consistent experience, we recommend using
 [pre-commit](https://pre-commit.com/) - a tool that runs a set of checks before
 you commit your code.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-# Development - Contributing ð£ First, you might want to see the basic ways
-to [help AuthX and get help](help.md) ## Developing If you already cloned the
+--- hide: - navigation --- First, you might want to see the basic ways to [help
+AuthX and get help](../faq/help.md) ## Developing If you already cloned the
 repository and you know that you need to deep dive into the code, here is a
 guideline to set up your environment: ### Virtual environment with `uv` You can
 create a virtual environment in a directory using Python's [`uv`](https://
 github.com/astral-sh/uv) module:
 ```console pip install uv uv venv ```
 That will create a directory `.venv` with the python binaries and then you will
 be able to install packages for that isolated environment. ### Activate the
@@ -24,20 +24,20 @@
 your local environment and not any other that could be installed globally. ###
 pip After activating the environment as described above, Now lets install all
 the package that you need to develop authx:
 ```console $ uv pip install -r requirements/all.txt ---> 100% ```
 It will install all the dependencies in your local environment. #### Including
 The Dependencies file contains all the dependencies that you need to develop
 AuthX, which are: - The Base Dependencies - the ones that are needed to run
-AuthX. [See Installation](installation.md). ### Format For Providing a good and
-consistent experience, we recommend using [pre-commit](https://pre-commit.com/
-) - a tool that runs a set of checks before you commit your code. #### Git
-Hooks First you need to install the [pre-commit](https://pre-commit.com/) tool,
-which is installed before with the Dev Dependencies. Now, install the pre-
-commit hooks in your `.git/hooks/` directory:
+AuthX. [See Installation](../get-started/installation.md). ### Format For
+Providing a good and consistent experience, we recommend using [pre-commit]
+(https://pre-commit.com/) - a tool that runs a set of checks before you commit
+your code. #### Git Hooks First you need to install the [pre-commit](https://
+pre-commit.com/) tool, which is installed before with the Dev Dependencies.
+Now, install the pre-commit hooks in your `.git/hooks/` directory:
 ```console $ pre-commit install ```
 This one will provide a linting check before you commit your code. ####
 Including The `.pre-commit-config.yaml` contains the following configuration
 with the linting packages. - `pre-commit-hooks` - Some out-of-the-box hooks for
 pre-commit. - `ruff-pre-commit` - A tool to check Python code for errors. -
 `black` - A tool to format Python code. - `pyupgrade` - A tool to upgrade
 Python syntax. ## Documentation First, make sure you set up your environment as
```

### Comparing `authx-1.0.1b1/docs/faq.md` & `authx-1.1.0/docs/faq/faq.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Frequently Asked Questions 🍂
 
-![image](header.svg)
+![image](../img/header.svg)
 
 ## What is the purpose of this project?
 
 - This Project is an Authentication Package helping to Add a Fully registration
   and authentication or authorization system to your FastAPI project. Is
   designed to be as customizable and adaptable as possible, so that you can use
   it as you want.
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-# Frequently Asked Questions ð ![image](header.svg) ## What is the purpose
-of this project? - This Project is an Authentication Package helping to Add a
-Fully registration and authentication or authorization system to your FastAPI
-project. Is designed to be as customizable and adaptable as possible, so that
-you can use it as you want. For example, you can use it to create a simple
-authentication system for your FastAPI project, Or Provide a Cache Service for
-your MicroService or API to store the data in a database using Redis and
-MongoDB. ## How to use this project? - Reading the documentation is the best
-way to get started, but if you have any questions, please feel free to contact
-me, I will try as much as I can to help and provide some real world example. ##
-How to Support Project? You can financially support the author (me) through
-_G_i_t_h_u_b_ _S_p_o_n_s_o_r_s. And you can also become a Silver or Gold sponsor for AuthX,
-just contact me by email. - Email: _h_e_l_l_o_@_y_e_z_z_._m_e ### Basic References I use the
-following reference to get The package done: -
+# Frequently Asked Questions ð ![image](../img/header.svg) ## What is the
+purpose of this project? - This Project is an Authentication Package helping to
+Add a Fully registration and authentication or authorization system to your
+FastAPI project. Is designed to be as customizable and adaptable as possible,
+so that you can use it as you want. For example, you can use it to create a
+simple authentication system for your FastAPI project, Or Provide a Cache
+Service for your MicroService or API to store the data in a database using
+Redis and MongoDB. ## How to use this project? - Reading the documentation is
+the best way to get started, but if you have any questions, please feel free to
+contact me, I will try as much as I can to help and provide some real world
+example. ## How to Support Project? You can financially support the author (me)
+through _G_i_t_h_u_b_ _S_p_o_n_s_o_r_s. And you can also become a Silver or Gold sponsor for
+AuthX, just contact me by email. - Email: _h_e_l_l_o_@_y_e_z_z_._m_e ### Basic References I
+use the following reference to get The package done: -
 fastapi.tiangolo.com/> -
 pydantic-docs.helpmanual.io/> -
 indominusbyte.github.io/fastapi-jwt-auth/> -
 camillovisini.com/article/abstracting-fastapi-services/> -
 pyjwt.readthedocs.io/en/latest/> ## License ð This project is licensed under
 the terms of the MIT License.
```

### Comparing `authx-1.0.1b1/docs/header.svg` & `authx-1.1.0/docs/img/header.svg`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/help.md` & `authx-1.1.0/docs/faq/help.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,77 @@
-# Help AuthX - Get Help 🦥
+# Help and Support
 
-Do you like **AuthX**?
+## Do you like **AuthX**?
 
 Would you like to help AuthX, other users, and the author?
 
 Or would you like to get help with **AuthX**?
 
 There are very simple ways to help (several involve just one or two clicks).
 
 And there are several ways to get help too.
 
 ## Follow AuthX's Author
 
-<a href="https://twitter.com/THyasser1" class="external-link" target="_blank">Follow
-@THyasser1 on **Twitter**</a> to get the latest news about **AuthX**.
+[Follow @THyasser1 on **Twitter**](https://x.com/THyasser1) to get the latest news about **AuthX**.
 
 ## Star **AuthX** in GitHub
 
 You can "star" AuthX in GitHub (clicking the star button at the top right):
 <a href="https://github.com/yezz123/AuthX" class="external-link" target="_blank">https://github.com/yezz123/AuthX</a>.
 ⭐️
 
 By adding a star, other users will be able to find it more easily and see that
 it has been already useful for others.
 
 ## Watch the GitHub repository for releases
 
-You can "watch" AuthX in GitHub (clicking the "watch" button at the top right):
-<a href="https://github.com/yezz123/AuthX class="external-link"
-target="\_blank">https://github.com/yezz123/AuthX</a>. 👀
+You can "watch" AuthX in GitHub (clicking the "watch" button at the top right): [yezz123/AuthX](https://github.com/yezz123/AuthX). 👀
 
 There you can select **"Releases only"**.
 
 By doing it, you will receive notifications (in your email) whenever there's a
 new release (a new version) of **AuthX** with bug fixes and new features.
 
 ## Help Author with issues in GitHub
 
-You can see
-<a href="https://github.com/yezz123/AuthX/issues" class="external-link" target="_blank">existing
-issues</a> and try and help others, most of the times they are questions that
-you might already know the answer for. 🤓
-
-## Watch the GitHub repository
-
-You can "watch" AuthX in GitHub (clicking the "watch" button at the top right):
-<a href="https://github.com/yezz123/AuthX class="external-link"
-target="\_blank">https://github.com/yezz123/AuthX</a>. 👀
-
-If you select "Watching" instead of "Releases only" you will receive
-notifications when someone creates a new issue.
-
-Then you can try and help them solve those issues.
+You can see [existing issues](https://github.com/yezz123/AuthX/issues) and try and help others, most of the times they are questions that you might already know the answer for. 🤓
 
 ## Create issues
 
-You can
-<a href="https://github.com/yezz123/AuthX/issues/new/choose" class="external-link" target="_blank">create
-a new issue</a> in the GitHub repository, for example to:
+You can [create a new issue](https://github.com/yezz123/AuthX/issues/new) in the GitHub repository, for example to:
 
 - Ask a **question** or ask about a **problem**.
 - Suggest a new **feature**.
 
 **Note**: if you create an issue, then I'm going to ask you to also help others.
 😉
 
 ## Create a Pull Request
 
-You can [contribute](contributing.md) to the source code with Pull Requests, for
+You can [contribute](../development/contributing.md) to the source code with Pull Requests, for
 example:
 
-- To fix a typo you found on the documentation.
-- To help [translate the documentation](contributing.md) to your language.
-  - You can also help to review the translations created by others.
+- To help [fix the documentation](../development/contributing.md) in general.
+  - You can also help to review the documentation and suggest improvements.
 - To propose new documentation sections.
 - To fix an existing issue/bug.
 - To add a new feature.
 
 ## Sponsor the author
 
 <p align="center">
 <a href="https://github.com/sponsors/yezz123" target="_blank">
 <img src="https://www.pngitem.com/pimgs/m/330-3302960_github-sponsorship-logo-with-smiling-cat-and-heart.png" alt="Buy Me A Coffee"/>
 </a>
 </p>
 
 And you can also become a Silver or Gold sponsor for AuthX, just contact me by email. 🏅🎉
 
-- Email: <a href="mailto:hello@yezz.me" class="external-link" target="_blank">hello@yezz.me</a>
+- Email: [hello@yezz.me](mailto:hello@yezz.me)
 
 ## Sponsor the tools that power AuthX
 
 As you have seen in the documentation, AuthX stands on the shoulders of giants,
 FastAPI, Starlette and Pydantic.
 
 You can also sponsor:
```

#### html2text {}

```diff
@@ -1,36 +1,33 @@
-# Help AuthX - Get Help ð¦¥ Do you like **AuthX**? Would you like to help
-AuthX, other users, and the author? Or would you like to get help with
-**AuthX**? There are very simple ways to help (several involve just one or two
-clicks). And there are several ways to get help too. ## Follow AuthX's Author
-_F_o_l_l_o_w_ _@_T_H_y_a_s_s_e_r_1_ _o_n_ _*_*_T_w_i_t_t_e_r_*_* to get the latest news about **AuthX**. ##
-Star **AuthX** in GitHub You can "star" AuthX in GitHub (clicking the star
-button at the top right): _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_e_z_z_1_2_3_/_A_u_t_h_X. â­ï¸ By adding a
-star, other users will be able to find it more easily and see that it has been
-already useful for others. ## Watch the GitHub repository for releases You can
-"watch" AuthX in GitHub (clicking the "watch" button at the top right): _h_t_t_p_s_:_/
-_/_g_i_t_h_u_b_._c_o_m_/_y_e_z_z_1_2_3_/_A_u_t_h_X. ð There you can select **"Releases only"**. By
-doing it, you will receive notifications (in your email) whenever there's a new
-release (a new version) of **AuthX** with bug fixes and new features. ## Help
-Author with issues in GitHub You can see _e_x_i_s_t_i_n_g_ _i_s_s_u_e_s and try and help
+# Help and Support ## Do you like **AuthX**? Would you like to help AuthX,
+other users, and the author? Or would you like to get help with **AuthX**?
+There are very simple ways to help (several involve just one or two clicks).
+And there are several ways to get help too. ## Follow AuthX's Author [Follow
+@THyasser1 on **Twitter**](https://x.com/THyasser1) to get the latest news
+about **AuthX**. ## Star **AuthX** in GitHub You can "star" AuthX in GitHub
+(clicking the star button at the top right): _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_e_z_z_1_2_3_/_A_u_t_h_X.
+â­ï¸ By adding a star, other users will be able to find it more easily and
+see that it has been already useful for others. ## Watch the GitHub repository
+for releases You can "watch" AuthX in GitHub (clicking the "watch" button at
+the top right): [yezz123/AuthX](https://github.com/yezz123/AuthX). ð There
+you can select **"Releases only"**. By doing it, you will receive notifications
+(in your email) whenever there's a new release (a new version) of **AuthX**
+with bug fixes and new features. ## Help Author with issues in GitHub You can
+see [existing issues](https://github.com/yezz123/AuthX/issues) and try and help
 others, most of the times they are questions that you might already know the
-answer for. ð¤ ## Watch the GitHub repository You can "watch" AuthX in GitHub
-(clicking the "watch" button at the top right): _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_e_z_z_1_2_3_/
-_A_u_t_h_X. ð If you select "Watching" instead of "Releases only" you will
-receive notifications when someone creates a new issue. Then you can try and
-help them solve those issues. ## Create issues You can _c_r_e_a_t_e_ _a_ _n_e_w_ _i_s_s_u_e in
-the GitHub repository, for example to: - Ask a **question** or ask about a
-**problem**. - Suggest a new **feature**. **Note**: if you create an issue,
-then I'm going to ask you to also help others. ð ## Create a Pull Request
-You can [contribute](contributing.md) to the source code with Pull Requests,
-for example: - To fix a typo you found on the documentation. - To help
-[translate the documentation](contributing.md) to your language. - You can also
-help to review the translations created by others. - To propose new
-documentation sections. - To fix an existing issue/bug. - To add a new feature.
-## Sponsor the author
+answer for. ð¤ ## Create issues You can [create a new issue](https://
+github.com/yezz123/AuthX/issues/new) in the GitHub repository, for example to:
+- Ask a **question** or ask about a **problem**. - Suggest a new **feature**.
+**Note**: if you create an issue, then I'm going to ask you to also help
+others. ð ## Create a Pull Request You can [contribute](../development/
+contributing.md) to the source code with Pull Requests, for example: - To help
+[fix the documentation](../development/contributing.md) in general. - You can
+also help to review the documentation and suggest improvements. - To propose
+new documentation sections. - To fix an existing issue/bug. - To add a new
+feature. ## Sponsor the author
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 And you can also become a Silver or Gold sponsor for AuthX, just contact me by
-email. ðð - Email: _h_e_l_l_o_@_y_e_z_z_._m_e ## Sponsor the tools that power AuthX As
-you have seen in the documentation, AuthX stands on the shoulders of giants,
-FastAPI, Starlette and Pydantic. You can also sponsor: - _S_e_b_a_s_t_i_Ã_¡_n_ _R_a_m_Ã_­_r_e_z_ 
-_(_F_a_s_t_A_P_I_) - _S_a_m_u_e_l_ _C_o_l_v_i_n_ _(_P_y_d_a_n_t_i_c_) - _E_n_c_o_d_e_ _(_S_t_a_r_l_e_t_t_e_,_ _U_v_i_c_o_r_n_) --- Thanks!
-ð
+email. ðð - Email: [hello@yezz.me](mailto:hello@yezz.me) ## Sponsor the
+tools that power AuthX As you have seen in the documentation, AuthX stands on
+the shoulders of giants, FastAPI, Starlette and Pydantic. You can also sponsor:
+- _S_e_b_a_s_t_i_Ã_¡_n_ _R_a_m_Ã_­_r_e_z_ _(_F_a_s_t_A_P_I_) - _S_a_m_u_e_l_ _C_o_l_v_i_n_ _(_P_y_d_a_n_t_i_c_) - _E_n_c_o_d_e_ _(_S_t_a_r_l_e_t_t_e_,
+_U_v_i_c_o_r_n_) --- Thanks! ð
```

### Comparing `authx-1.0.1b1/docs/index.md` & `authx-1.1.0/docs/index.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# AuthenticationX 💫
+---
+hide:
+  - navigation
+---
 
 <p align="center">
 <a href="https://authx.yezz.me" target="_blank">
     <img src="https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png" alt="AuthX">
 </a>
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
@@ -34,48 +37,42 @@
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **AuthX** is designed to be as
 customizable and adaptable as possible.
 
-!!! warning
-
-    [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to development of authx V1 which is not yet ready for production use.
-
-    If you're an Authx user, you probably want either Authx V0.9 [Documentation](https://authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-fix) git branch.
-
-## Installation 📦
+## Installation
 
 <div class="termy">
 
 ```console
 $ pip install authx
 
 ---> 100%
 ```
 
 </div>
 
-## Features 🔧
+## Features
 
 - Support Python 3.8+ & Pydantic 2.0+.
 - Multiple customizable authentication backend:
   - JWT authentication backend included
     - JWT encoding/decoding for application authentication
     - Automatic detection of JWTs in requests:
       - JWTs in headers
       - JWTs in cookies
       - JWTs in query parameters
       - JWTs in request bodies
   - Cookie authentication backend included
-- middleware for authentication and authorization through JWT.
+- Middleware for authentication and authorization through JWT.
 - Extensible Error Handling System.
 
-### Extra Features 🎁
+### Extra Features
 
 !!! notes
 
     AuthX is designed to be as customizable and adaptable as possible.
 
     So you need to install [`authx-extra`](https://github.com/yezz123/authx-extra) to get extra features.
 
@@ -83,15 +80,15 @@
 - Support HTTPCache.
 - Support Sessions and Pre-built CRUD functions and Instance to launch Redis.
 - Support Middleware of [pyinstrument](https://pyinstrument.readthedocs.io/) to check your service performance.
 - Support Middleware for collecting and exposing [Prometheus](https://prometheus.io/) metrics.
 
 **Note:** Check [Release Notes](https://authx.yezz.me/release/).
 
-## Project using 🚀
+## Project using
 
 Here is a simple way to kickstart your project with AuthX:
 
 ```python
 from fastapi import FastAPI, Depends, HTTPException
 from authx import AuthX, AuthXConfig, RequestToken
 
@@ -117,21 +114,7 @@
 def get_protected(token: RequestToken = Depends()):
      try:
           auth.verify_token(token=token)
           return {"message": "Hello world !"}
      except Exception as e:
           raise HTTPException(401, detail={"message": str(e)}) from e
 ```
-
-## Links 🔗
-
-- [Homepage](https://authx.yezz.me/)
-- [FAQ](https://authx.yezz.me/faq/)
-- [Release - AuthX](https://authx.yezz.me/release/)
-- [MIT License](https://authx.yezz.me/license/)
-- [Code of Conduct](https://authx.yezz.me/code_of_conduct/)
-- [Contributing](https://authx.yezz.me/contributing/)
-- [Help - Sponsors](https://authx.yezz.me/help/)
-
-## License 📝
-
-This project is licensed under the terms of the MIT License.
```

### Comparing `authx-1.0.1b1/docs/installation.md` & `authx-1.1.0/docs/get-started/installation.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/license.md` & `authx-1.1.0/docs/faq/license.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/css/termynal.css` & `authx-1.1.0/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/extra/Cache.md` & `authx-1.1.0/docs/extra/Cache.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/extra/Metrics.md` & `authx-1.1.0/docs/extra/Metrics.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/extra/OAuth2.md` & `authx-1.1.0/docs/extra/OAuth2.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/extra/Sessions.md` & `authx-1.1.0/docs/extra/Sessions.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/extra/profiler.md` & `authx-1.1.0/docs/extra/profiler.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/get-started/basic-usage.md` & `authx-1.1.0/docs/get-started/basic-usage.md`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/js/custom.js` & `authx-1.1.0/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/docs/js/termynal.js` & `authx-1.1.0/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/requirements/linting.txt` & `authx-1.1.0/requirements/linting.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,41 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --output-file=requirements/linting.txt requirements/linting.in
-#
-black==24.2.0
-    # via -r requirements/linting.in
+# This file was autogenerated by uv via the following command:
+#    uv pip compile requirements/linting.in -o requirements/linting.txt
+black==24.3.0
 cfgv==3.4.0
     # via pre-commit
 click==8.1.7
     # via black
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.13.3
     # via virtualenv
-identify==2.5.33
+identify==2.5.35
     # via pre-commit
-mypy==1.8.0
-    # via -r requirements/linting.in
+mypy==1.9.0
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 nodeenv==1.8.0
     # via pre-commit
-packaging==23.2
+packaging==24.0
     # via black
 pathspec==0.12.1
     # via black
 platformdirs==4.2.0
     # via
     #   black
     #   virtualenv
-pre-commit==3.6.2
-    # via -r requirements/linting.in
-pyupgrade==3.15.1
-    # via -r requirements/linting.in
+pre-commit==3.7.0
+pyupgrade==3.15.2
 pyyaml==6.0.1
     # via pre-commit
-ruff==0.2.2
-    # via -r requirements/linting.in
+ruff==0.3.5
+setuptools==69.2.0
+    # via nodeenv
 tokenize-rt==5.2.0
     # via pyupgrade
-typing-extensions==4.9.0
+typing-extensions==4.10.0
     # via mypy
-virtualenv==20.25.0
+virtualenv==20.25.1
     # via pre-commit
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `authx-1.0.1b1/requirements/testing.txt` & `authx-1.1.0/requirements/testing.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,52 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --output-file=requirements/testing.txt requirements/testing.in
-#
-anyio==4.2.0
+# This file was autogenerated by uv via the following command:
+#    uv pip compile requirements/testing.in -o requirements/testing.txt
+anyio==4.3.0
     # via httpx
 certifi==2024.2.2
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.3.2
     # via requests
-coverage[toml]==7.4.1
-    # via
-    #   coverage
-    #   pytest-cov
+coverage==7.4.4
+    # via pytest-cov
 freezegun==1.4.0
-    # via -r requirements/testing.in
-greenlet==3.0.3
-    # via sqlalchemy
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
-httpx==0.26.0
-    # via -r requirements/testing.in
+httpx==0.27.0
 idna==3.6
     # via
     #   anyio
     #   httpx
     #   requests
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
-    # via -r requirements/testing.in
-packaging==23.2
+packaging==24.0
     # via pytest
 pluggy==1.4.0
     # via pytest
-pytest==8.0.1
+pytest==8.1.1
     # via
-    #   -r requirements/testing.in
     #   pytest-asyncio
     #   pytest-cov
-pytest-asyncio==0.23.5
-    # via -r requirements/testing.in
-pytest-cov==4.1.0
-    # via -r requirements/testing.in
-python-dateutil==2.8.2
+pytest-asyncio==0.23.6
+pytest-cov==5.0.0
+python-dateutil==2.9.0.post0
     # via freezegun
 requests==2.31.0
-    # via -r requirements/testing.in
 six==1.16.0
     # via python-dateutil
-sniffio==1.3.0
+sniffio==1.3.1
     # via
     #   anyio
     #   httpx
-sqlalchemy==2.0.27
-    # via -r requirements/testing.in
-typing-extensions==4.9.0
+sqlalchemy==2.0.29
+typing-extensions==4.10.0
     # via sqlalchemy
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
 websockets==12.0
-    # via -r requirements/testing.in
```

### Comparing `authx-1.0.1b1/scripts/clean.sh` & `authx-1.1.0/scripts/clean.sh`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 rm -f `find . -type f -name '*.py[co]' `
 rm -f `find . -type f -name '*~' `
 rm -f `find . -type f -name '.*~' `
 rm -f `find . -type f -name .coverage`
 rm -f `find . -type f -name coverage.xml`
 rm -f `find . -type f -name ".coverage.*"`
 rm -rf `find . -name __pycache__`
-rm -rf `find . -name authx_profiling_results.html`
-rm -rf `find . -name authx_profiling_results.json`
-rm -rf `find . -name users.db`
 rm -rf `find . -type d -name '*.egg-info' `
 rm -rf `find . -type d -name 'pip-wheel-metadata' `
 rm -rf `find . -type d -name .pytest_cache`
 rm -rf `find . -type d -name .cache`
 rm -rf `find . -type d -name .mypy_cache`
 rm -rf `find . -type d -name htmlcov`
 rm -rf `find . -type d -name "*.egg-info"`
```

### Comparing `authx-1.0.1b1/tests/test_authx.py` & `authx-1.1.0/tests/test_authx.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_callback.py` & `authx-1.1.0/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_config.py` & `authx-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_core.py` & `authx-1.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_dependencies.py` & `authx-1.1.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_errors.py` & `authx-1.1.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_schema.py` & `authx-1.1.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/test_token.py` & `authx-1.1.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/internal/test_logger.py` & `authx-1.1.0/tests/internal/test_logger.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/internal/test_memory.py` & `authx-1.1.0/tests/internal/test_memory.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/internal/test_signature.py` & `authx-1.1.0/tests/internal/test_signature.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/tests/internal/test_utils.py` & `authx-1.1.0/tests/internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/.gitignore` & `authx-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/LICENSE` & `authx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `authx-1.0.1b1/README.md` & `authx-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AuthenticationX 💫
+# Authx
 
 <p align="center">
 <a href="https://authx.yezz.me" target="_blank">
     <img src="https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png" alt="AuthX">
 </a>
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
@@ -34,50 +34,44 @@
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **AuthX** is designed to be as
 customizable and adaptable as possible.
 
-> **Notes**:
->
-> [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to development of authx V1 which is not yet ready for production use.
->
->If you're a Authx user, you probably want either Authx V0.9 [Documentation](https://authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-fix) git branch.
-
-## Features 🔧
+## Features
 
 - [x] Support Python 3.8+ & Pydantic 2.0+.
 - [x] Multiple customizable authentication backend:
   - [x] JWT authentication backend included
     - [x] JWT encoding/decoding for application authentication
     - [x] Automatic detection of JWTs in requests:
       - [x] JWTs in headers
       - [x] JWTs in cookies
       - [x] JWTs in query parameters
       - [x] JWTs in request bodies
   - [x] Cookie authentication backend included
-- [x] middleware for authentication and authorization through JWT.
+- [x] Middleware for authentication and authorization through JWT.
 - [x] Extensible Error Handling System.
 
-### Extra Features 🎁
+### Extra Features
 
 AuthX is designed to be as customizable and adaptable as possible.
 
 So you need to install [`authx-extra`](https://github.com/yezz123/authx-extra) to get extra features.
 
 - [x] Using Redis as a session store & cache.
 - [x] Support HTTPCache.
 - [x] Support Sessions and Pre-built CRUD functions and Instance to launch Redis.
 - [x] Support Middleware of [pyinstrument](https://pyinstrument.readthedocs.io/) to check your service performance.
 - [x] Support Middleware for collecting and exposing [Prometheus](https://prometheus.io/) metrics.
 
 **Note:** Check [Release Notes](https://authx.yezz.me/release/).
 
-## Project using 🚀
+## Project using
 
 Here is a simple way to kickstart your project with AuthX:
 
 ```python
 from fastapi import FastAPI, Depends, HTTPException
 from authx import AuthX, AuthXConfig, RequestToken
 
@@ -104,44 +98,41 @@
      try:
           auth.verify_token(token=token)
           return {"message": "Hello world !"}
      except Exception as e:
           raise HTTPException(401, detail={"message": str(e)}) from e
 ```
 
-## Contributors and sponsors 👏
+## Contributors and sponsors
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-
-[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
-
+[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Thanks goes to these wonderful people
 ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://yezz.me"><img src="https://avatars.githubusercontent.com/u/52716203?v=4?s=100" width="100px;" alt="Yasser Tahiri"/><br /><sub><b>Yasser Tahiri</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=yezz123" title="Code">💻</a> <a href="https://github.com/yezz123/authx/commits?author=yezz123" title="Documentation">📖</a> <a href="#maintenance-yezz123" title="Maintenance">🚧</a> <a href="#infra-yezz123" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://soubai.me"><img src="https://avatars.githubusercontent.com/u/11523791?v=4?s=100" width="100px;" alt="Abderrahim SOUBAI-ELIDRISI"/><br /><sub><b>Abderrahim SOUBAI-ELIDRISI</b></sub></a><br /><a href="https://github.com/yezz123/authx/pulls?q=is%3Apr+reviewed-by%3AAbderrahimSoubaiElidrissi" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/yezz123/authx/commits?author=AbderrahimSoubaiElidrissi" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://smakosh.com"><img src="https://avatars.githubusercontent.com/u/20082141?v=4?s=100" width="100px;" alt="Ismail Ghallou "/><br /><sub><b>Ismail Ghallou </b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=smakosh" title="Code">💻</a> <a href="#security-smakosh" title="Security">🛡️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://talentuno.com/en/matchmakers"><img src="https://talentuno.com/assets/img/talentuno/mm/mm-letsdoit_num1.png?s=100" width="100px;" alt="talentuno LLC"/><br /><sub><b>talentuno LLC</b></sub></a><br /><a href="#financial-talentuno" title="Financial">💵</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://www.stryker.com/us/en/index.html"><img src="https://res.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco,dpr_1/v1492757324/sdovorqhcnnkgybhf05h.jpg?s=100" width="100px;" alt="Cactus LLC"/><br /><sub><b>Cactus LLC</b></sub></a><br /><a href="#financial-Cactus" title="Financial">💵</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/MojixCoder"><img src="https://avatars.githubusercontent.com/u/76670309?v=4?s=100" width="100px;" alt="MojixCoder"/><br /><sub><b>MojixCoder</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=MojixCoder" title="Code">💻</a> <a href="https://github.com/yezz123/authx/issues?q=author%3AMojixCoder" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://sralab.com"><img src="https://avatars.githubusercontent.com/u/1815?v=4?s=100" width="100px;" alt="Stéphane Raimbault"/><br /><sub><b>Stéphane Raimbault</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=stephane" title="Code">💻</a> <a href="#plugin-stephane" title="Plugin/utility libraries">🔌</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/theoohoho"><img src="https://avatars.githubusercontent.com/u/31537466?v=4?s=100" width="100px;" alt="theoohoho"/><br /><sub><b>theoohoho</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=theoohoho" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://yogeshupadhyay.netlify.app/"><img src="https://avatars.githubusercontent.com/u/53992168?v=4?s=100" width="100px;" alt="Yogesh Upadhyay"/><br /><sub><b>Yogesh Upadhyay</b></sub></a><br /><a href="https://github.com/yezz123/authx/issues?q=author%3AYogeshUpdhyay" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/iftenet"><img src="https://avatars.githubusercontent.com/u/1397880?v=4?s=100" width="100px;" alt="Roman"/><br /><sub><b>Roman</b></sub></a><br /><a href="https://github.com/yezz123/authx/issues?q=author%3Aiftenet" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/today/author/alobbs"><img src="https://avatars.githubusercontent.com/u/170559?v=4?s=100" width="100px;" alt="Alvaro Lopez Ortega"/><br /><sub><b>Alvaro Lopez Ortega</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=alobbs" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pinchXOXO"><img src="https://avatars.githubusercontent.com/u/68501799?v=4?s=100" width="100px;" alt="Devy Santo"/><br /><sub><b>Devy Santo</b></sub></a><br /><a href="#infra-pinchXOXO" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
@@ -156,20 +147,10 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the
 [all-contributors](https://github.com/all-contributors/all-contributors)
 specification. Contributions of any kind welcome!
 
-## Links 🔗
-
-- [Homepage](https://authx.yezz.me/)
-- [FAQ](https://authx.yezz.me/faq/)
-- [Release - AuthX](https://authx.yezz.me/release/)
-- [MIT License](https://authx.yezz.me/license/)
-- [Code of Conduct](https://authx.yezz.me/code_of_conduct/)
-- [Contributing](https://authx.yezz.me/contributing/)
-- [Help - Sponsors](https://authx.yezz.me/help/)
-
-## License 📄
+## License
 
 This project is licensed under the terms of the MIT License.
```

### Comparing `authx-1.0.1b1/pyproject.toml` & `authx-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Framework :: FastAPI",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
-    "Framework :: Pydantic :: 1",
+    "Framework :: Pydantic :: 2",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -42,17 +42,17 @@
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "fastapi >=0.65.2,<0.110.0",
+    "fastapi >=0.100.0,<0.111.0",
     "pyjwt[crypto] >=2.6.0,<3.0.0",
-    "pydantic >=2.0.0,<2.6.1",
+    "pydantic >=2.0.0,<2.6.3",
     "pydantic-settings >=2.1.0",
     "python-dateutil>=2.8,<3.0.0",
     "pytz>=2023.3,<2025.0",
     "python-jose>=3.3.0,<4.0.0",
 ]
 
 dynamic = ["version"]
@@ -78,23 +78,22 @@
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
-    "B008",  # do not perform function calls in argument defaults
-    "C901",  # too complex
-    "F811",  # redefinition of unused
     "B018",  # Found useless expression.
-    "E721",  # Do not compare types, use `isinstance()`
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
+"authx/token.py" = ["C901"]
+"authx/main.py" = ["B008"]
+"tests/utils.py" = ["B008"]
 
 [tool.ruff.lint.isort]
 known-third-party = ["pydantic", "typing_extensions", "sqlalchemy"]
 
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
```

### Comparing `authx-1.0.1b1/PKG-INFO` & `authx-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: authx
-Version: 1.0.1b1
+Version: 1.1.0
 Summary: Ready to use and customizable Authentications and Oauth2 management for FastAPI
 Project-URL: Homepage, https://github.com/yezz123/authx
 Project-URL: Documentation, https://authx.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
-Classifier: Framework :: Pydantic :: 1
+Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -27,24 +27,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: fastapi<0.110.0,>=0.65.2
+Requires-Dist: fastapi<0.111.0,>=0.100.0
 Requires-Dist: pydantic-settings>=2.1.0
-Requires-Dist: pydantic<2.6.1,>=2.0.0
+Requires-Dist: pydantic<2.6.3,>=2.0.0
 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0
 Requires-Dist: python-dateutil<3.0.0,>=2.8
 Requires-Dist: python-jose<4.0.0,>=3.3.0
 Requires-Dist: pytz<2025.0,>=2023.3
 Description-Content-Type: text/markdown
 
-# AuthenticationX 💫
+# Authx
 
 <p align="center">
 <a href="https://authx.yezz.me" target="_blank">
     <img src="https://user-images.githubusercontent.com/52716203/136962014-280d82b0-0640-4ee5-9a11-b451b338f6d8.png" alt="AuthX">
 </a>
 <p align="center">
     <em>Ready-to-use and customizable Authentications and Oauth2 management for FastAPI ⚡</em>
@@ -76,50 +76,44 @@
 
 ---
 
 Add a Fully registration and authentication or authorization system to your
 [FastAPI](https://fastapi.tiangolo.com/) project. **AuthX** is designed to be as
 customizable and adaptable as possible.
 
-> **Notes**:
->
-> [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to development of authx V1 which is not yet ready for production use.
->
->If you're a Authx user, you probably want either Authx V0.9 [Documentation](https://authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-fix) git branch.
-
-## Features 🔧
+## Features
 
 - [x] Support Python 3.8+ & Pydantic 2.0+.
 - [x] Multiple customizable authentication backend:
   - [x] JWT authentication backend included
     - [x] JWT encoding/decoding for application authentication
     - [x] Automatic detection of JWTs in requests:
       - [x] JWTs in headers
       - [x] JWTs in cookies
       - [x] JWTs in query parameters
       - [x] JWTs in request bodies
   - [x] Cookie authentication backend included
-- [x] middleware for authentication and authorization through JWT.
+- [x] Middleware for authentication and authorization through JWT.
 - [x] Extensible Error Handling System.
 
-### Extra Features 🎁
+### Extra Features
 
 AuthX is designed to be as customizable and adaptable as possible.
 
 So you need to install [`authx-extra`](https://github.com/yezz123/authx-extra) to get extra features.
 
 - [x] Using Redis as a session store & cache.
 - [x] Support HTTPCache.
 - [x] Support Sessions and Pre-built CRUD functions and Instance to launch Redis.
 - [x] Support Middleware of [pyinstrument](https://pyinstrument.readthedocs.io/) to check your service performance.
 - [x] Support Middleware for collecting and exposing [Prometheus](https://prometheus.io/) metrics.
 
 **Note:** Check [Release Notes](https://authx.yezz.me/release/).
 
-## Project using 🚀
+## Project using
 
 Here is a simple way to kickstart your project with AuthX:
 
 ```python
 from fastapi import FastAPI, Depends, HTTPException
 from authx import AuthX, AuthXConfig, RequestToken
 
@@ -146,44 +140,41 @@
      try:
           auth.verify_token(token=token)
           return {"message": "Hello world !"}
      except Exception as e:
           raise HTTPException(401, detail={"message": str(e)}) from e
 ```
 
-## Contributors and sponsors 👏
+## Contributors and sponsors
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-
-[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
-
+[![All Contributors](https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Thanks goes to these wonderful people
 ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://yezz.me"><img src="https://avatars.githubusercontent.com/u/52716203?v=4?s=100" width="100px;" alt="Yasser Tahiri"/><br /><sub><b>Yasser Tahiri</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=yezz123" title="Code">💻</a> <a href="https://github.com/yezz123/authx/commits?author=yezz123" title="Documentation">📖</a> <a href="#maintenance-yezz123" title="Maintenance">🚧</a> <a href="#infra-yezz123" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://soubai.me"><img src="https://avatars.githubusercontent.com/u/11523791?v=4?s=100" width="100px;" alt="Abderrahim SOUBAI-ELIDRISI"/><br /><sub><b>Abderrahim SOUBAI-ELIDRISI</b></sub></a><br /><a href="https://github.com/yezz123/authx/pulls?q=is%3Apr+reviewed-by%3AAbderrahimSoubaiElidrissi" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/yezz123/authx/commits?author=AbderrahimSoubaiElidrissi" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://smakosh.com"><img src="https://avatars.githubusercontent.com/u/20082141?v=4?s=100" width="100px;" alt="Ismail Ghallou "/><br /><sub><b>Ismail Ghallou </b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=smakosh" title="Code">💻</a> <a href="#security-smakosh" title="Security">🛡️</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://talentuno.com/en/matchmakers"><img src="https://talentuno.com/assets/img/talentuno/mm/mm-letsdoit_num1.png?s=100" width="100px;" alt="talentuno LLC"/><br /><sub><b>talentuno LLC</b></sub></a><br /><a href="#financial-talentuno" title="Financial">💵</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://www.stryker.com/us/en/index.html"><img src="https://res.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco,dpr_1/v1492757324/sdovorqhcnnkgybhf05h.jpg?s=100" width="100px;" alt="Cactus LLC"/><br /><sub><b>Cactus LLC</b></sub></a><br /><a href="#financial-Cactus" title="Financial">💵</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/MojixCoder"><img src="https://avatars.githubusercontent.com/u/76670309?v=4?s=100" width="100px;" alt="MojixCoder"/><br /><sub><b>MojixCoder</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=MojixCoder" title="Code">💻</a> <a href="https://github.com/yezz123/authx/issues?q=author%3AMojixCoder" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://sralab.com"><img src="https://avatars.githubusercontent.com/u/1815?v=4?s=100" width="100px;" alt="Stéphane Raimbault"/><br /><sub><b>Stéphane Raimbault</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=stephane" title="Code">💻</a> <a href="#plugin-stephane" title="Plugin/utility libraries">🔌</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/theoohoho"><img src="https://avatars.githubusercontent.com/u/31537466?v=4?s=100" width="100px;" alt="theoohoho"/><br /><sub><b>theoohoho</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=theoohoho" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://yogeshupadhyay.netlify.app/"><img src="https://avatars.githubusercontent.com/u/53992168?v=4?s=100" width="100px;" alt="Yogesh Upadhyay"/><br /><sub><b>Yogesh Upadhyay</b></sub></a><br /><a href="https://github.com/yezz123/authx/issues?q=author%3AYogeshUpdhyay" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/iftenet"><img src="https://avatars.githubusercontent.com/u/1397880?v=4?s=100" width="100px;" alt="Roman"/><br /><sub><b>Roman</b></sub></a><br /><a href="https://github.com/yezz123/authx/issues?q=author%3Aiftenet" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/today/author/alobbs"><img src="https://avatars.githubusercontent.com/u/170559?v=4?s=100" width="100px;" alt="Alvaro Lopez Ortega"/><br /><sub><b>Alvaro Lopez Ortega</b></sub></a><br /><a href="https://github.com/yezz123/authx/commits?author=alobbs" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pinchXOXO"><img src="https://avatars.githubusercontent.com/u/68501799?v=4?s=100" width="100px;" alt="Devy Santo"/><br /><sub><b>Devy Santo</b></sub></a><br /><a href="#infra-pinchXOXO" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
@@ -198,20 +189,10 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the
 [all-contributors](https://github.com/all-contributors/all-contributors)
 specification. Contributions of any kind welcome!
 
-## Links 🔗
-
-- [Homepage](https://authx.yezz.me/)
-- [FAQ](https://authx.yezz.me/faq/)
-- [Release - AuthX](https://authx.yezz.me/release/)
-- [MIT License](https://authx.yezz.me/license/)
-- [Code of Conduct](https://authx.yezz.me/code_of_conduct/)
-- [Contributing](https://authx.yezz.me/contributing/)
-- [Help - Sponsors](https://authx.yezz.me/help/)
-
-## License 📄
+## License
 
 This project is licensed under the terms of the MIT License.
```

#### html2text {}

```diff
@@ -1,93 +1,80 @@
-Metadata-Version: 2.1 Name: authx Version: 1.0.1b1 Summary: Ready to use and
+Metadata-Version: 2.3 Name: authx Version: 1.1.0 Summary: Ready to use and
 customizable Authentications and Oauth2 management for FastAPI Project-URL:
 Homepage, https://github.com/yezz123/authx Project-URL: Documentation, https://
 authx.yezz.me/ Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri
 yezz.me> License-Expression: MIT License-File: LICENSE Keywords:
 Authentication,Cookie,FastAPI,JWT,Oauth2,Pydantic Classifier: Development
 Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier: Framework ::
 FastAPI Classifier: Framework :: Pydantic Classifier: Framework :: Pydantic ::
-1 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+2 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist:
-fastapi<0.110.0,>=0.65.2 Requires-Dist: pydantic-settings>=2.1.0 Requires-Dist:
-pydantic<2.6.1,>=2.0.0 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0 Requires-
-Dist: python-dateutil<3.0.0,>=2.8 Requires-Dist: python-jose<4.0.0,>=3.3.0
-Requires-Dist: pytz<2025.0,>=2023.3 Description-Content-Type: text/markdown #
-AuthenticationX ð«
+fastapi<0.111.0,>=0.100.0 Requires-Dist: pydantic-settings>=2.1.0 Requires-
+Dist: pydantic<2.6.3,>=2.0.0 Requires-Dist: pyjwt[crypto]<3.0.0,>=2.6.0
+Requires-Dist: python-dateutil<3.0.0,>=2.8 Requires-Dist: python-
+jose<4.0.0,>=3.3.0 Requires-Dist: pytz<2025.0,>=2023.3 Description-Content-
+Type: text/markdown # Authx
                                     _[_A_u_t_h_X_]
 RReeaaddyy--ttoo--uussee aanndd ccuussttoommiizzaabbllee AAuutthheennttiiccaattiioonnss aanndd OOaauutthh22 mmaannaaggeemmeenntt ffoorr FFaassttAAPPII
                                       ?â??¡
 _[_l_i_n_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_y_e_z_z_1_2_3_/_a_u_t_h_x_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
                      _b_a_d_g_e_._s_v_g_]_[_T_e_s_t_]_[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _2_]
 --- **Source Code**:
 github.com/yezz123/authx> **Documentation**:
 authx.yezz.me/> --- Add a Fully registration and authentication or
 authorization system to your [FastAPI](https://fastapi.tiangolo.com/) project.
-**AuthX** is designed to be as customizable and adaptable as possible. >
-**Notes**: > > [Authx V0.9.x](https://authx-v0.yezz.me/) This branch relates to
-development of authx V1 which is not yet ready for production use. > >If you're
-a Authx user, you probably want either Authx V0.9 [Documentation](https://
-authx-v0.yezz.me/) or, [0.X.X-fix](https://github.com/yezz123/authx/tree/0.X.X-
-fix) git branch. ## Features ð§ - [x] Support Python 3.8+ & Pydantic 2.0+. -
-[x] Multiple customizable authentication backend: - [x] JWT authentication
-backend included - [x] JWT encoding/decoding for application authentication -
-[x] Automatic detection of JWTs in requests: - [x] JWTs in headers - [x] JWTs
-in cookies - [x] JWTs in query parameters - [x] JWTs in request bodies - [x]
-Cookie authentication backend included - [x] middleware for authentication and
-authorization through JWT. - [x] Extensible Error Handling System. ### Extra
-Features ð AuthX is designed to be as customizable and adaptable as
-possible. So you need to install [`authx-extra`](https://github.com/yezz123/
-authx-extra) to get extra features. - [x] Using Redis as a session store &
-cache. - [x] Support HTTPCache. - [x] Support Sessions and Pre-built CRUD
-functions and Instance to launch Redis. - [x] Support Middleware of
-[pyinstrument](https://pyinstrument.readthedocs.io/) to check your service
-performance. - [x] Support Middleware for collecting and exposing [Prometheus]
-(https://prometheus.io/) metrics. **Note:** Check [Release Notes](https://
-authx.yezz.me/release/). ## Project using ð Here is a simple way to
-kickstart your project with AuthX: ```python from fastapi import FastAPI,
-Depends, HTTPException from authx import AuthX, AuthXConfig, RequestToken app =
-FastAPI() config = AuthXConfig( JWT_ALGORITHM = "HS256", JWT_SECRET_KEY =
-"SECRET_KEY", JWT_TOKEN_LOCATION = ["headers"], ) auth = AuthX(config=config)
-auth.handle_errors(app) @app.get('/login') def login(username: str, password:
-str): if username == "xyz" and password == "xyz": token =
-auth.create_access_token(uid=username) return {"access_token": token} raise
-HTTPException(401, detail={"message": "Invalid credentials"}) @app.get("/
-protected", dependencies=[Depends(auth.get_token_from_request)]) def
-get_protected(token: RequestToken = Depends()): try: auth.verify_token
-(token=token) return {"message": "Hello world !"} except Exception as e: raise
-HTTPException(401, detail={"message": str(e)}) from e ``` ## Contributors and
-sponsors ð [![All Contributors](https://img.shields.io/badge/
-all_contributors-11-orange.svg?style=flat-square)](#contributors-) Thanks goes
-to these wonderful people ([emoji key](https://allcontributors.org/docs/en/
-emoji-key)):
-  _[_Y_a_s_s_e_r   _[_A_b_d_e_r_r_a_h_i_m  _[_I_s_m_a_i_l  _[_t_a_l_e_n_t_u_n_o  _[_C_a_c_t_u_s   _[_M_o_j_i_x_C_o_d_e_r_] _[_S_t_Ã_©_p_h_a_n_e
-  _T_a_h_i_r_i_]     _S_O_U_B_A_I_-   _G_h_a_l_l_o_u_ _]    _L_L_C_]       _L_L_C_]     _MM_oo_jj_ii_xx_CC_oo_dd_ee_rr  _R_a_i_m_b_a_u_l_t_]
-  _YY_aa_ss_ss_ee_rr     _E_L_I_D_R_I_S_I_]   _II_ss_mm_aa_ii_ll   _tt_aa_ll_ee_nn_tt_uu_nn_oo  _CC_aa_cc_tt_uu_ss_ _LL_LL_CC  _ð___» _ð___   _SS_tt_?Ã_?©_pp_hh_aa_nn_ee
-  _TT_aa_hh_ii_rr_ii    _AA_bb_dd_ee_rr_rr_aa_hh_ii_mm  _GG_hh_aa_ll_ll_oo_uu_      _LL_LL_CC        _ð___µ                 _RR_aa_ii_mm_bb_aa_uu_ll_tt
- _ð___» _ð___    _SS_OO_UU_BB_AA_II_--     _ð___»       _ð___µ                            _ð___» _ð___
- _ð___§ _ð___   _EE_LL_II_DD_RR_II_SS_II    _ð___¡_ï_¸_
-             _ð___ _ð___
-_[_t_h_e_o_o_h_o_h_o_]   _[_Y_o_g_e_s_h    _[_R_o_m_a_n_]    _[_A_l_v_a_r_o
- _tt_hh_ee_oo_oo_hh_oo_hh_oo   _U_p_a_d_h_y_a_y_]    _RR_oo_mm_aa_nn      _L_o_p_e_z
-   _ð___       _YY_oo_gg_ee_ss_hh      _ð___      _O_r_t_e_g_a_]
-             _UU_pp_aa_dd_hh_yy_aa_yy                _AA_ll_vv_aa_rr_oo
-               _ð___                  _LL_oo_pp_ee_zz
-                                     _OO_rr_tt_ee_gg_aa
-                                      _ð___
+**AuthX** is designed to be as customizable and adaptable as possible. ##
+Features - [x] Support Python 3.8+ & Pydantic 2.0+. - [x] Multiple customizable
+authentication backend: - [x] JWT authentication backend included - [x] JWT
+encoding/decoding for application authentication - [x] Automatic detection of
+JWTs in requests: - [x] JWTs in headers - [x] JWTs in cookies - [x] JWTs in
+query parameters - [x] JWTs in request bodies - [x] Cookie authentication
+backend included - [x] Middleware for authentication and authorization through
+JWT. - [x] Extensible Error Handling System. ### Extra Features AuthX is
+designed to be as customizable and adaptable as possible. So you need to
+install [`authx-extra`](https://github.com/yezz123/authx-extra) to get extra
+features. - [x] Using Redis as a session store & cache. - [x] Support
+HTTPCache. - [x] Support Sessions and Pre-built CRUD functions and Instance to
+launch Redis. - [x] Support Middleware of [pyinstrument](https://
+pyinstrument.readthedocs.io/) to check your service performance. - [x] Support
+Middleware for collecting and exposing [Prometheus](https://prometheus.io/
+) metrics. **Note:** Check [Release Notes](https://authx.yezz.me/release/). ##
+Project using Here is a simple way to kickstart your project with AuthX:
+```python from fastapi import FastAPI, Depends, HTTPException from authx import
+AuthX, AuthXConfig, RequestToken app = FastAPI() config = AuthXConfig
+( JWT_ALGORITHM = "HS256", JWT_SECRET_KEY = "SECRET_KEY", JWT_TOKEN_LOCATION =
+["headers"], ) auth = AuthX(config=config) auth.handle_errors(app) @app.get('/
+login') def login(username: str, password: str): if username == "xyz" and
+password == "xyz": token = auth.create_access_token(uid=username) return
+{"access_token": token} raise HTTPException(401, detail={"message": "Invalid
+credentials"}) @app.get("/protected", dependencies=[Depends
+(auth.get_token_from_request)]) def get_protected(token: RequestToken = Depends
+()): try: auth.verify_token(token=token) return {"message": "Hello world !"}
+except Exception as e: raise HTTPException(401, detail={"message": str(e)})
+from e ``` ## Contributors and sponsors [![All Contributors](https://
+img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square)]
+(#contributors-) Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
+_[_Y_a_s_s_e_r_ _T_a_h_i_r_i_]    _[_A_b_d_e_r_r_a_h_i_m     _[_I_s_m_a_i_l_ _G_h_a_l_l_o_u_ _] _[_M_o_j_i_x_C_o_d_e_r_]   _[_S_t_Ã_©_p_h_a_n_e
+ _YY_aa_ss_ss_ee_rr_ _TT_aa_hh_ii_rr_ii   _S_O_U_B_A_I_-_E_L_I_D_R_I_S_I_]   _II_ss_mm_aa_ii_ll_ _GG_hh_aa_ll_ll_oo_uu_    _MM_oo_jj_ii_xx_CC_oo_dd_ee_rr    _R_a_i_m_b_a_u_l_t_]
+_ð___» _ð___ _ð___§  _AA_bb_dd_ee_rr_rr_aa_hh_ii_mm_ _SS_OO_UU_BB_AA_II_--   _ð___» _ð___¡_ï_¸_      _ð___» _ð___    _SS_tt_?Ã_?©_pp_hh_aa_nn_ee
+     _ð___            _EE_LL_II_DD_RR_II_SS_II                                       _RR_aa_ii_mm_bb_aa_uu_ll_tt
+                    _ð___ _ð___                                       _ð___» _ð___
+   _[_t_h_e_o_o_h_o_h_o_]  _[_Y_o_g_e_s_h_ _U_p_a_d_h_y_a_y_]         _[_R_o_m_a_n_]    _[_A_l_v_a_r_o_ _L_o_p_e_z _[_D_e_v_y_ _S_a_n_t_o_]
+    _tt_hh_ee_oo_oo_hh_oo_hh_oo    _YY_oo_gg_ee_ss_hh_ _UU_pp_aa_dd_hh_yy_aa_yy           _RR_oo_mm_aa_nn        _O_r_t_e_g_a_]     _DD_ee_vv_yy_ _SS_aa_nn_tt_oo
+      _ð___             _ð___                _ð___      _AA_ll_vv_aa_rr_oo_ _LL_oo_pp_ee_zz      _ð___
+                                                        _OO_rr_tt_ee_gg_aa
+                                                         _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
-welcome! ## Links ð - [Homepage](https://authx.yezz.me/) - [FAQ](https://
-authx.yezz.me/faq/) - [Release - AuthX](https://authx.yezz.me/release/) - [MIT
-License](https://authx.yezz.me/license/) - [Code of Conduct](https://
-authx.yezz.me/code_of_conduct/) - [Contributing](https://authx.yezz.me/
-contributing/) - [Help - Sponsors](https://authx.yezz.me/help/) ## License ð
-This project is licensed under the terms of the MIT License.
+welcome! ## License This project is licensed under the terms of the MIT
+License.
```

