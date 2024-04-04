# Comparing `tmp/orchestrator_core-2.1.2rc4.tar.gz` & `tmp/orchestrator_core-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-2.1.2rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-2.1.2rc4.tar` & `orchestrator_core-2.2.0.tar`

### file list

```diff
@@ -1,545 +1,535 @@
--rw-r--r--   0        0        0      342 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.coveragerc
--rw-r--r--   0        0        0     1564 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1149 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      502 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/dependabot.yml
--rw-r--r--   0        0        0     2620 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      346 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      583 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/issues.yml
--rw-r--r--   0        0        0      550 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1215 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2255 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.gitignore
--rw-r--r--   0        0        0     2599 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/.stignore
--rw-r--r--   0        0        0    30927 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/CHANGELOG.md
--rw-r--r--   0        0        0      333 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/Dockerfile
--rw-r--r--   0        0        0    11409 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/LICENSE
--rw-r--r--   0        0        0      150 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/NOTICE
--rw-r--r--   0        0        0     5595 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/README.md
--rw-r--r--   0        0        0      196 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/codecov.yml
--rw-r--r--   0        0        0       45 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/api.md
--rw-r--r--   0        0        0     5505 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/callbacks.md
--rw-r--r--   0        0        0    30737 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13882 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    24530 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/graphql.md
--rw-r--r--   0        0        0    48994 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2500 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11462 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0      802 2024-03-28 13:03:01.629907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1311 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1398 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1138 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/contributing/guidelines.md
--rw-r--r--   0        0        0     9997 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/css/custom.css
--rw-r--r--   0        0        0      656 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/css/style.css
--rw-r--r--   0        0        0     2165 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/getting-started/development.md
--rw-r--r--   0        0        0     3438 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/getting-started/prepare-source-folder.md
--rw-r--r--   0        0        0    17905 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/img/WFO-Emblem-White.png
--rw-r--r--   0        0        0      842 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/img/favicon.ico
--rw-r--r--   0        0        0     4020 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/index.md
--rw-r--r--   0        0        0     3897 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/js/termynal.js
--rw-r--r--   0        0        0    11084 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/migration-guide/2.0.md
--rw-r--r--   0        0        0     9063 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3719 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     6048 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3087 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5602 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4623 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7447 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3697 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3051 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6156 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1953 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3991 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3596 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2024-03-28 13:03:01.633907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2141 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2878 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      785 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3632 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2024-03-28 13:03:01.637907 orchestrator_core-2.1.2rc4/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0     5478 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/mkdocs.yml
--rw-r--r--   0        0        0     1262 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/mutmut_config.py
--rw-r--r--   0        0        0       70 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/nitpick-style.toml
--rw-r--r--   0        0        0     1098 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     3144 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2849 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1284 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    14407 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2914 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3669 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2755 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     6106 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2977 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    13616 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      963 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1827 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     2071 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1722 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/ws.py
--rw-r--r--   0        0        0     1502 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    12323 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5996 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/api/models.py
--rw-r--r--   0        0        0     8365 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/app.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13792 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6775 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     2172 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10474 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9379 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    23981 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1399 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     7377 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0      173 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/README
--rw-r--r--   0        0        0      307 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
--rw-r--r--   0        0        0      115 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
--rw-r--r--   0        0        0       82 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
--rw-r--r--   0        0        0      307 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
--rw-r--r--   0        0        0      115 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
--rw-r--r--   0        0        0       82 2024-03-28 13:03:01.641907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
--rw-r--r--   0        0        0      234 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
--rw-r--r--   0        0        0      131 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
--rw-r--r--   0        0        0       82 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     2007 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/enums.py
--rw-r--r--   0        0        0     5452 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     6341 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2073 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5285 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1379 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1878 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4541 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1815 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     8026 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      759 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      538 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      532 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      361 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      431 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/additional_create_imports.j2
--rw-r--r--   0        0        0       25 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/additional_create_steps.j2
--rw-r--r--   0        0        0      394 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/additional_modify_imports.j2
--rw-r--r--   0        0        0       25 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/additional_modify_steps.j2
--rw-r--r--   0        0        0       25 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0      282 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0      361 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/create_data_head.j2
--rw-r--r--   0        0        0     4806 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      298 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/enums.j2
--rw-r--r--   0        0        0      523 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
--rw-r--r--   0        0        0      277 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      904 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4719 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2901 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1365 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2454 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      545 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     1274 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/shared_workflows.j2
--rw-r--r--   0        0        0      291 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/subscription_model_registry.j2
--rw-r--r--   0        0        0     1883 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1802 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1677 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      985 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2315 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      857 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20371 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8979 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4110 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2970 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10269 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/database.py
--rw-r--r--   0        0        0      335 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3367 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0      774 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/__init__.py
--rw-r--r--   0        0        0      999 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/bool_filter.py
--rw-r--r--   0        0        0      970 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/is_like_filter.py
--rw-r--r--   0        0        0     2528 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/range_filter.py
--rw-r--r--   0        0        0     1011 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/values_in_column_filter.py
--rw-r--r--   0        0        0     6659 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1936 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     2666 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/product_block.py
--rw-r--r--   0        0        0     2038 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/resource_type.py
--rw-r--r--   0        0        0      532 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/search_filters/__init__.py
--rw-r--r--   0        0        0     3739 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/search_filters/inferred_filter.py
--rw-r--r--   0        0        0     3344 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0     2168 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/filters/workflow.py
--rw-r--r--   0        0        0      283 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/helpers.py
--rw-r--r--   0        0        0    25499 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/models.py
--rw-r--r--   0        0        0      162 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     2175 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      244 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0     2501 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      500 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0      547 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/product_block.py
--rw-r--r--   0        0        0      547 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/resource_type.py
--rw-r--r--   0        0        0     4455 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0     1370 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0      506 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/db/sorting/workflow.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    18847 2024-03-28 13:03:01.645907 orchestrator_core-2.1.2rc4/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/devtools/scripts/__init__.py
--rw-r--r--   0        0        0     8359 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/devtools/scripts/migrate_20.py
--rw-r--r--   0        0        0     2494 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2508 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3114 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3271 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      894 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    59706 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/domain/base.py
--rw-r--r--   0        0        0      989 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/domain/helpers.py
--rw-r--r--   0        0        0     2882 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     1268 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0      892 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0      888 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0     2002 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/__init__.py
--rw-r--r--   0        0        0     1687 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/customer_contact_list.py
--rw-r--r--   0        0        0      708 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/customer_id.py
--rw-r--r--   0        0        0      779 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/display_subscription.py
--rw-r--r--   0        0        0     2065 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/network_type_validators.py
--rw-r--r--   0        0        0     2114 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/forms/validators/product_id.py
--rw-r--r--   0        0        0     1378 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     6161 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/autoregistration.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4304 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1746 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     5826 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/error_handler_extension.py
--rw-r--r--   0        0        0     2413 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      851 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0      934 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/customer.py
--rw-r--r--   0        0        0      636 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/helpers.py
--rw-r--r--   0        0        0     4473 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2566 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     2752 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/product_block.py
--rw-r--r--   0        0        0     2745 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/resource_type.py
--rw-r--r--   0        0        0     3700 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     4996 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0     2671 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/workflow.py
--rw-r--r--   0        0        0     6463 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schema.py
--rw-r--r--   0        0        0     1003 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/__init__.py
--rw-r--r--   0        0        0      115 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/customer.py
--rw-r--r--   0        0        0      203 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     5414 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2134 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0     1203 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      755 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      999 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     8379 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0     1140 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     3813 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      524 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1191 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0     1002 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0     4188 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/get_subscription_product_blocks.py
--rw-r--r--   0        0        0     2156 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/is_query_detailed.py
--rw-r--r--   0        0        0     1370 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/override_class.py
--rw-r--r--   0        0        0      902 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/to_graphql_result_page.py
--rw-r--r--   0        0        0       39 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3382 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40911 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2698 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1265 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    39307 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      950 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1214 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1603 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5106 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7964 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0     1014 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0      591 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
--rw-r--r--   0        0        0      755 2024-03-28 13:03:01.649907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
--rw-r--r--   0        0        0      967 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
--rw-r--r--   0        0        0     4491 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
--rw-r--r--   0        0        0     1036 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
--rw-r--r--   0        0        0     5480 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
--rw-r--r--   0        0        0     2246 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/py.typed
--rw-r--r--   0        0        0     1066 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1526 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1234 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2195 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2772 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      888 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1286 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1356 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      802 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3438 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1698 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1792 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      973 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3366 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1030 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1977 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1744 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/security.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3635 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/celery.py
--rw-r--r--   0        0        0      876 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/fixed_inputs.py
--rw-r--r--   0        0        0    28515 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1933 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/products.py
--rw-r--r--   0        0        0      884 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/resource_types.py
--rw-r--r--   0        0        0     2723 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/settings.py
--rw-r--r--   0        0        0    25733 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5867 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1713 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/translations.py
--rw-r--r--   0        0        0     1638 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/services/workflows.py
--rw-r--r--   0        0        0     3634 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/targets.py
--rw-r--r--   0        0        0    16236 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/types.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5584 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6172 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     5270 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/enrich_process.py
--rw-r--r--   0        0        0     4707 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8063 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     1322 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/get_updated_properties.py
--rw-r--r--   0        0        0     3212 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8341 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/json.py
--rw-r--r--   0        0        0     5582 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/redis.py
--rw-r--r--   0        0        0    15382 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/search_query.py
--rw-r--r--   0        0        0     3393 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2364 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    12998 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/strings.py
--rw-r--r--   0        0        0      896 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1366 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/version.py
--rw-r--r--   0        0        0     4828 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     4596 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3324 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2924 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    42882 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflow.py
--rw-r--r--   0        0        0     4048 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2164 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9528 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1614 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2349 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8496 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    13025 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     5072 2024-03-28 13:03:01.653907 orchestrator_core-2.1.2rc4/pyproject.toml
--rw-r--r--   0        0        0     2725 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/setup.cfg
--rw-r--r--   0        0        0      665 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/setup.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1851 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2887 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5160 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1626 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1139 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3055 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    21796 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15509 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3863 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     8209 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2614 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     3000 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     3005 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    41173 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     3457 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0     3777 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/api/test_ws.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/__init__.py
--rw-r--r--   0        0        0      744 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate.sh
--rw-r--r--   0        0        0      885 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/alembic.ini
--rw-r--r--   0        0        0      233 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/main.py
--rw-r--r--   0        0        0     2821 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/env.py
--rw-r--r--   0        0        0       98 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/script.py.mako
--rw-r--r--   0        0        0      315 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
--rw-r--r--   0        0        0     2227 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
--rw-r--r--   0        0        0     3852 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
--rw-r--r--   0        0        0      467 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1995 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
--rw-r--r--   0        0        0      812 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_types/__init__.py
--rw-r--r--   0        0        0      764 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_types/example1.py
--rw-r--r--   0        0        0      559 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_types/example2.py
--rw-r--r--   0        0        0     1499 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
--rw-r--r--   0        0        0     1499 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
--rw-r--r--   0        0        0     2442 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
--rw-r--r--   0        0        0     2014 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
--rw-r--r--   0        0        0     1345 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
--rw-r--r--   0        0        0     1010 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
--rw-r--r--   0        0        0      902 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
--rw-r--r--   0        0        0      872 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
--rw-r--r--   0        0        0      755 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
--rw-r--r--   0        0        0      405 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
--rw-r--r--   0        0        0      415 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/translations/en-GB.json
--rw-r--r--   0        0        0      701 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/__init__.py
--rw-r--r--   0        0        0     3940 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
--rw-r--r--   0        0        0     3602 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
--rw-r--r--   0        0        0      620 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
--rw-r--r--   0        0        0     1560 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
--rw-r--r--   0        0        0     1025 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
--rw-r--r--   0        0        0     2683 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
--rw-r--r--   0        0        0     2508 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
--rw-r--r--   0        0        0        1 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
--rw-r--r--   0        0        0     1220 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
--rw-r--r--   0        0        0     1273 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/shared.py
--rw-r--r--   0        0        0     2656 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config1.yaml
--rw-r--r--   0        0        0      549 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config2.yaml
--rw-r--r--   0        0        0      590 2024-03-28 13:03:01.657907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config3.yaml
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/generator/__init__.py
--rw-r--r--   0        0        0      812 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/generator/test_enums.py
--rw-r--r--   0        0        0     2509 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_cli_generate.py
--rw-r--r--   0        0        0     2930 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_generate_code.py
--rw-r--r--   0        0        0    26343 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27644 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/config.py
--rw-r--r--   0        0        0    23677 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    53002 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8230 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4670 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     1992 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_lifecycle.py
--rw-r--r--   0        0        0     2841 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7794 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1645 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2970 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1606 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2573 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2518 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1194 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1123 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2172 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4217 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3428 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2951 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2272 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2256 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1639 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1838 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      644 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0      451 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/workflows.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/network_type_validators/__init__.py
--rw-r--r--   0        0        0     4759 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/network_type_validators/test_bfd.py
--rw-r--r--   0        0        0     1826 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/network_type_validators/test_mtu.py
--rw-r--r--   0        0        0     4939 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_customer_contact_list.py
--rw-r--r--   0        0        0      495 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_customer_id.py
--rw-r--r--   0        0        0     1746 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_display_subscription.py
--rw-r--r--   0        0        0     4109 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/__init__.py
--rw-r--r--   0        0        0      690 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/conftest.py
--rw-r--r--   0        0        0     2316 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_customer.py
--rw-r--r--   0        0        0    18790 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     8516 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0    10214 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_product_blocks.py
--rw-r--r--   0        0        0     5636 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_resource_types.py
--rw-r--r--   0        0        0     5179 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0     2915 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_sort_and_filter_fields.py
--rw-r--r--   0        0        0    47358 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0     6683 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_workflows.py
--rw-r--r--   0        0        0      608 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_autoregistration.py
--rw-r--r--   0        0        0     7669 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_is_query_detailed.py
--rw-r--r--   0        0        0     3042 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_is_querying_page_data.py
--rw-r--r--   0        0        0     8760 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_override_class.py
--rw-r--r--   0        0        0      631 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/helpers.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    28556 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1155 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     6171 2024-03-28 13:03:01.661907 orchestrator_core-2.1.2rc4/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     6650 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      379 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    17406 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3486 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3529 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_get_updated_properties.py
--rw-r--r--   0        0        0     3052 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     4613 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_search_query.py
--rw-r--r--   0        0        0     1144 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11471 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/websocket/__init__.py
--rw-r--r--   0        0        0     3561 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/websocket/test_broadcast.py
--rw-r--r--   0        0        0    14040 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2094 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2443 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2746 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     5363 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_async_workflow.py
--rw-r--r--   0        0        0     3480 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1884 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2024-03-28 13:03:01.665907 orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4573 1970-01-01 00:00:00.000000 orchestrator_core-2.1.2rc4/PKG-INFO
+-rw-r--r--   0        0        0      339 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.coveragerc
+-rw-r--r--   0        0        0     1564 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1149 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      502 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2620 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      346 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      583 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/issues.yml
+-rw-r--r--   0        0        0      550 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1215 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2255 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.gitignore
+-rw-r--r--   0        0        0     2599 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/.stignore
+-rw-r--r--   0        0        0    30927 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/Dockerfile
+-rw-r--r--   0        0        0    11409 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/LICENSE
+-rw-r--r--   0        0        0      150 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/NOTICE
+-rw-r--r--   0        0        0     5595 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/README.md
+-rw-r--r--   0        0        0      196 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/codecov.yml
+-rw-r--r--   0        0        0       45 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/api.md
+-rw-r--r--   0        0        0     5505 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/callbacks.md
+-rw-r--r--   0        0        0    30737 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13882 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    24522 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/graphql.md
+-rw-r--r--   0        0        0    48994 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2500 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11462 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0      802 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2024-04-04 07:11:02.220201 orchestrator_core-2.2.0/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1311 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1398 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1138 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0     9997 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/css/custom.css
+-rw-r--r--   0        0        0      656 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/css/style.css
+-rw-r--r--   0        0        0     2165 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/getting-started/development.md
+-rw-r--r--   0        0        0     3438 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/getting-started/prepare-source-folder.md
+-rw-r--r--   0        0        0    17905 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/img/WFO-Emblem-White.png
+-rw-r--r--   0        0        0      842 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/img/favicon.ico
+-rw-r--r--   0        0        0     4020 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/js/termynal.js
+-rw-r--r--   0        0        0    11084 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/migration-guide/2.0.md
+-rw-r--r--   0        0        0     9063 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3719 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     6048 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3087 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5602 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4623 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7447 2024-04-04 07:11:02.224201 orchestrator_core-2.2.0/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3697 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3051 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6156 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1953 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3991 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3596 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2141 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2878 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      785 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3632 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2024-04-04 07:11:02.228201 orchestrator_core-2.2.0/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0     5478 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/mutmut_config.py
+-rw-r--r--   0        0        0       70 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/nitpick-style.toml
+-rw-r--r--   0        0        0     1095 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     3145 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1284 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    14531 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     4021 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     4806 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     3657 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     6106 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2977 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    15675 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      963 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1827 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     2563 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1722 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/ws.py
+-rw-r--r--   0        0        0     1502 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    10612 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5996 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/api/models.py
+-rw-r--r--   0        0        0     8365 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13792 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6775 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     2172 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10474 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9379 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    23981 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1399 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     7377 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/README
+-rw-r--r--   0        0        0      307 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      307 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-04 07:11:02.232201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0      234 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
+-rw-r--r--   0        0        0      131 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     2007 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/enums.py
+-rw-r--r--   0        0        0     5452 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     6341 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2073 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5285 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1379 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1878 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4541 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1815 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     8026 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      759 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      538 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      532 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      361 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      431 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/additional_create_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      394 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0       25 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0      282 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0      361 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/create_data_head.j2
+-rw-r--r--   0        0        0     4806 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      298 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/enums.j2
+-rw-r--r--   0        0        0      523 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
+-rw-r--r--   0        0        0      277 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      904 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4719 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2901 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1365 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2454 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      545 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     1274 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/shared_workflows.j2
+-rw-r--r--   0        0        0      291 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/subscription_model_registry.j2
+-rw-r--r--   0        0        0     1883 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1802 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1677 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      985 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2315 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      857 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20371 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8979 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4110 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2970 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10269 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/database.py
+-rw-r--r--   0        0        0      371 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     4916 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4098 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0      899 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     1089 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/product_block.py
+-rw-r--r--   0        0        0      889 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/resource_type.py
+-rw-r--r--   0        0        0      562 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/search_filters/__init__.py
+-rw-r--r--   0        0        0     5170 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/search_filters/inferred_filter.py
+-rw-r--r--   0        0        0     1466 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0     1276 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/filters/workflow.py
+-rw-r--r--   0        0        0      283 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/helpers.py
+-rw-r--r--   0        0        0    24840 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/models.py
+-rw-r--r--   0        0        0      162 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     2175 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      353 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0     1987 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      570 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0      617 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/product_block.py
+-rw-r--r--   0        0        0      617 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/resource_type.py
+-rw-r--r--   0        0        0     4455 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0     1441 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0      576 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/db/sorting/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    18847 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     8359 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/devtools/scripts/migrate_20.py
+-rw-r--r--   0        0        0     2494 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2508 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.236201 orchestrator_core-2.2.0/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3271 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      894 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    59246 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/domain/base.py
+-rw-r--r--   0        0        0      989 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/domain/helpers.py
+-rw-r--r--   0        0        0     2882 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     1268 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0      892 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/__init__.py
+-rw-r--r--   0        0        0     1505 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/customer_contact_list.py
+-rw-r--r--   0        0        0      708 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/customer_id.py
+-rw-r--r--   0        0        0      779 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/display_subscription.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/network_type_validators.py
+-rw-r--r--   0        0        0     2114 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/forms/validators/product_id.py
+-rw-r--r--   0        0        0     1378 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     6161 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/autoregistration.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4304 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1746 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     5826 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/extensions/error_handler_extension.py
+-rw-r--r--   0        0        0     2413 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      851 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/customer.py
+-rw-r--r--   0        0        0      636 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/helpers.py
+-rw-r--r--   0        0        0     4491 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2562 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     2748 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/product_block.py
+-rw-r--r--   0        0        0     2741 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/resource_type.py
+-rw-r--r--   0        0        0     3700 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     5531 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0     2681 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/resolvers/workflow.py
+-rw-r--r--   0        0        0     6699 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schema.py
+-rw-r--r--   0        0        0     1003 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/customer.py
+-rw-r--r--   0        0        0      203 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3475 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2134 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0     1203 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      755 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      999 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7958 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0     1140 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     3813 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      524 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1191 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0     1002 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0     3897 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/get_subscription_product_blocks.py
+-rw-r--r--   0        0        0     2156 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/is_query_detailed.py
+-rw-r--r--   0        0        0     1370 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/override_class.py
+-rw-r--r--   0        0        0      902 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/graphql/utils/to_graphql_result_page.py
+-rw-r--r--   0        0        0       39 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3382 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40911 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2698 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1265 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    39307 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      950 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1214 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1603 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5106 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7964 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0     1014 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      591 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0      967 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
+-rw-r--r--   0        0        0     4491 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
+-rw-r--r--   0        0        0     1036 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
+-rw-r--r--   0        0        0     5480 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
+-rw-r--r--   0        0        0     2246 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/py.typed
+-rw-r--r--   0        0        0     1066 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1526 2024-04-04 07:11:02.240201 orchestrator_core-2.2.0/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1234 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2195 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2708 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1286 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1356 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      802 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     2693 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1698 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1792 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      973 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3366 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1030 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1977 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1744 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/celery.py
+-rw-r--r--   0        0        0      876 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/fixed_inputs.py
+-rw-r--r--   0        0        0    28515 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1933 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/products.py
+-rw-r--r--   0        0        0      884 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/resource_types.py
+-rw-r--r--   0        0        0     2723 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    25733 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5867 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1713 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     1638 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/services/workflows.py
+-rw-r--r--   0        0        0     3634 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/targets.py
+-rw-r--r--   0        0        0    16236 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5584 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0      875 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/deprecation_logger.py
+-rw-r--r--   0        0        0     6172 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4658 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/enrich_process.py
+-rw-r--r--   0        0        0     4250 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     2665 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/fixed_inputs.py
+-rw-r--r--   0        0        0     8063 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     1322 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/get_updated_properties.py
+-rw-r--r--   0        0        0     3212 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8341 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     5582 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0    15801 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/search_query.py
+-rw-r--r--   0        0        0    12998 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     1366 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/version.py
+-rw-r--r--   0        0        0     4828 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     4596 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3324 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2924 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    42689 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4048 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9528 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2349 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8511 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12929 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     5073 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2725 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/setup.cfg
+-rw-r--r--   0        0        0      665 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/setup.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.244201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2887 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1626 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1139 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3055 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    21379 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15509 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3863 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     8209 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2614 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     3000 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     3005 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    41173 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     3457 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0     3777 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/api/test_ws.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate.sh
+-rw-r--r--   0        0        0      885 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/alembic.ini
+-rw-r--r--   0        0        0      233 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/main.py
+-rw-r--r--   0        0        0     2821 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/env.py
+-rw-r--r--   0        0        0       98 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/script.py.mako
+-rw-r--r--   0        0        0      315 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
+-rw-r--r--   0        0        0     2227 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
+-rw-r--r--   0        0        0     3852 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
+-rw-r--r--   0        0        0      467 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
+-rw-r--r--   0        0        0      812 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_types/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_types/example1.py
+-rw-r--r--   0        0        0      559 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_types/example2.py
+-rw-r--r--   0        0        0     1499 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
+-rw-r--r--   0        0        0     1499 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
+-rw-r--r--   0        0        0     2442 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
+-rw-r--r--   0        0        0     2014 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
+-rw-r--r--   0        0        0     1345 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
+-rw-r--r--   0        0        0     1010 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
+-rw-r--r--   0        0        0      902 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
+-rw-r--r--   0        0        0      872 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
+-rw-r--r--   0        0        0      755 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
+-rw-r--r--   0        0        0      405 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
+-rw-r--r--   0        0        0      415 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/translations/en-GB.json
+-rw-r--r--   0        0        0      701 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
+-rw-r--r--   0        0        0     3602 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
+-rw-r--r--   0        0        0      620 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
+-rw-r--r--   0        0        0     1560 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
+-rw-r--r--   0        0        0     1025 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
+-rw-r--r--   0        0        0     2683 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
+-rw-r--r--   0        0        0     2508 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
+-rw-r--r--   0        0        0        1 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
+-rw-r--r--   0        0        0     1220 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
+-rw-r--r--   0        0        0     1273 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/shared.py
+-rw-r--r--   0        0        0     2656 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config1.yaml
+-rw-r--r--   0        0        0      549 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config2.yaml
+-rw-r--r--   0        0        0      590 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config3.yaml
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/generator/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/generator/test_enums.py
+-rw-r--r--   0        0        0     2509 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/test_cli_generate.py
+-rw-r--r--   0        0        0     2930 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/test_generate_code.py
+-rw-r--r--   0        0        0    26343 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27644 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2024-04-04 07:11:02.248201 orchestrator_core-2.2.0/test/unit_tests/config.py
+-rw-r--r--   0        0        0    23677 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    53002 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8230 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4670 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     1992 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/domain/test_lifecycle.py
+-rw-r--r--   0        0        0     2841 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2970 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1606 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2573 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2518 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1194 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1123 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2172 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4217 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3428 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2951 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2272 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2256 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1639 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1838 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      644 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0      451 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/fixtures/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     4706 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/forms/test_customer_contact_list.py
+-rw-r--r--   0        0        0      495 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/forms/test_customer_id.py
+-rw-r--r--   0        0        0     1746 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/forms/test_display_subscription.py
+-rw-r--r--   0        0        0     4109 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/conftest.py
+-rw-r--r--   0        0        0     2316 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_customer.py
+-rw-r--r--   0        0        0    18677 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     8514 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0    10211 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_product_blocks.py
+-rw-r--r--   0        0        0     5635 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_resource_types.py
+-rw-r--r--   0        0        0     5179 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0     2939 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_sort_and_filter_fields.py
+-rw-r--r--   0        0        0     3239 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_subscription.py
+-rw-r--r--   0        0        0    48728 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0     6682 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/test_workflows.py
+-rw-r--r--   0        0        0      608 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_autoregistration.py
+-rw-r--r--   0        0        0     7669 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_is_query_detailed.py
+-rw-r--r--   0        0        0     3042 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_is_querying_page_data.py
+-rw-r--r--   0        0        0     8760 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_override_class.py
+-rw-r--r--   0        0        0      631 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    28556 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1155 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     6171 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     6650 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      379 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    17406 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3486 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3529 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_get_updated_properties.py
+-rw-r--r--   0        0        0     3052 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     4613 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_search_query.py
+-rw-r--r--   0        0        0    11471 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/websocket/__init__.py
+-rw-r--r--   0        0        0     3561 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/websocket/test_broadcast.py
+-rw-r--r--   0        0        0    14040 2024-04-04 07:11:02.252201 orchestrator_core-2.2.0/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2746 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     5378 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/test_async_workflow.py
+-rw-r--r--   0        0        0     3495 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1884 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2024-04-04 07:11:02.256201 orchestrator_core-2.2.0/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 orchestrator_core-2.2.0/PKG-INFO
```

### Comparing `orchestrator_core-2.1.2rc4/.github/ISSUE_TEMPLATE/bug-report.yml` & `orchestrator_core-2.2.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/ISSUE_TEMPLATE/feature-request.yml` & `orchestrator_core-2.2.0/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/README.md` & `orchestrator_core-2.2.0/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/build-push-container.yml` & `orchestrator_core-2.2.0/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/codeql-analysis.yml` & `orchestrator_core-2.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/issues.yml` & `orchestrator_core-2.2.0/.github/workflows/issues.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/publish-package.yml` & `orchestrator_core-2.2.0/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/run-linting-tests.yml` & `orchestrator_core-2.2.0/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/run-unit-tests.yml` & `orchestrator_core-2.2.0/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.github/workflows/scheduled-build.yml` & `orchestrator_core-2.2.0/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.gitignore` & `orchestrator_core-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.pre-commit-config.yaml` & `orchestrator_core-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/.stignore` & `orchestrator_core-2.2.0/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/CHANGELOG.md` & `orchestrator_core-2.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/LICENSE` & `orchestrator_core-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/README.md` & `orchestrator_core-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/callbacks.md` & `orchestrator_core-2.2.0/docs/architecture/application/callbacks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/cli.md` & `orchestrator_core-2.2.0/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/domainmodels.md` & `orchestrator_core-2.2.0/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/forms.md` & `orchestrator_core-2.2.0/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/graphql.md` & `orchestrator_core-2.2.0/docs/architecture/application/graphql.md`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
 ```python
 import structlog
 from sqlalchemy import func, select
 
 from orchestrator.db import db
 from orchestrator.db.filters import Filter
 from orchestrator.db.range.range import apply_range_to_statement
-from orchestrator.db.sorting.sorting import Sort
+from orchestrator.db.sorting import Sort
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers.helpers import rows_from_statement
 from orchestrator.graphql.schemas.customer import CustomerType
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils.create_resolver_error_handler import (
     create_resolver_error_handler,
 )
```

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/openapi.json` & `orchestrator_core-2.2.0/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/python.md` & `orchestrator_core-2.2.0/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/scaling.md` & `orchestrator_core-2.2.0/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/tasks.md` & `orchestrator_core-2.2.0/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/websockets.md` & `orchestrator_core-2.2.0/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/application/workflow.md` & `orchestrator_core-2.2.0/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/context.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/node.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/node.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/port.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/port.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/standards.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-2.2.0/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/architecture/tldr.md` & `orchestrator_core-2.2.0/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/contributing/guidelines.md` & `orchestrator_core-2.2.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/contributing/testing.md` & `orchestrator_core-2.2.0/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/css/style.css` & `orchestrator_core-2.2.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/css/termynal.css` & `orchestrator_core-2.2.0/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/getting-started/base.md` & `orchestrator_core-2.2.0/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/getting-started/development.md` & `orchestrator_core-2.2.0/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/getting-started/prepare-source-folder.md` & `orchestrator_core-2.2.0/docs/getting-started/prepare-source-folder.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/img/WFO-Emblem-White.png` & `orchestrator_core-2.2.0/docs/img/WFO-Emblem-White.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/img/favicon.ico` & `orchestrator_core-2.2.0/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/index.md` & `orchestrator_core-2.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/js/custom.js` & `orchestrator_core-2.2.0/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/js/termynal.js` & `orchestrator_core-2.2.0/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/migration-guide/2.0.md` & `orchestrator_core-2.2.0/docs/migration-guide/2.0.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/domain-models.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/overview.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/scenario.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-2.2.0/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/create-user.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/database-migration.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/debian.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/docker.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/domain-models.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/explore.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/input-forms.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/macos.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/modify-user.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/overview.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/scenario.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/start-applications.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-2.2.0/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/images/metadata_products.png` & `orchestrator_core-2.2.0/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-2.2.0/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/mkdocs.yml` & `orchestrator_core-2.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/mutmut_config.py` & `orchestrator_core-2.2.0/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/__init__.py` & `orchestrator_core-2.2.0/orchestrator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "2.1.2rc4"
+__version__ = "2.2.0"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/__init__.py` & `orchestrator_core-2.2.0/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/api.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 api_router = APIRouter()
 api_router.include_router(
     fixed_input.router,
     prefix="/fixed_inputs",
     tags=["Core", "Fixed Inputs"],
     dependencies=[Depends(opa_security_default)],
 )
+
 api_router.include_router(
     processes.router, prefix="/processes", tags=["Core", "Processes"], dependencies=[Depends(opa_security_default)]
 )
 api_router.include_router(processes.ws_router, prefix="/processes", tags=["Core", "Processes"])
 
 api_router.include_router(
     product_blocks.router,
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-2.2.0/orchestrator/utils/fixed_inputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2024 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -10,30 +10,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
 from typing import Any
 
-import structlog
-from fastapi.routing import APIRouter
 from more_itertools import first_true, one
 from sqlalchemy.exc import NoResultFound
+from structlog import get_logger
 
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY
-from orchestrator.schemas import FixedInputConfigurationSchema
 from orchestrator.services import products
 
-router = APIRouter()
+logger = get_logger(__name__)
 
-logger = structlog.get_logger(__name__)
 
-
-@router.get("/configuration", response_model=FixedInputConfigurationSchema)
-def fi_configuration() -> dict[str, Any]:  # noqa: C901
+def fixed_input_configuration() -> dict[str, Any]:  # noqa: C901
     product_tags = products.get_tags()
 
     data: dict = {"fixed_inputs": [], "by_tag": {}}
     for tag in product_tags:
         data["by_tag"][tag] = []
 
     for product_name, model in SUBSCRIPTION_MODEL_REGISTRY.items():
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import struct
 import zlib
 from http import HTTPStatus
 from typing import Any
 from uuid import UUID
 
 import structlog
-from deprecated import deprecated
 from fastapi import Request
 from fastapi.param_functions import Body, Depends, Header
 from fastapi.routing import APIRouter
 from fastapi.websockets import WebSocket
 from fastapi_etag.dependency import CacheHit
 from more_itertools import chunked
 from sentry_sdk.tracing import trace
@@ -39,17 +38,17 @@
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import ProcessSubscriptionTable, ProcessTable, SubscriptionTable, db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.process import filter_processes
 from orchestrator.db.sorting import Sort, SortOrder
 from orchestrator.db.sorting.process import sort_processes
 from orchestrator.schemas import (
-    ProcessDeprecationsSchema,
     ProcessIdSchema,
     ProcessResumeAllSchema,
+    ProcessSchema,
     ProcessStatusCounts,
     ProcessSubscriptionBaseSchema,
     ProcessSubscriptionSchema,
     Reporter,
 )
 from orchestrator.security import oidc_user
 from orchestrator.services.processes import (
@@ -62,14 +61,15 @@
     load_process,
     resume_process,
     start_process,
 )
 from orchestrator.services.settings import get_engine_settings
 from orchestrator.settings import app_settings
 from orchestrator.types import JSON, State
+from orchestrator.utils.deprecation_logger import deprecated_endpoint
 from orchestrator.utils.enrich_process import enrich_process
 from orchestrator.websocket import WS_CHANNELS, send_process_data_to_websocket, websocket_manager
 from orchestrator.workflow import ProcessStatus
 
 router = APIRouter()
 
 logger = structlog.get_logger(__name__)
@@ -227,39 +227,49 @@
         abort_process(process, user, broadcast_func=broadcast_func)
         return
     except Exception as e:
         raise_status(HTTPStatus.INTERNAL_SERVER_ERROR, str(e))
 
 
 @router.get(
-    "/process-subscriptions-by-subscription-id/{subscription_id}", response_model=list[ProcessSubscriptionSchema]
+    "/process-subscriptions-by-subscription-id/{subscription_id}",
+    response_model=list[ProcessSubscriptionSchema],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
 )
 def process_subscriptions_by_subscription_id(subscription_id: UUID) -> list[ProcessSubscriptionSchema]:
     stmt = (
         select(ProcessSubscriptionTable)
         .options(contains_eager(ProcessSubscriptionTable.process))
         .join(ProcessTable)
         .filter(ProcessSubscriptionTable.subscription_id == subscription_id)
         .order_by(ProcessTable.started_at.asc())
     )
     return list(db.session.scalars(stmt))
 
 
-@deprecated("Changed to '/process-subscriptions-by-process_id/{process_id}' from version 1.2.3, will be removed in 1.4")
-@router.get("/process-subscriptions-by-pid/{pid}", response_model=list[ProcessSubscriptionBaseSchema])
-def process_subscriptions_by_process_pid(pid: UUID) -> list[ProcessSubscriptionTable]:
-    return list(db.session.scalars(select(ProcessSubscriptionTable).filter_by(process_id=pid)))
-
-
-@router.get("/process-subscriptions-by-process_id/{process_id}", response_model=list[ProcessSubscriptionBaseSchema])
+@router.get(
+    "/process-subscriptions-by-process_id/{process_id}",
+    response_model=list[ProcessSubscriptionBaseSchema],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def process_subscriptions_by_process_process_id(process_id: UUID) -> list[ProcessSubscriptionTable]:
     return list(db.session.scalars(select(ProcessSubscriptionTable).filter_by(process_id=process_id)))
 
 
-@router.get("/statuses", response_model=list[ProcessStatus])
+@router.get(
+    "/statuses",
+    response_model=list[ProcessStatus],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def statuses() -> list[str]:
     return [status.value for status in ProcessStatus]
 
 
 @router.get("/status-counts", response_model=ProcessStatusCounts)
 def status_counts() -> ProcessStatusCounts:
     """Retrieve status counts for processes and tasks."""
@@ -272,30 +282,31 @@
     rows = db.session.execute(stmt).all()
     return ProcessStatusCounts(
         process_counts={status: num_processes for is_task, status, num_processes in rows if not is_task},
         task_counts={status: num_processes for is_task, status, num_processes in rows if is_task},
     )
 
 
-@router.get("/assignees", response_model=list[Assignee])
+@router.get(
+    "/assignees",
+    response_model=list[Assignee],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def assignees() -> list[str]:
     return [assignee.value for assignee in Assignee]
 
 
-@deprecated("product (UUID) changed to product_id from version 1.2.3, will be removed in 1.4")
-def convert_to_old_process(process: dict) -> dict:
-    return {**process, "product": process["product_id"]}
-
-
-@router.get("/{process_id}", response_model=ProcessDeprecationsSchema)
+@router.get("/{process_id}", response_model=ProcessSchema)
 def show(process_id: UUID) -> dict[str, Any]:
     process = _get_process(process_id)
     p = load_process(process)
 
-    return convert_to_old_process(enrich_process(process, p))
+    return enrich_process(process, p)
 
 
 def handle_process_error(message: str, **kwargs: Any) -> None:
     logger.debug(message, **kwargs)
     raise_status(HTTPStatus.BAD_REQUEST, message)
 
 
@@ -306,15 +317,15 @@
     for p in results:
         checksum = zlib.crc32(p.process_id.bytes, checksum)
         last_modified_as_bytes = struct.pack("d", p.last_modified_at.timestamp())
         checksum = zlib.crc32(last_modified_as_bytes, checksum)
     return checksum
 
 
-@router.get("/", response_model=list[ProcessDeprecationsSchema])
+@router.get("/", response_model=list[ProcessSchema])
 def processes_filterable(  # noqa: C901
     response: Response,
     range: str | None = None,
     sort: str | None = None,
     filter: str | None = None,
     if_none_match: str | None = Header(None),
 ) -> list[dict[str, Any]]:
@@ -354,15 +365,15 @@
     response.headers["ETag"] = f'W/"{entity_tag}"'
 
     # When the If-None-Match header contains the same CRC we can be sure that the resource has not changed,
     # so we can skip serialization at the backend and rerendering at the frontend.
     if if_none_match == entity_tag:
         raise CacheHit(HTTPStatus.NOT_MODIFIED, headers=dict(response.headers))
 
-    return [convert_to_old_process(enrich_process(p)) for p in results]
+    return [enrich_process(p) for p in results]
 
 
 ws_router = APIRouter()
 
 if app_settings.ENABLE_WEBSOCKETS:
 
     @ws_router.websocket("/all/")
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,48 +10,75 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from http import HTTPStatus
 from uuid import UUID
 
-from fastapi.param_functions import Body
+from fastapi.params import Body, Depends
 from fastapi.routing import APIRouter
 from sqlalchemy import select
 
 from orchestrator.api.error_handling import raise_status
 from orchestrator.api.models import delete, save, update
 from orchestrator.db import ProductBlockTable, ResourceTypeTable, db
 from orchestrator.schemas import ResourceTypeBaseSchema, ResourceTypeSchema
 from orchestrator.services.resource_types import get_resource_types
+from orchestrator.utils.deprecation_logger import deprecated_endpoint
 
 router = APIRouter()
 
 
-@router.get("/", response_model=list[ResourceTypeSchema])
+@router.get(
+    "/",
+    response_model=list[ResourceTypeSchema],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def fetch() -> list[ResourceTypeTable]:
     return get_resource_types()
 
 
-@router.get("/{resource_type_id}", response_model=ResourceTypeSchema)
+@router.get(
+    "/{resource_type_id}",
+    response_model=ResourceTypeSchema,
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def resource_type_by_id(resource_type_id: UUID) -> ResourceTypeTable:
     resource_type_stmt = select(ResourceTypeTable).filter_by(resource_type_id=resource_type_id)
     resource_type = db.session.scalars(resource_type_stmt).first()
     if not resource_type:
         raise_status(HTTPStatus.NOT_FOUND, f"Resource type {resource_type_id} not found")
     return resource_type
 
 
-@router.post("/", response_model=None, status_code=HTTPStatus.NO_CONTENT)
-def save_resource_type(data: ResourceTypeBaseSchema = Body(...)) -> None:
+@router.post(
+    "/",
+    response_model=None,
+    status_code=HTTPStatus.NO_CONTENT,
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
+def save_resource_type(data: ResourceTypeBaseSchema = Body(...)) -> None:  # type: ignore
     return save(ResourceTypeTable, data)
 
 
-@router.put("/", response_model=None, status_code=HTTPStatus.NO_CONTENT)
-def update_resource_type(data: ResourceTypeSchema = Body(...)) -> None:
+@router.put(
+    "/",
+    response_model=None,
+    status_code=HTTPStatus.NO_CONTENT,
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
+def update_resource_type(data: ResourceTypeSchema = Body(...)) -> None:  # type: ignore
     return update(ResourceTypeTable, data)
 
 
 @router.delete("/{resource_type_id}", response_model=None, status_code=HTTPStatus.NO_CONTENT)
 def delete_resource_type(resource_type_id: UUID) -> None:
     product_blocks_stmt = select(ProductBlockTable).filter(
         ProductBlockTable.resource_types.any(ResourceTypeTable.resource_type_id == str(resource_type_id))
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,33 +8,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module that implements workflows related API endpoints."""
-
-
+from fastapi import Depends
 from fastapi.routing import APIRouter
 from sqlalchemy import select
 
 from orchestrator.db import ProductTable, WorkflowTable, db
 from orchestrator.schemas import WorkflowSchema, WorkflowWithProductTagsSchema
 from orchestrator.services.workflows import get_workflows
+from orchestrator.utils.deprecation_logger import deprecated_endpoint
 
 router = APIRouter()
 
 
-@router.get("/", response_model=list[WorkflowSchema])
+@router.get(
+    "/",
+    response_model=list[WorkflowSchema],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def get_all(target: str | None = None, include_steps: bool = False) -> list[WorkflowSchema]:
     filters = {"target": target} if target else None
     return list(get_workflows(filters=filters, include_steps=include_steps))
 
 
-@router.get("/with_product_tags", response_model=list[WorkflowWithProductTagsSchema])
+@router.get(
+    "/with_product_tags",
+    response_model=list[WorkflowWithProductTagsSchema],
+    deprecated=True,
+    description="This endpoint is deprecated and will be removed in a future release. Please use the GraphQL query",
+    dependencies=[Depends(deprecated_endpoint)],
+)
 def get_all_with_product_tags() -> list[WorkflowWithProductTagsSchema]:
     all_workflows = get_workflows()
 
     def add_product_tags(wf: WorkflowSchema) -> WorkflowWithProductTagsSchema:
         products_stmt = (
             select(ProductTable)
             .with_only_columns(ProductTable.tag.distinct())
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/api_v1/endpoints/ws.py` & `orchestrator_core-2.2.0/orchestrator/api/api_v1/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/error_handling.py` & `orchestrator_core-2.2.0/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/helpers.py` & `orchestrator_core-2.2.0/orchestrator/api/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 from dataclasses import dataclass
 from datetime import datetime
 from http import HTTPStatus
 from shlex import shlex
 from typing import Any
 from uuid import UUID
 
-from deprecated import deprecated
-from more_itertools import chunked, first
+from more_itertools import chunked
 from sqlalchemy import Select, String, cast, func, select
 from sqlalchemy.sql import expression
 from starlette.responses import Response
 from structlog import get_logger
 
 from orchestrator.api.error_handling import raise_status
-from orchestrator.db import ProcessTable, ProductTable, SubscriptionTable, db
+from orchestrator.db import ProductTable, SubscriptionTable, db
 from orchestrator.db.models import SubscriptionSearchView
 from orchestrator.db.range.range import Selectable, apply_range_to_statement
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.utils.search_query import create_ts_query_string
 
 logger = get_logger(__name__)
 
@@ -216,59 +215,14 @@
     last_step: str | None
     subscriptions: list[_Subscription]
     workflow: str
     workflow_target: str | None
     is_task: bool
 
 
-@deprecated(
-    "consolidated with `show_process` into enrich_process in `orchestrator.utils.enrich_process` from version 1.2.3, will be removed in 1.4"
-)
-def enrich_process(p: ProcessTable) -> _ProcessListItem:
-    # p.subscriptions is a non JSON serializable AssociationProxy
-    # So we need to build a list of Subscriptions here.
-    subscriptions: list[_Subscription] = []
-    for sub in p.subscriptions:
-        prod = sub.product
-
-        subscription = _Subscription(
-            customer_id=sub.customer_id,
-            description=sub.description,
-            end_date=sub.end_date if sub.end_date else None,
-            insync=sub.insync,
-            start_date=sub.start_date if sub.start_date else None,
-            status=sub.status,
-            subscription_id=sub.subscription_id,
-            product=ProductEnriched(
-                product_id=prod.product_id,
-                description=prod.description,
-                name=prod.name,
-                tag=prod.tag,
-                status=prod.status,
-                product_type=prod.product_type,
-            ),
-        )
-        subscriptions.append(subscription)
-
-    return _ProcessListItem(
-        assignee=p.assignee,
-        created_by=p.created_by,
-        failed_reason=p.failed_reason,
-        last_modified_at=p.last_modified_at,
-        pid=p.process_id,
-        started_at=p.started_at.timestamp(),
-        last_status=p.last_status,
-        last_step=p.last_step,
-        subscriptions=subscriptions,
-        workflow=str(p.workflow_name),
-        workflow_target=first([ps.workflow_target for ps in p.process_subscriptions], None),
-        is_task=p.is_task,
-    )
-
-
 def update_in(dct: dict | list, path: str, value: Any, sep: str = ".") -> None:
     """Update a value in a dict or list based on a path."""
     for x in path.split(sep):
         prev: dict | list
         if x.isdigit() and isinstance(dct, list):
             prev = dct
             dct = dct[int(x)]
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/api/models.py` & `orchestrator_core-2.2.0/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/app.py` & `orchestrator_core-2.2.0/orchestrator/app.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/__init__.py` & `orchestrator_core-2.2.0/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/database.py` & `orchestrator_core-2.2.0/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-2.2.0/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generate.py` & `orchestrator_core-2.2.0/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/enums.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-2.2.0/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-2.2.0/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/lazy_workflow_instance.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/lazy_workflow_instance.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/shared_workflows.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/shared_workflows.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-2.2.0/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-2.2.0/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/main.py` & `orchestrator_core-2.2.0/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-2.2.0/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-2.2.0/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/migration_helpers.py` & `orchestrator_core-2.2.0/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/cli/scheduler.py` & `orchestrator_core-2.2.0/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/config/__init__.py` & `orchestrator_core-2.2.0/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/config/assignee.py` & `orchestrator_core-2.2.0/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/__init__.py` & `orchestrator_core-2.2.0/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/database.py` & `orchestrator_core-2.2.0/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/bool_filter.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/display_subscription.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Annotated
+from uuid import UUID
 
-from collections.abc import Callable
+from pydantic import Field
 
-from sqlalchemy import ColumnClause
-
-from orchestrator.db.filters.filters import QueryType
-
-
-def generic_bool_filter(field: ColumnClause) -> Callable[[QueryType, str], QueryType]:
-    def bool_filter(query: QueryType, value: str) -> QueryType:
-        value_as_bool = value.lower() in ("yes", "y", "true", "1")
-        return query.filter(field.is_(value_as_bool))
-
-    return bool_filter
+DisplaySubscription = Annotated[
+    UUID, Field(frozen=True, json_schema_extra={"format": "subscription", "type": "string"})
+]
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/filters/generic_filters/is_like_filter.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/customer_id.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,12 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Annotated
 
+from pydantic import Field
 
-from collections.abc import Callable
-
-from sqlalchemy import ColumnClause, String, cast
-
-from orchestrator.db.filters.filters import QueryType
-
-
-def generic_is_like_filter(field: ColumnClause) -> Callable[[QueryType, str], QueryType]:
-    def like_filter(query: QueryType, value: str) -> QueryType:
-        return query.filter(cast(field, String).ilike("%" + value + "%"))
-
-    return like_filter
+CustomerId = Annotated[str, Field(json_schema_extra={"format": "customerId"})]
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/models.py` & `orchestrator_core-2.2.0/orchestrator/db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from __future__ import annotations
 
 from datetime import datetime, timezone
 
 import sqlalchemy
 import structlog
-from deprecated import deprecated
 from more_itertools import first_true
 from sqlalchemy import (
     TIMESTAMP,
     Boolean,
     CheckConstraint,
     Column,
     ForeignKey,
@@ -105,19 +104,14 @@
     )
     process_subscriptions = relationship("ProcessSubscriptionTable", lazy=True, passive_deletes=True)
     subscriptions = association_proxy("process_subscriptions", "subscription")
 
     workflow = relationship("WorkflowTable", back_populates="processes")
 
     @property
-    @deprecated("Changed to 'process_id' from version 1.2.3, will be removed in 1.4")
-    def pid(self) -> Column:
-        return self.process_id
-
-    @property
     def workflow_name(self) -> Column:
         return self.workflow.name
 
 
 class ProcessStepTable(BaseModel):
     __tablename__ = "process_steps"
 
@@ -128,41 +122,26 @@
     name = mapped_column(String(), nullable=False)
     status = mapped_column(String(50), nullable=False)
     state = mapped_column(pg.JSONB(), nullable=False)  # type: ignore
     created_by = mapped_column(String(255), nullable=True)
     executed_at = mapped_column(UtcTimestamp, server_default=text("statement_timestamp()"), nullable=False)
     commit_hash = mapped_column(String(40), nullable=True, default=GIT_COMMIT_HASH)
 
-    @property
-    @deprecated("Changed to 'step_id' from version 1.2.3, will be removed in 1.4")
-    def stepid(self) -> Column:
-        return self.step_id
-
-    @property
-    @deprecated("Changed to 'process_id' from version 1.2.3, will be removed in 1.4")
-    def pid(self) -> Column:
-        return self.process_id
-
 
 class ProcessSubscriptionTable(BaseModel):
     __tablename__ = "processes_subscriptions"
 
     id = mapped_column(UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True)
     process_id = mapped_column("pid", UUIDType, ForeignKey("processes.pid", ondelete="CASCADE"), index=True)
     process = relationship("ProcessTable", back_populates="process_subscriptions")
     subscription_id = mapped_column(UUIDType, ForeignKey("subscriptions.subscription_id"), nullable=False, index=True)
     subscription = relationship("SubscriptionTable", lazy=True)
     created_at = mapped_column(UtcTimestamp, server_default=text("current_timestamp()"), nullable=False)
     workflow_target = mapped_column(String(255), nullable=False, server_default=Target.CREATE)
 
-    @property
-    @deprecated("Changed to 'process_id' from version 1.2.3, will be removed in 1.4")
-    def pid(self) -> Column:
-        return self.process_id
-
 
 processes_subscriptions_ix = Index(
     "processes_subscriptions_ix", ProcessSubscriptionTable.process_id, ProcessSubscriptionTable.subscription_id
 )
 
 product_product_block_association = Table(
     "product_product_blocks",
@@ -559,15 +538,15 @@
     __tablename__ = "subscriptions"
 
     subscription_id = mapped_column(UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True)
     description = mapped_column(Text(), nullable=False)
     status = mapped_column(String(STATUS_LENGTH), nullable=False, index=True)
     product_id = mapped_column(UUIDType, ForeignKey("products.product_id"), nullable=False, index=True)
     product = relationship("ProductTable")
-    customer_id = mapped_column(String, index=True)
+    customer_id = mapped_column(String, index=True, nullable=False)
     insync = mapped_column(Boolean())
     start_date = mapped_column(UtcTimestamp, nullable=True)
     end_date = mapped_column(UtcTimestamp)
     note = mapped_column(Text())
 
     instances = relationship(
         "SubscriptionInstanceTable",
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/range/range.py` & `orchestrator_core-2.2.0/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/sorting/process.py` & `orchestrator_core-2.2.0/orchestrator/db/sorting/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Callable
 
 from sqlalchemy import Column, Select
 from sqlalchemy.inspection import inspect
 from sqlalchemy.sql import expression
 
-from orchestrator.db import ProcessSubscriptionTable, ProcessTable, ProductTable, SubscriptionTable, WorkflowTable
-from orchestrator.db.sorting.sorting import QueryType, SortOrder, generic_column_sort, generic_sort
+from orchestrator.db import ProcessSubscriptionTable, ProcessTable, ProductTable, SubscriptionTable
+from orchestrator.db.filters import create_memoized_field_list
+from orchestrator.db.sorting import QueryType, SortOrder, generic_column_sort, generic_sort
 from orchestrator.utils.helpers import to_camel
 
 PROCESS_CAMEL_SORT = {
     to_camel(key): generic_column_sort(value, ProcessTable) for key, value in inspect(ProcessTable).columns.items()
 }
 PROCESS_SNAKE_SORT = {
     key: generic_column_sort(value, ProcessTable) for key, value in inspect(ProcessTable).columns.items()
@@ -39,16 +40,11 @@
 PROCESS_SORT_FUNCTIONS_BY_COLUMN = (
     PROCESS_PRODUCT_SORT
     | PROCESS_CAMEL_SORT
     | PROCESS_SNAKE_SORT
     | {
         "workflowTarget": generic_process_relation_sort(ProcessSubscriptionTable.workflow_target),
         "subscriptions": generic_process_relation_sort(SubscriptionTable.description),
-        "workflow": generic_process_relation_sort(WorkflowTable.name),  # TODO: deprecated, remove in 1.4
-        "status": generic_column_sort(ProcessTable.last_status, ProcessTable),  # TODO: deprecated, remove in 1.4
-        "creator": generic_column_sort(ProcessTable.created_by, ProcessTable),  # TODO: deprecated, remove in 1.4
-        "started": generic_column_sort(ProcessTable.started_at, ProcessTable),  # TODO: deprecated, remove in 1.4
-        "modified": generic_column_sort(ProcessTable.last_modified_at, ProcessTable),  # TODO: deprecated, remove in 1.4
     }
 )
-process_sort_fields = list(PROCESS_SORT_FUNCTIONS_BY_COLUMN.keys())
+process_sort_fields = create_memoized_field_list(PROCESS_SORT_FUNCTIONS_BY_COLUMN)
 sort_processes = generic_sort(PROCESS_SORT_FUNCTIONS_BY_COLUMN)
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/sorting/product_block.py` & `orchestrator_core-2.2.0/orchestrator/db/sorting/product_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from sqlalchemy.inspection import inspect
 
 from orchestrator.db import ProductBlockTable
-from orchestrator.db.sorting.sorting import generic_column_sort, generic_sort
+from orchestrator.db.filters import create_memoized_field_list
+from orchestrator.db.sorting import generic_column_sort, generic_sort
 from orchestrator.utils.helpers import to_camel
 
 PRODUCT_BLOCK_SORT_FUNCTIONS_BY_COLUMN = {
     to_camel(key): generic_column_sort(value, ProductBlockTable)
     for key, value in inspect(ProductBlockTable).columns.items()
 }
 
-product_block_sort_fields = list(PRODUCT_BLOCK_SORT_FUNCTIONS_BY_COLUMN.keys())
+product_block_sort_fields = create_memoized_field_list(PRODUCT_BLOCK_SORT_FUNCTIONS_BY_COLUMN)
 sort_product_blocks = generic_sort(PRODUCT_BLOCK_SORT_FUNCTIONS_BY_COLUMN)
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/sorting/resource_type.py` & `orchestrator_core-2.2.0/orchestrator/db/sorting/resource_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from sqlalchemy.inspection import inspect
 
 from orchestrator.db import ResourceTypeTable
-from orchestrator.db.sorting.sorting import generic_column_sort, generic_sort
+from orchestrator.db.filters import create_memoized_field_list
+from orchestrator.db.sorting import generic_column_sort, generic_sort
 from orchestrator.utils.helpers import to_camel
 
 RESOURCE_TYPE_SORT_FUNCTIONS_BY_COLUMN = {
     to_camel(key): generic_column_sort(value, ResourceTypeTable)
     for key, value in inspect(ResourceTypeTable).columns.items()
 }
 
-resource_type_sort_fields = list(RESOURCE_TYPE_SORT_FUNCTIONS_BY_COLUMN.keys())
+resource_type_sort_fields = create_memoized_field_list(RESOURCE_TYPE_SORT_FUNCTIONS_BY_COLUMN)
 sort_resource_types = generic_sort(RESOURCE_TYPE_SORT_FUNCTIONS_BY_COLUMN)
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/sorting/sorting.py` & `orchestrator_core-2.2.0/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/db/sorting/subscription.py` & `orchestrator_core-2.2.0/orchestrator/db/sorting/subscription.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Callable
 
 from sqlalchemy import Column
 from sqlalchemy.inspection import inspect
 from sqlalchemy.sql import expression
 
 from orchestrator.db import ProductTable, SubscriptionTable
-from orchestrator.db.sorting.sorting import QueryType, SortOrder, generic_column_sort, generic_sort
+from orchestrator.db.filters import create_memoized_field_list
+from orchestrator.db.sorting import QueryType, SortOrder, generic_column_sort, generic_sort
 from orchestrator.utils.helpers import to_camel
 
 
 def generic_subscription_relation_sort(field: Column) -> Callable[[QueryType, SortOrder], QueryType]:
     def sort_function(query: QueryType, order: SortOrder) -> QueryType:
         if order == SortOrder.DESC:
             return query.order_by(expression.desc(field))
@@ -28,9 +29,10 @@
     for [key, value] in inspect(SubscriptionTable).columns.items()
 }
 
 SUBSCRIPTION_SORT_FUNCTIONS_BY_COLUMN = (
     SUBSCRIPTION_PRODUCT_SORT | subscription_table_sort | {"tag": SUBSCRIPTION_PRODUCT_SORT["productTag"]}
 )
 
-subscription_sort_fields = list(SUBSCRIPTION_SORT_FUNCTIONS_BY_COLUMN.keys())
+
+subscription_sort_fields = create_memoized_field_list(SUBSCRIPTION_SORT_FUNCTIONS_BY_COLUMN)
 sort_subscriptions = generic_sort(SUBSCRIPTION_SORT_FUNCTIONS_BY_COLUMN)
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/devtools/populator.py` & `orchestrator_core-2.2.0/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/devtools/scripts/migrate_20.py` & `orchestrator_core-2.2.0/orchestrator/devtools/scripts/migrate_20.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/distlock/__init__.py` & `orchestrator_core-2.2.0/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-2.2.0/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-2.2.0/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-2.2.0/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-2.2.0/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/domain/__init__.py` & `orchestrator_core-2.2.0/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/domain/base.py` & `orchestrator_core-2.2.0/orchestrator/domain/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
-import warnings
 from collections import defaultdict
 from collections.abc import Callable
 from datetime import datetime
 from inspect import get_annotations
 from itertools import groupby, zip_longest
 from operator import attrgetter
 from typing import (
@@ -27,15 +26,14 @@
     cast,
     get_args,
     get_type_hints,
 )
 from uuid import UUID, uuid4
 
 import structlog
-import typing_extensions
 from more_itertools import first, flatten, one, only
 from pydantic import BaseModel, ConfigDict, Field, ValidationError
 from pydantic.fields import PrivateAttr
 from sqlalchemy import select
 from sqlalchemy.orm import selectinload
 
 from orchestrator.db import (
@@ -421,23 +419,14 @@
             else:
                 saved, depends_on_instance = product_block_models.save(subscription_id=subscription_id, status=status)
                 depends_on_instances[product_block_field] = [depends_on_instance]
                 saved_instances.extend(saved)
 
         return saved_instances, depends_on_instances
 
-    @typing_extensions.deprecated("dict() is deprecated and will be removed in the future, use model_dump() instead")
-    def dict(self, *args: Any, **kwargs: Any) -> dict[str, Any]:
-        warnings.warn(
-            "dict() is deprecated and will be removed in the future, use model_dump() instead",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.model_dump(*args, **kwargs)
-
 
 def get_depends_on_product_block_type_list(
     product_block_types: dict[str, type["ProductBlockModel"] | tuple[type["ProductBlockModel"]]]
 ) -> list[type["ProductBlockModel"]]:
     product_blocks_types_in_model = []
     for product_block_type in product_block_types.values():
         if is_union_type(product_block_type):
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/domain/helpers.py` & `orchestrator_core-2.2.0/orchestrator/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/domain/lifecycle.py` & `orchestrator_core-2.2.0/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/exception_handlers.py` & `orchestrator_core-2.2.0/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/__init__.py` & `orchestrator_core-2.2.0/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/network_type_validators.py` & `orchestrator_core-2.2.0/orchestrator/utils/deprecation_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright 2019-2020 SURF.
+# Copyright 2019-2024 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import structlog
+from starlette.requests import Request
+from structlog import get_logger
 
-from orchestrator.forms.validators.network_type_validators import BFD, MTU
+logger = get_logger(__name__)
 
-# TODO: Deprecated, file will be deleted in the future
-logger = structlog.get_logger(__name__)
-logger.warn("DEPRECATED import: BFD and MTU validators are moved to 'orchestrator.forms.validators'")
-__all__ = ["BFD", "MTU"]
+
+def deprecated_endpoint(request: Request) -> None:
+    logger.warning(
+        "This function is deprecated. Please use the GraphQL query instead", method=request.method, url=str(request.url)
+    )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/validators/__init__.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from nwastdlib.vlans import VlanRanges
 from orchestrator.forms.validators.customer_contact_list import customer_contact_list
 from orchestrator.forms.validators.customer_id import CustomerId
 from orchestrator.forms.validators.display_subscription import DisplaySubscription
-from orchestrator.forms.validators.network_type_validators import BFD, MTU
 from orchestrator.forms.validators.product_id import ProductId, ProductIdError, product_id
 from pydantic_forms.types import strEnum
 from pydantic_forms.validators import (
     Accept,
     Choice,
     ContactPerson,
     ContactPersonName,
@@ -60,12 +60,10 @@
     "Timestamp",
     "migration_summary",
     "product_id",
     "remove_empty_items",
     "strEnum",
     "timestamp",
     "unique_conlist",
-    "BFD",
-    "MTU",
     "VlanRanges",
     "customer_contact_list",
 ]
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/validators/customer_contact_list.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/customer_contact_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     customer_key: Optional[str] = "customer",
     min_items: Optional[int] = None,
     max_items: Optional[int] = None,
 ) -> type[list[T]]:
     def json_schema_extra() -> Generator:
         if customer_id:
             yield "customerId", customer_id
-            yield "organisationId", customer_id  # TODO: deprecated, remove in the future
         if customer_key:
             yield "customerKey", customer_key
-            yield "organisationKey", customer_key  # TODO: deprecated, remove in the future
 
     return Annotated[  # type: ignore
         conlist(ContactPerson, min_length=min_items, max_length=max_items),
         BeforeValidator(remove_empty_items),
         Field(json_schema_extra=dict(json_schema_extra())),
     ]
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/validators/customer_id.py` & `orchestrator_core-2.2.0/orchestrator/targets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-# Copyright 2019-2023 SURF.
+# Copyright 2019-2020 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Annotated
 
-from pydantic import Field
+import strawberry
 
-CustomerId = Annotated[str, Field(json_schema_extra={"format": "customerId"})]
+from orchestrator.types import strEnum
+
+
+@strawberry.enum
+class Target(strEnum):
+    CREATE = "CREATE"
+    MODIFY = "MODIFY"
+    TERMINATE = "TERMINATE"
+    SYSTEM = "SYSTEM"
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/validators/display_subscription.py` & `orchestrator_core-2.2.0/orchestrator/workflows/removed_workflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright 2019-2023 SURF.
+# Copyright 2019-2020 SURF.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Annotated
-from uuid import UUID
 
-from pydantic import Field
 
-DisplaySubscription = Annotated[
-    UUID, Field(frozen=True, json_schema_extra={"format": "subscription", "type": "string"})
-]
+from orchestrator.workflow import StepList, workflow
+
+
+# This workflow has been made to create the initial import process for a SN7 subscription
+# it does not do anything but is needed for the correct showing in the GUI.
+@workflow("Dummy workflow to replace removed workflows")
+def removed_workflow() -> StepList:
+    return StepList()
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/forms/validators/product_id.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/product_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/__init__.py` & `orchestrator_core-2.2.0/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/autoregistration.py` & `orchestrator_core-2.2.0/orchestrator/graphql/autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-2.2.0/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-2.2.0/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/extensions/error_handler_extension.py` & `orchestrator_core-2.2.0/orchestrator/graphql/extensions/error_handler_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/pagination.py` & `orchestrator_core-2.2.0/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/__init__.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/customer.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/helpers.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,8 +92,10 @@
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_processes = []
     if is_querying_page_data(info):
         processes = rows_from_statement(stmt, ProcessTable)
         is_detailed = _is_process_detailed(info)
         graphql_processes = [ProcessType.from_pydantic(_enrich_process(process, is_detailed)) for process in processes]
-    return to_graphql_result_page(graphql_processes, first, after, total, process_sort_fields, process_filter_fields)
+    return to_graphql_result_page(
+        graphql_processes, first, after, total, process_sort_fields(), process_filter_fields()
+    )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from sqlalchemy import func, select
 
 from orchestrator.db import db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.product import PRODUCT_TABLE_COLUMN_CLAUSES, filter_products, product_filter_fields
 from orchestrator.db.models import ProductTable
 from orchestrator.db.range.range import apply_range_to_statement
+from orchestrator.db.sorting import Sort
 from orchestrator.db.sorting.product import product_sort_fields, sort_products
-from orchestrator.db.sorting.sorting import Sort
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers.helpers import rows_from_statement
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils import create_resolver_error_handler, is_querying_page_data, to_graphql_result_page
 from orchestrator.utils.search_query import create_sqlalchemy_select
 
@@ -50,8 +50,8 @@
     total = db.session.scalar(select(func.count()).select_from(stmt.subquery()))
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_products = []
     if is_querying_page_data(info):
         products = rows_from_statement(stmt, ProductTable, unique=True)
         graphql_products = [ProductType.from_pydantic(p) for p in products]
-    return to_graphql_result_page(graphql_products, first, after, total, product_sort_fields, product_filter_fields)
+    return to_graphql_result_page(graphql_products, first, after, total, product_sort_fields(), product_filter_fields())
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/product_block.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/product_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from orchestrator.db.filters.product_block import (
     PRODUCT_BLOCK_TABLE_COLUMN_CLAUSES,
     filter_product_blocks,
     product_block_filter_fields,
 )
 from orchestrator.db.models import ProductBlockTable
 from orchestrator.db.range.range import apply_range_to_statement
+from orchestrator.db.sorting import Sort
 from orchestrator.db.sorting.product_block import product_block_sort_fields, sort_product_blocks
-from orchestrator.db.sorting.sorting import Sort
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers.helpers import rows_from_statement
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils import create_resolver_error_handler, is_querying_page_data, to_graphql_result_page
 from orchestrator.utils.search_query import create_sqlalchemy_select
 
@@ -57,9 +57,9 @@
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_product_blocks = []
     if is_querying_page_data(info):
         product_blocks = rows_from_statement(stmt, ProductBlockTable)
         graphql_product_blocks = [ProductBlock.from_pydantic(p) for p in product_blocks]
     return to_graphql_result_page(
-        graphql_product_blocks, first, after, total, product_block_sort_fields, product_block_filter_fields
+        graphql_product_blocks, first, after, total, product_block_sort_fields(), product_block_filter_fields()
     )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/resource_type.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/resource_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from orchestrator.db.filters.resource_type import (
     RESOURCE_TYPE_TABLE_COLUMN_CLAUSES,
     filter_resource_types,
     resource_type_filter_fields,
 )
 from orchestrator.db.models import ResourceTypeTable
 from orchestrator.db.range import apply_range_to_statement
+from orchestrator.db.sorting import Sort
 from orchestrator.db.sorting.resource_type import resource_type_sort_fields, sort_resource_types
-from orchestrator.db.sorting.sorting import Sort
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers.helpers import rows_from_statement
 from orchestrator.graphql.schemas.resource_type import ResourceType
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils import create_resolver_error_handler, is_querying_page_data, to_graphql_result_page
 from orchestrator.utils.search_query import create_sqlalchemy_select
 
@@ -56,9 +56,9 @@
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_resource_types = []
     if is_querying_page_data(info):
         resource_types = rows_from_statement(stmt, ResourceTypeTable)
         graphql_resource_types = [ResourceType.from_pydantic(p) for p in resource_types]
     return to_graphql_result_page(
-        graphql_resource_types, first, after, total, resource_type_sort_fields, resource_type_filter_fields
+        graphql_resource_types, first, after, total, resource_type_sort_fields(), resource_type_filter_fields()
     )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import cast
+from uuid import UUID
 
 import structlog
 from pydantic.alias_generators import to_camel as to_lower_camel
 from sqlalchemy import Select, func, select
 
 from orchestrator.db import ProductTable, SubscriptionTable, db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.subscription import (
     filter_by_query_string,
     filter_subscriptions,
     subscription_filter_fields,
 )
 from orchestrator.db.range import apply_range_to_statement
 from orchestrator.db.sorting import Sort
-from orchestrator.db.sorting.subscription import sort_subscriptions, subscription_sort_fields
+from orchestrator.db.sorting.subscription import (
+    sort_subscriptions,
+    subscription_sort_fields,
+)
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.schemas.product import ProductModelGraphql
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils import (
     create_resolver_error_handler,
@@ -69,14 +73,24 @@
 def format_base_subscription(subscription: SubscriptionTable) -> SubscriptionInterface:
     from orchestrator.graphql import GRAPHQL_MODELS
 
     strawberry_type = GRAPHQL_MODELS["subscription"]
     return strawberry_type.from_pydantic(subscription)
 
 
+async def resolve_subscription(info: OrchestratorInfo, id: UUID) -> SubscriptionInterface | None:
+    stmt = select(SubscriptionTable).where(SubscriptionTable.subscription_id == id)
+
+    if subscription := db.session.scalar(stmt):
+        if _is_subscription_detailed(info):
+            return get_subscription_details(subscription)
+        return format_base_subscription(subscription)
+    return None
+
+
 async def resolve_subscriptions(
     info: OrchestratorInfo,
     filter_by: list[GraphqlFilter] | None = None,
     sort_by: list[GraphqlSort] | None = None,
     first: int = 10,
     after: int = 0,
     query: str | None = None,
@@ -88,15 +102,14 @@
     logger.debug(
         "resolve_subscription() called",
         range=[after, after + first],
         sort=sort_by,
         filter=pydantic_filter_by,
         query=query,
     )
-
     stmt = select(SubscriptionTable).join(ProductTable)
 
     stmt = filter_subscriptions(stmt, pydantic_filter_by, _error_handler)
     if query is not None:
         stmt = filter_by_query_string(stmt, query)
 
     stmt = cast(Select, sort_subscriptions(stmt, pydantic_sort_by, _error_handler))
@@ -106,10 +119,12 @@
     graphql_subscriptions = []
     if is_querying_page_data(info):
         subscriptions = db.session.scalars(stmt).all()
         if _is_subscription_detailed(info):
             graphql_subscriptions = [get_subscription_details(p) for p in subscriptions]
         else:
             graphql_subscriptions = [format_base_subscription(p) for p in subscriptions]
+    logger.info("Resolve subscriptions", filter_by=filter_by, total=graphql_subscriptions)
+
     return to_graphql_result_page(
-        graphql_subscriptions, first, after, total, subscription_sort_fields, subscription_filter_fields
+        graphql_subscriptions, first, after, total, subscription_sort_fields(), subscription_filter_fields()
     )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/resolvers/workflow.py` & `orchestrator_core-2.2.0/orchestrator/graphql/resolvers/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy.orm import selectinload
 
 from orchestrator.db import db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.workflow import WORKFLOW_TABLE_COLUMN_CLAUSES, filter_workflows, workflow_filter_fields
 from orchestrator.db.models import WorkflowTable
 from orchestrator.db.range.range import apply_range_to_statement
-from orchestrator.db.sorting.sorting import Sort
+from orchestrator.db.sorting import Sort
 from orchestrator.db.sorting.workflow import sort_workflows, workflow_sort_fields
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers.helpers import rows_from_statement
 from orchestrator.graphql.schemas.workflow import Workflow
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils import create_resolver_error_handler, is_querying_page_data, to_graphql_result_page
 from orchestrator.utils.search_query import create_sqlalchemy_select
@@ -52,8 +52,10 @@
 
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_workflows = []
     if is_querying_page_data(info):
         workflows = rows_from_statement(stmt, WorkflowTable, unique=True)
         graphql_workflows = [Workflow.from_pydantic(p) for p in workflows]
-    return to_graphql_result_page(graphql_workflows, first, after, total, workflow_sort_fields, workflow_filter_fields)
+    return to_graphql_result_page(
+        graphql_workflows, first, after, total, workflow_sort_fields(), workflow_filter_fields()
+    )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schema.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     resolve_product_blocks,
     resolve_products,
     resolve_resource_types,
     resolve_settings,
     resolve_subscriptions,
     resolve_workflows,
 )
+from orchestrator.graphql.resolvers.subscription import resolve_subscription
 from orchestrator.graphql.schemas import GRAPHQL_MODELS
 from orchestrator.graphql.schemas.customer import CustomerType
 from orchestrator.graphql.schemas.process import ProcessType
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.schemas.resource_type import ResourceType
 from orchestrator.graphql.schemas.settings import StatusType
@@ -73,14 +74,17 @@
     )
     resource_types: Connection[ResourceType] = authenticated_field(
         resolver=resolve_resource_types, description="Returns list of resource types"
     )
     workflows: Connection[Workflow] = authenticated_field(
         resolver=resolve_workflows, description="Returns list of workflows"
     )
+    subscription: SubscriptionInterface | None = authenticated_field(
+        resolver=resolve_subscription, description="Returns a single Subscription"
+    )
     subscriptions: Connection[SubscriptionInterface] = authenticated_field(
         resolver=resolve_subscriptions, description="Returns list of subscriptions"
     )
     settings: StatusType = authenticated_field(
         resolver=resolve_settings,
         description="Returns information about cache, workers, and global engine settings",
     )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/__init__.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/product.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/resource_type.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,14 @@
 
     @strawberry.field(description="Return all products block instances of a subscription")  # type: ignore
     async def product_block_instances(
         self, tags: list[str] | None = None, resource_types: list[str] | None = None
     ) -> list[ProductBlockInstance]:
         return await get_subscription_product_blocks(self.subscription_id, tags, resource_types)
 
-    @strawberry.field(description="Return all products blocks that are part of a subscription", deprecation_reason="changed to product_block_instances")  # type: ignore
-    async def product_blocks(
-        self, tags: list[str] | None = None, resource_types: list[str] | None = None
-    ) -> list[ProductBlockInstance]:
-        return await get_subscription_product_blocks(self.subscription_id, tags, resource_types)
-
     @strawberry.field(description="Return fixed inputs")  # type: ignore
     async def fixed_inputs(self) -> strawberry.scalars.JSON:
         fixed_inputs = get_fixed_inputs(filters=[FixedInputTable.product_id == self.product.product_id])  # type: ignore
         return [{"field": fi.name, "value": fi.value} for fi in fixed_inputs]
 
     @authenticated_field(description="Returns list of processes of the subscription")  # type: ignore
     async def processes(
@@ -111,15 +105,15 @@
 
         in_use_by_query = query_in_use_by_subscriptions(self.subscription_id)
         query_results = in_use_by_query.with_entities(SubscriptionTable.subscription_id).all()
         subscription_ids = [str(s.subscription_id) for s in query_results]
         if not subscription_ids:
             return EMPTY_PAGE
         filter_by_with_related_subscriptions = (filter_by or []) + [
-            GraphqlFilter(field="subscriptionIds", value=",".join(subscription_ids))
+            GraphqlFilter(field="subscriptionId", value="|".join(subscription_ids))
         ]
         return await resolve_subscriptions(info, filter_by_with_related_subscriptions, sort_by, first, after)
 
     @authenticated_field(description="Returns list of subscriptions that this subscription depends on")  # type: ignore
     async def depends_on_subscriptions(
         self,
         info: OrchestratorInfo,
@@ -133,15 +127,15 @@
 
         depends_on_query = query_depends_on_subscriptions(self.subscription_id)
         query_results = depends_on_query.with_entities(SubscriptionTable.subscription_id).all()
         subscription_ids = [str(s.subscription_id) for s in query_results]
         if not subscription_ids:
             return EMPTY_PAGE
         filter_by_with_related_subscriptions = (filter_by or []) + [
-            GraphqlFilter(field="subscriptionIds", value=",".join(subscription_ids))
+            GraphqlFilter(field="subscriptionId", value="|".join(subscription_ids))
         ]
         return await resolve_subscriptions(info, filter_by_with_related_subscriptions, sort_by, first, after)
 
     @strawberry.field(description="Returns customer of a subscription")  # type: ignore
     def customer(self) -> CustomerType:
         return CustomerType(
             customer_id=app_settings.DEFAULT_CUSTOMER_IDENTIFIER,
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/schemas/workflow.py` & `orchestrator_core-2.2.0/orchestrator/graphql/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/types.py` & `orchestrator_core-2.2.0/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/__init__.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/get_subscription_product_blocks.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/get_subscription_product_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,14 @@
     id: int
     parent: int | None
     subscription_instance_id: UUID
     owner_subscription_id: UUID
     in_use_by_relations: list[JSON]
     product_block_instance_values: JSON
 
-    @strawberry.field(description="Returns all resource types of a product block", deprecation_reason="changed to product_block_instance_values")  # type: ignore
-    async def resource_types(self) -> JSON:
-        return {v["field"]: v["value"] for v in self.product_block_instance_values}
-
 
 def is_product_block(candidate: Any) -> bool:
     if isinstance(candidate, dict):
         # TODO: also filter on tag (needs addition of tag in orchestrator endpoint)
         # NOTE: this crosses subscription boundaries. If needed we can add an additional filter to limit that.
         return candidate.get("owner_subscription_id", None)
     return False
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/is_query_detailed.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/override_class.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/graphql/utils/to_graphql_result_page.py` & `orchestrator_core-2.2.0/orchestrator/graphql/utils/to_graphql_result_page.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/alembic.ini` & `orchestrator_core-2.2.0/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/env.py` & `orchestrator_core-2.2.0/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/helpers.py` & `orchestrator_core-2.2.0/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-2.2.0/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-2.2.0/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py` & `orchestrator_core-2.2.0/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/__init__.py` & `orchestrator_core-2.2.0/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-2.2.0/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/scheduling.py` & `orchestrator_core-2.2.0/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-2.2.0/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/validate_products.py` & `orchestrator_core-2.2.0/orchestrator/schedules/validate_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 
 
 @scheduler(name="Validate Products and inactive subscriptions", time_unit="day", at="02:30")
 def validate_products() -> None:
     uncompleted_products = db.session.scalar(
         select(func.count())
         .select_from(ProcessTable)
-        .filter(ProcessTable.workflow_name == "validate_products", ProcessTable.last_status != "completed")
+        .filter(ProcessTable.workflow.name == "validate_products", ProcessTable.last_status != "completed")
     )
     if not uncompleted_products:
         start_process("task_validate_products")
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-2.2.0/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/__init__.py` & `orchestrator_core-2.2.0/orchestrator/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     GlobalStatusEnum,
     WorkerStatus,
 )
 from orchestrator.schemas.fixed_input import FixedInputConfigurationSchema, FixedInputSchema
 from orchestrator.schemas.problem_detail import ProblemDetailSchema
 from orchestrator.schemas.process import (
     ProcessBaseSchema,
-    ProcessDeprecationsSchema,
     ProcessIdSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessStatusCounts,
     ProcessSubscriptionBaseSchema,
     ProcessSubscriptionSchema,
     Reporter,
@@ -57,15 +56,14 @@
     "ProductCRUDSchema",
     "ProductBaseSchema",
     "ProductSchema",
     "ProcessSubscriptionSchema",
     "ProcessResumeAllSchema",
     "ProcessBaseSchema",
     "ProcessSchema",
-    "ProcessDeprecationsSchema",
     "ProcessIdSchema",
     "ProcessSubscriptionBaseSchema",
     "StepSchema",
     "SubscriptionDescriptionBaseSchema",
     "SubscriptionDescriptionSchema",
     "SubscriptionSchema",
     "SubscriptionDomainModelSchema",
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/base.py` & `orchestrator_core-2.2.0/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/engine_settings.py` & `orchestrator_core-2.2.0/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/fixed_input.py` & `orchestrator_core-2.2.0/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/problem_detail.py` & `orchestrator_core-2.2.0/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/process.py` & `orchestrator_core-2.2.0/orchestrator/schemas/process.py`

 * *Files 22% similar despite different names*

```diff
@@ -50,47 +50,32 @@
     status: str
     created_by: str | None = None
     executed: datetime | None = None
     commit_hash: str | None = None
     state: dict[str, Any] | None = None
     state_delta: dict[str, Any] | None = None
 
-    stepid: UUID | None = None  # TODO: will be removed in 1.4
-
 
 class ProcessSchema(ProcessBaseSchema):
     product_id: UUID | None = None
     customer_id: str | None = None
     workflow_target: Target | None = None
     subscriptions: list[SubscriptionSchema]
     current_state: dict[str, Any] | None = None
     steps: list[ProcessStepSchema] | None = None
     form: dict[str, Any] | None = None
 
 
-class ProcessDeprecationsSchema(ProcessSchema):
-    id: UUID | None = None  # TODO: will be removed in 1.4
-    pid: UUID | None = None  # TODO: will be removed in 1.4
-    workflow: str | None = None  # TODO: will be removed in 1.4
-    status: ProcessStatus | None = None  # TODO: will be removed in 1.4
-    step: str | None = None  # TODO: will be removed in 1.4
-    started: datetime | None = None  # TODO: will be removed in 1.4
-    last_modified: datetime | None = None  # TODO: will be removed in 1.4
-    product: UUID | None = None  # TODO: will be removed in 1.4
-    customer: str | None = None  # TODO: will be removed in 1.4
-
-
 class ProcessSubscriptionBaseSchema(OrchestratorBaseModel):
     id: UUID
     process_id: UUID
     subscription_id: UUID
     workflow_target: Target | None = None
     created_at: datetime
 
-    pid: UUID  # TODO: will be removed in 1.4
     model_config = ConfigDict(from_attributes=True)
 
 
 class ProcessSubscriptionSchema(ProcessSubscriptionBaseSchema):
     process: ProcessBaseSchema
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/product.py` & `orchestrator_core-2.2.0/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/product_block.py` & `orchestrator_core-2.2.0/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/resource_type.py` & `orchestrator_core-2.2.0/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/subscription.py` & `orchestrator_core-2.2.0/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-2.2.0/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/schemas/workflow.py` & `orchestrator_core-2.2.0/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/security.py` & `orchestrator_core-2.2.0/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/__init__.py` & `orchestrator_core-2.2.0/orchestrator/forms/validators/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/celery.py` & `orchestrator_core-2.2.0/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/fixed_inputs.py` & `orchestrator_core-2.2.0/orchestrator/services/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/processes.py` & `orchestrator_core-2.2.0/orchestrator/services/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,15 @@
             raise ValueError(step.status)
 
         result.append(process)
     return result
 
 
 def load_process(process: ProcessTable) -> ProcessStat:
-    workflow = get_workflow(str(process.workflow_name))
+    workflow = get_workflow(str(process.workflow.name))
 
     if not workflow:
         workflow = removed_workflow
 
     log = _restore_log(process.steps)
     pstate, remaining = _recoverwf(workflow, log)
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/products.py` & `orchestrator_core-2.2.0/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/resource_types.py` & `orchestrator_core-2.2.0/orchestrator/services/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/settings.py` & `orchestrator_core-2.2.0/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/subscriptions.py` & `orchestrator_core-2.2.0/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/tasks.py` & `orchestrator_core-2.2.0/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/translations.py` & `orchestrator_core-2.2.0/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/services/workflows.py` & `orchestrator_core-2.2.0/orchestrator/services/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/settings.py` & `orchestrator_core-2.2.0/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/types.py` & `orchestrator_core-2.2.0/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/__init__.py` & `orchestrator_core-2.2.0/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/crypt.py` & `orchestrator_core-2.2.0/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/datetime.py` & `orchestrator_core-2.2.0/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/docs.py` & `orchestrator_core-2.2.0/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/enrich_process.py` & `orchestrator_core-2.2.0/orchestrator/utils/enrich_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,28 +97,20 @@
         "product_id": subscriptions[0]["product"]["product_id"] if subscriptions else None,
         "customer_id": subscriptions[0]["customer_id"] if subscriptions else None,
         "assignee": process.assignee,
         "last_status": process.last_status,
         "last_step": process.last_step,
         "is_task": process.is_task,
         "workflow_id": process.workflow_id,
-        "workflow_name": process.workflow_name,
+        "workflow_name": process.workflow.name,
         "workflow_target": process.process_subscriptions[0].workflow_target if process.process_subscriptions else None,
         "failed_reason": process.failed_reason,
         "created_by": process.created_by,
         "started_at": process.started_at,
         "traceback": process.traceback,
         "last_modified_at": process.last_modified_at,
         "product": subscriptions[0]["product"] if subscriptions else None,
         "subscriptions": subscriptions,
         "steps": None,
         "form": None,
         "current_state": None,
-        "id": process.process_id,  # TODO: will be removed in 1.4
-        "pid": process.process_id,  # TODO: will be removed in 1.4
-        "workflow": process.workflow_name,  # TODO: will be removed in 1.4
-        "status": process.last_status,  # TODO: will be removed in 1.4
-        "step": process.last_step,  # TODO: will be removed in 1.4
-        "started": process.started_at,  # TODO: will be removed in 1.4
-        "last_modified": process.last_modified_at,  # TODO: will be removed in 1.4
-        "customer": subscriptions[0]["customer_id"] if subscriptions else None,  # TODO: will be removed in 1.4
     } | details
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/errors.py` & `orchestrator_core-2.2.0/orchestrator/utils/errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # limitations under the License.
 
 from functools import singledispatch
 from http import HTTPStatus
 from typing import Any, cast
 
 import structlog
-from deprecated import deprecated
 
 from nwastdlib.ex import show_ex
 from orchestrator.types import JSON, ErrorDict
 
 logger = structlog.get_logger(__name__)
 
 
@@ -67,32 +66,18 @@
 
     def __init__(self, message: str, details: JSON = None) -> None:
         super().__init__(message, details)
         self.message = message
         self.details = details
 
 
-@deprecated(
-    "Renamed the error 'ProcessFailure', `from orchestrator.errors import ProcessFailureError` removing in version 1.3.0"
-)
-class ProcessFailure(ProcessFailureError):  # noqa: N818
-    pass
-
-
 class InconsistentDataError(ProcessFailureError):
     pass
 
 
-@deprecated(
-    "Renamed the error 'InconsistentDataError', `from orchestrator.errors import InconsistentDataError` removing in version 1.3.0"
-)
-class InconsistentData(InconsistentDataError):  # noqa: N818
-    pass
-
-
 def is_api_exception(ex: Exception) -> bool:
     """Test for swagger-codegen ApiException.
 
     For each API, swagger-codegen generates a new ApiException class. These are not organized into
     a hierarchy. Hence, testing whether one is dealing with one of the ApiException classes without knowing how
     many there are and where they are located, needs some special logic.
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/functional.py` & `orchestrator_core-2.2.0/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/get_updated_properties.py` & `orchestrator_core-2.2.0/orchestrator/utils/get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/helpers.py` & `orchestrator_core-2.2.0/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/json.py` & `orchestrator_core-2.2.0/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/redis.py` & `orchestrator_core-2.2.0/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/search_query.py` & `orchestrator_core-2.2.0/orchestrator/utils/search_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,19 +359,22 @@
 
 
 class SQLAlchemyVisitor:
     def __init__(
         self,
         stmt: Select,
         mappings: dict[str, WhereCondGenerator],
-        base_table: type[BaseModel],
-        join_key: MappedColumn | InstrumentedAttribute,
+        *,
+        base_table: type[BaseModel] | None = None,
+        join_key: MappedColumn | InstrumentedAttribute | None = None,
     ):
         self.base_stmt = stmt
         self.mappings = mappings
+        # base_table and join_key are required for group terms, because of the union join
+        # If the query does not use grouping, these parameters are optional
         self.base_table = base_table
         self.join_key = join_key
 
     def visit_kv_term(self, stmt: Select, node: Node, is_negated: bool) -> Select:
         key_node, value_node = node[1]
         if key_node[0] == "Word":
             cond_expr_fn = self.mappings.get(camel_to_snake(key_node[1]))
@@ -394,14 +397,17 @@
 
     def visit_search_word(self, stmt: Select, node: Node, is_negated: bool) -> Select:
         # The dynamically generated list of expression may not be empty, so we prepend with a "default" False
         or_expr = or_(False, *(cond_expr_fn(node) for cond_expr_fn in self.mappings.values()))
         return stmt.where(or_expr if not is_negated else not_(or_expr))
 
     def visit_group(self, stmt: Select, node: Node, is_negated: bool) -> Select:
+        if self.join_key is None or self.base_table is None:
+            logger.error("Group statements not supported without a base_table and a join_key")
+            return stmt
         subquery = self.visit_query(self.base_stmt, node).cte()
         if is_negated:
             return stmt.outerjoin_from(
                 self.base_table, subquery, self.join_key == subquery.c[self.join_key.name]
             ).where(subquery.c[self.join_key.name].is_(None))
         return stmt.join_from(self.base_table, subquery, self.join_key == subquery.c[self.join_key.name])
 
@@ -442,8 +448,10 @@
 def create_sqlalchemy_select(
     stmt: Select,
     search_query: str,
     mappings: dict[str, WhereCondGenerator],
     base_table: type[BaseModel],
     join_key: MappedColumn | InstrumentedAttribute,
 ) -> Select | CompoundSelect:
-    return SQLAlchemyVisitor(stmt, mappings, base_table, join_key).visit(Parser(Lexer(search_query).lex()).parse())
+    return SQLAlchemyVisitor(stmt, mappings, base_table=base_table, join_key=join_key).visit(
+        Parser(Lexer(search_query).lex()).parse()
+    )
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/state.py` & `orchestrator_core-2.2.0/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/strings.py` & `orchestrator_core-2.2.0/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/utils/vlans.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_health.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from __future__ import annotations
 
-import warnings
+from http import HTTPStatus
+from unittest import mock
 
-from nwastdlib.vlans import VlanRanges
+from sqlalchemy.exc import OperationalError
 
-__all__ = [
-    "VlanRanges",
-]
-
-warnings.warn(
-    "VlanRanges will be removed from orchestrator-core in an upcoming release. "
-    "Please import it from nwastdlib (>= 1.5.0) instead.",
-    DeprecationWarning,
-    stacklevel=1,
-)
+
+def test_get_health(test_client):
+    response = test_client.get("/api/health/")
+    assert HTTPStatus.OK == response.status_code
+    assert response.json() == "OK"
+
+
+@mock.patch("orchestrator.db.db.session")
+def test_get_health_no_connection(mock_session, test_client):
+    mock_session.execute.side_effect = OperationalError("THIS", "IS", "KABOOM")
+    response = test_client.get("/api/health/")
+    assert response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/version.py` & `orchestrator_core-2.2.0/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/websocket/__init__.py` & `orchestrator_core-2.2.0/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-2.2.0/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-2.2.0/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-2.2.0/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflow.py` & `orchestrator_core-2.2.0/orchestrator/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     overload,
     runtime_checkable,
 )
 from uuid import UUID
 
 import strawberry
 import structlog
-from deprecated import deprecated
 from structlog.contextvars import bound_contextvars
 from structlog.stdlib import BoundLogger
 
 from nwastdlib import const, identity
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import db, transactional
 from orchestrator.services.settings import get_engine_settings
@@ -486,19 +485,14 @@
 class ProcessStat:
     process_id: UUID
     workflow: Workflow
     state: Process
     log: StepList
     current_user: str
 
-    @property
-    @deprecated("Changed to 'process_id' from version 1.2.3, will be removed in 1.4")
-    def pid(self) -> UUID:
-        return self.process_id
-
     def update(self, **vs: Any) -> ProcessStat:
         """Update ProcessStat.
 
         >>> pstat = ProcessStat('', None, {}, [], "")
         >>> pstat.update(state={"a": "b"})
         ProcessStat(process_id='', workflow=None, state={'a': 'b'}, log=[], current_user='')
         """
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/__init__.py` & `orchestrator_core-2.2.0/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/modify_note.py` & `orchestrator_core-2.2.0/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/steps.py` & `orchestrator_core-2.2.0/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-2.2.0/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-2.2.0/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-2.2.0/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-2.2.0/orchestrator/workflows/tasks/validate_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from more_itertools.more import one
 from more_itertools.recipes import first_true
 from pydantic import ValidationError
 from sqlalchemy import not_, select
 from sqlalchemy.orm import joinedload
 
 import orchestrator.workflows
-from orchestrator.api.api_v1.endpoints.fixed_input import fi_configuration
 from orchestrator.db import FixedInputTable, ProductTable, SubscriptionTable, WorkflowTable, db
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.services import products
 from orchestrator.services.products import get_products
 from orchestrator.services.translations import generate_translations
 from orchestrator.services.workflows import get_workflow_by_name, get_workflows
 from orchestrator.targets import Target
 from orchestrator.types import State
 from orchestrator.utils.errors import ProcessFailureError
+from orchestrator.utils.fixed_inputs import fixed_input_configuration as fi_configuration
 from orchestrator.workflow import StepList, done, init, step, workflow
 
 # Since these errors are probably programming failures we should not throw AssertionErrors
 
 
 @step("Check all workflows in database")
 def check_all_workflows_are_in_db() -> State:
```

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-2.2.0/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/orchestrator/workflows/utils.py` & `orchestrator_core-2.2.0/orchestrator/workflows/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
         user_input = yield _generate_modify_form(workflow_target, workflow_name)
 
         subscription = SubscriptionTable.query.get(user_input.subscription_id)
 
         begin_state = {
             "subscription_id": str(subscription.subscription_id),
             "product": str(subscription.product_id),
-            "organisation": subscription.customer_id,  # TODO: deprecated, remove in the future
             "customer_id": subscription.customer_id,
         }
 
         if initial_input_form is None:
             return begin_state
 
         form = form_inject_args(initial_input_form)({**state, **begin_state})
```

### Comparing `orchestrator_core-2.1.2rc4/pyproject.toml` & `orchestrator_core-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,29 @@
     "deprecated",
     "deepmerge==1.1.1",
     "fastapi~=0.110.0",
     "fastapi-etag==0.4.0",
     "more-itertools~=10.2.0",
     "itsdangerous",
     "Jinja2==3.1.3",
-    "orjson==3.9.15",
+    "orjson==3.10.0",
     "psycopg2-binary==2.9.9",
     "pydantic[email]~=2.5.1",
     "pydantic-settings~=2.2.1",
     "python-dateutil==2.8.2",
     "python-rapidjson>=1.9,<1.17",
     "pytz==2024.1",
     "redis==5.0.3",
     "schedule==1.1.0",
-    "sentry-sdk[fastapi]==1.43.0",
-    "SQLAlchemy==2.0.28",
+    "sentry-sdk[fastapi]==1.44.0",
+    "SQLAlchemy==2.0.29",
     "SQLAlchemy-Utils==0.41.2",
     "structlog",
-    "typer==0.9.0",
-    "uvicorn[standard]~=0.28.0",
+    "typer==0.12.0",
+    "uvicorn[standard]~=0.29.0",
     "nwa-stdlib~=1.7.0",
     "oauth2-lib~=1.5.0",
     "tabulate==0.9.0",
     "strawberry-graphql==0.210.0",
     "pydantic-forms==1.0.2",
     "ruff",
 ]
```

### Comparing `orchestrator_core-2.1.2rc4/setup.cfg` & `orchestrator_core-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/setup.py` & `orchestrator_core-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/conftest.py` & `orchestrator_core-2.2.0/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-2.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/acceptance_tests/test_test_product.py` & `orchestrator_core-2.2.0/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_caching.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_helpers.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_models.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_processes.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -398,69 +398,60 @@
 
 
 def test_processes_filterable(test_client, mocked_processes, generic_subscription_2, generic_subscription_1):
     response = test_client.get("/api/processes/")
     assert HTTPStatus.OK == response.status_code
     processes = response.json()
 
-    assert 9 == len(processes)
+    assert len(processes) == 9
     assert "workflow_for_testing_processes_py", processes[0]["workflow"]
 
     response = test_client.get("/api/processes?filter=lastStatus,completed")
-    assert 3 == len(response.json())
+    assert len(response.json()) == 3
     response = test_client.get("/api/processes?filter=lastStatus,suspended")
-    assert 2 == len(response.json())
+    assert len(response.json()) == 2
     response = test_client.get("/api/processes?filter=lastStatus,resumed")
-    assert 2 == len(response.json())
+    assert len(response.json()) == 2
 
     product_name = db.session.get(SubscriptionTable, generic_subscription_1).product.name
     response = test_client.get(f"/api/processes?filter=product,{product_name}")
-    assert 4 == len(response.json())
+    assert len(response.json()) == 4
     response = test_client.get("/api/processes?sort=assignee,asc")
     assert response.json()[0]["assignee"] == "NOC"
-    response = test_client.get("/api/processes?sort=startedAt&filter=isTask,y")
-    assert 4 == len(response.json())
+    response = test_client.get("/api/processes?sort=startedAt&filter=isTask,true")
+    assert len(response.json()) == 4
 
 
 def test_processes_filterable_response_model(
     test_client, mocked_processes, generic_subscription_2, generic_subscription_1
 ):
     response = test_client.get("/api/processes/?sort=startedAt,asc")
     assert HTTPStatus.OK == response.status_code
     processes = response.json()
     assert len(processes) == 9
     process = processes[0]
 
     assert len(process["subscriptions"]) == 1
 
     # Check if the other fields are filled with correct data
-    del process["id"]  # skip process_id as it's dynamic
-    del process["pid"]  # skip process_id as it's dynamic
     del process["process_id"]  # skip process_id as it's dynamic
     del process["product_id"]  # skip product_id as it's dynamic
-    del process["product"]  # skip product as it's dynamic
     del process["workflow_id"]  # skip workflow_id as it's dynamic
     del process["subscriptions"]
     assert process == {
         "customer_id": "2f47f65a-0911-e511-80d0-005056956c1a",
-        "customer": "2f47f65a-0911-e511-80d0-005056956c1a",
-        "workflow": "workflow_for_testing_processes_py",
         "workflow_name": "workflow_for_testing_processes_py",
         "is_task": False,
         "assignee": "SYSTEM",
-        "status": "completed",
         "last_status": "completed",
-        "step": "Modify",
         "last_step": "Modify",
         "failed_reason": None,
         "traceback": None,
         "created_by": None,
-        "started": 1578994200.0,
         "started_at": 1578994200.0,
-        "last_modified": 1578994800.0,
         "last_modified_at": 1578994800.0,
         "current_state": None,
         "steps": None,
         "form": None,
         "workflow_target": "CREATE",
     }
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_products.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_settings.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_workflows.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/api/test_ws.py` & `orchestrator_core-2.2.0/test/unit_tests/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate.sh` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate.sh`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/alembic.ini` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/env.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_blocks/example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_blocks/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_blocks/example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_blocks/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_types/example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_types/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/products/product_types/example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/products/product_types/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/__init__.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/generate/workflows/shared.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/generate/workflows/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config1.yaml` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config1.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config2.yaml` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config2.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/data/product_config3.yaml` & `orchestrator_core-2.2.0/test/unit_tests/cli/data/product_config3.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/generator/test_enums.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/generator/test_enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_cli_generate.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/test_cli_generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_generate_code.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/test_generate_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-2.2.0/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/conftest.py` & `orchestrator_core-2.2.0/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base.py` & `orchestrator_core-2.2.0/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-2.2.0/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-2.2.0/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/domain/test_lifecycle.py` & `orchestrator_core-2.2.0/test/unit_tests/domain/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/processes.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-2.2.0/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_customer_contact_list.py` & `orchestrator_core-2.2.0/test/unit_tests/forms/test_customer_contact_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,34 +51,29 @@
             }
         },
         "additionalProperties": False,
         "properties": {
             "customer_contacts": {
                 "customerKey": "customer",
                 "items": {"$ref": "#/$defs/ContactPerson"},
-                "organisationKey": "customer",
                 "title": "Customer Contacts",
                 "type": "array",
             },
             "customer_contacts_customer": {
                 "customerId": customer_id_str,
                 "customerKey": "key",
                 "items": {"$ref": "#/$defs/ContactPerson"},
                 "minItems": 1,
-                "organisationId": customer_id_str,
-                "organisationKey": "key",
                 "title": "Customer Contacts Customer",
                 "type": "array",
             },
             "customer_contacts_customer2": {
                 "customerId": customer_id_str,
                 "customerKey": "foo",
                 "items": {"$ref": "#/$defs/ContactPerson"},
-                "organisationId": customer_id_str,
-                "organisationKey": "foo",
                 "title": "Customer Contacts Customer2",
                 "type": "array",
             },
         },
         "required": ["customer_contacts", "customer_contacts_customer", "customer_contacts_customer2"],
         "title": "unknown",
         "type": "object",
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_display_subscription.py` & `orchestrator_core-2.2.0/test/unit_tests/forms/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-2.2.0/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/conftest.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_customer.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,22 +403,19 @@
     processes = processes_data["page"]
     pageinfo = processes_data["pageInfo"]
 
     assert errors == [
         {
             "message": (
                 "Invalid filter arguments (invalid_filters=['test'] "
-                "valid_filter_keys=['assignee', 'createdBy', 'created_by', "
-                "'creator', 'customer', 'failedReason', 'failed_reason', "
-                "'isTask', 'is_task', 'istask', 'lastModifiedAt', 'lastStatus', "
-                "'lastStep', 'last_modified_at', 'last_status', 'last_step', "
-                "'processId', 'process_id', 'product', 'productTag', 'startedAt', "
-                "'started_at', 'status', 'subscriptionId', 'subscription_id', "
-                "'subscriptions', 'tag', 'target', 'traceback', 'workflowId', "
-                "'workflowName', 'workflow_id', 'workflow_name'])"
+                "valid_filter_keys=['assignee', 'createdBy', "
+                "'customer', 'failedReason', 'isTask', 'lastModifiedAt', 'lastStatus', "
+                "'lastStep', 'processId', 'product', 'productDescription', 'startedAt', "
+                "'subscriptionId', 'tag', 'target', 'traceback', 'workflowId', "
+                "'workflowName'])"
             ),
             "path": [None, "processes", "Query"],
             "extensions": {"error_type": "internal_error"},
         }
     ]
     assert pageinfo == {
         "hasPreviousPage": False,
@@ -431,18 +428,20 @@
     for process in processes:
         assert process["lastStatus"] == "COMPLETED"
 
 
 @pytest.mark.parametrize(
     "query_args,num_results",
     [
-        ({"query_string": "is_task:no", "first": 20}, 6),
-        ({"query_string": 'is_task:"yes"', "first": 20}, 13),
-        ({"query_string": "is_task:(y|n)", "first": 20}, 19),
+        ({"query_string": "isTask:no", "first": 20}, 0),
+        ({"filter_by": [{"field": "isTask", "value": "false"}], "first": 20}, 6),
+        ({"query_string": 'isTask:"true"', "first": 20}, 13),
+        ({"query_string": "isTask:(true|false)", "first": 20}, 19),
         ({"query_string": "nonsense"}, 0),
+        ({"filter_by": [{"field": "assignee", "value": ""}]}, 0),
         ({"query_string": None, "first": 100}, 19),
         ({"query_string": "one"}, 8),
         ({"query_string": "two"}, 7),
         ({"query_string": "product:(1 | 3)"}, 8),
         ({"query_string": "tag:gen1"}, 8),
         ({"query_string": "tag:gEN2"}, 7),
         ({"query_string": "-tag:gen*"}, 4),
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_product.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_product.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     product_names = [product["name"] for product in products]
     assert product_names == ["Product 2", "Product 3", "ProductSubListUnion", "ProductSubOne", "ProductSubTwo"]
 
 
 @pytest.mark.parametrize(
     "query_args",
     [
-        {"filter_by": [{"field": "product_blocks", "value": "PB_1-PB_3"}]},
+        {"filter_by": [{"field": "productBlock", "value": "PB_1|PB_3"}]},
         {"query_string": "product_block:(PB_1|PB_3)"},
         {"query_string": "productBlock:PB_1 | product_block:PB_3"},
     ],
 )
 def test_products_filter_by_product_block(
     test_client, generic_product_1, generic_product_2, generic_product_3, query_args
 ):
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_product_blocks.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_product_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     assert product_blocks[0]["name"] == "PB_2"
     assert product_blocks[1]["name"] == "PB_3"
 
 
 @pytest.mark.parametrize(
     "query_args",
     [
-        {"filter_by": [{"field": "resource_types", "value": "rt_1"}]},
+        {"filter_by": [{"field": "resourceType", "value": "rt_1"}]},
         {"query_string": "resourceType:rt_1"},
     ],
 )
 def test_product_blocks_filter_by_resource_types(test_client, query_args):
     data = get_product_blocks_query(**query_args, sort_by=[{"field": "name", "order": "ASC"}])
     response: Response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     assert HTTPStatus.OK == response.status_code
@@ -267,15 +267,15 @@
         "totalItems": 1,
     }
     assert product_blocks[0]["name"] == "PB_1"
 
 
 def test_product_blocks_filter_by_products(test_client):
     data = get_product_blocks_query(
-        filter_by=[{"field": "products", "value": "Product 1-Product 3"}],
+        filter_by=[{"field": "product", "value": "Product 1|Product 3"}],
         sort_by=[{"field": "name", "order": "ASC"}],
     )
     response: Response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     product_blocks_data = result["data"]["productBlocks"]
     product_blocks = product_blocks_data["page"]
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_resource_types.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_resource_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     }
     assert [rt["resourceType"] for rt in resource_types] == ["rt_1", "rt_2", "rt_3"]
 
 
 @pytest.mark.parametrize(
     "query_args",
     [
-        {"filter_by": [{"field": "productBlocks", "value": "PB_1"}]},
+        {"filter_by": [{"field": "productBlock", "value": "PB_1"}]},
         {"query_string": '"product_block":"PB_1"'},
         {"query_string": "productBlock:PB_1"},
         # {"query_string": "PB_1"}, Trouble comparing arbitrary text with UUID columns
     ],
 )
 def test_resource_types_filter_by_product_blocks(test_client, query_args):
     data = get_resource_types_query(**query_args, sort_by=[{"field": "resourceType", "order": "ASC"}])
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_sort_and_filter_fields.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_sort_and_filter_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,20 +47,20 @@
         }
     ).encode("utf-8")
 
 
 @pytest.mark.parametrize(
     "type_name, sort_fields, filter_fields",
     [
-        ("processes", process_sort_fields, process_filter_fields),
-        ("subscriptions", subscription_sort_fields, subscription_filter_fields),
-        ("products", product_sort_fields, product_filter_fields),
-        ("productBlocks", product_block_sort_fields, product_block_filter_fields),
-        ("workflows", workflow_sort_fields, workflow_filter_fields),
-        ("resourceTypes", resource_type_sort_fields, resource_type_filter_fields),
+        ("processes", process_sort_fields(), process_filter_fields()),
+        ("subscriptions", subscription_sort_fields(), subscription_filter_fields()),
+        ("products", product_sort_fields(), product_filter_fields()),
+        ("productBlocks", product_block_sort_fields(), product_block_filter_fields()),
+        ("workflows", workflow_sort_fields(), workflow_filter_fields()),
+        ("resourceTypes", resource_type_sort_fields(), resource_type_filter_fields()),
     ],
 )
 def test_process_sort_and_filter_fields_in_page_info(test_client, type_name, sort_fields, filter_fields):
     data = get_page_info_sort_and_filter_fields(type_name)
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     assert HTTPStatus.OK == response.status_code
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,21 +731,21 @@
     product_type_1_subscriptions_factory(30)
 
     data = get_subscriptions_query(first=1, filter_by=[{"field": "startDate", "value": "2023-05-24"}])
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     first_subscription = response.json()["data"]["subscriptions"]["page"][0]
 
     first_subscription_date = datetime.datetime.fromisoformat(first_subscription["startDate"])
-    higher_then_date = first_subscription_date.isoformat()
-    lower_then_date = (first_subscription_date + datetime.timedelta(days=3)).isoformat()
+    higher_than_date = first_subscription_date.isoformat()
+    lower_than_date = (first_subscription_date + datetime.timedelta(days=3)).isoformat()
 
     data = get_subscriptions_query(
         filter_by=[
-            {"field": "startDateGte", "value": higher_then_date},
-            {"field": "startDateLte", "value": lower_then_date},
+            {"field": "startDate", "value": f">={higher_than_date}"},
+            {"field": "startDate", "value": f"<={lower_than_date}"},
         ]
     )
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
@@ -760,15 +760,15 @@
         "hasNextPage": False,
         "startCursor": 0,
         "endCursor": 3,
         "totalItems": 4,
     }
 
     for subscription in subscriptions:
-        assert higher_then_date <= subscription["startDate"] <= lower_then_date
+        assert higher_than_date <= subscription["startDate"] <= lower_than_date
 
 
 def test_subscriptions_filtering_with_invalid_filter(
     test_client, product_type_1_subscriptions_factory, generic_product_type_1
 ):
     # when
 
@@ -799,20 +799,16 @@
     subscriptions = subscriptions_data["page"]
     pageinfo = subscriptions_data["pageInfo"]
 
     assert errors == [
         {
             "message": (
                 "Invalid filter arguments (invalid_filters=['test'] "
-                "valid_filter_keys=['description', 'endDate', 'endDateGt', "
-                "'endDateGte', 'endDateLt', 'endDateLte', 'endDateNe', 'insync', "
-                "'note', 'product', 'startDate', 'startDateGt', 'startDateGte', "
-                "'startDateLt', 'startDateLte', 'startDateNe', 'status', "
-                "'statuses', 'subscriptionId', 'subscriptionIds', 'tag', 'tags', "
-                "'tsv'])"
+                "valid_filter_keys=['customerId', 'description', 'endDate', 'insync', "
+                "'note', 'product', 'productId', 'startDate', 'status', 'subscriptionId', 'tag'])"
             ),
             "path": [None, "subscriptions", "Query"],
             "extensions": {"error_type": "internal_error"},
         }
     ]
     assert pageinfo == {
         "hasPreviousPage": False,
@@ -830,34 +826,40 @@
     "query_args",
     [
         lambda sid: {"filter_by": [{"field": "subscriptionId", "value": sid}]},
         lambda sid: {"query_string": f"subscription_id:{sid}"},
         lambda sid: {"query_string": f"subscriptionId:{sid}"},
         lambda sid: {"query_string": f"{sid}"},
         lambda sid: {"query_string": f"{sid.split('-')[0]}"},
+        lambda sid: {"filter_by": [{"field": "customerId", "value": CUSTOMER_ID.split("-")[0]}]},
+        lambda sid: {"query_string": CUSTOMER_ID.split("-")[0]},
     ],
 )
 def test_single_subscription(test_client, product_type_1_subscriptions_factory, generic_product_type_1, query_args):
-    # when
+    # given
 
     _, GenericProductOne = generic_product_type_1
     subscription_ids = product_type_1_subscriptions_factory(30)
 
-    do_refresh_subscriptions_search_view()
-
     subscription_id = subscription_ids[10]
     subscription = db.session.execute(
         select(SubscriptionTable).filter(SubscriptionTable.subscription_id == subscription_id)
     ).scalar_one_or_none()
+    subscription.customer_id = CUSTOMER_ID
     subscription.customer_descriptions = [
-        SubscriptionCustomerDescriptionTable(customer_id=CUSTOMER_ID, description="customer alias")
+        SubscriptionCustomerDescriptionTable(
+            subscription_id=subscription_id, customer_id=CUSTOMER_ID, description="customer alias"
+        )
     ]
     db.session.add(subscription)
     db.session.commit()
 
+    do_refresh_subscriptions_search_view()
+
+    # when
     data = get_subscriptions_query(**query_args(subscription_id))
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     subscription = GenericProductOne.from_subscription(subscription_id)
 
     # then
 
@@ -911,14 +913,55 @@
             ],
             "inUseByRelations": [],
         },
     ]
 
 
 @pytest.mark.parametrize(
+    "query_args,total_items",
+    [
+        (lambda ids: {}, 33),
+        (lambda ids: {"filter_by": [{"field": "subscriptionId", "value": f"{ids[0]}|{ids[1]}"}]}, 2),
+        (lambda ids: {"filter_by": [{"field": "subscriptionId", "value": "|".join(ids[3:8])}]}, 5),
+    ],
+)
+def test_multiple_subscriptions(
+    test_client, product_type_1_subscriptions_factory, generic_product_type_1, query_args, total_items
+):
+    # given
+
+    _, GenericProductOne = generic_product_type_1
+    subscription_ids = product_type_1_subscriptions_factory(30)
+
+    do_refresh_subscriptions_search_view()
+
+    # when
+    data = get_subscriptions_query(first=100, **query_args(subscription_ids))
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
+
+    # then
+
+    assert HTTPStatus.OK == response.status_code
+    result = response.json()
+    subscriptions_data = result["data"]["subscriptions"]
+    subscriptions = subscriptions_data["page"]
+    pageinfo = subscriptions_data["pageInfo"]
+
+    assert "errors" not in result
+    assert len(subscriptions) == total_items
+    assert pageinfo == {
+        "hasPreviousPage": False,
+        "hasNextPage": False,
+        "startCursor": 0,
+        "endCursor": total_items - 1,
+        "totalItems": total_items,
+    }
+
+
+@pytest.mark.parametrize(
     "query_args",
     [
         lambda sid: {"filter_by": [{"field": "subscriptionId", "value": sid}]},
         lambda sid: {"query_string": sid},
     ],
 )
 def test_single_subscription_with_processes(
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/test_workflows.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/test_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     expected_workflows = ["task_clean_up_tasks", "task_resume_workflows", "task_validate_products"]
     assert [rt["name"] for rt in workflows] == expected_workflows
 
 
 @pytest.mark.parametrize(
     "query_args",
     [
-        {"filter_by": [{"field": "products", "value": "Product 1"}]},
+        {"filter_by": [{"field": "product", "value": "Product 1"}]},
         {"query_string": 'product:"Product 1"'},
     ],
 )
 def test_workflows_filter_by_product(test_client, query_args):
     data = get_workflows_query(**query_args, sort_by=[{"field": "name", "order": "ASC"}])
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     assert HTTPStatus.OK == response.status_code
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_autoregistration.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_is_query_detailed.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_is_querying_page_data.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_is_querying_page_data.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/graphql/utils/test_override_class.py` & `orchestrator_core-2.2.0/test/unit_tests/graphql/utils/test_override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/helpers.py` & `orchestrator_core-2.2.0/test/unit_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-2.2.0/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/services/test_processes.py` & `orchestrator_core-2.2.0/test/unit_tests/services/test_processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     process_id = uuid4()
     pstat = ProcessStat(process_id, simple_workflow, None, None, current_user="user")
 
     _db_create_process(pstat)
 
     process = db.session.get(ProcessTable, process_id)
     assert process
-    assert process.workflow_name == "wf name"
+    assert process.workflow.name == "wf name"
     assert process.is_task
 
 
 def test_process_log_db_step_success(simple_workflow):
     process_id = uuid4()
     p = ProcessTable(
         process_id=process_id,
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/services/test_products.py` & `orchestrator_core-2.2.0/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-2.2.0/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/services/test_translations.py` & `orchestrator_core-2.2.0/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/test_db.py` & `orchestrator_core-2.2.0/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/test_workflow.py` & `orchestrator_core-2.2.0/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_errors.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_functional.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_get_updated_properties.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_json.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_search_query.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/utils/test_state.py` & `orchestrator_core-2.2.0/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/websocket/test_broadcast.py` & `orchestrator_core-2.2.0/test/unit_tests/websocket/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/__init__.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     res = extract_state(result)
     state = {"process_id": res["process_id"], "reporter": "john.doe", "tasks_removed": 1}
     assert_state(result, state)
 
     processes = db.session.scalars(select(ProcessTable)).all()
 
     assert len(processes) == 3
-    assert sorted(p.workflow_name for p in processes) == sorted(
+    assert sorted(p.workflow.name for p in processes) == sorted(
         ["nice and new task", "nice process", "task_clean_up_tasks"]
     )
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_async_workflow.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/test_async_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,30 +120,30 @@
         response = test_client.post("/api/processes/multiple_callback_wf", json=[{}])
         assert response.status_code == 201
         process_id = response.json()["id"]
 
         # Check process status
         response = test_client.get(f"api/processes/{process_id}")
         response_data = response.json()
-        assert response_data["status"] == "awaiting_callback"
+        assert response_data["last_status"] == "awaiting_callback"
         state = response_data["current_state"]
         assert state["phase"] == "DRY_RUN"
         assert state["__step_group"] == "Dry run"
         assert state["__sub_step"] == "Dry run - Await callback"
         assert "callback_route" in state
 
         # Continue workflow 1
         callback_route1 = state["callback_route"]
         response = test_client.post(callback_route1, json={"ext_data": "12345", "other": "useless data"})
         assert response.status_code == 200
 
         # Check process status
         response = test_client.get(f"api/processes/{process_id}")
         response_data = response.json()
-        assert response_data["status"] == "awaiting_callback"
+        assert response_data["last_status"] == "awaiting_callback"
         state = response_data["current_state"]
         assert state["dr_ext_data"] == "12345"
         assert state["phase"] == "FOR_REAL"
         assert state["__step_group"] == "For real"
         assert state["__sub_step"] == "For real - Await callback"
         assert "callback_route" in state
 
@@ -155,13 +155,13 @@
         response = test_client.post(callback_route2, json={"ext_data": "56789", "other": "very useful data"})
         assert response.status_code == 200
 
         # Final check
         response = test_client.get(f"api/processes/{process_id}")
         response_data = response.json()
 
-        assert response_data["status"] == "completed"
+        assert response_data["last_status"] == "completed"
 
         state = response_data["current_state"]
         assert state["ext_data"] == "56789"
 
         assert state["phase"] is None
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/test_config_db_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from more_itertools.more import one
 from more_itertools.recipes import first_true
 from sqlalchemy import not_, select
 from sqlalchemy.orm import joinedload
 
-from orchestrator.api.api_v1.endpoints.fixed_input import fi_configuration
 from orchestrator.db import ProductTable, WorkflowTable, db
 from orchestrator.db.models import FixedInputTable
 from orchestrator.services import products
 from orchestrator.services.products import get_products
 from orchestrator.targets import Target
+from orchestrator.utils.fixed_inputs import fixed_input_configuration as fi_configuration
 from orchestrator.workflows import ALL_WORKFLOWS
 
 
 def test_all_workflows_have_matching_targets_and_descriptions():
     for key, lazy_wf in ALL_WORKFLOWS.items():
         workflow = lazy_wf.instantiate()
         db_workflow = db.session.scalars(WorkflowTable.select().where(WorkflowTable.name == key)).first()
```

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-2.2.0/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.1.2rc4/PKG-INFO` & `orchestrator_core-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 2.1.2rc4
+Version: 2.2.0
 Summary: This is the orchestrator workflow engine.
 Requires-Python: >=3.11,<3.13
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -32,29 +32,29 @@
 Requires-Dist: deprecated
 Requires-Dist: deepmerge==1.1.1
 Requires-Dist: fastapi~=0.110.0
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=10.2.0
 Requires-Dist: itsdangerous
 Requires-Dist: Jinja2==3.1.3
-Requires-Dist: orjson==3.9.15
+Requires-Dist: orjson==3.10.0
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic[email]~=2.5.1
 Requires-Dist: pydantic-settings~=2.2.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson>=1.9,<1.17
 Requires-Dist: pytz==2024.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: schedule==1.1.0
-Requires-Dist: sentry-sdk[fastapi]==1.43.0
-Requires-Dist: SQLAlchemy==2.0.28
+Requires-Dist: sentry-sdk[fastapi]==1.44.0
+Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: SQLAlchemy-Utils==0.41.2
 Requires-Dist: structlog
-Requires-Dist: typer==0.9.0
-Requires-Dist: uvicorn[standard]~=0.28.0
+Requires-Dist: typer==0.12.0
+Requires-Dist: uvicorn[standard]~=0.29.0
 Requires-Dist: nwa-stdlib~=1.7.0
 Requires-Dist: oauth2-lib~=1.5.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.210.0
 Requires-Dist: pydantic-forms==1.0.2
 Requires-Dist: ruff
 Requires-Dist: celery~=5.3.1 ; extra == "celery"
```

