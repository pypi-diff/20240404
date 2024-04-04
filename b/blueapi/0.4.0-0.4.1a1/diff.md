# Comparing `tmp/blueapi-0.4.0.tar.gz` & `tmp/blueapi-0.4.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.4.0.tar", last modified: Tue Feb 27 10:14:53 2024, max compression
+gzip compressed data, was "blueapi-0.4.1a1.tar", last modified: Wed Apr  3 14:42:31 2024, max compression
```

## Comparing `blueapi-0.4.0.tar` & `blueapi-0.4.1a1.tar`

### file list

```diff
@@ -1,218 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.068474 blueapi-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.040475 blueapi-0.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-27 10:14:46.000000 blueapi-0.4.0/.devcontainer/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-02-27 10:14:46.000000 blueapi-0.4.0/.devcontainer/container-startup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-27 10:14:46.000000 blueapi-0.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.040475 blueapi-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.036475 blueapi-0.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.040475 blueapi-0.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3023 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/asyncapi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/backstage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-27 10:14:46.000000 blueapi-0.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-27 10:14:46.000000 blueapi-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-27 10:14:46.000000 blueapi-0.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-27 10:14:46.000000 blueapi-0.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-27 10:14:46.000000 blueapi-0.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-27 10:14:46.000000 blueapi-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-27 10:14:46.000000 blueapi-0.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-27 10:14:46.000000 blueapi-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-02-27 10:14:53.068474 blueapi-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-27 10:14:46.000000 blueapi-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-27 10:14:46.000000 blueapi-0.4.0/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-27 10:14:46.000000 blueapi-0.4.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/config/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-27 10:14:46.000000 blueapi-0.4.0/config/adsim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-27 10:14:46.000000 blueapi-0.4.0/config/bl38p.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-27 10:14:46.000000 blueapi-0.4.0/config/bl45p.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-27 10:14:46.000000 blueapi-0.4.0/config/defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.044475 blueapi-0.4.0/docs/developer/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/decisions/0002-no-queues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/decisions/0003-api-case.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/explanations/type_validators.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/developer/tutorials/dev-run.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/images/blueapi-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   377607 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/images/blueapi.png
--rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/images/bluesky-events.png
--rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/images/debug-vscode.png
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.048475 blueapi-0.4.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/how-to/add-plans-and-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/how-to/configure-app.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/how-to/run-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/asyncapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/messaging-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/reference/rest-spec.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-27 10:14:46.000000 blueapi-0.4.0/docs/user/tutorials/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.036475 blueapi-0.4.0/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-02-27 10:14:46.000000 blueapi-0.4.0/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-02-27 10:14:46.000000 blueapi-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 10:14:53.068474 blueapi-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.040475 blueapi-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.052475 blueapi-0.4.0/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.056475 blueapi-0.4.0/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.056475 blueapi-0.4.0/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/bluesky_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.056475 blueapi-0.4.0/src/blueapi/data_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/data_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/data_management/visit_directory_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.056475 blueapi-0.4.0/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.056475 blueapi-0.4.0/src/blueapi/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/preprocessors/attach_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.060474 blueapi-0.4.0/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/handler_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/service/subprocess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.060474 blueapi-0.4.0/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/startup/example_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/startup/example_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.060474 blueapi-0.4.0/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/invalid_config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/ophyd_async_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.060474 blueapi-0.4.0/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-27 10:14:46.000000 blueapi-0.4.0/src/blueapi/worker/worker_busy_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-02-27 10:14:53.000000 blueapi-0.4.0/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 10:14:52.000000 blueapi-0.4.0/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.060474 blueapi-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/core/fake_device_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/core/fake_plan_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/data_management/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/data_management/test_visit_directory_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/example_yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/example_yaml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/example_yaml/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/example_yaml/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/example_yaml/rest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/example_yaml/valid_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/preprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/preprocessors/test_attach_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/service/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/service/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/service/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/service/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/service/test_subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/utils/test_thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:14:53.064474 blueapi-0.4.0/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/worker/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-02-27 10:14:46.000000 blueapi-0.4.0/tests/worker/test_reworker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.294497 blueapi-0.4.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.266497 blueapi-0.4.1a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.266497 blueapi-0.4.1a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.262497 blueapi-0.4.1a1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.266497 blueapi-0.4.1a1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.266497 blueapi-0.4.1a1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.270497 blueapi-0.4.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/asyncapi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/backstage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.270497 blueapi-0.4.1a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-03 14:42:31.294497 blueapi-0.4.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.270497 blueapi-0.4.1a1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/config/adsim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/config/bl38p.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/config/bl45p.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/config/defaults.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/container-startup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.270497 blueapi-0.4.1a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.270497 blueapi-0.4.1a1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.274497 blueapi-0.4.1a1/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions/0002-no-queues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions/0003-api-case.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions/0004-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations/type_validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.274497 blueapi-0.4.1a1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/add-plans-and-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/configure-app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/run-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to/write-plans.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.274497 blueapi-0.4.1a1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/images/blueapi-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   377607 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/images/blueapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/images/bluesky-events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/images/debug-vscode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/asyncapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/messaging-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference/rest-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/tutorials/dev-run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/tutorials/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.262497 blueapi-0.4.1a1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:42:31.294497 blueapi-0.4.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.262497 blueapi-0.4.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.278497 blueapi-0.4.1a1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/bluesky_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/data_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/data_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/data_management/visit_directory_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/preprocessors/attach_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.282497 blueapi-0.4.1a1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/service/subprocess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/startup/example_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/startup/example_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/invalid_config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/ophyd_async_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/utils/thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/src/blueapi/worker/worker_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 14:42:31.000000 blueapi-0.4.1a1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/core/fake_device_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/core/fake_plan_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.286497 blueapi-0.4.1a1/tests/data_management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/data_management/test_visit_directory_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/example_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/example_yaml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/example_yaml/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/example_yaml/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/example_yaml/rest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/example_yaml/valid_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/preprocessors/test_attach_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/service/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/service/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/service/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/service/test_subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/test_ophyd_async_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/utils/test_thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:42:31.290497 blueapi-0.4.1a1/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/worker/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13000 2024-04-03 14:42:27.000000 blueapi-0.4.1a1/tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.0/.devcontainer/Dockerfile` & `blueapi-0.4.1a1/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-# This file is for use as a devcontainer and a runtime container
-#
-# The devcontainer should use the build target and run as root with podman
+# The devcontainer should use the developer target and run as root with podman
 # or docker with user namespaces.
-#
-FROM python:3.11 as build
+ARG PYTHON_VERSION=3.11
+FROM python:${PYTHON_VERSION} as developer
 
-ARG PIP_OPTIONS=.
+# Add any system dependencies for the developer/build environment here
+RUN apt-get update && apt-get install -y --no-install-recommends \
+    graphviz \
+    && rm -rf /var/lib/apt/lists/*
 
-# Add any system dependencies for the developer/build environment here e.g.
-# RUN apt-get update && apt-get upgrade -y && \
-#     apt-get install -y --no-install-recommends \
-#     desired-packages \
-#     && rm -rf /var/lib/apt/lists/*
-
-# set up a virtual environment and put it in PATH
+# Set up a virtual environment and put it in PATH
 RUN python -m venv /venv
 ENV PATH=/venv/bin:$PATH
 
-# Copy any required context for the pip install over
+# The build stage installs the context into the venv
+FROM developer as build
 COPY . /context
 WORKDIR /context
+RUN pip install .
 
-# install python package into /venv
-RUN pip install ${PIP_OPTIONS}
-
-FROM python:3.11 as runtime
-
+# The runtime stage copies the built venv into a slim runtime container
+FROM python:${PYTHON_VERSION}-slim as runtime
 # Add apt-get system dependecies for runtime here if needed
-
-# copy the virtual environment from the build stage and put it in PATH
 COPY --from=build /venv/ /venv/
 COPY ./container-startup.sh /container-startup.sh
 ENV PATH=/venv/bin:$PATH
 
 
 RUN mkdir -p /.cache/pip; chmod -R 777 /venv /.cache/pip
```

### Comparing `blueapi-0.4.0/.devcontainer/devcontainer.json` & `blueapi-0.4.1a1/.devcontainer/devcontainer.json`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
-        "dockerfile": "Dockerfile",
-        "target": "build",
-        // Only upgrade pip, we will install the project below
-        "args": {
-            "PIP_OPTIONS": "--upgrade pip"
-        }
+        "dockerfile": "../Dockerfile",
+        "target": "developer"
     },
     "remoteEnv": {
+        // Allow X11 apps to run inside the container
         "DISPLAY": "${localEnv:DISPLAY}"
     },
-    // Add the URLs of features you want added when the container is built.
-    "features": {
-        "ghcr.io/devcontainers/features/common-utils:1": {
-            "username": "none",
-            "upgradePackages": false
-        }
-    },
-    // Set *default* container specific settings.json values on container create.
-    "settings": {
-        "python.defaultInterpreterPath": "/venv/bin/python"
-    },
     "customizations": {
         "vscode": {
+            // Set *default* container specific settings.json values on container create.
+            "settings": {
+                "python.defaultInterpreterPath": "/venv/bin/python"
+            },
             // Add the IDs of extensions you want installed when the container is created.
             "extensions": [
                 "ms-python.python",
+                "github.vscode-github-actions",
                 "tamasfe.even-better-toml",
                 "redhat.vscode-yaml",
-                "ryanluker.vscode-coverage-gutters"
+                "ryanluker.vscode-coverage-gutters",
+                "charliermarsh.ruff",
+                "ms-azuretools.vscode-docker"
             ]
         }
     },
-    // Make sure the files we are mapping into the container exist on the host
-    "initializeCommand": "bash -c 'for i in $HOME/.inputrc; do [ -f $i ] || touch $i; done'",
+    "features": {
+        // Some default things like git config
+        "ghcr.io/devcontainers/features/common-utils:2": {
+            "upgradePackages": false
+        }
+    },
     "runArgs": [
+        // Allow the container to access the host X11 display and EPICS CA
         "--net=host",
-        "--security-opt=label=type:container_runtime_t"
-    ],
-    "mounts": [
-        "source=${localEnv:HOME}/.ssh,target=/root/.ssh,type=bind",
-        "source=${localEnv:HOME}/.inputrc,target=/root/.inputrc,type=bind",
-        // map in home directory - not strictly necessary but useful
-        "source=${localEnv:HOME},target=${localEnv:HOME},type=bind,consistency=cached"
+        // Make sure SELinux does not disable with access to host filesystems like tmp
+        "--security-opt=label=disable"
     ],
-    // make the workspace folder the same inside and outside of the container
-    "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
-    "workspaceFolder": "${localWorkspaceFolder}",
+    // Mount the parent as /workspaces so we can pip install peers as editable
+    "workspaceMount": "source=${localWorkspaceFolder}/..,target=/workspaces,type=bind",
     // After the container is created, install the python project in editable form
-    "postCreateCommand": "pip install -e .[dev]"
+    "postCreateCommand": "pip install $([ -f dev-requirements.txt ] && echo '-c dev-requirements.txt') -e '.[dev]' && pre-commit install"
 }
```

### Comparing `blueapi-0.4.0/.github/CONTRIBUTING.rst` & `blueapi-0.4.1a1/.github/CONTRIBUTING.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-Contributing to the project
-===========================
+# Contribute to the project
 
 Contributions and issues are most welcome! All issues and pull requests are
-handled through GitHub_. Also, please check for any existing issues before
+handled through [GitHub](https://github.com/DiamondLightSource/blueapi/issues). Also, please check for any existing issues before
 filing a new one. If you have a great idea but it involves big changes, please
 file a ticket before making a pull request! We want to make sure you don't spend
 your time coding something that might not fit the scope of the project.
 
-.. _GitHub: https://github.com/DiamondLightSource/blueapi/issues
+## Issue or Discussion?
 
-Issue or Discussion?
---------------------
-
-Github also offers discussions_ as a place to ask questions and share ideas. If
+Github also offers [discussions](https://github.com/DiamondLightSource/blueapi/discussions) as a place to ask questions and share ideas. If
 your issue is open ended and it is not obvious when it can be "closed", please
 raise it as a discussion instead.
 
-.. _discussions: https://github.com/DiamondLightSource/blueapi/discussions
-
-Code coverage
--------------
+## Code Coverage
 
 While 100% code coverage does not make a library bug-free, it significantly
 reduces the number of easily caught bugs! Please make sure coverage remains the
 same or is improved by a pull request!
 
-Developer guide
----------------
+## Developer Information
+
+It is recommended that developers use a [vscode devcontainer](https://code.visualstudio.com/docs/devcontainers/containers). This repository contains configuration to set up a containerized development environment that suits its own needs.
 
-The `Developer Guide`_ contains information on setting up a development
-environment, running the tests and what standards the code and documentation
-should follow.
+This project was created using the [Diamond Light Source Copier Template](https://github.com/DiamondLightSource/python-copier-template) for Python projects.
 
-.. _Developer Guide: https://diamondlightsource.github.io/blueapi/main/developer/how-to/contribute.html
+For more information on common tasks like setting up a developer environment, running the tests, and setting a pre-commit hook, see the template's [How-to guides](https://diamondlightsource.github.io/python-copier-template/2.0.1/how-to.html).
```

### Comparing `blueapi-0.4.0/.github/pages/make_switcher.py` & `blueapi-0.4.1a1/.github/pages/make_switcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
-from typing import List, Optional
+from typing import Optional
 
 
-def report_output(stdout: bytes, label: str) -> List[str]:
+def report_output(stdout: bytes, label: str) -> list[str]:
     ret = stdout.decode().strip().split("\n")
     print(f"{label}: {ret}")
     return ret
 
 
-def get_branch_contents(ref: str) -> List[str]:
+def get_branch_contents(ref: str) -> list[str]:
     """Get the list of directories in a branch."""
     stdout = check_output(["git", "ls-tree", "-d", "--name-only", ref])
     return report_output(stdout, "Branch contents")
 
 
-def get_sorted_tags_list() -> List[str]:
+def get_sorted_tags_list() -> list[str]:
     """Get a list of sorted tags in descending order from the repository."""
     stdout = check_output(["git", "tag", "-l", "--sort=-v:refname"])
     return report_output(stdout, "Tags list")
 
 
-def get_versions(ref: str, add: Optional[str], remove: Optional[str]) -> List[str]:
+def get_versions(ref: str, add: Optional[str]) -> list[str]:
     """Generate the file containing the list of all GitHub Pages builds."""
     # Get the directories (i.e. builds) from the GitHub Pages branch
     try:
         builds = set(get_branch_contents(ref))
     except CalledProcessError:
         builds = set()
         logging.warning(f"Cannot get {ref} contents")
 
     # Add and remove from the list of builds
     if add:
         builds.add(add)
-    if remove:
-        assert remove in builds, f"Build '{remove}' not in {sorted(builds)}"
-        builds.remove(remove)
 
     # Get a sorted list of tags
     tags = get_sorted_tags_list()
 
     # Make the sorted versions list from main branches and tags
-    versions: List[str] = []
+    versions: list[str] = []
     for version in ["master", "main"] + tags:
         if version in builds:
             versions.append(version)
             builds.remove(version)
 
     # Add in anything that is left to the bottom
     versions += sorted(builds)
     print(f"Sorted versions: {versions}")
     return versions
 
 
 def write_json(path: Path, repository: str, versions: str):
     org, repo_name = repository.split("/")
     struct = [
-        dict(version=version, url=f"https://{org}.github.io/{repo_name}/{version}/")
+        {"version": version, "url": f"https://{org}.github.io/{repo_name}/{version}/"}
         for version in versions
     ]
     text = json.dumps(struct, indent=2)
     print(f"JSON switcher:\n{text}")
-    path.write_text(text)
+    path.write_text(text, encoding="utf-8")
 
 
 def main(args=None):
     parser = ArgumentParser(
-        description="Make a versions.txt file from gh-pages directories"
+        description="Make a versions.json file from gh-pages directories"
     )
     parser.add_argument(
         "--add",
         help="Add this directory to the list of existing directories",
     )
     parser.add_argument(
-        "--remove",
-        help="Remove this directory from the list of existing directories",
-    )
-    parser.add_argument(
         "repository",
         help="The GitHub org and repository name: ORG/REPO",
     )
     parser.add_argument(
         "output",
         type=Path,
         help="Path of write switcher.json to",
     )
     args = parser.parse_args(args)
 
     # Write the versions file
-    versions = get_versions("origin/gh-pages", args.add, args.remove)
+    versions = get_versions("origin/gh-pages", args.add)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `blueapi-0.4.0/.github/workflows/helm.yml` & `blueapi-0.4.1a1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/.gitignore` & `blueapi-0.4.1a1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
-.venv
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
@@ -63,7 +62,9 @@
 # likely venv names
 .venv*
 venv*
 
 # further build artifacts
 lockfiles/
 
+# ruff cache
+.ruff_cache/
```

### Comparing `blueapi-0.4.0/.vscode/launch.json` & `blueapi-0.4.1a1/.vscode/launch.json`

 * *Files 15% similar despite different names*

```diff
@@ -14,27 +14,25 @@
                 "--reload"
             ],
             "jinja": true,
             "justMyCode": true
         },
         {
             "name": "Debug Unit Test",
-            "type": "python",
+            "type": "debugpy",
             "request": "launch",
             "justMyCode": false,
             "program": "${file}",
             "purpose": [
                 "debug-test"
             ],
             "console": "integratedTerminal",
             "env": {
-                // The default config in setup.cfg's "[tool:pytest]" adds coverage.
-                // Cannot have coverage and debugging at the same time.
-                // https://github.com/microsoft/vscode-python/issues/693
-                "PYTEST_ADDOPTS": "--no-cov"
+                // Enable break on exception when debugging tests (see: tests/conftest.py)
+                "PYTEST_RAISE": "1",
             },
         },
         {
             "name": "Run Service",
             "type": "python",
             "request": "launch",
             "justMyCode": false,
```

### Comparing `blueapi-0.4.0/LICENSE` & `blueapi-0.4.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/PKG-INFO` & `blueapi-0.4.1a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.0
-Summary: Lightweight Bluesky-as-a-service wrapper application. Also usable as a library.
+Version: 0.4.1a1
+Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,15 +208,15 @@
 Project-URL: GitHub, https://github.com/DiamondLightSource/blueapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bluesky
 Requires-Dist: ophyd
 Requires-Dist: nslsii
 Requires-Dist: pyepics
 Requires-Dist: aioca
 Requires-Dist: pydantic<2.0
@@ -225,96 +225,72 @@
 Requires-Dist: PyYAML
 Requires-Dist: click<8.1.4
 Requires-Dist: fastapi[all]<0.99
 Requires-Dist: uvicorn
 Requires-Dist: requests
 Requires-Dist: dls-bluesky-core
 Requires-Dist: dls-dodal
-Requires-Dist: typing_extensions<4.6
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: flake8-isort; extra == "dev"
-Requires-Dist: Flake8-pyproject; extra == "dev"
+Requires-Dist: copier; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinxcontrib-openapi; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 
-blueapi
-===========================
-
-|code_ci| |docs_ci| |coverage| |pypi_version| |license|
-
-Lightweight bluesky-as-a-service wrapper application. Also usable as a library. 
+[![CI](https://github.com/DiamondLightSource/blueapi/actions/workflows/ci.yml/badge.svg)](https://github.com/DiamondLightSource/blueapi/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/DiamondLightSource/blueapi/branch/main/graph/badge.svg)](https://codecov.io/gh/DiamondLightSource/blueapi)
+[![PyPI](https://img.shields.io/pypi/v/blueapi.svg)](https://pypi.org/project/blueapi)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# blueapi
+
+Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
+
+Source          | <https://github.com/DiamondLightSource/blueapi>
+:---:           | :---:
+PyPI            | `pip install blueapi`
+Docker          | `docker run ghcr.io/diamondlightsource/blueapi:latest`
+Documentation   | <https://diamondlightsource.github.io/blueapi>
+Releases        | <https://github.com/DiamondLightSource/blueapi/releases>
+
+This module wraps [bluesky](https://blueskyproject.io/bluesky) plans and devices
+inside a server and exposes endpoints to send commands/receive data. Useful for
+installation at labs where multiple people may control equipment, possibly from
+remote locations.
 
-============== ==============================================================
-PyPI           ``pip install blueapi``
-Source code    https://github.com/DiamondLightSource/blueapi
-Documentation  https://DiamondLightSource.github.io/blueapi
-Releases       https://github.com/DiamondLightSource/blueapi/releases
-============== ==============================================================
-
-This module wraps bluesky_ plans and devices inside a server and exposes endpoints to send commands/receive data.
-Useful for installation at labs where multiple people may control equipment, 
-possibly from remote locations.
-
-|concept|
+![concept][]
 
 The main premise of blueapi is to minimize the boilerplate required to get plans
-and devices up and running by generating an API for your lab out of type-annotated 
-plans. For example, take the following plan:
-
-.. code:: python
+and devices up and running by generating an API for your lab out of
+type-annotated plans. For example, take the following plan:
 
+```python
     import bluesky.plans as bp
     from blueapi.core import MsgGenerator
 
     def my_plan(foo: str, bar: int) -> MsgGenerator:
         yield from bp.scan(...)
+```
 
-Blueapi's job is to detect this plan and automatically add it to the lab's API so it
-can be invoked easily with a few REST calls. 
-
-.. _bluesky: https://blueskyproject.io/bluesky
-
-.. |code_ci| image:: https://github.com/DiamondLightSource/blueapi/actions/workflows/code.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/blueapi/actions/workflows/code.yml
-    :alt: Code CI
-
-.. |docs_ci| image:: https://github.com/DiamondLightSource/blueapi/actions/workflows/docs.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/blueapi/actions/workflows/docs.yml
-    :alt: Docs CI
-
-.. |coverage| image:: https://codecov.io/gh/DiamondLightSource/blueapi/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/DiamondLightSource/blueapi
-    :alt: Test Coverage
-
-.. |pypi_version| image:: https://img.shields.io/pypi/v/blueapi.svg
-    :target: https://pypi.org/project/blueapi
-    :alt: Latest PyPI version
-
-.. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: Apache License
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Blueapi's job is to detect this plan and automatically add it to the lab's API
+so it can be invoked easily with a few REST calls. 
 
+<!-- README only content. Anything below this line won't be included in index.md -->
 
-.. |concept| image:: docs/images/blueapi.png
-    :width: 800px
+See https://diamondlightsource.github.io/blueapi for more detailed documentation.
 
-See https://DiamondLightSource.github.io/blueapi for more detailed documentation.
+[concept]: https://raw.githubusercontent.com/DiamondLightSource/blueapi/main/docs/images/blueapi.png
```

### Comparing `blueapi-0.4.0/catalog-info.yaml` & `blueapi-0.4.1a1/catalog-info.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
   description: Lightweight wrapper service around Bluesky Run Engine
   annotations:
     github.com/project-slug: DiamondLightSource/blueapi
     diamond.ac.uk/viewdocs-url: https://diamondlightsource.github.io/blueapi
 spec:
   type: service
   lifecycle: production
-  owner: user:vid18871 # TODO: owner: DAQ-Core
-  #  system: Athena  # TODO: Define Athena system: presumably same location as DAQ-Core/DAQ?
+  owner: group:data-acquisition
+  system: athena
   providesApis:
     - blueapiControl
     - blueapiEvents
 ---
 apiVersion: backstage.io/v1alpha1
 kind: API
 metadata:
@@ -25,23 +25,23 @@
   annotations:
     github.com/project-slug: DiamondLightSource/blueapi
 spec:
   type: openapi
   lifecycle: production
   owner: user:vid18871
   definition:
-    $text: ./docs/user/reference/openapi.yaml
+    $text: ./docs/reference/openapi.yaml
 ---
 apiVersion: backstage.io/v1alpha1
 kind: API
 metadata:
   name: blueapiEvents
   title: Athena BlueAPI Events
   description: Event topics which can be listened to over a message bus
   annotations:
     github.com/project-slug: DiamondLightSource/blueapi
 spec:
   type: asyncapi
   lifecycle: production
   owner: user:vid18871
   definition:
-    $text: ./docs/user/reference/asyncapi.yaml
+    $text: ./docs/reference/asyncapi.yaml
```

### Comparing `blueapi-0.4.0/docs/conf.py` & `blueapi-0.4.1a1/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 import sys
 from pathlib import Path
 from subprocess import check_output
 
+import requests
+
 import blueapi
 
 # -- General configuration ------------------------------------------------
 
 # General information about the project.
 project = "blueapi"
 
@@ -38,20 +40,25 @@
     "sphinx.ext.viewcode",
     # Adds the inheritance-diagram generation directive
     "sphinx.ext.inheritance_diagram",
     # Add a copy button to each code block
     "sphinx_copybutton",
     # For the card element
     "sphinx_design",
+    # So we can write markdown files
+    "myst_parser",
     # OpenAPI directive
     "sphinxcontrib.openapi",
     # For documenting the CLI
     "sphinx_click.ext",
 ]
 
+# So we can use the ::: syntax
+myst_enable_extensions = ["colon_fence"]
+
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
 nitpicky = True
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
@@ -80,44 +87,31 @@
 # Output graphviz directive produced images in a scalable format
 graphviz_output_format = "svg"
 
 # The name of a reST role (builtin or Sphinx extension) to use as the default
 # role, that is, for text marked up `like this`
 default_role = "any"
 
-# The suffix of source filenames.
-source_suffix = ".rst"
-
 # The master toctree document.
 master_doc = "index"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # These patterns also affect html_static_path and html_extra_path
 exclude_patterns = ["_build"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # This means you can link things like `str` and `asyncio` to the relevant
 # docs in the python documentation.
-intersphinx_mapping = dict(python=("https://docs.python.org/3/", None))
+intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
 
 # A dictionary of graphviz graph attributes for inheritance diagrams.
-inheritance_graph_attrs = dict(rankdir="TB")
-
-# Common links that should be available on every page
-rst_epilog = """
-.. _Diamond Light Source: http://www.diamond.ac.uk
-.. _black: https://github.com/psf/black
-.. _flake8: https://flake8.pycqa.org/en/latest/
-.. _isort: https://github.com/PyCQA/isort
-.. _mypy: http://mypy-lang.org/
-.. _pre-commit: https://pre-commit.com/
-"""
+inheritance_graph_attrs = {"rankdir": "TB"}
 
 # Ignore localhost links for periodic check that links in docs are valid
 linkcheck_ignore = [r"http://localhost:\d+/"]
 
 # Set copy-button to ignore python and bash prompts
 # https://sphinx-copybutton.readthedocs.io/en/latest/use.html#using-regexp-prompt-identifiers
 copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
@@ -125,68 +119,68 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-github_repo = project
+github_repo = "blueapi"
 github_user = "DiamondLightSource"
 switcher_json = f"https://{github_user}.github.io/{github_repo}/switcher.json"
-# Don't check switcher if it doesn't exist, but warn in a non-failing way
-# TODO: Enable this again after all branches have published an updated switcher
-check_switcher = False
-if not check_switcher:
+switcher_exists = requests.get(switcher_json).ok
+if not switcher_exists:
     print(
         "*** Can't read version switcher, is GitHub pages enabled? \n"
         "    Once Docs CI job has successfully run once, set the "
         "Github pages source branch to be 'gh-pages' at:\n"
         f"    https://github.com/{github_user}/{github_repo}/settings/pages",
         file=sys.stderr,
     )
 
 # Theme options for pydata_sphinx_theme
-html_theme_options = dict(
-    logo=dict(
-        text=project,
-    ),
-    use_edit_page_button=True,
-    github_url=f"https://github.com/{github_user}/{github_repo}",
-    icon_links=[
-        dict(
-            name="PyPI",
-            url=f"https://pypi.org/project/{project}",
-            icon="fas fa-cube",
-        )
-    ],
-    switcher=dict(
-        json_url=switcher_json,
-        version_match=version,
-    ),
-    check_switcher=check_switcher,
-    navbar_end=["theme-switcher", "icon-links", "version-switcher"],
-    external_links=[
-        dict(
-            name="Release Notes",
-            url=f"https://github.com/{github_user}/{github_repo}/releases",
-        )
+# We don't check switcher because there are 3 possible states for a repo:
+# 1. New project, docs are not published so there is no switcher
+# 2. Existing project with latest skeleton, switcher exists and works
+# 3. Existing project with old skeleton that makes broken switcher,
+#    switcher exists but is broken
+# Point 3 makes checking switcher difficult, because the updated skeleton
+# will fix the switcher at the end of the docs workflow, but never gets a chance
+# to complete as the docs build warns and fails.
+html_theme_options = {
+    "logo": {
+        "text": project,
+    },
+    "use_edit_page_button": True,
+    "github_url": f"https://github.com/{github_user}/{github_repo}",
+    "icon_links": [
+        {
+            "name": "PyPI",
+            "url": f"https://pypi.org/project/{project}",
+            "icon": "fas fa-cube",
+        }
     ],
-    navigation_with_keys=True,
-)
+    "switcher": {
+        "json_url": switcher_json,
+        "version_match": version,
+    },
+    "check_switcher": False,
+    "navbar_end": ["theme-switcher", "icon-links", "version-switcher"],
+    "navigation_with_keys": False,
+}
 
 # A dictionary of values to pass into the template engine’s context for all pages
-html_context = dict(
-    github_user=github_user,
-    github_repo=project,
-    github_version=version,
-    doc_path="docs",
-)
+html_context = {
+    "github_user": github_user,
+    "github_repo": project,
+    "github_version": version,
+    "doc_path": "docs",
+}
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = False
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
 html_show_copyright = False
 
 # Logo
 html_logo = "images/blueapi-logo.svg"
-html_favicon = "images/blueapi-logo.svg"
+html_favicon = html_logo
```

### Comparing `blueapi-0.4.0/docs/developer/explanations/architecture.rst` & `blueapi-0.4.1a1/docs/explanations/architecture.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * Communicating with the outside world, accepting instructions to run plans, providing updates on plan progress etc.
 
 These responsibilities are kept separate in the codebase to ensure a clean, maintainable architecture.
 
 Key Components
 --------------
 
-.. figure:: ../../images/blueapi-architecture.png
+.. figure:: ../images/blueapi-architecture.png
     :width: 600px
     :align: center
 
     main components
 
 
 The ``BlueskyContext`` Object
```

### Comparing `blueapi-0.4.0/docs/developer/explanations/decisions/0002-no-queues.rst` & `blueapi-0.4.1a1/docs/explanations/decisions/0002-no-queues.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/developer/explanations/decisions/0003-api-case.rst` & `blueapi-0.4.1a1/docs/explanations/decisions/0003-api-case.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/developer/explanations/events.rst` & `blueapi-0.4.1a1/docs/explanations/events.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 sometimes assumes intuitive behaviour. The worker replaces the human and so must fill in the
 gaps.
 
 The base engine programatically emits data events conforming to the `bluesky event model`_. These
 are meant to be handled by other subscribing code (e.g. databroker) and are decoupled from concerns such as whether
 a plan has started, finished, paused, errored etc. See the example below:
 
-.. figure:: ../../images/bluesky-events.png
+.. figure:: ../images/bluesky-events.png
     :width: 600px
     :align: center
 
     sequence of event emission compared to plan start/finish, in a complicated case
 
 Note the gap between the start of the plan and the issue of the first `run start document`_, and the similar gap
 for the stop document vs end of the plan, thsse are typically used for setup and cleanup.
```

### Comparing `blueapi-0.4.0/docs/developer/explanations/lifecycle.rst` & `blueapi-0.4.1a1/docs/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/developer/explanations/type_validators.rst` & `blueapi-0.4.1a1/docs/explanations/type_validators.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/developer/tutorials/dev-run.rst` & `blueapi-0.4.1a1/docs/tutorials/dev-run.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Run/Debug in a Developer Environment 
 ====================================
 
 Assuming you have setup a developer environment, you can run a development version of the bluesky worker.
 
-.. seealso:: `./dev-install`
+.. seealso:: https://diamondlightsource.github.io/python-copier-template/main/how-to/dev-install.html
 
 
 Start Bluesky Worker
 --------------------
 
 Ensure you are inside your virtual environment:
 
 .. code:: shell
 
     source venv/bin/activate
 
 
-You will need to follow the instructions for setting up ActiveMQ as in `../../user/how-to/run-cli`. 
+You will need to follow the instructions for setting up ActiveMQ as in `../how-to/run-cli`. 
 
 The worker will be available from the command line (``blueapi serve``), but can be started from vscode with additional 
 debugging capabilities.
 
 1. Navigate to "Run and Debug" in the left hand menu.
 2. Select "Worker Service" from the debug configuration.
 3. Click the green "Run Button"
 
-.. figure:: ../../images/debug-vscode.png
+.. figure:: ../images/debug-vscode.png
     :align: center
 
     debug in vscode
```

### Comparing `blueapi-0.4.0/docs/images/blueapi-architecture.png` & `blueapi-0.4.1a1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/images/blueapi-logo.svg` & `blueapi-0.4.1a1/docs/images/blueapi-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/images/blueapi.png` & `blueapi-0.4.1a1/docs/images/blueapi.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/images/bluesky-events.png` & `blueapi-0.4.1a1/docs/images/bluesky-events.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/images/debug-vscode.png` & `blueapi-0.4.1a1/docs/images/debug-vscode.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/user/how-to/add-plans-and-devices.rst` & `blueapi-0.4.1a1/docs/how-to/add-plans-and-devices.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 The code can be in any pip-installable package, such as:
 
 * A package on pypi
 * A Github repository
 * A local directory with a ``pyproject.toml`` file or similar.
 
-The easiest place to put the code is a repository created with the `python skeleton`_. Which can then become any of the above.
+The easiest place to put the code is a repository created with the `python-copier-template`_. Which can then become any of the above.
 
-.. seealso:: Guide to setting up a new Python project with an environment and a standard set of tools: `New Skeleton Project Tutorial`_
+.. seealso:: Guide to setting up a new Python project with an environment and a standard set of tools: `Create a new repo from the template`_
 
 For development purposes this code should be installed into your environment with 
 
 .. code:: shell
 
   pip install -e path/to/package
 
@@ -110,9 +110,9 @@
   scratch:
     hostPath: path/to/scratch/area  # e.g. /dls_sw/<my_beamline>/software/blueapi/scratch
 
 You can then clone projects into the scratch directory and blueapi will automatically incorporate them on startup. You must still include configuration to load the plans and devices from specific modules within those packages, see above. 
 
 
 .. _dodal: https://github.com/DiamondLightSource/dodal
-.. _`python skeleton`: https://diamondlightsource.github.io/python3-pip-skeleton/main/index.html
-.. _`New Skeleton Project Tutorial`: https://diamondlightsource.github.io/python3-pip-skeleton-cli/main/user/tutorials/new.html
+.. _`python-copier-template`: https://diamondlightsource.github.io/python-copier-template/main/index.html
+.. _`Create a new repo from the template`: https://diamondlightsource.github.io/python-copier-template/main/tutorials/create-new.html
```

### Comparing `blueapi-0.4.0/docs/user/how-to/configure-app.rst` & `blueapi-0.4.1a1/docs/how-to/configure-app.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/user/how-to/run-cli.rst` & `blueapi-0.4.1a1/docs/how-to/run-cli.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. seealso:: 
     You must have access to the ``blueapi`` command either via the container or pip installing.
     `./run-container` and `../tutorials/installation`
 
 
 .. seealso:: 
-    In a developer environment, the worker can also be run from vscode: `../../developer/tutorials/dev-run`.
+    In a developer environment, the worker can also be run from vscode: `../tutorials/dev-run`.
 
 
 Basic Introspection
 -------------------
 
 The worker can tell you which plans and devices are available via:
```

### Comparing `blueapi-0.4.0/docs/user/reference/asyncapi.yaml` & `blueapi-0.4.1a1/docs/reference/asyncapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/docs/user/reference/openapi.yaml` & `blueapi-0.4.1a1/docs/reference/openapi.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -84,30 +84,14 @@
             $ref: '#/components/schemas/PlanModel'
           title: Plans
           type: array
       required:
       - plans
       title: PlanResponse
       type: object
-    RunPlan:
-      additionalProperties: false
-      description: Task that will run a plan
-      properties:
-        name:
-          description: Name of plan to run
-          title: Name
-          type: string
-        params:
-          description: Values for parameters to plan, if any
-          title: Params
-          type: object
-      required:
-      - name
-      title: RunPlan
-      type: object
     StateChangeRequest:
       additionalProperties: false
       description: Request to change the state of the worker.
       properties:
         defer:
           default: false
           description: Should worker defer Pausing until the next checkpoint
@@ -119,14 +103,30 @@
           description: The reason for the current run to be aborted
           title: Reason
           type: string
       required:
       - new_state
       title: StateChangeRequest
       type: object
+    Task:
+      additionalProperties: false
+      description: Task that will run a plan
+      properties:
+        name:
+          description: Name of plan to run
+          title: Name
+          type: string
+        params:
+          description: Values for parameters to plan, if any
+          title: Params
+          type: object
+      required:
+      - name
+      title: Task
+      type: object
     TaskResponse:
       additionalProperties: false
       description: Acknowledgement that a task has started, includes its ID
       properties:
         task_id:
           description: Unique identifier for the task
           title: Task Id
@@ -315,15 +315,15 @@
           application/json:
             example:
               name: count
               params:
                 detectors:
                 - x
             schema:
-              $ref: '#/components/schemas/RunPlan'
+              $ref: '#/components/schemas/Task'
         required: true
       responses:
         '201':
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/TaskResponse'
```

### Comparing `blueapi-0.4.0/docs/user/tutorials/installation.rst` & `blueapi-0.4.1a1/docs/tutorials/installation.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-Installation
-============
+# Installation
 
-Check your version of python
-----------------------------
+## Check your version of python
 
-You will need python 3.9 or later. You can check your version of python by
-typing into a terminal::
+You will need python 3.8 or later. You can check your version of python by
+typing into a terminal:
 
-    $ python3 --version
+```
+$ python3 --version
+```
 
-
-Create a virtual environment
-----------------------------
+## Create a virtual environment
 
 It is recommended that you install into a “virtual environment” so this
-installation will not interfere with any existing Python software::
-
-    $ python3 -m venv /path/to/venv
-    $ source /path/to/venv/bin/activate
+installation will not interfere with any existing Python software:
 
+```
+$ python3 -m venv /path/to/venv
+$ source /path/to/venv/bin/activate
+```
 
-Installing the library
-----------------------
+## Installing the library
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use `pip` to install the library and its dependencies:
 
-    $ python3 -m pip install blueapi
+```
+$ python3 -m pip install blueapi
+```
 
 If you require a feature that is not currently released you can also install
-from github::
+from github:
 
-    $ python3 -m pip install git+https://github.com/DiamondLightSource/blueapi.git
+```
+$ python3 -m pip install git+https://github.com/DiamondLightSource/blueapi.git
+```
 
 The library should now be installed and the commandline interface on your path.
-You can check the version that has been installed by typing::
+You can check the version that has been installed by typing:
 
-    $ blueapi --version
+```
+$ blueapi --version
+```
```

### Comparing `blueapi-0.4.0/docs/user/tutorials/quickstart.rst` & `blueapi-0.4.1a1/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/Chart.yaml` & `blueapi-0.4.1a1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.4.1a1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/templates/deployment.yaml` & `blueapi-0.4.1a1/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/templates/ingress.yaml` & `blueapi-0.4.1a1/helm/blueapi/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.4.1a1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/helm/blueapi/values.yaml` & `blueapi-0.4.1a1/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/pyproject.toml` & `blueapi-0.4.1a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
+requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blueapi"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-description = "Lightweight Bluesky-as-a-service wrapper application. Also usable as a library."
+description = "Lightweight bluesky-as-a-service wrapper application. Also usable as a library."
 dependencies = [
     "bluesky",
     "ophyd",
     "nslsii",
     "pyepics",
     "aioca",
     "pydantic<2.0",
     "stomp.py",
     "aiohttp",
     "PyYAML",
     "click<8.1.4",
     "fastapi[all]<0.99",
     "uvicorn",
     "requests",
-    "dls-bluesky-core", #requires ophyd-async
+    "dls-bluesky-core",  #requires ophyd-async
     "dls-dodal",
-    "typing_extensions<4.6",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
-    "black",
-    "mypy",
-    "flake8-isort",
-    "Flake8-pyproject",
+    "copier",
+    "myst-parser",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
+    "mypy",
     "pytest-cov",
     "pytest-asyncio",
+    "ruff",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-click",
     "sphinx-design",
     "sphinxcontrib-openapi",
     "tox-direct",
     "types-mock",
@@ -73,28 +72,14 @@
 [tool.setuptools_scm]
 write_to = "src/blueapi/_version.py"
 
 [tool.mypy]
 ignore_missing_imports = true # Ignore missing stubs in imported modules
 namespace_packages = false    # rely only on __init__ files to determine fully qualified module names.
 
-[tool.isort]
-float_to_top = true
-profile = "black"
-
-[tool.flake8]
-extend-ignore = [
-    "E203", # See https://github.com/PyCQA/pycodestyle/issues/373
-    "F811", # support typing.overload decorator
-    "F722", # allow Annotated[typ, some_func("some string")]
-]
-max-line-length = 88 # Respect black's line length (default 88),
-exclude = [".tox", "venv"]
-
-
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
     --cov=blueapi --cov-report term --cov-report xml:cov.xml
     --ignore=src/blueapi/startup
     """
@@ -118,23 +103,44 @@
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
 
-[testenv:{pre-commit,mypy,pytest,docs}]
+[testenv:{pre-commit,type-checking,tests,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
-allowlist_externals = 
-    pytest 
+allowlist_externals =
+    pytest
     pre-commit
     mypy
     sphinx-build
     sphinx-autobuild
 commands =
-    pytest: pytest {posargs}
-    mypy: mypy src tests {posargs}
     pre-commit: pre-commit run --all-files {posargs}
+    type-checking: mypy src tests {posargs}
+    tests: pytest --cov=blueapi --cov-report term --cov-report xml:cov.xml {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
+
+[tool.ruff]
+src = ["src", "tests"]
+line-length = 88
+lint.select = [
+    "B",  # flake8-bugbear - https://docs.astral.sh/ruff/rules/#flake8-bugbear-b
+    "C4", # flake8-comprehensions - https://docs.astral.sh/ruff/rules/#flake8-comprehensions-c4
+    "E",  # pycodestyle errors - https://docs.astral.sh/ruff/rules/#error-e
+    "F",  # pyflakes rules - https://docs.astral.sh/ruff/rules/#pyflakes-f
+    "W",  # pycodestyle warnings - https://docs.astral.sh/ruff/rules/#warning-w
+    "I",  # isort - https://docs.astral.sh/ruff/rules/#isort-i
+    "UP", # pyupgrade - https://docs.astral.sh/ruff/rules/#pyupgrade-up
+]
+
+[tool.ruff.lint.flake8-bugbear]
+extend-immutable-calls = [
+    "fastapi.Depends",
+    "fastapi.Body",
+    "fastapi.Task",
+    "dls_bluesky_core.core.inject",
+]
```

### Comparing `blueapi-0.4.0/src/blueapi/cli/amq.py` & `blueapi-0.4.1a1/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/cli/cli.py` & `blueapi-0.4.1a1/src/blueapi/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from collections import deque
 from functools import wraps
 from pathlib import Path
 from pprint import pprint
-from typing import Optional, Tuple, Union
+from typing import Optional, Union
 
 import click
 from requests.exceptions import ConnectionError
 
 from blueapi import __version__
 from blueapi.cli.amq import AmqClient
 from blueapi.config import ApplicationConfig, ConfigLoader
@@ -19,26 +19,26 @@
 from blueapi.service.model import WorkerTask
 from blueapi.service.openapi import (
     DOCS_SCHEMA_LOCATION,
     generate_schema,
     print_schema_as_yaml,
     write_schema_as_yaml,
 )
-from blueapi.worker import ProgressEvent, RunPlan, WorkerEvent, WorkerState
+from blueapi.worker import ProgressEvent, Task, WorkerEvent, WorkerState
 
 from .rest import BlueapiRestClient
 
 
 @click.group(invoke_without_command=True)
 @click.version_option(version=__version__, prog_name="blueapi")
 @click.option(
     "-c", "--config", type=Path, help="Path to configuration YAML file", multiple=True
 )
 @click.pass_context
-def main(ctx: click.Context, config: Union[Optional[Path], Tuple[Path, ...]]) -> None:
+def main(ctx: click.Context, config: Union[Optional[Path], tuple[Path, ...]]) -> None:
     # if no command is supplied, run with the options passed
 
     config_loader = ConfigLoader(ApplicationConfig)
     if config is not None:
         configs = (config,) if isinstance(config, Path) else config
         for path in configs:
             if path.exists():
@@ -178,15 +178,15 @@
     finished_event: deque[WorkerEvent] = deque()
 
     def store_finished_event(event: WorkerEvent) -> None:
         if event.is_complete():
             finished_event.append(event)
 
     parameters = parameters or "{}"
-    task = RunPlan(name=name, params=json.loads(parameters))
+    task = Task(name=name, params=json.loads(parameters))
 
     resp = client.create_task(task)
     task_id = resp.task_id
 
     with amq_client:
         amq_client.subscribe_to_topics(task_id, on_event=store_finished_event)
         updated = client.update_worker_task(WorkerTask(task_id=task_id))
```

### Comparing `blueapi-0.4.0/src/blueapi/cli/rest.py` & `blueapi-0.4.1a1/src/blueapi/cli/rest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Any, Callable, Literal, Mapping, Optional, Type, TypeVar
+from collections.abc import Mapping
+from typing import Any, Callable, Literal, Optional, TypeVar
 
 import requests
 from pydantic import parse_obj_as
 
 from blueapi.config import RestConfig
 from blueapi.service.model import (
     DeviceModel,
     DeviceResponse,
     PlanModel,
     PlanResponse,
     TaskResponse,
     WorkerTask,
 )
-from blueapi.worker import RunPlan, TrackableTask, WorkerState
+from blueapi.worker import Task, TrackableTask, WorkerState
 
 from .amq import BlueskyRemoteError
 
 T = TypeVar("T")
 
 
 def _is_exception(response: requests.Response) -> bool:
@@ -52,31 +53,29 @@
         return self._request_and_deserialize(
             "/worker/state",
             target_type=WorkerState,
             method="PUT",
             data={"new_state": state, "defer": defer},
         )
 
-    def get_task(self, task_id: str) -> TrackableTask[RunPlan]:
-        return self._request_and_deserialize(
-            f"/tasks/{task_id}", TrackableTask[RunPlan]
-        )
+    def get_task(self, task_id: str) -> TrackableTask[Task]:
+        return self._request_and_deserialize(f"/tasks/{task_id}", TrackableTask[Task])
 
     def get_active_task(self) -> WorkerTask:
         return self._request_and_deserialize("/worker/task", WorkerTask)
 
-    def create_task(self, task: RunPlan) -> TaskResponse:
+    def create_task(self, task: Task) -> TaskResponse:
         return self._request_and_deserialize(
             "/tasks",
             TaskResponse,
             method="POST",
             data=task.dict(),
         )
 
-    def clear_pending_task(self, task_id: str) -> TaskResponse:
+    def clear_task(self, task_id: str) -> TaskResponse:
         return self._request_and_deserialize(
             f"/tasks/{task_id}", TaskResponse, method="DELETE"
         )
 
     def update_worker_task(self, task: WorkerTask) -> WorkerTask:
         return self._request_and_deserialize(
             "/worker/task",
@@ -96,15 +95,15 @@
             method="PUT",
             data={"new_state": state, "reason": reason},
         )
 
     def _request_and_deserialize(
         self,
         suffix: str,
-        target_type: Type[T],
+        target_type: type[T],
         data: Optional[Mapping[str, Any]] = None,
         method="GET",
         raise_if: Callable[[requests.Response], bool] = _is_exception,
     ) -> T:
         url = self._url(suffix)
         response = requests.request(method, url, json=data)
         if raise_if(response):
```

### Comparing `blueapi-0.4.0/src/blueapi/cli/updates.py` & `blueapi-0.4.1a1/src/blueapi/cli/updates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import itertools
-from typing import Dict, Mapping, Optional, Union
+from collections.abc import Mapping
+from typing import Optional, Union
 
 from tqdm import tqdm
 
 from blueapi.worker import ProgressEvent, StatusView, WorkerEvent
 
 _BAR_FMT = "{desc}: |{bar}| {percentage:3.0f}% [{elapsed}/{remaining}]"
 
 
 class ProgressBarRenderer:
-    _bars: Dict[str, tqdm]
+    _bars: dict[str, tqdm]
     _count: itertools.count
 
     def __init__(self) -> None:
         self._bars = {}
         self._count = itertools.count()
 
     def update(self, status_view: Mapping[str, StatusView]) -> None:
```

### Comparing `blueapi-0.4.0/src/blueapi/config.py` & `blueapi-0.4.1a1/src/blueapi/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
+from collections.abc import Mapping
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Generic, Literal, Mapping, Optional, Type, TypeVar, Union
+from typing import Any, Generic, Literal, Optional, TypeVar, Union
 
 import yaml
 from pydantic import BaseModel, Field, ValidationError, parse_obj_as, validator
 
 from blueapi.utils import BlueapiBaseModel, InvalidConfigError
 
 LogLevel = Literal["NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
@@ -120,33 +121,33 @@
     """
     Small utility class for loading config from various sources.
     You must define a config schema as a dataclass (or series of
     nested dataclasses) that can then be loaded from some combination
     of default values, dictionaries, YAML/JSON files etc.
     """
 
-    _schema: Type[C]
-    _values: Dict[str, Any]
+    _schema: type[C]
+    _values: dict[str, Any]
 
-    def __init__(self, schema: Type[C]) -> None:
+    def __init__(self, schema: type[C]) -> None:
         self._schema = schema
         self._values = {}
 
     def use_values(self, values: Mapping[str, Any]) -> None:
         """
         Use all values provided in the config, override any defaults
         and values set by previous calls into this class.
 
         Args:
             values (Mapping[str, Any]): Dictionary of override values,
                                         does not need to be exhaustive
                                         if defaults provided.
         """
 
-        def recursively_update_map(old: Dict[str, Any], new: Mapping[str, Any]) -> None:
+        def recursively_update_map(old: dict[str, Any], new: Mapping[str, Any]) -> None:
             for key in new:
                 if (
                     key in old
                     and isinstance(old[key], dict)
                     and isinstance(new[key], dict)
                 ):
                     recursively_update_map(old[key], new[key])
```

### Comparing `blueapi-0.4.0/src/blueapi/core/__init__.py` & `blueapi-0.4.1a1/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/core/bluesky_types.py` & `blueapi-0.4.1a1/src/blueapi/core/bluesky_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 import inspect
-from typing import Any, Callable, Mapping, Optional, Type, Union, get_type_hints
+from collections.abc import Mapping
+from typing import (
+    Any,
+    Callable,
+    Optional,
+    Protocol,
+    Union,
+    get_type_hints,
+    runtime_checkable,
+)
 
 from bluesky.protocols import (
     Checkable,
     Configurable,
     Flyable,
     HasHints,
     HasName,
@@ -20,19 +29,14 @@
 )
 from dls_bluesky_core.core import MsgGenerator, PlanGenerator
 from ophyd_async.core import Device as AsyncDevice
 from pydantic import BaseModel, Field
 
 from blueapi.utils import BlueapiBaseModel
 
-try:
-    from typing import Protocol, runtime_checkable
-except ImportError:
-    from typing_extensions import Protocol, runtime_checkable  # type: ignore
-
 PlanWrapper = Callable[[MsgGenerator], MsgGenerator]
 
 #: An object that encapsulates the device to do useful things to produce
 # data (e.g. move and read)
 Device = Union[
     Checkable,
     Flyable,
@@ -58,22 +62,22 @@
 def is_bluesky_compatible_device(obj: Any) -> bool:
     is_object = not inspect.isclass(obj)
     # We must separately check if Obj refers to an instance rather than a
     # class, as both follow the protocols but only one is a "device".
     return is_object and _follows_bluesky_protocols(obj)
 
 
-def is_bluesky_compatible_device_type(cls: Type[Any]) -> bool:
+def is_bluesky_compatible_device_type(cls: type[Any]) -> bool:
     # We must separately check if Obj refers to an class rather than an
     # instance, as both follow the protocols but only one is a type.
     return inspect.isclass(cls) and _follows_bluesky_protocols(cls)
 
 
 def _follows_bluesky_protocols(obj: Any) -> bool:
-    return any(map(lambda protocol: isinstance(obj, protocol), BLUESKY_PROTOCOLS))
+    return any(isinstance(obj, protocol) for protocol in BLUESKY_PROTOCOLS)
 
 
 def is_bluesky_plan_generator(func: PlanGenerator) -> bool:
     try:
         return get_type_hints(func).get("return") is MsgGenerator
     except TypeError:
         # get_type_hints fails on some objects (such as Union or Optional)
@@ -85,15 +89,15 @@
     A plan that can be run
     """
 
     name: str = Field(description="Referenceable name of the plan")
     description: Optional[str] = Field(
         description="Description/docstring of the plan", default=None
     )
-    model: Type[BaseModel] = Field(
+    model: type[BaseModel] = Field(
         description="Validation model of the parameters for the plan"
     )
 
 
 class DataEvent(BlueapiBaseModel):
     """
     Event representing collection of some data. Conforms to the Bluesky event model:
```

### Comparing `blueapi-0.4.0/src/blueapi/core/context.py` & `blueapi-0.4.1a1/src/blueapi/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import functools
 import logging
+from collections.abc import Sequence
 from dataclasses import dataclass, field
 from importlib import import_module
 from inspect import Parameter, signature
 from types import ModuleType
 from typing import (
     Any,
     Callable,
-    Dict,
     Generic,
-    List,
     Optional,
-    Sequence,
-    Tuple,
-    Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
     get_type_hints,
 )
 
@@ -56,30 +52,30 @@
     The context holds the RunEngine and any plans/devices that you may want to use.
     """
 
     run_engine: RunEngine = field(
         default_factory=lambda: RunEngine(context_managers=[])
     )
     plan_wrappers: Sequence[PlanWrapper] = field(default_factory=list)
-    plans: Dict[str, Plan] = field(default_factory=dict)
-    devices: Dict[str, Device] = field(default_factory=dict)
-    plan_functions: Dict[str, PlanGenerator] = field(default_factory=dict)
+    plans: dict[str, Plan] = field(default_factory=dict)
+    devices: dict[str, Device] = field(default_factory=dict)
+    plan_functions: dict[str, PlanGenerator] = field(default_factory=dict)
     sim: bool = field(default=False)
 
-    _reference_cache: Dict[Type, Type] = field(default_factory=dict)
+    _reference_cache: dict[type, type] = field(default_factory=dict)
 
     def wrap(self, plan: MsgGenerator) -> MsgGenerator:
         wrapped_plan = functools.reduce(
             lambda wrapped, next_wrapper: next_wrapper(wrapped),
             self.plan_wrappers,
             plan,
         )
         yield from wrapped_plan
 
-    def find_device(self, addr: Union[str, List[str]]) -> Optional[Device]:
+    def find_device(self, addr: Union[str, list[str]]) -> Optional[Device]:
         """
         Find a device in this context, allows for recursive search.
 
         Args:
             addr (Union[str, List[str]]): Address of the device, examples:
                                           "motors", "motors.x"
 
@@ -195,15 +191,15 @@
             if isinstance(device, HasName):
                 name = device.name
             else:
                 raise KeyError(f"Must supply a name for this device: {device}")
 
         self.devices[name] = device
 
-    def _reference(self, target: Type) -> Type:
+    def _reference(self, target: type) -> type:
         """
         Create an intermediate reference type for the required ``target`` type that
         will return an existing device during pydantic deserialisation/validation
 
         Args:
             target: Expected type of the device that is expected for IDs being
                 deserialised by the return type
@@ -234,15 +230,15 @@
 
             self._reference_cache[target] = Reference
 
         return self._reference_cache[target]
 
     def _type_spec_for_function(
         self, func: Callable[..., Any]
-    ) -> dict[str, Tuple[Type, Any]]:
+    ) -> dict[str, tuple[type, Any]]:
         """
         Parse a function signature and build map of field types and default
         values that can be used to deserialise arguments from external sources.
         Any references to any of the bluesky protocols are replaced with an
         intermediate reference type that allows existing devices to be returned
         for device ID strings.
 
@@ -267,15 +263,15 @@
             factory = None if no_default else DefaultFactory(para.default)
             new_args[name] = (
                 self._convert_type(arg_type),
                 FieldInfo(default_factory=factory),
             )
         return new_args
 
-    def _convert_type(self, typ: Type) -> Type:
+    def _convert_type(self, typ: type) -> type:
         """
         Recursively convert a type to something that can be deserialised by
         pydantic. Bluesky protocols (and types that extend them) are replaced
         with an intermediate reference types that allows the current context to
         be used to look up an existing device when deserialising device ID
         strings.
```

### Comparing `blueapi-0.4.0/src/blueapi/core/device_lookup.py` & `blueapi-0.4.1a1/src/blueapi/core/device_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Any, List, Optional, TypeVar
+from typing import Any, Optional, TypeVar
 
 from .bluesky_types import Device, is_bluesky_compatible_device
 
 #: Device obeying Bluesky protocols
 D = TypeVar("D", bound=Device)
 
 
-def find_component(obj: Any, addr: List[str]) -> Optional[D]:
+def find_component(obj: Any, addr: list[str]) -> Optional[D]:
     """
     Best effort function to locate a child device, either in a dictionary of
     devices or a device with child attributes.
 
     Args:
         obj (Any): Root device or dictionary of devices
         addr (List[str]): Address of target device e.g. motors.x
```

### Comparing `blueapi-0.4.0/src/blueapi/core/event.py` & `blueapi-0.4.1a1/src/blueapi/core/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 from abc import ABC, abstractmethod
-from typing import Callable, Dict, Generic, Optional, TypeVar
+from typing import Callable, Generic, Optional, TypeVar
 
 #: Event type
 E = TypeVar("E")
 
 #: Subscription token type
 S = TypeVar("S")
 
@@ -43,15 +43,15 @@
 
 
 class EventPublisher(EventStream[E, int]):
     """
     Simple Observable that can be fed values to publish
     """
 
-    _subscriptions: Dict[int, Callable[[E, Optional[str]], None]]
+    _subscriptions: dict[int, Callable[[E, Optional[str]], None]]
     _count: itertools.count
 
     def __init__(self) -> None:
         self._subscriptions = {}
         self._count = itertools.count()
 
     def subscribe(self, callback: Callable[[E, Optional[str]], None]) -> int:
```

### Comparing `blueapi-0.4.0/src/blueapi/data_management/visit_directory_provider.py` & `blueapi-0.4.1a1/src/blueapi/data_management/visit_directory_provider.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/messaging/base.py` & `blueapi-0.4.1a1/src/blueapi/messaging/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from concurrent.futures import Future
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable, Optional
 
 from .context import MessageContext
 
 MessageListener = Callable[[MessageContext, Any], None]
 
 
 class DestinationProvider(ABC):
@@ -82,15 +82,15 @@
             DestinationProvider: Destination provider
         """
 
     def send_and_receive(
         self,
         destination: str,
         obj: Any,
-        reply_type: Type = str,
+        reply_type: type = str,
         correlation_id: Optional[str] = None,
     ) -> Future:
         """
         Send a message expecting a single reply.
 
         Args:
             destination (str): Destination to send the message
```

### Comparing `blueapi-0.4.0/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.4.1a1/src/blueapi/messaging/stomptemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import json
 import logging
 import time
 import uuid
 from dataclasses import dataclass
 from threading import Event
-from typing import Any, Callable, Dict, List, Optional, Set
+from typing import Any, Callable, Optional
 
 import stomp
 from pydantic import parse_obj_as
 from stomp.exception import ConnectFailedException
 from stomp.utils import Frame
 
 from blueapi.config import BasicAuthentication, StompConfig
@@ -70,16 +70,16 @@
     """
 
     _conn: stomp.Connection
     _reconnect_policy: StompReconnectPolicy
     _authentication: BasicAuthentication
     _sub_num: itertools.count
     _listener: stomp.ConnectionListener
-    _subscriptions: Dict[str, Subscription]
-    _pending_subscriptions: Set[str]
+    _subscriptions: dict[str, Subscription]
+    _pending_subscriptions: set[str]
     _disconnected: Event
 
     # Stateless implementation means attribute can be static
     _destination_provider: DestinationProvider = StompDestinationProvider()
 
     def __init__(
         self,
@@ -129,30 +129,30 @@
         destination: str,
         message: str,
         on_reply: Optional[MessageListener] = None,
         correlation_id: Optional[str] = None,
     ) -> None:
         LOGGER.info(f"SENDING {message} to {destination}")
 
-        headers: Dict[str, Any] = {"JMSType": "TextMessage"}
+        headers: dict[str, Any] = {"JMSType": "TextMessage"}
         if on_reply is not None:
             reply_queue_name = self.destinations.temporary_queue(str(uuid.uuid1()))
             headers = {**headers, "reply-to": reply_queue_name}
             self.subscribe(reply_queue_name, on_reply)
         if correlation_id:
             headers = {**headers, CORRELATION_ID_HEADER: correlation_id}
         self._conn.send(headers=headers, body=message, destination=destination)
 
     def subscribe(self, destination: str, callback: MessageListener) -> None:
         LOGGER.debug(f"New subscription to {destination}")
         obj_type = determine_deserialization_type(callback, default=str)
 
         def wrapper(frame: Frame) -> None:
             as_dict = json.loads(frame.body)
-            value = parse_obj_as(obj_type, as_dict)
+            value: Any = parse_obj_as(obj_type, as_dict)
 
             context = MessageContext(
                 frame.headers["destination"],
                 frame.headers.get("reply-to"),
                 frame.headers.get(CORRELATION_ID_HEADER),
             )
             callback(context, value)
@@ -189,15 +189,15 @@
             )
             connected.wait()
         except ConnectFailedException as ex:
             LOGGER.exception(msg="Failed to connect to message bus", exc_info=ex)
 
         self._ensure_subscribed()
 
-    def _ensure_subscribed(self, sub_ids: Optional[List[str]] = None) -> None:
+    def _ensure_subscribed(self, sub_ids: Optional[list[str]] = None) -> None:
         # We must defer subscription until after connection, because stomp literally
         # sends a SUB to the broker. But it still nice to be able to call subscribe
         # on template before it connects, then just run the subscribes after connection.
         if self._conn.is_connected():
             for sub_id in sub_ids or self._subscriptions.keys():
                 sub = self._subscriptions[sub_id]
                 LOGGER.info(f"Subscribing to {sub.destination}")
```

### Comparing `blueapi-0.4.0/src/blueapi/messaging/utils.py` & `blueapi-0.4.1a1/src/blueapi/messaging/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inspect
-from typing import Type
 
 from .base import MessageListener
 
 
 def determine_deserialization_type(
-    listener: MessageListener, default: Type = str
-) -> Type:
+    listener: MessageListener, default: type = str
+) -> type:
     """
     Inspect a message listener function to determine the type to deserialize
     a message to
 
     Args:
         listener (MessageListener): The function that takes a deserialized message
         default (Type, optional): If the type cannot be determined, what default
```

### Comparing `blueapi-0.4.0/src/blueapi/preprocessors/attach_metadata.py` & `blueapi-0.4.1a1/src/blueapi/preprocessors/attach_metadata.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/service/handler.py` & `blueapi-0.4.1a1/src/blueapi/service/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import List, Mapping, Optional
+from collections.abc import Mapping
+from typing import Optional
 
 from blueapi.config import ApplicationConfig
 from blueapi.core import BlueskyContext
 from blueapi.core.event import EventStream
 from blueapi.data_management.visit_directory_provider import (
     LocalVisitServiceClient,
     VisitDirectoryProvider,
@@ -12,16 +13,16 @@
 )
 from blueapi.messaging import StompMessagingTemplate
 from blueapi.messaging.base import MessagingTemplate
 from blueapi.preprocessors.attach_metadata import attach_metadata
 from blueapi.service.handler_base import BlueskyHandler
 from blueapi.service.model import DeviceModel, PlanModel, WorkerTask
 from blueapi.worker.event import WorkerState
-from blueapi.worker.reworker import RunEngineWorker
-from blueapi.worker.task import RunPlan
+from blueapi.worker.reworker import TaskWorker
+from blueapi.worker.task import Task
 from blueapi.worker.worker import TrackableTask, Worker
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Handler(BlueskyHandler):
     _context: BlueskyContext
@@ -38,15 +39,15 @@
         worker: Optional[Worker] = None,
     ) -> None:
         self._config = config or ApplicationConfig()
         self._context = context or BlueskyContext()
 
         self._context.with_config(self._config.env)
 
-        self._worker = worker or RunEngineWorker(
+        self._worker = worker or TaskWorker(
             self._context,
             broadcast_statuses=self._config.env.events.broadcast_status_events,
         )
         self._messaging_template = (
             messaging_template
             or StompMessagingTemplate.autoconfigured(self._config.stomp)
         )
@@ -83,33 +84,33 @@
     def stop(self) -> None:
         self._initialized = False
         self._worker.stop()
         if self._messaging_template.is_connected():
             self._messaging_template.disconnect()
 
     @property
-    def plans(self) -> List[PlanModel]:
+    def plans(self) -> list[PlanModel]:
         return [PlanModel.from_plan(plan) for plan in self._context.plans.values()]
 
     def get_plan(self, name: str) -> PlanModel:
         return PlanModel.from_plan(self._context.plans[name])
 
     @property
-    def devices(self) -> List[DeviceModel]:
+    def devices(self) -> list[DeviceModel]:
         return [
             DeviceModel.from_device(device) for device in self._context.devices.values()
         ]
 
     def get_device(self, name: str) -> DeviceModel:
         return DeviceModel.from_device(self._context.devices[name])
 
-    def submit_task(self, task: RunPlan) -> str:
+    def submit_task(self, task: Task) -> str:
         return self._worker.submit_task(task)
 
-    def clear_pending_task(self, task_id: str) -> str:
+    def clear_task(self, task_id: str) -> str:
         return self._worker.clear_task(task_id)
 
     def begin_task(self, task: WorkerTask) -> WorkerTask:
         if task.task_id is not None:
             self._worker.begin_task(task.task_id)
         return task
 
@@ -127,19 +128,19 @@
     def resume_worker(self) -> None:
         self._worker.resume()
 
     def cancel_active_task(self, failure: bool, reason: Optional[str]):
         self._worker.cancel_active_task(failure, reason)
 
     @property
-    def pending_tasks(self) -> List[TrackableTask]:
-        return self._worker.get_pending_tasks()
+    def tasks(self) -> list[TrackableTask]:
+        return self._worker.get_tasks()
 
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask]:
-        return self._worker.get_pending_task(task_id)
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask]:
+        return self._worker.get_task_by_id(task_id)
 
     @property
     def initialized(self) -> bool:
         return self._initialized
 
 
 HANDLER: Optional[Handler] = None
```

### Comparing `blueapi-0.4.0/src/blueapi/service/handler_base.py` & `blueapi-0.4.1a1/src/blueapi/service/handler_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from abc import ABC, abstractmethod
-from typing import List, Optional
+from typing import Optional
 
 from blueapi.service.model import DeviceModel, PlanModel, WorkerTask
 from blueapi.worker.event import WorkerState
-from blueapi.worker.task import RunPlan
+from blueapi.worker.task import Task
 from blueapi.worker.worker import TrackableTask
 
 
 class BlueskyHandler(ABC):
     """Interface between web application and underlying Bluesky context and worker"""
 
     @property
     @abstractmethod
-    def plans(self) -> List[PlanModel]:
+    def plans(self) -> list[PlanModel]:
         """
         All available plans in the BlueskyContext
         """
 
     @abstractmethod
     def get_plan(self, name: str) -> PlanModel:
         """
         Retrieve plan by name from the BlueskyContext
         """
 
     @property
     @abstractmethod
-    def devices(self) -> List[DeviceModel]:
+    def devices(self) -> list[DeviceModel]:
         """
         All available devices in the BlueskyContext
         """
 
     @abstractmethod
     def get_device(self, name: str) -> DeviceModel:
         """
         Retrieve device by name from the BlueskyContext
         """
 
     @abstractmethod
-    def submit_task(self, task: RunPlan) -> str:
+    def submit_task(self, task: Task) -> str:
         """
         Submit a task to be run on begin_task
         """
 
     @abstractmethod
-    def clear_pending_task(self, task_id: str) -> str:
-        """Remove a pending task from the worker"""
+    def clear_task(self, task_id: str) -> str:
+        """Remove a task from the worker"""
 
     @abstractmethod
     def begin_task(self, task: WorkerTask) -> WorkerTask:
-        """Trigger a pending task. Will fail if the worker is busy"""
+        """Trigger a task. Will fail if the worker is busy"""
 
     @property
     @abstractmethod
     def active_task(self) -> Optional[TrackableTask]:
         """Task the worker is currently running"""
 
     @property
@@ -71,20 +71,20 @@
     @abstractmethod
     def cancel_active_task(self, failure: bool, reason: Optional[str]) -> None:
         """Remove the currently active task from the worker if there is one
         Returns the task_id of the active task"""
 
     @property
     @abstractmethod
-    def pending_tasks(self) -> List[TrackableTask]:
-        """Return a list of all tasks pending on the worker,
+    def tasks(self) -> list[TrackableTask]:
+        """Return a list of all tasks on the worker,
         any one of which can be triggered with begin_task"""
 
     @abstractmethod
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask]:
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask]:
         """Returns a task matching the task ID supplied,
         if the worker knows of it"""
 
     @abstractmethod
     def start(self):
         """Start the handler"""
```

### Comparing `blueapi-0.4.0/src/blueapi/service/main.py` & `blueapi-0.4.1a1/src/blueapi/service/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import asynccontextmanager
-from typing import Dict, Optional, Set
+from typing import Optional
 
 from fastapi import (
     BackgroundTasks,
     Body,
     Depends,
     FastAPI,
     HTTPException,
@@ -12,15 +12,15 @@
     status,
 )
 from pydantic import ValidationError
 from starlette.responses import JSONResponse
 from super_state_machine.errors import TransitionError
 
 from blueapi.config import ApplicationConfig
-from blueapi.worker import RunPlan, TrackableTask, WorkerState
+from blueapi.worker import Task, TrackableTask, WorkerState
 
 from .handler_base import BlueskyHandler
 from .model import (
     DeviceModel,
     DeviceResponse,
     EnvironmentResponse,
     PlanModel,
@@ -137,36 +137,34 @@
     "/tasks",
     response_model=TaskResponse,
     status_code=status.HTTP_201_CREATED,
 )
 def submit_task(
     request: Request,
     response: Response,
-    task: RunPlan = Body(
-        ..., example=RunPlan(name="count", params={"detectors": ["x"]})
-    ),
+    task: Task = Body(..., example=Task(name="count", params={"detectors": ["x"]})),  # noqa: B008
     handler: BlueskyHandler = Depends(get_handler),
 ):
     """Submit a task to the worker."""
     try:
         task_id: str = handler.submit_task(task)
         response.headers["Location"] = f"{request.url}/{task_id}"
         return TaskResponse(task_id=task_id)
     except ValidationError as e:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=e.errors()
-        )
+        ) from e
 
 
 @app.delete("/tasks/{task_id}", status_code=status.HTTP_200_OK)
 def delete_submitted_task(
     task_id: str,
     handler: BlueskyHandler = Depends(get_handler),
 ) -> TaskResponse:
-    return TaskResponse(task_id=handler.clear_pending_task(task_id))
+    return TaskResponse(task_id=handler.clear_task(task_id))
 
 
 @app.put(
     "/worker/task",
     response_model=WorkerTask,
     responses={status.HTTP_409_CONFLICT: {"worker": "already active"}},
 )
@@ -188,18 +186,18 @@
     response_model=TrackableTask,
 )
 def get_task(
     task_id: str,
     handler: BlueskyHandler = Depends(get_handler),
 ) -> TrackableTask:
     """Retrieve a task"""
-    pending = handler.get_pending_task(task_id)
-    if pending is None:
+    task = handler.get_task_by_id(task_id)
+    if task is None:
         raise KeyError
-    return pending
+    return task
 
 
 @app.get("/worker/task")
 def get_active_task(handler: BlueskyHandler = Depends(get_handler)) -> WorkerTask:
     active = handler.active_task
     if active is not None:
         return WorkerTask(task_id=active.task_id)
@@ -210,15 +208,15 @@
 @app.get("/worker/state")
 def get_state(handler: BlueskyHandler = Depends(get_handler)) -> WorkerState:
     """Get the State of the Worker"""
     return handler.state
 
 
 # Map of current_state: allowed new_states
-_ALLOWED_TRANSITIONS: Dict[WorkerState, Set[WorkerState]] = {
+_ALLOWED_TRANSITIONS: dict[WorkerState, set[WorkerState]] = {
     WorkerState.RUNNING: {
         WorkerState.PAUSED,
         WorkerState.ABORTING,
         WorkerState.STOPPING,
     },
     WorkerState.PAUSED: {
         WorkerState.RUNNING,
```

### Comparing `blueapi-0.4.0/src/blueapi/service/model.py` & `blueapi-0.4.1a1/src/blueapi/service/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Iterable, List, Optional
+from collections.abc import Iterable
+from typing import Any, Optional
 
 from bluesky.protocols import HasName
 from pydantic import Field
 
 from blueapi.core import BLUESKY_PROTOCOLS, Device, Plan
 from blueapi.utils import BlueapiBaseModel
 from blueapi.worker import Worker, WorkerState
@@ -12,15 +13,15 @@
 
 class DeviceModel(BlueapiBaseModel):
     """
     Representation of a device
     """
 
     name: str = Field(description="Name of the device")
-    protocols: List[str] = Field(
+    protocols: list[str] = Field(
         description="Protocols that a device conforms to, indicating its capabilities"
     )
 
     @classmethod
     def from_device(cls, device: Device) -> "DeviceModel":
         name = device.name if isinstance(device, HasName) else _UNKNOWN_NAME
         return cls(name=name, protocols=list(_protocol_names(device)))
@@ -41,15 +42,15 @@
 
 
 class DeviceResponse(BlueapiBaseModel):
     """
     Response to a query for devices
     """
 
-    devices: List[DeviceModel] = Field(description="Devices available to use in plans")
+    devices: list[DeviceModel] = Field(description="Devices available to use in plans")
 
 
 class PlanModel(BlueapiBaseModel):
     """
     Representation of a plan
     """
 
@@ -81,15 +82,15 @@
 
 
 class PlanResponse(BlueapiBaseModel):
     """
     Response to a query for plans
     """
 
-    plans: List[PlanModel] = Field(description="Plans available to use by a worker")
+    plans: list[PlanModel] = Field(description="Plans available to use by a worker")
 
 
 class TaskResponse(BlueapiBaseModel):
     """
     Acknowledgement that a task has started, includes its ID
     """
```

### Comparing `blueapi-0.4.0/src/blueapi/service/openapi.py` & `blueapi-0.4.1a1/src/blueapi/service/openapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """Generate openapi.json."""
 
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Mapping
 
 import yaml
 from fastapi.openapi.utils import get_openapi
 from pyparsing import Any
 
 from blueapi.service.main import app
 
-DOCS_SCHEMA_LOCATION = (
-    Path(__file__).parents[3] / "docs" / "user" / "reference" / "openapi.yaml"
-)
+DOCS_SCHEMA_LOCATION = Path(__file__).parents[3] / "docs" / "reference" / "openapi.yaml"
 
 
 def generate_schema() -> Mapping[str, Any]:
     return get_openapi(
         title=app.title,
         version=app.version,
         openapi_version=app.openapi_version,
```

### Comparing `blueapi-0.4.0/src/blueapi/service/subprocess_handler.py` & `blueapi-0.4.1a1/src/blueapi/service/subprocess_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import signal
+from collections.abc import Iterable
 from multiprocessing import Pool, set_start_method
 from multiprocessing.pool import Pool as PoolClass
-from typing import Callable, Iterable, List, Optional
+from typing import Callable, Optional
 
 from blueapi.config import ApplicationConfig
 from blueapi.service.handler import get_handler, setup_handler, teardown_handler
 from blueapi.service.handler_base import BlueskyHandler, HandlerNotStartedError
 from blueapi.service.model import DeviceModel, PlanModel, WorkerTask
 from blueapi.worker.event import WorkerState
-from blueapi.worker.task import RunPlan
+from blueapi.worker.task import Task
 from blueapi.worker.worker import TrackableTask
 
 set_start_method("spawn", force=True)
 LOGGER = logging.getLogger(__name__)
 
 
 def _init_worker():
@@ -61,32 +62,32 @@
         if arguments is None:
             arguments = []
         if self._subprocess is None:
             raise HandlerNotStartedError("Subprocess handler has not been started")
         return self._subprocess.apply(function, arguments)
 
     @property
-    def plans(self) -> List[PlanModel]:
+    def plans(self) -> list[PlanModel]:
         return self._run_in_subprocess(plans)
 
     def get_plan(self, name: str) -> PlanModel:
         return self._run_in_subprocess(get_plan, [name])
 
     @property
-    def devices(self) -> List[DeviceModel]:
+    def devices(self) -> list[DeviceModel]:
         return self._run_in_subprocess(devices)
 
     def get_device(self, name: str) -> DeviceModel:
         return self._run_in_subprocess(get_device, [name])
 
-    def submit_task(self, task: RunPlan) -> str:
+    def submit_task(self, task: Task) -> str:
         return self._run_in_subprocess(submit_task, [task])
 
-    def clear_pending_task(self, task_id: str) -> str:
-        return self._run_in_subprocess(clear_pending_task, [task_id])
+    def clear_task(self, task_id: str) -> str:
+        return self._run_in_subprocess(clear_task_by_id, [task_id])
 
     def begin_task(self, task: WorkerTask) -> WorkerTask:
         return self._run_in_subprocess(begin_task, [task])
 
     @property
     def active_task(self) -> Optional[TrackableTask]:
         return self._run_in_subprocess(active_task)
@@ -101,50 +102,50 @@
     def resume_worker(self) -> None:
         return self._run_in_subprocess(resume_worker)
 
     def cancel_active_task(self, failure: bool, reason: Optional[str]) -> None:
         return self._run_in_subprocess(cancel_active_task, [failure, reason])
 
     @property
-    def pending_tasks(self) -> List[TrackableTask]:
-        return self._run_in_subprocess(pending_tasks)
+    def tasks(self) -> list[TrackableTask]:
+        return self._run_in_subprocess(tasks)
 
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask]:
-        return self._run_in_subprocess(get_pending_task, [task_id])
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask]:
+        return self._run_in_subprocess(get_task_by_id, [task_id])
 
     @property
     def initialized(self) -> bool:
         return self._initialized
 
 
 # Free functions (passed to subprocess) for each of the methods required by Handler
 
 
-def plans() -> List[PlanModel]:
+def plans() -> list[PlanModel]:
     return get_handler().plans
 
 
 def get_plan(name: str):
     return get_handler().get_plan(name)
 
 
-def devices() -> List[DeviceModel]:
+def devices() -> list[DeviceModel]:
     return get_handler().devices
 
 
 def get_device(name: str) -> DeviceModel:
     return get_handler().get_device(name)
 
 
-def submit_task(task: RunPlan) -> str:
+def submit_task(task: Task) -> str:
     return get_handler().submit_task(task)
 
 
-def clear_pending_task(task_id: str) -> str:
-    return get_handler().clear_pending_task(task_id)
+def clear_task_by_id(task_id: str) -> str:
+    return get_handler().clear_task(task_id)
 
 
 def begin_task(task: WorkerTask) -> WorkerTask:
     return get_handler().begin_task(task)
 
 
 def active_task() -> Optional[TrackableTask]:
@@ -163,13 +164,13 @@
     return get_handler().resume_worker()
 
 
 def cancel_active_task(failure: bool, reason: Optional[str]) -> None:
     return get_handler().cancel_active_task(failure, reason)
 
 
-def pending_tasks() -> List[TrackableTask]:
-    return get_handler().pending_tasks
+def tasks() -> list[TrackableTask]:
+    return get_handler().tasks
 
 
-def get_pending_task(task_id: str) -> Optional[TrackableTask]:
-    return get_handler().get_pending_task(task_id)
+def get_task_by_id(task_id: str) -> Optional[TrackableTask]:
+    return get_handler().get_task_by_id(task_id)
```

### Comparing `blueapi-0.4.0/src/blueapi/startup/example_devices.py` & `blueapi-0.4.1a1/src/blueapi/startup/example_devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/startup/example_plans.py` & `blueapi-0.4.1a1/src/blueapi/startup/example_plans.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import List
-
 from bluesky.protocols import Movable, Readable
 from dls_bluesky_core.core import inject
 from dls_bluesky_core.plans import count
 from dls_bluesky_core.stubs import move
 
 from blueapi.core import MsgGenerator
 
 
 def stp_snapshot(
-    detectors: List[Readable],
+    detectors: list[Readable],
     temperature: Movable = inject("sample_temperature"),
     pressure: Movable = inject("sample_pressure"),
 ) -> MsgGenerator:
     """
     Moves devices for pressure and temperature (defaults fetched from the context)
     and captures a single frame from a collection of devices
     Args:
```

### Comparing `blueapi-0.4.0/src/blueapi/startup/simmotor.py` & `blueapi-0.4.1a1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/utils/__init__.py` & `blueapi-0.4.1a1/src/blueapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/utils/base_model.py` & `blueapi-0.4.1a1/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/utils/modules.py` & `blueapi-0.4.1a1/src/blueapi/utils/modules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Iterable
 from types import ModuleType
-from typing import Any, Iterable, List
+from typing import Any
 
 
 def load_module_all(mod: ModuleType) -> Iterable[Any]:
     """
     If __export__ is defined for the module, try importing those functions as plans,
     else load the global variables exported via the `__all__` magic variable.
     Dynamic equivalent to `from my_module import *`. Use everything that doesn't start
@@ -17,15 +18,15 @@
     Args:
         mod (ModuleType): The module to extract globals from
 
     Yields:
         Iterator[Iterable[Any]]: Each successive variable in globals
     """
 
-    def get_named_subset(names: List[str]):
+    def get_named_subset(names: list[str]):
         for name in names:
             yield getattr(mod, name)
 
     if "__export__" in mod.__dict__:
         yield from get_named_subset(mod.__dict__["__export__"])
     elif "__all__" in mod.__dict__:
         yield from get_named_subset(mod.__dict__["__all__"])
```

### Comparing `blueapi-0.4.0/src/blueapi/utils/serialization.py` & `blueapi-0.4.1a1/src/blueapi/utils/serialization.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     """
 
     if isinstance(obj, BaseModel):
         # Serialize by alias so that our camelCase models leave the service
         # with camelCase field names
         return obj.dict(by_alias=True)
     elif hasattr(obj, "__pydantic_model__"):
-        return serialize(getattr(obj, "__pydantic_model__"))
+        return serialize(obj.__pydantic_model__)
     else:
         return obj
```

### Comparing `blueapi-0.4.0/src/blueapi/utils/thread_exception.py` & `blueapi-0.4.1a1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/worker/__init__.py` & `blueapi-0.4.1a1/src/blueapi/worker/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .event import ProgressEvent, StatusView, TaskStatus, WorkerEvent, WorkerState
 from .multithread import run_worker_in_own_thread
-from .reworker import RunEngineWorker
-from .task import RunPlan, Task
+from .reworker import TaskWorker
+from .task import Task
 from .worker import TrackableTask, Worker
-from .worker_busy_error import WorkerBusyError
+from .worker_errors import WorkerAlreadyStartedError, WorkerBusyError
 
 __all__ = [
     "run_worker_in_own_thread",
-    "RunEngineWorker",
+    "TaskWorker",
     "Task",
     "Worker",
-    "RunPlan",
     "WorkerEvent",
     "WorkerState",
     "StatusView",
     "ProgressEvent",
     "TaskStatus",
     "TrackableTask",
     "WorkerBusyError",
+    "WorkerAlreadyStartedError",
 ]
```

### Comparing `blueapi-0.4.0/src/blueapi/worker/event.py` & `blueapi-0.4.1a1/src/blueapi/worker/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Mapping
 from enum import Enum
-from typing import List, Mapping, Optional, Union
+from typing import Optional, Union
 
 from bluesky.run_engine import RunEngineStateMachine
 from pydantic import Field
 from super_state_machine.extras import PropertyMachine, ProxyString
 
 from blueapi.utils import BlueapiBaseModel
 
@@ -106,16 +107,16 @@
     """
     Event describing the state of the worker and any tasks it's running.
     Includes error and warning information.
     """
 
     state: WorkerState
     task_status: Optional[TaskStatus] = None
-    errors: List[str] = Field(default_factory=list)
-    warnings: List[str] = Field(default_factory=list)
+    errors: list[str] = Field(default_factory=list)
+    warnings: list[str] = Field(default_factory=list)
 
     def is_error(self) -> bool:
         return (self.task_status is not None and self.task_status.task_failed) or bool(
             self.errors
         )
 
     def is_complete(self) -> bool:
```

### Comparing `blueapi-0.4.0/src/blueapi/worker/multithread.py` & `blueapi-0.4.1a1/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/src/blueapi/worker/reworker.py` & `blueapi-0.4.1a1/src/blueapi/worker/reworker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import uuid
+from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from functools import partial
 from queue import Full, Queue
 from threading import Event, RLock
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, Union
+from typing import Any, Optional, Union
 
 from bluesky.protocols import Status
 from super_state_machine.errors import TransitionError
 
 from blueapi.core import (
     BlueskyContext,
     DataEvent,
@@ -24,44 +25,44 @@
     TaskStatus,
     WorkerEvent,
     WorkerState,
 )
 from .multithread import run_worker_in_own_thread
 from .task import Task
 from .worker import TrackableTask, Worker
-from .worker_busy_error import WorkerBusyError
+from .worker_errors import WorkerAlreadyStartedError, WorkerBusyError
 
 LOGGER = logging.getLogger(__name__)
 
 DEFAULT_START_STOP_TIMEOUT: float = 30.0
 
 
-class RunEngineWorker(Worker[Task]):
+class TaskWorker(Worker[Task]):
     """
     Worker wrapping BlueskyContext that can work in its own thread/process
 
     Args:
         ctx: Context to work with
         stop_timeout: If the worker is told to stop, number of seconds to wait for
             graceful shutdown before raising an exception. Defaults to 30.0.
     """
 
     _ctx: BlueskyContext
     _start_stop_timeout: float
 
-    _pending_tasks: Dict[str, TrackableTask]
+    _tasks: dict[str, TrackableTask]
 
     _state: WorkerState
-    _errors: List[str]
-    _warnings: List[str]
+    _errors: list[str]
+    _warnings: list[str]
     _task_channel: Queue  # type: ignore
     _current: Optional[TrackableTask]
     _status_lock: RLock
-    _status_snapshot: Dict[str, StatusView]
-    _completed_statuses: Set[str]
+    _status_snapshot: dict[str, StatusView]
+    _completed_statuses: set[str]
     _worker_events: EventPublisher[WorkerEvent]
     _progress_events: EventPublisher[ProgressEvent]
     _data_events: EventPublisher[DataEvent]
     _started: Event
     _stopping: Event
     _stopped: Event
 
@@ -70,15 +71,15 @@
         ctx: BlueskyContext,
         start_stop_timeout: float = DEFAULT_START_STOP_TIMEOUT,
         broadcast_statuses: bool = True,
     ) -> None:
         self._ctx = ctx
         self._start_stop_timeout = start_stop_timeout
 
-        self._pending_tasks = {}
+        self._tasks = {}
 
         self._state = WorkerState.from_bluesky_state(ctx.run_engine.state)
         self._errors = []
         self._warnings = []
         self._task_channel = Queue(maxsize=1)
         self._current = None
         self._worker_events = EventPublisher()
@@ -90,15 +91,15 @@
         self._started = Event()
         self._stopping = Event()
         self._stopped = Event()
         self._stopped.set()
         self._broadcast_statuses = broadcast_statuses
 
     def clear_task(self, task_id: str) -> str:
-        task = self._pending_tasks.pop(task_id)
+        task = self._tasks.pop(task_id)
         return task.task_id
 
     def cancel_active_task(
         self,
         failure: bool = False,
         reason: Optional[str] = None,
     ) -> str:
@@ -108,35 +109,35 @@
             raise TransitionError("Attempted to cancel while no active Task")
         if failure:
             self._ctx.run_engine.abort(reason)
         else:
             self._ctx.run_engine.stop()
         return self._current.task_id
 
-    def get_pending_tasks(self) -> List[TrackableTask[Task]]:
-        return list(self._pending_tasks.values())
+    def get_tasks(self) -> list[TrackableTask[Task]]:
+        return list(self._tasks.values())
 
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask[Task]]:
-        return self._pending_tasks.get(task_id)
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask[Task]]:
+        return self._tasks.get(task_id)
 
     def get_active_task(self) -> Optional[TrackableTask[Task]]:
         return self._current
 
     def begin_task(self, task_id: str) -> None:
-        task = self._pending_tasks.get(task_id)
+        task = self._tasks.get(task_id)
         if task is not None:
             self._submit_trackable_task(task)
         else:
             raise KeyError(f"No pending task with ID {task_id}")
 
     def submit_task(self, task: Task) -> str:
         task.prepare_params(self._ctx)  # Will raise if parameters are invalid
         task_id: str = str(uuid.uuid4())
         trackable_task = TrackableTask(task_id=task_id, task=task)
-        self._pending_tasks[task_id] = trackable_task
+        self._tasks[task_id] = trackable_task
         return task_id
 
     def _submit_trackable_task(self, trackable_task: TrackableTask) -> None:
         if self.state is not WorkerState.IDLE:
             raise WorkerBusyError(f"Worker is in state {self.state}")
 
         task_started = Event()
@@ -151,23 +152,23 @@
         LOGGER.info(f"Submitting: {trackable_task}")
         try:
             sub = self.worker_events.subscribe(mark_task_as_started)
             self._task_channel.put_nowait(trackable_task)
             task_started.wait(timeout=5.0)
             if not task_started.is_set():
                 raise TimeoutError("Failed to start plan within timeout")
-        except Full:
+        except Full as f:
             LOGGER.error("Cannot submit task while another is running")
-            raise WorkerBusyError("Cannot submit task while another is running")
+            raise WorkerBusyError("Cannot submit task while another is running") from f
         finally:
             self.worker_events.unsubscribe(sub)
 
     def start(self) -> None:
         if self._started.is_set():
-            raise Exception("Worker is already running")
+            raise WorkerAlreadyStartedError("Worker is already running")
         self._wait_until_stopped()
         run_worker_in_own_thread(self)
         self._wait_until_started()
 
     def stop(self) -> None:
         LOGGER.info("Attempting to stop worker")
```

### Comparing `blueapi-0.4.0/src/blueapi/worker/task.py` & `blueapi-0.4.1a1/src/blueapi/worker/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Any, Mapping
+from collections.abc import Mapping
+from typing import Any
 
 from pydantic import BaseModel, Field
 
 from blueapi.core import BlueskyContext
 from blueapi.utils import BlueapiBaseModel
 
 LOGGER = logging.getLogger(__name__)
@@ -28,24 +29,14 @@
         func = ctx.plan_functions[self.name]
         prepared_params = self.prepare_params(ctx)
         plan_generator = func(**prepared_params.dict())
         wrapped_plan_generator = ctx.wrap(plan_generator)
         ctx.run_engine(wrapped_plan_generator)
 
 
-# Here for backward compatibility pending
-# https://github.com/DiamondLightSource/blueapi/issues/253
-class RunPlan(Task):
-    """
-    Task that will run a plan
-    """
-
-    ...
-
-
 def _lookup_params(ctx: BlueskyContext, task: Task) -> BaseModel:
     """
     Checks plan parameters against context
 
     Args:
         ctx: Context holding plans and devices
         plan: Plan object including schema
```

### Comparing `blueapi-0.4.0/src/blueapi/worker/worker.py` & `blueapi-0.4.1a1/src/blueapi/worker/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Generic, List, Optional, TypeVar
+from typing import Generic, Optional, TypeVar
 
 from pydantic import Field
 
 from blueapi.core import DataEvent, EventStream
 from blueapi.utils import BlueapiBaseModel
 
 from .event import ProgressEvent, WorkerEvent, WorkerState
@@ -16,35 +16,35 @@
     A representation of a task that the worker recognizes
     """
 
     task_id: str
     task: T
     is_complete: bool = False
     is_pending: bool = True
-    errors: List[str] = Field(default_factory=list)
+    errors: list[str] = Field(default_factory=list)
 
 
 class Worker(ABC, Generic[T]):
     """
     Entity that takes and runs tasks. Intended to be a central,
     atomic worker rather than a load distributor
     """
 
     @abstractmethod
-    def get_pending_tasks(self) -> List[TrackableTask[T]]:
+    def get_tasks(self) -> list[TrackableTask[T]]:
         """
-        Return a list of all tasks pending on the worker,
+        Return a list of all tasks on the worker,
         any one of which can be triggered with begin_task.
 
         Returns:
             List[TrackableTask[T]]: List of task objects
         """
 
     @abstractmethod
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask[T]]:
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask[T]]:
         """
         Returns a task matching the task ID supplied,
         if the worker knows of it.
 
         Args:
             task_id: The ID of the task
 
@@ -61,15 +61,15 @@
             Optional[TrackableTask[T]]: The current task,
                 None if the worker is idle.
         """
 
     @abstractmethod
     def clear_task(self, task_id: str) -> str:
         """
-        Remove a pending task from the worker
+        Remove a task from the worker
 
         Args:
             task_id: The ID of the task to be removed
         Returns:
             task_id of the removed task
         """
```

### Comparing `blueapi-0.4.0/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.4.1a1/src/blueapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.0
-Summary: Lightweight Bluesky-as-a-service wrapper application. Also usable as a library.
+Version: 0.4.1a1
+Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,15 +208,15 @@
 Project-URL: GitHub, https://github.com/DiamondLightSource/blueapi
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bluesky
 Requires-Dist: ophyd
 Requires-Dist: nslsii
 Requires-Dist: pyepics
 Requires-Dist: aioca
 Requires-Dist: pydantic<2.0
@@ -225,96 +225,72 @@
 Requires-Dist: PyYAML
 Requires-Dist: click<8.1.4
 Requires-Dist: fastapi[all]<0.99
 Requires-Dist: uvicorn
 Requires-Dist: requests
 Requires-Dist: dls-bluesky-core
 Requires-Dist: dls-dodal
-Requires-Dist: typing_extensions<4.6
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: flake8-isort; extra == "dev"
-Requires-Dist: Flake8-pyproject; extra == "dev"
+Requires-Dist: copier; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinxcontrib-openapi; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-urllib3; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 
-blueapi
-===========================
-
-|code_ci| |docs_ci| |coverage| |pypi_version| |license|
-
-Lightweight bluesky-as-a-service wrapper application. Also usable as a library. 
+[![CI](https://github.com/DiamondLightSource/blueapi/actions/workflows/ci.yml/badge.svg)](https://github.com/DiamondLightSource/blueapi/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/DiamondLightSource/blueapi/branch/main/graph/badge.svg)](https://codecov.io/gh/DiamondLightSource/blueapi)
+[![PyPI](https://img.shields.io/pypi/v/blueapi.svg)](https://pypi.org/project/blueapi)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# blueapi
+
+Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
+
+Source          | <https://github.com/DiamondLightSource/blueapi>
+:---:           | :---:
+PyPI            | `pip install blueapi`
+Docker          | `docker run ghcr.io/diamondlightsource/blueapi:latest`
+Documentation   | <https://diamondlightsource.github.io/blueapi>
+Releases        | <https://github.com/DiamondLightSource/blueapi/releases>
+
+This module wraps [bluesky](https://blueskyproject.io/bluesky) plans and devices
+inside a server and exposes endpoints to send commands/receive data. Useful for
+installation at labs where multiple people may control equipment, possibly from
+remote locations.
 
-============== ==============================================================
-PyPI           ``pip install blueapi``
-Source code    https://github.com/DiamondLightSource/blueapi
-Documentation  https://DiamondLightSource.github.io/blueapi
-Releases       https://github.com/DiamondLightSource/blueapi/releases
-============== ==============================================================
-
-This module wraps bluesky_ plans and devices inside a server and exposes endpoints to send commands/receive data.
-Useful for installation at labs where multiple people may control equipment, 
-possibly from remote locations.
-
-|concept|
+![concept][]
 
 The main premise of blueapi is to minimize the boilerplate required to get plans
-and devices up and running by generating an API for your lab out of type-annotated 
-plans. For example, take the following plan:
-
-.. code:: python
+and devices up and running by generating an API for your lab out of
+type-annotated plans. For example, take the following plan:
 
+```python
     import bluesky.plans as bp
     from blueapi.core import MsgGenerator
 
     def my_plan(foo: str, bar: int) -> MsgGenerator:
         yield from bp.scan(...)
+```
 
-Blueapi's job is to detect this plan and automatically add it to the lab's API so it
-can be invoked easily with a few REST calls. 
-
-.. _bluesky: https://blueskyproject.io/bluesky
-
-.. |code_ci| image:: https://github.com/DiamondLightSource/blueapi/actions/workflows/code.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/blueapi/actions/workflows/code.yml
-    :alt: Code CI
-
-.. |docs_ci| image:: https://github.com/DiamondLightSource/blueapi/actions/workflows/docs.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/blueapi/actions/workflows/docs.yml
-    :alt: Docs CI
-
-.. |coverage| image:: https://codecov.io/gh/DiamondLightSource/blueapi/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/DiamondLightSource/blueapi
-    :alt: Test Coverage
-
-.. |pypi_version| image:: https://img.shields.io/pypi/v/blueapi.svg
-    :target: https://pypi.org/project/blueapi
-    :alt: Latest PyPI version
-
-.. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: Apache License
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Blueapi's job is to detect this plan and automatically add it to the lab's API
+so it can be invoked easily with a few REST calls. 
 
+<!-- README only content. Anything below this line won't be included in index.md -->
 
-.. |concept| image:: docs/images/blueapi.png
-    :width: 800px
+See https://diamondlightsource.github.io/blueapi for more detailed documentation.
 
-See https://DiamondLightSource.github.io/blueapi for more detailed documentation.
+[concept]: https://raw.githubusercontent.com/DiamondLightSource/blueapi/main/docs/images/blueapi.png
```

### Comparing `blueapi-0.4.0/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.4.1a1/src/blueapi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,81 @@
+.copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
+Dockerfile
 LICENSE
-README.rst
+README.md
 catalog-info.yaml
 codecov.yml
+container-startup.sh
 pyproject.toml
-.devcontainer/Dockerfile
-.devcontainer/container-startup.sh
 .devcontainer/devcontainer.json
-.github/CONTRIBUTING.rst
+.github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
+.github/workflows/_check.yml
+.github/workflows/_container.yml
+.github/workflows/_dist.yml
+.github/workflows/_docs.yml
+.github/workflows/_pypi.yml
+.github/workflows/_release.yml
+.github/workflows/_test.yml
+.github/workflows/_tox.yml
 .github/workflows/asyncapi.yml
 .github/workflows/backstage.yml
-.github/workflows/code.yml
-.github/workflows/docs.yml
-.github/workflows/docs_clean.yml
+.github/workflows/ci.yml
 .github/workflows/helm.yml
-.github/workflows/linkcheck.yml
+.github/workflows/periodic.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 config/adsim.yaml
 config/bl38p.yaml
 config/bl45p.yaml
 config/defaults.yaml
 docs/conf.py
-docs/genindex.rst
-docs/index.rst
-docs/developer/index.rst
-docs/developer/explanations/architecture.rst
-docs/developer/explanations/decisions.rst
-docs/developer/explanations/events.rst
-docs/developer/explanations/lifecycle.rst
-docs/developer/explanations/type_validators.rst
-docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
-docs/developer/explanations/decisions/0002-no-queues.rst
-docs/developer/explanations/decisions/0003-api-case.rst
-docs/developer/how-to/build-docs.rst
-docs/developer/how-to/contribute.rst
-docs/developer/how-to/lint.rst
-docs/developer/how-to/make-release.rst
-docs/developer/how-to/run-tests.rst
-docs/developer/how-to/static-analysis.rst
-docs/developer/how-to/update-tools.rst
-docs/developer/reference/standards.rst
-docs/developer/tutorials/dev-install.rst
-docs/developer/tutorials/dev-run.rst
+docs/explanations.md
+docs/genindex.md
+docs/how-to.md
+docs/index.md
+docs/reference.md
+docs/tutorials.md
+docs/explanations/architecture.rst
+docs/explanations/decisions.md
+docs/explanations/events.rst
+docs/explanations/lifecycle.rst
+docs/explanations/type_validators.rst
+docs/explanations/decisions/0001-record-architecture-decisions.rst
+docs/explanations/decisions/0002-no-queues.rst
+docs/explanations/decisions/0003-api-case.rst
+docs/explanations/decisions/0004-switched-to-python-copier-template.md
+docs/explanations/decisions/COPYME
+docs/how-to/add-plans-and-devices.rst
+docs/how-to/configure-app.rst
+docs/how-to/contribute.md
+docs/how-to/run-cli.rst
+docs/how-to/run-container.rst
+docs/how-to/write-plans.rst
 docs/images/blueapi-architecture.png
 docs/images/blueapi-logo.svg
 docs/images/blueapi.png
 docs/images/bluesky-events.png
 docs/images/debug-vscode.png
-docs/user/index.rst
-docs/user/explanations/docs-structure.rst
-docs/user/how-to/add-plans-and-devices.rst
-docs/user/how-to/configure-app.rst
-docs/user/how-to/run-cli.rst
-docs/user/how-to/run-container.rst
-docs/user/reference/api.rst
-docs/user/reference/asyncapi.yaml
-docs/user/reference/cli.rst
-docs/user/reference/messaging-spec.rst
-docs/user/reference/openapi.yaml
-docs/user/reference/rest-spec.rst
-docs/user/tutorials/installation.rst
-docs/user/tutorials/quickstart.rst
+docs/reference/api.md
+docs/reference/asyncapi.yaml
+docs/reference/cli.rst
+docs/reference/messaging-spec.rst
+docs/reference/openapi.yaml
+docs/reference/rest-spec.rst
+docs/tutorials/dev-run.rst
+docs/tutorials/installation.md
+docs/tutorials/quickstart.rst
 helm/blueapi/.helmignore
 helm/blueapi/Chart.yaml
 helm/blueapi/values.yaml
 helm/blueapi/templates/NOTES.txt
 helm/blueapi/templates/_helpers.tpl
 helm/blueapi/templates/configmap.yaml
 helm/blueapi/templates/deployment.yaml
@@ -130,15 +133,15 @@
 src/blueapi/utils/thread_exception.py
 src/blueapi/worker/__init__.py
 src/blueapi/worker/event.py
 src/blueapi/worker/multithread.py
 src/blueapi/worker/reworker.py
 src/blueapi/worker/task.py
 src/blueapi/worker/worker.py
-src/blueapi/worker/worker_busy_error.py
+src/blueapi/worker/worker_errors.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_config.py
 tests/core/__init__.py
 tests/core/fake_device_module.py
 tests/core/fake_plan_module.py
@@ -160,10 +163,11 @@
 tests/service/test_rest_api.py
 tests/service/test_subprocess_handler.py
 tests/utils/__init__.py
 tests/utils/hasall.py
 tests/utils/lacksall.py
 tests/utils/test_base_model.py
 tests/utils/test_modules.py
+tests/utils/test_ophyd_async_connect.py
 tests/utils/test_thread_exception.py
 tests/worker/devices.py
 tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.0/tests/conftest.py` & `blueapi-0.4.1a1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 
 # Based on https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option  # noqa: E501
-from typing import Iterator
+from collections.abc import Iterator
 from unittest.mock import MagicMock
 
 import pytest
 from bluesky import RunEngine
 from bluesky.run_engine import RunEngineStateMachine, TransitionError
 from fastapi.testclient import TestClient
 
+from blueapi.core import BlueskyContext
 from blueapi.service.handler import Handler
 from blueapi.service.main import app, get_handler
-from src.blueapi.core import BlueskyContext
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--skip-stomp",
         action="store_true",
         default=False,
@@ -65,15 +65,15 @@
     request.addfinalizer(clean_event_loop)
     return RE
 
 
 @pytest.fixture
 def handler(RE: RunEngine) -> Iterator[Handler]:
     context: BlueskyContext = BlueskyContext(run_engine=MagicMock())
-    context.run_engine.state = RunEngineStateMachine.States.IDLE
+    context.run_engine.state = RunEngineStateMachine.States.IDLE  # type: ignore
     handler = Handler(context=context, messaging_template=MagicMock())
 
     yield handler
     handler.stop()
 
 
 @pytest.fixture
```

### Comparing `blueapi-0.4.0/tests/core/fake_device_module.py` & `blueapi-0.4.1a1/tests/core/fake_device_module.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/tests/core/test_context.py` & `blueapi-0.4.1a1/tests/core/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from typing import Dict, List, Type, Union
 from unittest.mock import patch
 
 import pytest
 from bluesky.protocols import Descriptor, Movable, Readable, Reading, SyncOrAsync
 from dls_bluesky_core.core import MsgGenerator, PlanGenerator, inject
 from ophyd.sim import SynAxis, SynGauss
 from pydantic import ValidationError, parse_obj_as
@@ -47,16 +46,19 @@
     ...
 
 
 def has_default_reference(m: Movable = inject(SIM_MOTOR_NAME)) -> MsgGenerator:
     yield from []
 
 
+MOVABLE_DEFAULT = [inject(SIM_MOTOR_NAME)]
+
+
 def has_default_nested_reference(
-    m: list[Movable] = [inject(SIM_MOTOR_NAME)],
+    m: list[Movable] = MOVABLE_DEFAULT,
 ) -> MsgGenerator:
     yield from []
 
 
 #
 # Dummy devices
 #
@@ -94,20 +96,20 @@
     ctx = BlueskyContext()
     ctx.device(sim_motor)
     ctx.device(sim_detector)
     return ctx
 
 
 class SomeConfigurable:
-    def read_configuration(self) -> SyncOrAsync[Dict[str, Reading]]:  # type: ignore
+    def read_configuration(self) -> SyncOrAsync[dict[str, Reading]]:  # type: ignore
         ...
 
     def describe_configuration(  # type: ignore
         self,
-    ) -> SyncOrAsync[Dict[str, Descriptor]]: ...
+    ) -> SyncOrAsync[dict[str, Descriptor]]: ...
 
 
 @pytest.fixture
 def some_configurable() -> SomeConfigurable:
     return SomeConfigurable()
 
 
@@ -188,17 +190,15 @@
             device_module, some_argument=1, another_argument="two"
         )
 
 
 @pytest.mark.parametrize(
     "addr", ["sim", "sim_det", "sim.setpoint", ["sim"], ["sim", "setpoint"]]
 )
-def test_lookup_device(
-    devicey_context: BlueskyContext, addr: Union[str, List[str]]
-) -> None:
+def test_lookup_device(devicey_context: BlueskyContext, addr: str | list[str]) -> None:
     device = devicey_context.find_device(addr)
     assert is_bluesky_compatible_device(device)
 
 
 def test_lookup_nonexistant_device(devicey_context: BlueskyContext) -> None:
     assert devicey_context.find_device("foo") is None
 
@@ -262,15 +262,15 @@
 
 def test_device_reference_cache(empty_context: BlueskyContext) -> None:
     assert empty_context._reference(Movable) is empty_context._reference(Movable)
     assert empty_context._reference(Movable) is not empty_context._reference(Readable)
 
 
 def test_reference_type_conversion(empty_context: BlueskyContext) -> None:
-    movable_ref: Type = empty_context._reference(Movable)
+    movable_ref: type = empty_context._reference(Movable)
     assert empty_context._convert_type(Movable) == movable_ref
     assert (
         empty_context._convert_type(dict[Movable, list[tuple[int, Movable]]])
         == dict[movable_ref, list[tuple[int, movable_ref]]]  # type: ignore
     )
```

### Comparing `blueapi-0.4.0/tests/core/test_event.py` & `blueapi-0.4.1a1/tests/core/test_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from collections.abc import Iterable
 from concurrent.futures import Future
 from dataclasses import dataclass
 from queue import Queue
-from typing import Iterable
 
 import pytest
 
 from blueapi.core import EventPublisher
 
 _TIMEOUT: float = 10.0
```

### Comparing `blueapi-0.4.0/tests/data_management/test_visit_directory_provider.py` & `blueapi-0.4.1a1/tests/data_management/test_visit_directory_provider.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/tests/messaging/test_stomptemplate.py` & `blueapi-0.4.1a1/tests/messaging/test_stomptemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import itertools
+from collections.abc import Iterable
 from concurrent.futures import Future
 from queue import Queue
-from typing import Any, Iterable, List, Type
+from typing import Any
+from unittest.mock import ANY, MagicMock, patch
 
 import pytest
-from mock import ANY, MagicMock, patch
 from pydantic import BaseModel, BaseSettings, Field
 from stomp import Connection
 from stomp.exception import ConnectFailedException
 
 from blueapi.config import StompConfig
 from blueapi.messaging import MessageContext, MessagingTemplate, StompMessagingTemplate
 
 _TIMEOUT: float = 10.0
 _COUNT = itertools.count()
 
 
 class StompTestingSettings(BaseSettings):
-    blueapi_test_stomp_ports: List[int] = Field(default=[61613])
+    blueapi_test_stomp_ports: list[int] = Field(default=[61613])
 
     def test_stomp_configs(self) -> Iterable[StompConfig]:
         for port in self.blueapi_test_stomp_ports:
             yield StompConfig(port=port)
 
 
 @pytest.fixture(params=StompTestingSettings().test_stomp_configs())
@@ -118,15 +119,15 @@
 
 @pytest.mark.stomp
 @pytest.mark.parametrize(
     "message,message_type",
     [("test", str), (1, int), (Foo(a=1, b="test"), Foo)],
 )
 def test_deserialization(
-    template: MessagingTemplate, test_queue: str, message: Any, message_type: Type
+    template: MessagingTemplate, test_queue: str, message: Any, message_type: type
 ) -> None:
     def server(ctx: MessageContext, message: message_type) -> None:  # type: ignore
         reply_queue = ctx.reply_destination
         if reply_queue is None:
             raise RuntimeError("reply queue is None")
         template.send(reply_queue, message, correlation_id=ctx.correlation_id)
```

### Comparing `blueapi-0.4.0/tests/messaging/test_utils.py` & `blueapi-0.4.1a1/tests/messaging/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import Any, Mapping
+from typing import Any
 
 import pytest
 
 from blueapi.messaging.utils import determine_deserialization_type
 
 
 @dataclass
```

### Comparing `blueapi-0.4.0/tests/preprocessors/test_attach_metadata.py` & `blueapi-0.4.1a1/tests/preprocessors/test_attach_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Mapping
+from typing import Any, Callable
 
 import bluesky.plan_stubs as bps
 import bluesky.plans as bp
 import pytest
 from bluesky import RunEngine
 from bluesky.preprocessors import (
     run_decorator,
@@ -88,23 +89,23 @@
         self,
         name: str,
         provider: DirectoryProvider,
     ) -> None:
         self._name = name
         self._provider = provider
 
-    async def read(self) -> Dict[str, Reading]:
+    async def read(self) -> dict[str, Reading]:
         return {
             f"{self.name}_data": {
                 "value": "test",
                 "timestamp": 0.0,
             },
         }
 
-    async def describe(self) -> Dict[str, DataKey]:
+    async def describe(self) -> dict[str, DataKey]:
         directory_info = self._provider()
         path = f"{directory_info.directory_path}/{directory_info.filename_prefix}"
         return {
             f"{self.name}_data": {
                 "dtype": "string",
                 "shape": [1],
                 "source": path,
@@ -122,52 +123,52 @@
 
     @property
     def parent(self) -> None:
         return None
 
 
 @pytest.fixture(params=[1, 2])
-def detectors(request, provider: VisitDirectoryProvider) -> List[Readable]:
+def detectors(request, provider: VisitDirectoryProvider) -> list[Readable]:
     number_of_detectors = request.param
     return [
         FakeDetector(
             name=f"test_detector_{i}",
             provider=provider,
         )
         for i in range(number_of_detectors)
     ]
 
 
-def simple_run(detectors: List[Readable]) -> MsgGenerator:
+def simple_run(detectors: list[Readable]) -> MsgGenerator:
     yield from bp.count(detectors)
 
 
-def multi_run(detectors: List[Readable]) -> MsgGenerator:
+def multi_run(detectors: list[Readable]) -> MsgGenerator:
     yield from bp.count(detectors)
     yield from bp.count(detectors)
 
 
-def multi_nested_plan(detectors: List[Readable]) -> MsgGenerator:
+def multi_nested_plan(detectors: list[Readable]) -> MsgGenerator:
     yield from simple_run(detectors)
     yield from simple_run(detectors)
 
 
-def multi_run_single_stage(detectors: List[Readable]) -> MsgGenerator:
+def multi_run_single_stage(detectors: list[Readable]) -> MsgGenerator:
     def stageless_count() -> MsgGenerator:
         return (yield from bps.one_shot(detectors))
 
     def inner_plan() -> MsgGenerator:
         yield from run_wrapper(stageless_count())
         yield from run_wrapper(stageless_count())
 
     yield from stage_wrapper(inner_plan(), detectors)
 
 
 def multi_run_single_stage_multi_group(
-    detectors: List[Readable],
+    detectors: list[Readable],
 ) -> MsgGenerator:
     def stageless_count() -> MsgGenerator:
         return (yield from bps.one_shot(detectors))
 
     def inner_plan() -> MsgGenerator:
         yield from run_wrapper(stageless_count(), md={DATA_SESSION: 1})
         yield from run_wrapper(stageless_count(), md={DATA_SESSION: 1})
@@ -175,31 +176,31 @@
         yield from run_wrapper(stageless_count(), md={DATA_SESSION: 2})
 
     yield from stage_wrapper(inner_plan(), detectors)
 
 
 @run_decorator(md={DATA_SESSION: 12345})
 @set_run_key_decorator("outer")
-def nested_run_with_metadata(detectors: List[Readable]) -> MsgGenerator:
+def nested_run_with_metadata(detectors: list[Readable]) -> MsgGenerator:
     yield from set_run_key_wrapper(bp.count(detectors), "inner")
     yield from set_run_key_wrapper(bp.count(detectors), "inner")
 
 
 @run_decorator()
 @set_run_key_decorator("outer")
 def nested_run_without_metadata(
-    detectors: List[Readable],
+    detectors: list[Readable],
 ) -> MsgGenerator:
     yield from set_run_key_wrapper(bp.count(detectors), "inner")
     yield from set_run_key_wrapper(bp.count(detectors), "inner")
 
 
 def test_simple_run_gets_scan_number(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
 ) -> None:
     docs = collect_docs(
         run_engine,
         simple_run(detectors),
         provider,
     )
@@ -207,16 +208,16 @@
     assert docs[0].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert_all_detectors_used_collection_numbers(docs, detectors, [RUN_0])
 
 
 @pytest.mark.parametrize("plan", [multi_run, multi_nested_plan])
 def test_multi_run_gets_scan_numbers(
     run_engine: RunEngine,
-    detectors: List[Readable],
-    plan: Callable[[List[Readable]], MsgGenerator],
+    detectors: list[Readable],
+    plan: Callable[[list[Readable]], MsgGenerator],
     provider: DirectoryProvider,
 ) -> None:
     """Test is here to demonstrate that multi run plans will overwrite files."""
     docs = collect_docs(
         run_engine,
         plan(detectors),
         provider,
@@ -226,15 +227,15 @@
     assert start_docs[0].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert start_docs[1].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert_all_detectors_used_collection_numbers(docs, detectors, [RUN_0, RUN_0])
 
 
 def test_multi_run_single_stage(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
 ) -> None:
     docs = collect_docs(
         run_engine,
         multi_run_single_stage(detectors),
         provider,
     )
@@ -250,15 +251,15 @@
             RUN_0,
         ],
     )
 
 
 def test_multi_run_single_stage_multi_group(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
 ) -> None:
     docs = collect_docs(
         run_engine,
         multi_run_single_stage_multi_group(detectors),
         provider,
     )
@@ -278,15 +279,15 @@
             RUN_0,
         ],
     )
 
 
 def test_nested_run_with_metadata(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
 ) -> None:
     """Test is here to demonstrate that nested runs will be treated as a single run.
 
     That means detectors in such runs will overwrite files.
     """
     docs = collect_docs(
@@ -300,15 +301,15 @@
     assert start_docs[1].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert start_docs[2].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert_all_detectors_used_collection_numbers(docs, detectors, [RUN_0, RUN_0])
 
 
 def test_nested_run_without_metadata(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
 ) -> None:
     """Test is here to demonstrate that nested runs will be treated as a single run.
 
     That means detectors in such runs will overwrite files.
     """
     docs = collect_docs(
@@ -322,30 +323,30 @@
     assert start_docs[1].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert start_docs[2].doc[DATA_SESSION] == f"{DATA_GROUP_NAME}-0"
     assert_all_detectors_used_collection_numbers(docs, detectors, [RUN_0, RUN_0])
 
 
 def test_visit_directory_provider_fails(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
     client: MockVisitServiceClient,
 ) -> None:
     client.always_fail()
     with pytest.raises(ValueError):
         collect_docs(
             run_engine,
             simple_run(detectors),
             provider,
         )
 
 
 def test_visit_directory_provider_fails_after_one_sucess(
     run_engine: RunEngine,
-    detectors: List[Readable],
+    detectors: list[Readable],
     provider: DirectoryProvider,
     client: MockVisitServiceClient,
 ) -> None:
     collect_docs(
         run_engine,
         simple_run(detectors),
         provider,
@@ -359,40 +360,40 @@
         )
 
 
 def collect_docs(
     run_engine: RunEngine,
     plan: MsgGenerator,
     provider: DirectoryProvider,
-) -> List[DataEvent]:
+) -> list[DataEvent]:
     events = []
 
     def on_event(name: str, doc: Mapping[str, Any]) -> None:
         events.append(DataEvent(name=name, doc=doc))
 
     wrapped_plan = attach_metadata(plan, provider)
     run_engine(wrapped_plan, on_event)
     return events
 
 
 def assert_all_detectors_used_collection_numbers(
-    docs: List[DataEvent],
-    detectors: List[Readable],
-    source_history: List[Path],
+    docs: list[DataEvent],
+    detectors: list[Readable],
+    source_history: list[Path],
 ) -> None:
     descriptors = find_descriptor_docs(docs)
     assert len(descriptors) == len(source_history)
 
     for descriptor, expected_source in zip(descriptors, source_history):
         for detector in detectors:
             source = descriptor.doc.get("data_keys", {}).get(f"{detector.name}_data")[
                 "source"
             ]
             assert Path(source) == expected_source
 
 
-def find_start_docs(docs: List[DataEvent]) -> List[DataEvent]:
+def find_start_docs(docs: list[DataEvent]) -> list[DataEvent]:
     return list(filter(lambda event: event.name == "start", docs))
 
 
-def find_descriptor_docs(docs: List[DataEvent]) -> List[DataEvent]:
+def find_descriptor_docs(docs: list[DataEvent]) -> list[DataEvent]:
     return list(filter(lambda event: event.name == "descriptor", docs))
```

### Comparing `blueapi-0.4.0/tests/service/test_handler.py` & `blueapi-0.4.1a1/tests/service/test_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from unittest.mock import Mock, patch
+
 import pytest
-from mock import Mock, patch
 
 from blueapi.service.handler import (
     Handler,
     get_handler,
     setup_handler,
     teardown_handler,
 )
```

### Comparing `blueapi-0.4.0/tests/service/test_openapi.py` & `blueapi-0.4.1a1/tests/service/test_openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import mock
+from unittest import mock
+from unittest.mock import Mock, PropertyMock
+
 import pytest
 import yaml
-from mock import Mock, PropertyMock
 
 from blueapi.service.openapi import DOCS_SCHEMA_LOCATION, generate_schema
 
 
 @mock.patch("blueapi.service.openapi.app")
 def test_generate_schema(mock_app: Mock) -> None:
     from blueapi.service.main import app
```

### Comparing `blueapi-0.4.0/tests/service/test_rest_api.py` & `blueapi-0.4.1a1/tests/service/test_rest_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from fastapi.testclient import TestClient
 from pydantic import BaseModel
 
 from blueapi.core.bluesky_types import Plan
 from blueapi.service.handler import Handler
 from blueapi.service.main import get_handler, setup_handler, teardown_handler
 from blueapi.service.model import WorkerTask
-from blueapi.worker.task import RunPlan
-from src.blueapi.worker import WorkerState
+from blueapi.worker import WorkerState
+from blueapi.worker.task import Task
 
-_TASK = RunPlan(name="count", params={"detectors": ["x"]})
+_TASK = Task(name="count", params={"detectors": ["x"]})
 
 
 def test_get_plans(handler: Handler, client: TestClient) -> None:
     class MyModel(BaseModel):
         id: str
 
     plan = Plan(name="my-plan", model=MyModel)
@@ -199,17 +199,17 @@
     assert response.json() == {"detail": "Item not found"}
 
 
 def test_create_task(handler: Handler, client: TestClient) -> None:
     response = client.post("/tasks", json=_TASK.dict())
     task_id = response.json()["task_id"]
 
-    pending = handler.get_pending_task(task_id)
-    assert pending is not None
-    assert pending.task == _TASK
+    t = handler.get_task_by_id(task_id)
+    assert t is not None
+    assert t.task == _TASK
 
 
 def test_put_plan_begins_task(handler: Handler, client: TestClient) -> None:
     handler.start()
     response = client.post("/tasks", json=_TASK.dict())
     task_id = response.json()["task_id"]
 
@@ -252,15 +252,15 @@
 ) -> None:
     task_name = "foo"
     task_params = {"detectors": ["x"]}
     task_json = {"name": task_name, "params": task_params}
 
     response = client.post("/tasks", json=task_json)
 
-    assert not handler.pending_tasks
+    assert not handler.tasks
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 def test_get_plan_returns_posted_plan(handler: Handler, client: TestClient) -> None:
     handler.start()
     post_response = client.post("/tasks", json=_TASK.dict())
     task_id = post_response.json()["task_id"]
@@ -281,15 +281,15 @@
 def test_put_plan_with_bad_params_fails(handler: Handler, client: TestClient) -> None:
     task_name = "count"
     task_params = {"motors": ["x"]}
     task_json = {"name": task_name, "params": task_params}
 
     response = client.post("/tasks", json=task_json)
 
-    assert not handler.pending_tasks
+    assert not handler.tasks
     assert response.status_code == status.HTTP_422_UNPROCESSABLE_ENTITY
 
 
 def test_get_state_updates(handler: Handler, client: TestClient) -> None:
     assert client.get("/worker/state").text == f'"{WorkerState.IDLE.name}"'
     handler._worker._on_state_change(  # type: ignore
         RunEngineStateMachine.States.RUNNING
@@ -387,46 +387,46 @@
     assert client.get("/worker/state").text == f'"{WorkerState.RUNNING.name}"'
 
 
 def test_clear_pending_task_no_longer_pending(handler: Handler, client: TestClient):
     response = client.post("/tasks", json=_TASK.dict())
     task_id = response.json()["task_id"]
 
-    pending = handler.get_pending_task(task_id)
-    assert pending is not None
-    assert pending.task == _TASK
+    t = handler.get_task_by_id(task_id)
+    assert t is not None
+    assert t.task == _TASK
 
     delete_response = client.delete(f"/tasks/{task_id}")
     assert delete_response.status_code is status.HTTP_200_OK
-    assert not handler.pending_tasks
-    assert handler.get_pending_task(task_id) is None
+    assert not handler.tasks
+    assert handler.get_task_by_id(task_id) is None
 
 
 def test_clear_not_pending_task_not_found(handler: Handler, client: TestClient):
     response = client.post("/tasks", json=_TASK.dict())
     task_id = response.json()["task_id"]
 
-    pending = handler.get_pending_task(task_id)
+    pending = handler.get_task_by_id(task_id)
     assert pending is not None
     assert pending.task == _TASK
 
     delete_response = client.delete("/tasks/wrong-task-id")
     assert delete_response.status_code is status.HTTP_404_NOT_FOUND
-    pending = handler.get_pending_task(task_id)
+    pending = handler.get_task_by_id(task_id)
     assert pending is not None
     assert pending.task == _TASK
 
 
 def test_clear_when_empty(handler: Handler, client: TestClient):
-    pending = handler.pending_tasks
+    pending = handler.tasks
     assert not pending
 
     delete_response = client.delete("/tasks/wrong-task-id")
     assert delete_response.status_code is status.HTTP_404_NOT_FOUND
-    assert not handler.pending_tasks
+    assert not handler.tasks
 
 
 @pytest.mark.parametrize(
     "worker_state,stops,aborts",
     [(WorkerState.STOPPING, 1, 0), (WorkerState.ABORTING, 0, 1)],
 )
 def test_delete_running_task(
@@ -439,15 +439,15 @@
     stop = mockable_state_machine._context.run_engine.stop = MagicMock()  # type: ignore
     abort = mockable_state_machine._context.run_engine.abort = (  # type: ignore
         MagicMock()
     )
 
     def start_task(_: str):
         mockable_state_machine._worker._current = (  # type: ignore
-            mockable_state_machine._worker.get_pending_task(task_id)
+            mockable_state_machine._worker.get_task_by_id(task_id)
         )
         mockable_state_machine._worker._on_state_change(  # type: ignore
             RunEngineStateMachine.States.RUNNING
         )
 
     mockable_state_machine._worker.begin_task = start_task  # type: ignore
     response = client.post("/tasks", json=_TASK.dict())
@@ -469,15 +469,15 @@
 def test_reason_passed_to_abort(mockable_state_machine: Handler, client: TestClient):
     abort = mockable_state_machine._context.run_engine.abort = (  # type: ignore
         MagicMock()
     )
 
     def start_task(_: str):
         mockable_state_machine._worker._current = (  # type: ignore
-            mockable_state_machine._worker.get_pending_task(task_id)
+            mockable_state_machine._worker.get_task_by_id(task_id)
         )
         mockable_state_machine._worker._on_state_change(  # type: ignore
             RunEngineStateMachine.States.RUNNING
         )
 
     mockable_state_machine._worker.begin_task = start_task  # type: ignore
     response = client.post("/tasks", json=_TASK.dict())
```

### Comparing `blueapi-0.4.0/tests/service/test_subprocess_handler.py` & `blueapi-0.4.1a1/tests/service/test_subprocess_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List, Optional
+from typing import Optional
+from unittest.mock import MagicMock, patch
 
 import pytest
-from mock import MagicMock, patch
 
 from blueapi.service.handler_base import BlueskyHandler, HandlerNotStartedError
 from blueapi.service.model import DeviceModel, PlanModel, WorkerTask
 from blueapi.service.subprocess_handler import SubprocessHandler
 from blueapi.worker.event import WorkerState
-from blueapi.worker.task import RunPlan
+from blueapi.worker.task import Task
 from blueapi.worker.worker import TrackableTask
 
 
 @pytest.fixture(scope="module")
 def sp_handler():
     sp_handler = SubprocessHandler()
     sp_handler.start()
@@ -21,15 +21,15 @@
 
 def test_initialize():
     sp_handler = SubprocessHandler()
     assert not sp_handler.initialized
     sp_handler.start()
     assert sp_handler.initialized
     # Run a single call to the handler for coverage of dispatch to subprocess
-    assert sp_handler.pending_tasks == []
+    assert sp_handler.tasks == []
     sp_handler.stop()
     assert not sp_handler.initialized
 
 
 def test_reload():
     sp_handler = SubprocessHandler()
     sp_handler.start()
@@ -38,39 +38,39 @@
     assert sp_handler.initialized
     sp_handler.stop()
 
 
 def test_raises_if_not_started():
     sp_handler = SubprocessHandler()
     with pytest.raises(HandlerNotStartedError):
-        sp_handler.state
+        assert sp_handler.state is None
 
 
 class DummyHandler(BlueskyHandler):
     @property
-    def plans(self) -> List[PlanModel]:
+    def plans(self) -> list[PlanModel]:
         return [PlanModel(name="plan1"), PlanModel(name="plan2")]
 
     def get_plan(self, name: str) -> PlanModel:
         return PlanModel(name="plan1")
 
     @property
-    def devices(self) -> List[DeviceModel]:
+    def devices(self) -> list[DeviceModel]:
         return [
             DeviceModel(name="device1", protocols=[]),
             DeviceModel(name="device2", protocols=[]),
         ]
 
     def get_device(self, name: str) -> DeviceModel:
         return DeviceModel(name="device1", protocols=[])
 
-    def submit_task(self, task: RunPlan) -> str:
+    def submit_task(self, task: Task) -> str:
         return "0"
 
-    def clear_pending_task(self, task_id: str) -> str:
+    def clear_task(self, task_id: str) -> str:
         return "1"
 
     def begin_task(self, task: WorkerTask) -> WorkerTask:
         return WorkerTask(task_id=task.task_id)
 
     @property
     def active_task(self) -> Optional[TrackableTask]:
@@ -83,22 +83,20 @@
     def pause_worker(self, defer: Optional[bool]) -> None: ...
 
     def resume_worker(self) -> None: ...
 
     def cancel_active_task(self, failure: bool, reason: Optional[str]) -> None: ...
 
     @property
-    def pending_tasks(self) -> List[TrackableTask]:
+    def tasks(self) -> list[TrackableTask]:
         return [
-            TrackableTask(
-                task_id="abc", task=RunPlan(name="sleep", params={"time": 0.0})
-            )
+            TrackableTask(task_id="abc", task=Task(name="sleep", params={"time": 0.0}))
         ]
 
-    def get_pending_task(self, task_id: str) -> Optional[TrackableTask]:
+    def get_task_by_id(self, task_id: str) -> Optional[TrackableTask]:
         return None
 
     def start(self): ...
 
     def stop(self): ...
 
     # Initialized is a special case as it is not delegated
@@ -106,15 +104,14 @@
     @property
     def initialized(self) -> bool:
         raise Exception("Not implemented")
 
 
 @patch("blueapi.service.subprocess_handler.get_handler")
 def test_method_routing(get_handler_mock: MagicMock):
-
     # Mock get_handler to prevent using a real internal handler
     dummy_handler = DummyHandler()
     get_handler_mock.return_value = dummy_handler
 
     # For above to work, prevent use of subprocess
     def run_in_same_process(func, args=None):
         if args is None:
@@ -133,20 +130,18 @@
     assert sp_handler.get_plan("name") == dummy_handler.get_plan("name")
 
     assert sp_handler.devices == dummy_handler.devices
 
     assert sp_handler.get_device("name") == dummy_handler.get_device("name")
 
     assert sp_handler.submit_task(
-        RunPlan(name="sleep", params={"time": 0.0})
-    ) == dummy_handler.submit_task(RunPlan(name="sleep", params={"time": 0.0}))
+        Task(name="sleep", params={"time": 0.0})
+    ) == dummy_handler.submit_task(Task(name="sleep", params={"time": 0.0}))
 
-    assert sp_handler.clear_pending_task("task_id") == dummy_handler.clear_pending_task(
-        "task_id"
-    )
+    assert sp_handler.clear_task("task_id") == dummy_handler.clear_task("task_id")
 
     assert sp_handler.begin_task(WorkerTask(task_id="foo")) == dummy_handler.begin_task(
         WorkerTask(task_id="foo")
     )
 
     assert sp_handler.active_task == dummy_handler.active_task
 
@@ -154,16 +149,16 @@
 
     sp_handler.pause_worker(True)
 
     sp_handler.resume_worker()
 
     sp_handler.cancel_active_task(True, "reason")
 
-    assert sp_handler.pending_tasks == dummy_handler.pending_tasks
+    assert sp_handler.tasks == dummy_handler.tasks
 
-    assert sp_handler.get_pending_task("task_id") == dummy_handler.get_pending_task(
+    assert sp_handler.get_task_by_id("task_id") == dummy_handler.get_task_by_id(
         "task_id"
     )
 
     assert sp_handler.start() == dummy_handler.start()
 
     assert sp_handler.stop() == dummy_handler.stop()
```

### Comparing `blueapi-0.4.0/tests/test_cli.py` & `blueapi-0.4.1a1/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
+from unittest.mock import Mock, patch
 
 import pytest
 from click.testing import CliRunner
 from fastapi.testclient import TestClient
-from mock import Mock, patch
 from pydantic import BaseModel
 from requests.exceptions import ConnectionError
 
 from blueapi import __version__
 from blueapi.cli.cli import main
 from blueapi.core.bluesky_types import Plan
 from blueapi.service.handler import Handler, teardown_handler
@@ -39,16 +39,16 @@
     assert result.stdout == expected
 
 
 def test_main_with_nonexistent_config_file():
     runner = CliRunner()
     result = runner.invoke(main, ["-c", "tests/non_existent.yaml"])
 
-    result.exit_code == 1
-    type(result.exception) is FileNotFoundError
+    assert result.exit_code == 1
+    assert type(result.exception) is FileNotFoundError
 
 
 @patch("requests.request")
 def test_connection_error_caught_by_wrapper_func(mock_requests: Mock):
     mock_requests.side_effect = ConnectionError()
     runner = CliRunner()
     result = runner.invoke(main, ["controller", "plans"])
```

### Comparing `blueapi-0.4.0/tests/test_config.py` & `blueapi-0.4.1a1/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
-from typing import Any, Type
+from typing import Any
+from unittest import mock
 
-import mock
 import pytest
 from pydantic import BaseModel, Field
 
 from blueapi.config import ApplicationConfig, BasicAuthentication, ConfigLoader
 from blueapi.utils import InvalidConfigError
 
 
@@ -52,15 +52,15 @@
 
 @pytest.fixture
 def default_yaml(package_root: Path) -> Path:
     return package_root.parent.parent / "config" / "defaults.yaml"
 
 
 @pytest.mark.parametrize("schema", [ConfigWithDefaults, NestedConfigWithDefaults])
-def test_load_defaults(schema: Type[Any]) -> None:
+def test_load_defaults(schema: type[Any]) -> None:
     loader = ConfigLoader(schema)
     assert loader.load() == schema()
 
 
 def test_load_some_defaults() -> None:
     loader = ConfigLoader(ConfigWithDefaults)
     loader.use_values({"foo": 4})
```

### Comparing `blueapi-0.4.0/tests/utils/test_thread_exception.py` & `blueapi-0.4.1a1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/tests/worker/devices.py` & `blueapi-0.4.1a1/tests/worker/devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.0/tests/worker/test_reworker.py` & `blueapi-0.4.1a1/tests/worker/test_reworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import itertools
 import threading
+from collections.abc import Iterable
 from concurrent.futures import Future
-from typing import Any, Callable, Iterable, List, Optional, TypeVar, Union
+from queue import Full
+from typing import Any, Callable, Optional, TypeVar, Union
+from unittest.mock import MagicMock, patch
 
 import pytest
 
 from blueapi.config import EnvironmentConfig, Source, SourceKind
 from blueapi.core import BlueskyContext, EventStream, MsgGenerator
 from blueapi.core.bluesky_types import DataEvent
 from blueapi.worker import (
     ProgressEvent,
-    RunEngineWorker,
-    RunPlan,
     Task,
     TaskStatus,
+    TaskWorker,
     TrackableTask,
     Worker,
+    WorkerAlreadyStartedError,
     WorkerBusyError,
     WorkerEvent,
     WorkerState,
 )
 
-_SIMPLE_TASK = RunPlan(name="sleep", params={"time": 0.0})
-_LONG_TASK = RunPlan(name="sleep", params={"time": 1.0})
-_INDEFINITE_TASK = RunPlan(
+_SIMPLE_TASK = Task(name="sleep", params={"time": 0.0})
+_LONG_TASK = Task(name="sleep", params={"time": 1.0})
+_INDEFINITE_TASK = Task(
     name="set_absolute",
     params={"movable": "fake_device", "value": 4.0},
 )
-_FAILING_TASK = RunPlan(name="failing_plan", params={})
+_FAILING_TASK = Task(name="failing_plan", params={})
 
 
 class FakeDevice:
     event: threading.Event
 
     @property
     def name(self) -> str:
@@ -65,15 +68,15 @@
     ctx.device(fake_device)
     ctx.with_config(ctx_config)
     return ctx
 
 
 @pytest.fixture
 def inert_worker(context: BlueskyContext) -> Worker[Task]:
-    return RunEngineWorker(context, start_stop_timeout=2.0)
+    return TaskWorker(context, start_stop_timeout=2.0)
 
 
 @pytest.fixture
 def worker(inert_worker: Worker[Task]) -> Iterable[Worker[Task]]:
     inert_worker.start()
     yield inert_worker
     inert_worker.stop()
@@ -99,77 +102,67 @@
     inert_worker.stop()
     inert_worker.start()
     inert_worker.stop()
 
 
 def test_multi_start(inert_worker: Worker) -> None:
     inert_worker.start()
-    with pytest.raises(Exception):
+    with pytest.raises(WorkerAlreadyStartedError):
         inert_worker.start()
     inert_worker.stop()
 
 
 def test_submit_task(worker: Worker) -> None:
-    assert worker.get_pending_tasks() == []
+    assert worker.get_tasks() == []
     task_id = worker.submit_task(_SIMPLE_TASK)
-    assert worker.get_pending_tasks() == [
-        TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
-    ]
+    assert worker.get_tasks() == [TrackableTask(task_id=task_id, task=_SIMPLE_TASK)]
 
 
 def test_submit_multiple_tasks(worker: Worker) -> None:
-    assert worker.get_pending_tasks() == []
+    assert worker.get_tasks() == []
     task_id_1 = worker.submit_task(_SIMPLE_TASK)
-    assert worker.get_pending_tasks() == [
-        TrackableTask(task_id=task_id_1, task=_SIMPLE_TASK)
-    ]
+    assert worker.get_tasks() == [TrackableTask(task_id=task_id_1, task=_SIMPLE_TASK)]
     task_id_2 = worker.submit_task(_LONG_TASK)
-    assert worker.get_pending_tasks() == [
+    assert worker.get_tasks() == [
         TrackableTask(task_id=task_id_1, task=_SIMPLE_TASK),
         TrackableTask(task_id=task_id_2, task=_LONG_TASK),
     ]
 
 
 def test_stop_with_task_pending(inert_worker: Worker) -> None:
     inert_worker.start()
     inert_worker.submit_task(_SIMPLE_TASK)
     inert_worker.stop()
 
 
 def test_restart_leaves_task_pending(worker: Worker) -> None:
     task_id = worker.submit_task(_SIMPLE_TASK)
-    assert worker.get_pending_tasks() == [
-        TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
-    ]
+    assert worker.get_tasks() == [TrackableTask(task_id=task_id, task=_SIMPLE_TASK)]
     worker.stop()
     worker.start()
-    assert worker.get_pending_tasks() == [
-        TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
-    ]
+    assert worker.get_tasks() == [TrackableTask(task_id=task_id, task=_SIMPLE_TASK)]
 
 
 def test_submit_before_start_pending(inert_worker: Worker) -> None:
     task_id = inert_worker.submit_task(_SIMPLE_TASK)
     inert_worker.start()
-    assert inert_worker.get_pending_tasks() == [
+    assert inert_worker.get_tasks() == [
         TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
     ]
     inert_worker.stop()
-    assert inert_worker.get_pending_tasks() == [
+    assert inert_worker.get_tasks() == [
         TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
     ]
 
 
 def test_clear_task(worker: Worker) -> None:
     task_id = worker.submit_task(_SIMPLE_TASK)
-    assert worker.get_pending_tasks() == [
-        TrackableTask(task_id=task_id, task=_SIMPLE_TASK)
-    ]
+    assert worker.get_tasks() == [TrackableTask(task_id=task_id, task=_SIMPLE_TASK)]
     assert worker.clear_task(task_id)
-    assert worker.get_pending_tasks() == []
+    assert worker.get_tasks() == []
 
 
 def test_clear_nonexistant_task(worker: Worker) -> None:
     with pytest.raises(KeyError):
         worker.clear_task("foo")
 
 
@@ -194,15 +187,15 @@
     active_task = worker.get_active_task()
     assert active_task is not None
     assert active_task.task == _SIMPLE_TASK
 
 
 def test_plan_failure_recorded_in_active_task(worker: Worker) -> None:
     task_id = worker.submit_task(_FAILING_TASK)
-    events_future: Future[List[WorkerEvent]] = take_events(
+    events_future: Future[list[WorkerEvent]] = take_events(
         worker.worker_events,
         lambda event: event.task_status is not None and event.task_status.task_failed,
     )
     worker.begin_task(task_id)
     events = events_future.result(timeout=5.0)
     assert events[-1].task_status is not None
     assert events[-1].task_status.task_failed
@@ -218,15 +211,15 @@
     task_ids = [worker.submit_task(_SIMPLE_TASK) for _ in range(num_runs)]
     event_sequences = [_sleep_events(task_id) for task_id in task_ids]
 
     for task_id, events in zip(task_ids, event_sequences):
         assert_run_produces_worker_events(events, worker, task_id)
 
 
-def _sleep_events(task_id: str) -> List[WorkerEvent]:
+def _sleep_events(task_id: str) -> list[WorkerEvent]:
     return [
         WorkerEvent(
             state=WorkerState.RUNNING,
             task_status=TaskStatus(
                 task_id=task_id, task_complete=False, task_failed=False
             ),
             errors=[],
@@ -252,50 +245,59 @@
 
 
 def test_no_additional_progress_events_after_complete(worker: Worker):
     """
     See https://github.com/bluesky/ophyd/issues/1115
     """
 
-    progress_events: List[ProgressEvent] = []
+    progress_events: list[ProgressEvent] = []
     worker.progress_events.subscribe(lambda event, id: progress_events.append(event))
 
-    task: Task = RunPlan(
-        name="move", params={"moves": {"additional_status_device": 5.0}}
-    )
+    task: Task = Task(name="move", params={"moves": {"additional_status_device": 5.0}})
     task_id = worker.submit_task(task)
     begin_task_and_wait_until_complete(worker, task_id)
 
     # Extract all the display_name fields from the events
     list_of_dict_keys = [pe.statuses.values() for pe in progress_events]
     status_views = [item for sublist in list_of_dict_keys for item in sublist]
     display_names = [view.display_name for view in status_views]
 
     assert "STATUS_AFTER_FINISH" not in display_names
 
 
+@patch("queue.Queue.put_nowait")
+def test_full_queue_raises_WorkerBusyError(put_nowait: MagicMock, worker: Worker):
+    def raise_full(item):
+        raise Full()
+
+    put_nowait.side_effect = raise_full
+    task = worker.submit_task(_SIMPLE_TASK)
+    with pytest.raises(WorkerBusyError):
+        worker.begin_task(task)
+
+
 #
 # Worker helpers
 #
 
 
 def assert_run_produces_worker_events(
-    expected_events: List[WorkerEvent],
+    expected_events: list[WorkerEvent],
     worker: Worker,
     task_id: str,
 ) -> None:
     assert begin_task_and_wait_until_complete(worker, task_id) == expected_events
 
 
 def begin_task_and_wait_until_complete(
     worker: Worker,
     task_id: str,
     timeout: float = 5.0,
-) -> List[WorkerEvent]:
-    events: "Future[List[WorkerEvent]]" = take_events(
+) -> list[WorkerEvent]:
+    events: "Future[list[WorkerEvent]]" = take_events(
         worker.worker_events,
         lambda event: event.is_complete(),
     )
 
     worker.begin_task(task_id)
     return events.result(timeout=timeout)
 
@@ -338,26 +340,26 @@
             ),
         ],
         worker,
     )
 
 
 def assert_running_count_plan_produces_ordered_worker_and_data_events(
-    expected_events: List[Union[WorkerEvent, DataEvent]],
+    expected_events: list[Union[WorkerEvent, DataEvent]],
     worker: Worker,
-    task: Task = RunPlan(name="count", params={"detectors": ["image_det"], "num": 1}),
+    task: Task = Task(name="count", params={"detectors": ["image_det"], "num": 1}),  # noqa: B008
     timeout: float = 5.0,
 ) -> None:
-    event_streams: List[EventStream[Any, int]] = [
+    event_streams: list[EventStream[Any, int]] = [
         worker.data_events,
         worker.worker_events,
     ]
 
     count = itertools.count()
-    events: "Future[List[Any]]" = take_events_from_streams(
+    events: "Future[list[Any]]" = take_events_from_streams(
         event_streams,
         lambda _: next(count) >= len(expected_events) - 1,
     )
 
     task_id = worker.submit_task(task)
     worker.begin_task(task_id)
     results = events.result(timeout=timeout)
@@ -374,40 +376,40 @@
 
 E = TypeVar("E")
 
 
 def take_n_events(
     stream: EventStream[E, Any],
     num: int,
-) -> "Future[List[E]]":
+) -> "Future[list[E]]":
     count = itertools.count()
     return take_events(stream, lambda _: next(count) >= num)
 
 
 def take_events(
     stream: EventStream[E, Any],
     cutoff_predicate: Callable[[E], bool],
-) -> "Future[List[E]]":
-    events: List[E] = []
-    future: "Future[List[E]]" = Future()
+) -> "Future[list[E]]":
+    events: list[E] = []
+    future: "Future[list[E]]" = Future()
 
     def on_event(event: E, event_id: Optional[str]) -> None:
         events.append(event)
         if cutoff_predicate(event):
             future.set_result(events)
 
     sub = stream.subscribe(on_event)
     future.add_done_callback(lambda _: stream.unsubscribe(sub))
     return future
 
 
 def take_events_from_streams(
-    streams: List[EventStream[Any, int]],
+    streams: list[EventStream[Any, int]],
     cutoff_predicate: Callable[[Any], bool],
-) -> "Future[List[Any]]":
+) -> "Future[list[Any]]":
     """Returns a collated list of futures for events in numerous event streams.
 
     The support for generic and algebraic types doesn't appear to extend to
     taking an arbitrary list of concrete types with single but differing
     generic arguments while also maintaining the generality of the argument
     types.
 
@@ -419,20 +421,24 @@
             EventStream[WorkerEvent, int],
             EventStream[DataEvent, int],
             EventStream[ProgressEvent, int]
         ]
     ]
 
     """
-    events: List[Any] = []
-    future: "Future[List[Any]]" = Future()
+    events: list[Any] = []
+    future: "Future[list[Any]]" = Future()
 
     def on_event(event: Any, event_id: Optional[str]) -> None:
         print(event)
         events.append(event)
         if cutoff_predicate(event):
             future.set_result(events)
 
     for stream in streams:
         sub = stream.subscribe(on_event)
-        future.add_done_callback(lambda _: stream.unsubscribe(sub))
+
+        def callback(unused: Future[list[Any]], stream=stream, sub=sub):
+            stream.unsubscribe(sub)
+
+        future.add_done_callback(callback)
     return future
```

